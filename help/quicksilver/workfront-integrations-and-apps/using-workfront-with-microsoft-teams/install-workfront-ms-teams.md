---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: Installera [!DNL Adobe Workfront] för Microsoft Teams
description: Med appen  [!DNL Adobe Workfront for Microsoft Teams] kan du utföra grundläggande åtgärder i [!DNL Workfront] utan att lämna dina [!DNL Microsoft Teams] chattkanaler.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Installera [!DNL Adobe Workfront] för Microsoft Teams

<!-- Audited: 1/2024 -->

<!--

>[!IMPORTANT]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->


Med appen [!DNL Adobe Workfront for Microsoft Teams] kan du utföra grundläggande åtgärder i [!DNL Workfront] utan att lämna dina [!DNL Microsoft Teams] chattkanaler.

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Om du vill använda [!DNL Adobe Workfront for Microsoft Teams integration] måste du använda en annan webbläsare än [!DNL Internet Explorer].


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: Standard</p>
    <p>Aktuell: [!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste vara teamägare i [!DNL Microsoft Teams] för att kunna installera [!DNL Workfront] för [!DNL Microsoft Teams].

## Installera [!DNL Workfront for Microsoft Teams]

Som teamägare i [!DNL Microsoft Teams] kan du installera appen [!DNL Workfront for Microsoft Teams] för vart och ett av dina team antingen från [!DNL Microsoft] Store eller från en fil som tillhandahålls av [!DNL Workfront].

### Installera [!DNL Workfront for Microsoft Teams] från [!DNL Microsoft] Store

1. Logga in på [!DNL Microsoft Teams] som teamägare.
1. Välj det team som du vill installera appen [!DNL Workfront for Microsoft Teams] för.
1. Klicka på **[!UICONTROL Store]** i sidans navigeringsfält.

1. Skriv *[!DNL Workfront]* i rutan **[!UICONTROL Search all]**.

1. Klicka på kortet **[!DNL Workfront]** och följ instruktionerna i guiden.
1. (Rekommenderas) Välj ett team i listrutan **[!UICONTROL Add to a team]** och aktivera alternativet **[!UICONTROL Yes]** för att lägga till programmet i ett team.

   ![ms_teams_add_to_a_team_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. För kanalen väljer du **[!UICONTROL General]** om du vill använda appen i den kanalen för det valda teamet och klickar sedan på **[!UICONTROL Set up]** för de funktioner du vill använda.

1. När installationen är klar visas ett meddelande om att installationen lyckades i [!UICONTROL General]-kanalen för det team du valde. Alla medlemmar i teamet kan se det här meddelandet.
1. (Valfritt) Fäst din [!DNL Workfront]-app för enklare åtkomst:

   1. Klicka på ikonen **[!UICONTROL More]** under meddelandefältet i [!UICONTROL General]-kanalen.

   1. För musen över appen [!DNL Workfront] i listan och klicka sedan på ikonen **[!UICONTROL More]** till höger om den.

   1. Klicka på **[!UICONTROL Pin]**.

      En [!DNL Workfront]-ikon läggs till under chattfältet. Du kommer snabbt åt området [!UICONTROL Search] härifrån.

      Mer information om hur du söker efter [!DNL Workfront] objekt finns i [Söka efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Klicka på **[!UICONTROL Log in to [!DNL Workfront]]** för att komma åt [!DNL Workfront from Microsoft Teams].

   Mer information om hur du loggar in på [!DNL Workfront] finns i avsnittet [Logga in på Workfront från Microsoft Teams](#log-in-to-workfront-from-microsoft-teams) i den här artikeln.

### Installera [!DNL Workfront for Microsoft Teams] från en privat fil

Om din organisation begränsar åtkomsten till hämtning av appar från [!DNL Microsoft] Store måste du kontakta vårt supportteam och begära en privat fil av appen [!DNL Workfront for Microsoft Teams] för att installera appen.

Mer information om hur du kontaktar vårt supportteam finns i [Kontakta kundsupport](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

Så här installerar du [!DNL Workfront for Microsoft Teams] från en privat fil:

1. Spara den privata filen som du har fått från [!DNL Workfront] på datorn.
1. Logga in på [!DNL Microsoft Teams] som [!DNL Microsoft] teamägare.
1. Klicka på ikonen **[!UICONTROL More]** för det team som du vill installera [!DNL Workfront for Microsoft Teams] för.

1. Klicka på **[!UICONTROL Manage Team]**.
1. Välj fliken **[!UICONTROL Apps]** och klicka sedan på **[!UICONTROL Upload a custom app]** i skärmens nedre högra hörn.

1. Bläddra efter den privata filen som du har sparat på datorn och följ sedan installationsstegen för att installera [!DNL Workfront for Microsoft Teams].
1. När installationen är klar visas ett meddelande om att installationen lyckades i den allmänna kanalen för det team du valde. Alla medlemmar i teamet kan se det här meddelandet.
1. (Valfritt) Klicka på ikonen **[!UICONTROL More]** (tre punkter) under fältet **[!UICONTROL Type your questions here]**.

1. (Valfritt) För musen över appen [!DNL Workfront] i listan och klicka sedan på ikonen **[!UICONTROL More]** till höger om den.

1. (Valfritt) Klicka på **[!UICONTROL Pin]**.

   Då läggs en [!DNL Workfront]-ikon till under fältet [!UICONTROL Type your questions here]. Du kommer snabbt åt området [!UICONTROL Search] härifrån.\
   Mer information om hur du söker efter Workfront-objekt finns i [Söka efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

## Logga in på [!DNL Workfront] från [!DNL Microsoft] team

Som [!DNL Microsoft Teams]-teamägare måste du installera [!DNL Workfront for Microsoft Teams]-appen för ditt team innan du eller någon i teamet kan logga in på [!DNL Workfront from Microsoft Teams].

När du är inloggad på [!DNL Workfront] från [!DNL Microsoft Teams] kan du ta emot [!DNL Workfront] meddelanden i [!DNL Workfront]-robotkanalen eller så kan du utföra vissa åtgärder i [!DNL Workfront] från [!DNL Microsoft Teams].

Mer information om hur du installerar appen [!DNL Workfront] finns i avsnittet [Installera [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) i den här artikeln.

Mer information om hur du får åtkomst till [!DNL Workfront] från [!DNL Microsoft Teams] för att utföra vissa åtgärder finns i [Åtkomst [!DNL Adobe Workfront] från [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md).

Logga in på [!DNL Workfront] från [!DNL Microsoft Teams]:

1. Gå till **[!UICONTROL General]**-kanalen för det team där [!DNL Workfront for Microsoft Teams]-appen har installerats och klicka på **[!UICONTROL Log in to Workfront]**.

   [!DNL Workfront]-chattkanalen läggs till i dina [!DNL Microsoft Teams]-chattkanaler.

1. Gå till chattkanalen [!DNL Workfront] i [!DNL Microsoft Teams] och skriv *[!UICONTROL log in]* i fältet **[!UICONTROL Type your questions here]**.

   eller

   Klicka på **[!UICONTROL Log in]**.

   En ny flik i webbläsaren öppnas.

1. Följ instruktionerna för att logga in på [!DNL Workfront] med Förbättrad autentisering, OAuth 2.0 eller din SAML-URL (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* När du uppmanas att ange domänen för ditt [!DNL Workfront]-konto skriver du den i det här formatet: *ditt företags sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront]-administratör har aktiverat den för den här integreringen.


1. Stäng webbläsarfliken som du använde för att logga in och gå tillbaka till [!DNL Microsoft Teams].

   Ett meddelande visas i chattkanalen [!DNL Workfront] som bekräftar att du har loggat in på [!DNL Workfront].
