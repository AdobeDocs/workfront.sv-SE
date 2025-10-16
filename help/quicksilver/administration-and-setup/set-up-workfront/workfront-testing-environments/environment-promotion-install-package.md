---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installera ett miljöerbjudande
description: Funktionen för att främja miljön är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Lär dig hur du installerar ett miljömarknadsföringspaket i en målmiljö.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# Installera ett miljöerbjudande

När du har skapat ett paket kan du installera det i en annan miljö.

Du måste installera ett paket i miljön som du vill kopiera objekt **till**. Om du till exempel konfigurerar ett projekt i din anpassade sandlådemiljö för uppdatering och befordrar det till din produktionsmiljö, måste du installera paketet i din produktionsmiljö.

>[!IMPORTANT]
>
>* Om din anpassade uppdateringssandlåda uppdateras medan du konfigurerar objekt för miljöbefordran, kommer den konfigurationen att förloras vid uppdateringen. Vi rekommenderar att du inte uppdaterar din anpassade uppdateringssandlåda om inte alla utestående miljöbefordringsobjekt och -paket har befordrats.
>* Objekt som skapas i målmiljön som en del av paketinstallationen har **inte** samma ID som objektet i den ursprungliga miljön. Detta beror på att ID:n tilldelas av systemet när objekt skapas.

## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime eller Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront-licenser</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td><p>Du måste vara Workfront-administratör.</p>
   </td>
  </tr>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Du måste skapa ett miljöerbjudande innan du kan installera det.

Instruktioner finns i [Skapa eller redigera ett miljöbefordringspaket](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Paketstatus för installation

Ett paket måste ha AKTIV status för att kunna installeras i din produktionsmiljö.

Vi rekommenderar att du flyttar paketet till TESTING-status och installerar det i en annan sandlåda för att testa paketet.  Om testet lyckas utan fel flyttar du paketet till ACTIVE för att installera det i produktionsmiljön.

Så här redigerar du ett pakets status:

1. Markera paketet enligt beskrivningen i [Redigera eller sammanställ ett befintligt paket](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) i artikeln Skapa och redigera miljöerbjudandepaket.
1. Klicka på **Redigera paket**.
1. Klicka på **Status**.
1. Välj önskad status i listrutan.

Mer information om status finns i [Miljöskyddsstatus](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) i artikeln Översikt över rörliga objekt mellan Workfront-miljöer.

## Installera ett paket

>[!NOTE]
>
>* Om du vill installera ett paket måste du vara inloggad i den miljö där du vill installera paketet. Det här är miljön som du kopierar objekt **till**.

1. Gå till den miljö där du vill installera paketet.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen och välj sedan **Miljökampanj**.
1. Välj paketet i listan som visas.
1. För varje objekt som har en kollision väljer du hur kollisionen ska lösas.

   Lös en kollision genom att klicka på listrutepilen bredvid objekttypen och välja den åtgärd som du vill utföra.

   Mer information finns i [Konflikter](#collisions) i den här artikeln
1. Om du vill distribuera paketet till den nya miljön klickar du på **Distribuera** längst upp till höger på skärmen.

## Konflikter

En kollision är ett objekt som finns i målmiljön för en installation som matchar ett av objekten som installeras från källmiljön. Konflikter upptäcks genom att källobjektens namn och ID jämförs med objekten i målmiljön. Konflikter upptäcks också genom att källobjekt jämförs med poster för tidigare installerade objekt.

När en kollision inträffar kan du välja hur kollisionen ska lösas. Konflikter löses på objektnivå.

Du kan visa kollisioner genom att klicka på listrutan bredvid varje objekttyp. Konflikter visas i kolumnen Konflikter.

>[!NOTE]
>
>Upptäckta kollisioner kanske inte är de objekt som du vill åsidosätta eller använda i installationen. Vi rekommenderar att du verifierar identifierade konflikter för att säkerställa att installationsmålen är korrekta.

Om du vill lösa en konflikt väljer du en åtgärd i kolumnen Distributionsåtgärd eller använder den standardåtgärd som redan visas.

* **Skapa med nytt namn**: Skapa ett nytt objekt i målmiljön. Om objektet finns i målmiljön kan du skapa ett nytt objekt med ett nytt namn. Om den inte finns i målmiljön kan du skapa objektet med ett nytt namn eller med namnet som objektet har i paketet.
* **Använd befintlig**: Objektet i paketet är inte installerat och objektet som redan fanns i målmiljön är oförändrat.
* **Skriv över**: Objektet i paketet ersätter det befintliga objektet i målmiljön.

  Du kan också välja vilka objekt som ska skrivas över även om en kollision inte upptäcks.

  Mer information om hur överskrivning påverkar överordnade och underordnade objekt finns i [Skriva över överordnade och underordnade objekt](#overwriting-parent-and-child-objects) i den här artikeln.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standardvärdena är `Create new` om objektet inte finns i målmiljön och `Use existing` om objektet finns i målmiljön. Du kan återställa standardmappningen genom att klicka på **Återställ till standardmappning**.

## Skriva över överordnade och underordnade objekt

Vissa objekt i erbjudandepaketet kan ha underordnade objekt. Ett projekt (överordnat projekt) har till exempel uppgifter (underordnade projekt). När du skriver över ett överordnat objekt hanteras underordnade objekt på följande sätt:

* Underordnade objekt som finns i både paketet och målet uppdateras i målet så att de matchar paketet.
* Underordnade objekt som finns i paketet men inte målet skapas.
* Underordnade objekt som finns i målet men inte i paketet ändras inte.

Den här funktionen påverkar följande överordnade och underordnade objekt:

| Överordnat objekt | Underordnade objekt |
|---|---|
| Projekt | Aktivitet<br>QueueDef (ködefinition)<br>RoutingRule |
| Mall | TemplateTask<br>QueueDef (ködefinition)<br>RoutingRule |
| Parameter (anpassat formulärfält) | ParameterOption (alternativet för anpassat formulärfält) |
| CalendarInfo | CalendarSection |
| QueueDef (ködefinition) | QueueTopicGroup<br>QueueTopic |

