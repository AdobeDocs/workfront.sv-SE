---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Skapa ett läsarkonto (tjänstkonto) för Snowflake
description: För att få tillgång till data i Workfront Data Lake måste du först skapa ett läsarkonto för Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Skapa ett läsarkonto (tjänstkonto) för Snowflake

För att få tillgång till data i Workfront-sjön måste du först skapa ett Snowflake-läsarkonto (eller tjänstkonto) för varje ny anslutning. När du har skapat en anslutning kan du hitta dess associerade URL och användarnamn genom att klicka på den på **Dataåtkomst** sida (**Huvudmeny** > **Inställningar** > **System** > **Dataåtkomst**) under **Befintliga anslutningar** -fliken.

Mer information om hur du använder en nyligen skapad anslutning med en extern produkt finns i [Upprätta en anslutning till Workfront Data Lake](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>TBD</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa ett läsarkonto

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Inställningar**.

1. Klicka på i den vänstra panelen **System** > **Dataåtkomst**.

1. Klicka **Skapa ny anslutning**

1. I fönstret som visas anger du ett namn för anslutningen i **Beskrivning av anslutningsreferens** och ett användarnamn i **Anslutningsanvändare** och sedan klicka **Generera anslutning**.

   ![Skapa läsarkonto](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Standardlösenord** kommer att genereras samt en URL där dina data kan visas via Snowflake. Du måste använda lösenordet tillsammans med det användarnamn du valde för att logga in på Snowflake för första gången, så se till att du sparar information om det samt URL:en. Markera rutan som anger att du har gjort det och klicka sedan **Stäng**.

   ![Lösenord för standardkonto](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öppna Snowflake med en webbläsare och gå till URL:en från det föregående steget, ange det användarnamn du valde och standardlösenordet från det föregående steget och klicka sedan på **Logga in**.

1. När du har loggat in för första gången uppmanas du att välja ett nytt lösenord. Ange ett lösenord i båda **Nytt lösenord** och **Bekräfta lösenord** fält och klicka sedan på **Skicka**.

   ![Återställ Snowflake-lösenord](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Nu kan du använda ditt användarnamn och nya lösenord för att komma åt din Workfront-datasjön i Snowflake eller det företagsvisualiseringsverktyg som du väljer.

## Återkalla ett läsarkonto

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Inställningar**.

1. Klicka på i den vänstra panelen **System** > **Dataåtkomst**.

1. Klicka på papperskorgsikonen ![Ikonen Ta bort](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) till höger om det konto du vill återkalla.

1. I fönstret som visas markerar du kryssrutan för att bekräfta och klickar sedan på **Ta bort**.
