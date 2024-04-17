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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Installera ett miljöerbjudande

>[!NOTE]
>
>Om du vill installera ett paket måste du vara inloggad i den miljö där du vill installera paketet. Det här är den miljö som du kopierar objekt i **till**.

1. Gå till den miljö där du vill installera paketet.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen väljer du **Miljömarknadsföring**.
1. Välj paketet i listan som visas.
1. För varje objekt som har en kollision väljer du hur kollisionen ska lösas.

   Lös en kollision genom att klicka på listrutepilen bredvid objekttypen och välja den åtgärd som du vill utföra.

   Mer information finns i [Konflikter](#collisions) i den här artikeln
1. Om du vill distribuera paketet till den nya miljön klickar du **Distribuera** längst upp till höger på skärmen.

## Konflikter

Konflikter inträffar när ett objekt som är en del av installationspaketet redan finns i målmiljön. När detta inträffar kan du välja hur kollisionen ska lösas. Konflikter löses på objektnivå.

Du kan visa kollisioner genom att klicka på listrutan bredvid varje objekttyp. Konflikter visas i kolumnen Konflikter.

Om du vill lösa en konflikt väljer du en åtgärd i kolumnen Distributionsåtgärd eller använder den standardåtgärd som redan visas.

* **Skapa med nytt namn**: Skapa ett nytt objekt i målmiljön. Om objektet finns i målmiljön kan du skapa ett nytt objekt med ett nytt namn. Om den inte finns i målmiljön kan du skapa objektet med ett nytt namn eller med namnet som objektet har i paketet.
* **Använd befintlig**: Objektet i paketet installeras inte och objektet som redan fanns i målmiljön ändras inte.
* **Skriv över**: Objektet i paketet ersätter det befintliga objektet i målmiljön.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standardvärden är `Create new` om objektet inte finns i målmiljön, och `Use existing` om objektet finns i målmiljön. Du kan återgå till standardmappningen genom att klicka på **Återställ till standardmappning**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
