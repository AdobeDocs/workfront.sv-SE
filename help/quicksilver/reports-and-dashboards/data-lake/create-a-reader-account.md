---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Skapa ett läsarkonto för Snowflake
description: För att få åtkomst till Data Connect-data måste du först skapa ett Snowflake-läsarkonto.
author: Courtney
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 32f738e56a471407997031e13bb22abe81ac535c
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 0%

---

# Skapa ett läsarkonto eller en anslutning till Snowflake

För att få tillgång till data i Data Connect måste du först skapa ett Snowflake-läsarkonto (eller tjänstkonto) för din organisation och sedan skapa en ny anslutning för varje användare eller verktyg som du vill ha tillgång till med Data Connect.

När du har skapat en anslutning kan du hitta dess associerade URL och användarnamn genom att klicka på den på sidan Dataanslutning (huvudmenyn > Inställningar > System > Dataanslutning) under fliken Befintliga anslutningar.

Mer information om hur du använder en nyligen skapad anslutning med en extern produkt finns i [Upprätta en anslutning till Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Ultimate</p>
    <p>Arbetsflöde Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett läsarkonto

Du måste skapa ett nytt Snowflake Reader-konto för din organisation innan du kan börja skapa anslutningar.

>[!IMPORTANT]
>
>Denna process får endast utföras en gång per organisation. Om knappen **Skapa Reader-konto** inte finns på den plats som beskrivs nedan har ditt läsarkonto redan skapats.

Så här skapar du ett läsarkonto:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataanslutning** i den vänstra panelen.

1. Klicka på knappen **Skapa Reader-konto** för att börja skapa din organisations läsarkonto. Processen är automatisk, men kan ta upp till 24 timmar att slutföra.

1. När det är klart visas ett dialogrutefönster där det förklaras att ditt läsarkonto nu är aktivt. Uppdatera webbläsarsidan för att få åtkomst till knappen **Skapa ny anslutning**.

![Dialogrutan för att skapa Reader-konto](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Skapa en anslutning

>[!IMPORTANT]
>
>I juni 2026 krävs användarnamn/lösenord för att använda multifaktorautentisering (MFA). Vi rekommenderar att du övergår till antingen RSA- eller PAT-baserad autentisering för tjänstanvändarkonton som används för att läsa in data från Data Connect till tredjepartsverktyg för visualisering, dataprocessorer och skript som inte fungerar med MFA i autentiseringsprocessen.


1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataanslutning** i den vänstra panelen.

1. Klicka på **Skapa ny anslutning**.

1. I fönstret som visas anger du ett namn för anslutningen i **Anslutningsreferensbeskrivning** och ett användarnamn i **Anslutningsanvändare**. Klicka sedan på **Skapa anslutning**.

   ![Skapa ny anslutning](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Välj en autentiseringsmetod för anslutningen:
   * [Lösenordsautentisering](#password-authentication)
   * [Autentisering med token för programmatisk åtkomst](#programmatic-access-token-authentication)
   * [RSA-nyckelautentisering](#rsa-key-authentication)

### Lösenordsautentisering

1. Klicka på **Lösenord** och sedan på **Skapa anslutning**.

1. Ett **standardlösenord** genereras samt en URL där dina data kan visas via Snowflake. Du måste använda lösenordet med det användarnamn du valde för att logga in på Snowflake för första gången, så se till att du sparar information om det och URL:en. Markera kryssrutan som hävdar att du har gjort det och klicka sedan på **Stäng**.

   ![Standardkontolösenord](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Öppna Snowflake med en webbläsare och gå till URL:en från det föregående steget, ange det användarnamn du valde och standardlösenordet från det föregående steget och klicka sedan på **Logga in**.

1. När du har loggat in för första gången uppmanas du att välja ett nytt lösenord. Ange ett lösenord i fälten **Nytt lösenord** och **Bekräfta lösenord** och klicka sedan på **Skicka**.

   ![Återställ Snowflake-lösenord](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Nu kan du använda ditt användarnamn och nya lösenord för att få åtkomst till Data Connect-datasjön i Snowflake eller det företagsvisualiseringsverktyg som du väljer.

### Autentisering med token för programmatisk åtkomst

1. Klicka på **Programmatisk åtkomsttoken**.

1. Ange ett förfallodatum för din token i fältet **Förfallodatum**. Du kan välja ett förfallodatum på upp till 365 dagar i framtiden.

1. Klicka på **Skapa anslutning**.

1. En PAT-token genereras som kan användas för autentisering, och din Snowflake-URL anges. Du kan använda PAT och det användarnamn du angav för att ansluta till Snowflake från ditt tredjepartsvisualiseringsverktyg eller din dataprocessor. Se till att du sparar både den och URL-adressen. Markera kryssrutan som hävdar att du har gjort det och klicka sedan på **Stäng**.

   ![dialogruta för programmatisk åtkomsttoken](/help/quicksilver/reports-and-dashboards/data-lake/assets/pat-test.png)


### RSA-nyckelautentisering

1. Klicka på **RSA-nyckel**.

1. Ange en offentlig RSA-nyckel i fältet **Offentlig RSA-nyckel**.

1. Klicka på **Skapa anslutning**.

1. En anslutning skapas och din URL till Snowflake-miljön anges. Du kan använda RSA-nyckeln och det användarnamn du angav för att ansluta till Snowflake från ditt tredjepartsvisualiseringsverktyg eller din dataprocessor.



Du måste använda RSA-nyckeln med det användarnamn du valde för att logga in på Snowflake, så att du kan registrera både den och URL:en. Markera kryssrutan som hävdar att du har gjort det och klicka sedan på **Stäng**.

![Dialogrutan för RSA-nyckel](assets/rsa-test.png)

## Återkalla ett läsarkonto

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataåtkomst** i den vänstra panelen.

1. Klicka på papperskorgsikonen ![Ta bort ikon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) till höger om det konto du vill återkalla.

1. Markera rutan för att bekräfta i fönstret som visas och klicka sedan på **Ta bort**.
