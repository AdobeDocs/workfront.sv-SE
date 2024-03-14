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
source-git-commit: 5ab9f7c975df86fa7a1f6d54a2fefcbd4cbd9248
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Installera ett miljöerbjudande


1. Gå till den miljö där du vill installera paketet. Det här är den miljö som du kopierar objekt i **till**.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen väljer du **Miljömarknadsföring**.
1. Välj paketet i listan som visas.
1. Klicka på **Installera** längst upp till höger på skärmen.
1. Mappa varje objekt i paketet till motsvarande objekt i målmiljön.

   Mer information finns i [Mappning](#mapping) i den här artikeln


## Mappning

Varje objekttyp visas i den vänstra navigeringen och på ett kort. På kortet visas objekt av den typen och om objekten finns i målmiljön. Du kan bestämma hur dessa objekt ska flyttas till målmiljön.

* Skapa nytt: Objektet finns i målmiljön
* Använd befintlig: Objektet i paketet installeras inte och objektet som redan fanns i målmiljön ändras inte.
* Skriv över befintligt: (Inte tillgängligt för närvarande) Objektet i paketet ersätter det befintliga objektet i målmiljön.
* Använd inte:Om du väljer Använd inte visas ett felmeddelande som anger hur det här alternativet påverkar andra objekt eller fält.

Standardvärden är `Create new` om objektet inte finns i målmiljön, och `Use existing` om objektet finns i målmiljön. Du kan återgå till standardmappningen genom att klicka på **Återställ till standardmappning**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
