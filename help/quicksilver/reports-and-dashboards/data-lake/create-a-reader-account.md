---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Skapa ett läsarkonto (tjänstkonto) för Snowflake
description: För att få åtkomst till data i Data Connect måste du först skapa ett läsarkonto i Snowflake.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Skapa ett läsarkonto (tjänstkonto) för Snowflake

För att få åtkomst till data i Data Connect måste du först skapa ett Snowflake-läsarkonto (eller tjänstkonto) för varje ny anslutning. När du har skapat en anslutning kan du hitta dess associerade URL och användarnamn genom att klicka på den på sidan **Dataåtkomst** (**Huvudmeny** > **Inställningar** > **System** > **Dataåtkomst**) på fliken **Befintliga anslutningar** .

Mer information om hur du använder en nyligen skapad anslutning med en extern produkt finns i [Upprätta en anslutning till Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Ingår i följande planer:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>Kan köpas som tillägg till följande planer:</p> 
    <ul>
        <li>Välj</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect är inte tillgängligt för tidigare Workfront-planer.</p> 
   </td> </td> 
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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett läsarkonto

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataåtkomst** i den vänstra panelen.

1. Klicka på **Skapa ny anslutning**

1. I fönstret som visas anger du ett namn för anslutningen i **Anslutningsreferensbeskrivning** och ett användarnamn i **Anslutningsanvändare**. Klicka sedan på **Skapa anslutning**.

   ![Skapa läsarkonto](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Ett **standardlösenord** genereras, liksom en URL där dina data kan visas via Snowflake. Du måste använda lösenordet tillsammans med det användarnamn du valde för att logga in på Snowflake för första gången, så se till att du sparar information om det samt URL:en. Markera kryssrutan som hävdar att du har gjort det och klicka sedan på **Stäng**.

   ![Standardkontolösenord](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öppna Snowflake med en webbläsare och gå till URL:en från det föregående steget, ange det användarnamn du valde och standardlösenordet från det föregående steget och klicka sedan på **Logga in**.

1. När du har loggat in för första gången uppmanas du att välja ett nytt lösenord. Ange ett lösenord i fälten **Nytt lösenord** och **Bekräfta lösenord** och klicka sedan på **Skicka**.

   ![Återställ Snowflake-lösenord](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Nu kan du använda ditt användarnamn och nya lösenord för att få åtkomst till Data Connect-datasjön i Snowflake eller det företagsvisualiseringsverktyg som du väljer.

## Återkalla ett läsarkonto

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataåtkomst** i den vänstra panelen.

1. Klicka på papperskorgsikonen ![Ta bort ikon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) till höger om det konto du vill återkalla.

1. Markera rutan för att bekräfta i fönstret som visas och klicka sedan på **Ta bort**.
