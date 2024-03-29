---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Skapa eller redigera ett miljöerbjudande
description: Funktionen för att främja miljön är avsedd att göra det möjligt att flytta konfigurationsrelaterade objekt från en miljö till en annan. Lär dig hur du skapar ett paket för miljöbefordran som du sedan kan installera i en annan miljö.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: c0a841d8f6a4431ff95c1b1d5904c8f41a7c82ca
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Skapa eller redigera ett miljöerbjudande

## Skapa ett paket

1. Gå till den miljö som du vill skapa paketet i. Det här är den miljö som du kopierar objekt i **från**.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen väljer du **Miljömarknadsföring**.
1. Klicka **Skapa paket**.

   Sidan Nytt kampanjpaket öppnas.

1. i **Paketnamn** anger du ett namn för paketet.
1. I **Beskrivning** anger du en beskrivning för det här paketet.
1. Om du vill lägga till ett objekt i paketet klickar du på **Lägg till objekt** i den vänstra navigeringen och välj den typ av objekt som du vill lägga till.
1. Markera ett eller flera objekt i listan eller skriv namnet i sökfältet och markera objektet när det visas i listan. Du kan markera mer än ett objekt i listan.
1. Klicka **Lägg till (X-objekt)** om du vill lägga till de markerade objekten i paketet.

   Om du t.ex. har valt tre projekt att lägga till i projektet, säger knappen **Lägg till 3 projekt**.

   Objekten som du har lagt till visas i området Paketinnehåll till höger på sidan.

1. Om du vill lägga till en annan typ av objekt upprepar du steg 7-9.
1. (Valfritt) Om du vill ta bort ett objekt från paketet håller du pekaren över objektet i paketinnehållsområdet och klickar på X:et bredvid objektet.
1. När du har lagt till alla önskade objekt i paketet klickar du på **Spara och stäng** om du vill spara paketet utan att montera det.

   eller

   Klicka **Spara och montera** för att spara och sätta ihop paketet.

   >[!NOTE]
   >
   >* Knapparna Spara, Stäng och Spara och Montera är tillgängliga om ett paket har både ett namn med fem eller fler tecken och minst ett objekt tillagt.
   >* Du kan inte montera ett paket som har en installationsbar status som Testing eller Aktiv.

## Redigera eller sätta ihop ett befintligt paket

1. Gå till den miljö som du vill skapa paketet i. Det här är den miljö som du kopierar objekt i **från**.
1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![Ikonen Inställningar](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen väljer du **Miljömarknadsföring**.
1. Välj paketet i listan som visas.
1. (Villkorligt) Om du vill visa arkiverade (inaktiverade) paket aktiverar du **Visa pensionerade paket** alternativ.
1. Om du vill visa innehållet, inklusive alla objekt och deras underordnade objekt, klickar du på den nedrullningsbara pilen bredvid objekttypen i **Innehåll** -avsnitt.
1. Om du vill visa tidigare installationer och installationsförsök för det här paketet klickar du på **Distributioner**.
1. Om du vill redigera paketet klickar du på **Redigera paket** längst upp till höger på skärmen.
1. Klicka på **Installera** längst upp till höger på skärmen.

   Instruktioner om hur du installerar ett paket finns i [Installera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


