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
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 66b9fc84c18bce2d0cecee9368a125570c822a54
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Installera ett miljöerbjudande

När du har skapat ett paket kan du installera det i en annan miljö.

## Förutsättningar

Du måste ha skapat ett paket innan du kan installera det.

Instruktioner finns i [Skapa eller redigera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Paketstatus för installation

Ett paket måste ha AKTIV status för att kunna installeras i din produktionsmiljö.

Vi rekommenderar att du flyttar paketet till TESTING-status och installerar det i en annan sandlåda för att testa paketet.  Om testet lyckas utan fel flyttar du paketet till ACTIVE för att installera det i produktionsmiljön.

Så här redigerar du ett pakets status:

1. Välj paketet enligt beskrivningen i  [Redigera eller sätta ihop ett befintligt paket](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) i artikeln Skapa och redigera miljöerbjudandepaket.
1. Klicka **Redigera paket**.
1. Klicka **Status**.
1. Välj önskad status i listrutan.

Mer information om status finns i [Status för miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) i artikeln Översikt över hur du flyttar objekt mellan Workfront-miljöer.

## Installera ett paket

>[!NOTE]
>
>* Om du vill installera ett paket måste du vara inloggad i den miljö där du vill installera paketet. Det här är den miljö som du kopierar objekt i **till**.

1. Gå till den miljö där du vill installera paketet.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen väljer du **Miljömarknadsföring**.
1. Välj paketet i listan som visas.
1. För varje objekt som har en kollision väljer du hur kollisionen ska lösas.

   Lös en kollision genom att klicka på listrutepilen bredvid objekttypen och välja den åtgärd som du vill utföra.

   Mer information finns i [Konflikter](#collisions) i den här artikeln
1. Om du vill distribuera paketet till den nya miljön klickar du **Distribuera** längst upp till höger på skärmen.

## Konflikter

Konflikter inträffar när ett objekt som ingår i installationspaketet har samma namn som ett objekt som redan finns i målmiljön. När detta inträffar kan du välja hur kollisionen ska lösas. Konflikter löses på objektnivå.

Du kan visa kollisioner genom att klicka på listrutan bredvid varje objekttyp. Konflikter visas i kolumnen Konflikter.

Om du vill lösa en konflikt väljer du en åtgärd i kolumnen Distributionsåtgärd eller använder den standardåtgärd som redan visas.

* **Skapa med nytt namn**: Skapa ett nytt objekt i målmiljön. Om objektet finns i målmiljön kan du skapa ett nytt objekt med ett nytt namn. Om den inte finns i målmiljön kan du skapa objektet med ett nytt namn eller med namnet som objektet har i paketet.
* **Använd befintlig**: Objektet i paketet installeras inte och objektet som redan fanns i målmiljön ändras inte.
* **Skriv över**: Objektet i paketet ersätter det befintliga objektet i målmiljön.

  Du kan också välja vilka objekt som ska skrivas över även om en kollision inte upptäcks.

  Mer information om hur överskrivning påverkar överordnade och underordnade objekt finns i [Skriva över överordnade och underordnade objekt](#overwriting-parent-and-child-objects) i den här artikeln.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standardvärden är `Create new` om objektet inte finns i målmiljön, och `Use existing` om objektet finns i målmiljön. Du kan återgå till standardmappningen genom att klicka på **Återställ till standardmappning**.

## Skriva över överordnade och underordnade objekt

Vissa objekt i erbjudandepaketet kan ha underordnade objekt. Ett projekt (överordnat projekt) har till exempel uppgifter (underordnade projekt). När du skriver över ett överordnat objekt hanteras underordnade objekt på följande sätt:

* Underordnade objekt som finns i både paketet och målet uppdateras i målet så att de matchar paketet.
* Underordnade objekt som finns i paketet men inte målet skapas.
* Underordnade objekt som finns i målet men inte i paketet ändras inte.

Den här funktionen påverkar följande överordnade och underordnade objekt:

| Överordnat objekt | Underordnade objekt |
|---|---|
| Projekt | Uppgift<br>QueueDef (ködefinition)<br>RoutingRule |
| Mall | TemplateTask<br>QueueDef (ködefinition)<br>RoutingRule |
| Parameter (anpassat formulärfält) | ParameterOption (alternativet för anpassat formulärfält) |
| CalendarInfo | CalendarSection |
| QueueDef (ködefinition) | QueueTopicGroup<br>QueueTopic |

