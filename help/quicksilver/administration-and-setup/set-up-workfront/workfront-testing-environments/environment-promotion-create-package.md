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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 2e4bcd6400971104e9138fab0faf20d33af32e51
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Skapa eller redigera ett miljöerbjudande

Du måste skapa ett paket i miljön som du vill kopiera objekt **från**. Om du till exempel konfigurerar ett projekt i din anpassade sandlådemiljö för uppdatering och befordrar det till din produktionsmiljö, måste du skapa paketet i din anpassade sandlådemiljö för uppdatering.

>[!IMPORTANT]
>
>Om din anpassade uppdateringssandlåda uppdateras medan du konfigurerar objekt för miljöbefordran, kommer den konfigurationen att förloras vid uppdateringen. Vi rekommenderar att du inte uppdaterar din anpassade uppdateringssandlåda om inte alla utestående miljöbefordringsobjekt och -paket har befordrats.

## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime eller Ultimate (endast nya planer)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenser</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa ett paket

1. Gå till den miljö som du vill skapa paketet i. Det här är miljön som du kopierar objekt **från**.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen och välj sedan **Miljökampanj**.
1. Klicka på **Skapa paket**.

   Sidan Nytt kampanjpaket öppnas.

1. Ange ett namn för paketet i fältet **Paketnamn**.
1. Ange en beskrivning för det här paketet i fältet **Beskrivning**.
1. Om du vill lägga till ett objekt i paketet väljer du den typ av objekt som du vill lägga till i den vänstra navigeringen.
1. Markera ett eller flera objekt i listan som visas, eller skriv namnet i sökfältet och markera objektet när det visas i listan. Du kan markera mer än ett objekt i listan.

   Listan innehåller upp till 500 objekt av den valda objekttypen. Om du vill söka efter ett objekt som inte finns med i listan använder du sökfältet.
1. Klicka på **Lägg till (X-objekt)** för att lägga till de markerade objekten i paketet.

   >[!INFO]
   >
   >**Exempel**
   >
   >Om du har valt tre projekt att lägga till i projektet visas knappen **Lägg till tre projekt**.

   Objekten som du har lagt till visas i området Paketinnehåll till höger på sidan.

1. Om du vill lägga till en annan typ av objekt upprepar du steg 7-9.
1. (Valfritt) Om du vill ta bort ett objekt från paketet håller du pekaren över objektet i paketinnehållsområdet och klickar på X:et bredvid objektet.
1. När du har lagt till alla önskade objekt i paketet klickar du på **Spara och stäng** för att spara paketet utan att montera det.

   eller

   Klicka på **Spara och sammanställ** för att spara och sätta ihop paketet.

   >[!NOTE]
   >
   >* Knapparna Spara, Stäng och Spara och Montera är tillgängliga om ett paket har både ett namn med fem eller fler tecken och minst ett objekt tillagt.
   >* Du kan inte montera ett paket som har en installationsbar status som Testing eller Aktiv.

## Redigera eller sätta ihop ett befintligt paket

Ett paket måste ha statusen `DRAFT` för att kunna redigeras.

1. Gå till den miljö i vilken du vill redigera paketet. Det här är miljön där paketet ursprungligen skapades.
1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **System** i den vänstra navigeringen och välj sedan **Miljökampanj**.
1. Välj paketet i listan som visas.
1. (Villkorligt) Aktivera alternativet **Visa inaktuella paket** om du vill visa inaktiverade paket.
1. (Valfritt) Om du vill visa innehållet, inklusive alla objekt och deras underordnade objekt, klickar du på listrutepilen bredvid objekttypen i avsnittet **Innehåll** .
1. (Valfritt) Om du vill visa tidigare installationer och installationsförsök för det här paketet klickar du på **Distributioner**.
1. (Valfritt) Om du vill redigera paketet klickar du på **Redigera paket** längst upp till höger på skärmen.
Ett paket måste ha statusen `DRAFT` för att kunna redigeras. Om du vill flytta paketet till `DRAFT`-status väljer du `Draft` i fältet **Status**. Du kan sedan fortsätta redigera paketet.
1. Installera paketet genom att klicka på **Installera** längst upp till höger på skärmen.

   Instruktioner om hur du installerar ett paket finns i [Installera ett miljöerbjudande](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
