---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]
description: Om du integrerar [!DNL Adobe Workfront] med [!DNL Slack] kan du komma åt [!DNL Workfront] från Slack eller utföra vissa åtgärder i [!DNL Workfront] med ett snedstreck-kommando. Integrationen kan användas från alla [!DNL Slack] miljöer, inklusive  [!DNL Slack] mobilappen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Åtkomst till [!DNL Adobe Workfront] från [!DNL Slack]

Genom att integrera [!DNL Adobe Workfront] med [!DNL Slack] kan du komma åt [!DNL Workfront] från [!DNL Slack] eller utföra vissa åtgärder i [!DNL Workfront] med hjälp av ett snedstreck-kommando. Integrationen kan användas från valfri [!DNL Slack]-miljö, inklusive [!DNL Slack]-mobilappen.

Du eller din [!DNL Slack]-administratör måste installera [!DNL Workfront]-appen i din [!DNL Slack]-instans innan du kan använda [!DNL Workfront] från [!DNL Slack]. Mer information finns i [Konfigurera Adobe Workfront för Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Alla</p>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Om snedstreckskommandon {#about-slash-commands}

När du använder [!DNL Slack] skriver du meddelanden i ett meddelandefält. När du börjar ett meddelande med ett snedstreck blir det ett kommando och fungerar annorlunda än ett enkelt meddelande. Kommandot instruerar [!DNL Slack] att utföra en åtgärd.

Du kan komma åt din [!DNL Workfront]-instans från [!DNL Slack] genom att skriva ett snedstreck i valfri [!DNL Slack]-kanal.

Kom ihåg följande när du använder ett snedstreck i [!DNL Slack] för att komma åt [!DNL Workfront]:

* Snedstreckskommandon är skiftlägeskänsliga.
* Kommandona för [!DNL Workfront] är bara synliga för dig, oavsett vilken kanal du skriver in dem i.
* Kommandot ska alltid börja med `/workfront` eller `/wf` följt av ett mellanslag och namnet på en åtgärd som du vill utföra i [!DNL Workfront].

  Detta anger att ditt kommando är avsett för appen [!DNL Workfront]. Kommandona för [!DNL Workfront] fungerar bara när du redan har konfigurerat [!DNL Workfront]-appen med din [!DNL Slack]-instans.

En lista med alla kommandon som du kan köra från Slack för [!DNL Workfront] finns i [Åtkomst [!DNL Workfront]  från ett snedstreck-kommando i [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Logga in på [!DNL Workfront] från [!DNL Slack] {#log-in-to-workfront-from-slack}

När du skriver ett kommando i meddelandefältet i Slack blir du först ombedd att logga in på [!DNL Workfront].\
En fullständig lista med [!DNL Workfront] kommandon från [!DNL Slack] finns i avsnittet [Åtkomst [!DNL Workfront]  från ett snedstreck i  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) i den här artikeln.

Logga in på [!DNL Workfront] från [!DNL Slack]:

1. Logga in på din [!DNL Slack]-instans.
1. Skriv något av följande kommandon från valfri kanal:\
   `/workfront log in`

   eller

   `/wf log in`

1. Klicka på länken [!DNL Workfront] **[!UICONTROL Log In]** som visas i svaret.\
   En ny flik öppnas med fält för [!DNL Workfront] autentiseringsuppgifter.

1. Följ instruktionerna för att logga in på [!DNL Workfront] med Förbättrad autentisering, OAuth 2.0 eller din SAML-URL (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* När du uppmanas att ange värddatorn för ditt [!DNL Workfront]-konto skriver du den i det här formatet: *ditt företags sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront]-administratör har aktiverat den för den här integreringen.


   Konfigurationssidan för [!DNL Workfront] meddelanden i [!DNL Slack] öppnas.

1. (Valfritt) Inaktivera alla [!DNL Workfront]-meddelanden som du inte vill ta emot i [!DNL Slack].

   Mer information om hur du konfigurerar [!DNL Workfront]-inställningar för [!DNL Slack] finns i avsnittet [Konfigurera inställningar](#configure-settings-configure-settings) i den här artikeln

1. Gå tillbaka till din [!DNL Slack]-kanal.

   Du är inloggad på [!DNL Workfront] från din [!DNL Slack]-instans.

## Åtkomst till [!DNL Workfront] från [!DNL Slack]

* [Om snedstreckskommandon](#about-slash-commands-about-slash-commands)
* [Åtkomst [!DNL Workfront] från en delad länk i [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Åtkomst till [!DNL Workfront] från ett snedstreck i [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om inloggning på [!DNL Workfront] från [!DNL Slack] finns i [Logga in på [!DNL Workfront] från [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront help`

   eller

   `/wf help`

1. Välj bland följande kommandon:

   * `/wf home`

     Visar knappar som du kan använda för att få åtkomst till listor med uppgifter, utgåvor och godkännanden. Om du klickar på någon av knapparna visas de första 20 objekten i varje lista i [!DNL Slack].

     Mer information om hur du hanterar [!DNL Workfront] arbetsobjekt från [!DNL Slack] finns i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Inkludera namnet på aktiviteten så som den kommer att visas i gränssnittet [!DNL Workfront].

     Lägger till en aktivitet i [!DNL Workfront].

     Mer information om hur du lägger till uppgifter i [!DNL Workfront] från Slack finns i avsnittet&quot;Skapa uppgifter från [!DNL Slack]&quot; i [Skapa uppgifter och ärenden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Inkludera namnet på problemet så som det kommer att visas i gränssnittet [!DNL Workfront].

     Lägger till ett problem i [!DNL Workfront]

     Mer information om hur du lägger till problem i [!DNL Workfront] från [!DNL Slack] finns i avsnittet&quot;Skapa problem från [!DNL Slack]&quot; i [Skapa aktiviteter och problem från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Visar listan över dina [!DNL Workfront]-favoriter.

     Mer information om hur du får åtkomst till dina favoriter från [!DNL Slack] finns i avsnittet [Åtkomst till din [!UICONTROL Favorites]-lista från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) i artikeln [Åtkomst till dina favoriter och senaste objekt från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Visar en lista över dina senast använda objekt i [!DNL Workfront].

     Mer information om hur du kommer åt dina senaste objekt från [!DNL Slack] finns i artikeln [Accessing Your [!UICONTROL Recent Items] List from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] and [!UICONTROL recent items from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Visar en lista över dina uppgifter.

     Mer information om hur du hanterar dina uppgifter från [!DNL Slack] finns i avsnittet Hantera dina uppgifter från [!DNL Slack] i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Visar en lista över dina problem.

     Mer information om hur du hanterar dina problem från [!DNL Slack] finns i avsnittet Hantera dina problem från [!DNL Slack] i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Visar dina [!DNL Workfront]-godkännanden.\

     Mer information om hur du hanterar dina godkännanden från [!DNL Slack] finns i avsnittet Hantera dina godkännanden från [!DNL Slack] i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Inkludera nyckelord.

     Sök efter ett specifikt nyckelord. Du kan söka efter följande typobjekt:

      * Projekt
      * Uppgift
      * Problem
      * Rapport
      * Folk
      * Mall
      * Dokument
      * Portfolio
      * Program
      * Kontrollpanel
      * Företag
      * Anteckning \

        Mer information om sökning i [!DNL Slack] finns i [Söka efter [!DNL Adobe Workfront] objekt från Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Loggar in dig på [!DNL Workfront] från [!DNL Slack].

   * `/wf log out`

     Loggar ut dig från [!DNL Workfront] från [!DNL Slack]. Du är fortfarande inloggad på [!DNL Workfront] om du har en separat [!DNL Workfront]-instans öppen på en annan webbläsarflik i ett annat program.
   * `/wf settings`

     Ger dig åtkomst till att konfigurera dina [!DNL Workfront]-inställningar i [!DNL Slack].

     Mer information om hur du konfigurerar [!DNL Workfront]-inställningar i Slack finns i [Konfigurera inställningar](#configure-settings-configure-settings).

   * `/wf help`
Visar en fullständig lista med kommandon för [!DNL Workfront].


   * `Visit Workfront Help`: Öppnar avsnittet [!UICONTROL Slack] på hjälpwebbplatsen för [!DNL Workfront] på en ny webbläsarflik.


1. (Valfritt) Om du vill ta bort meddelandet från ett kommando för du musen över det övre högra hörnet av det Slack-meddelande som innehåller kommandot, klickar på &#x200B;**[!UICONTROL Show message actions]** och sedan på **[!UICONTROL Delete message]**.

1. (Valfritt och villkorligt) Klicka på **[!UICONTROL Delete]** för att bekräfta att du vill ta bort det här meddelandet.

### Åtkomst till [!DNL Workfront] från en delad länk i [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Du kan komma åt [!DNL Workfront] objekt från en länk till de objekt som delas med dig i [!DNL Slack].

Mer information om åtkomst till [!DNL Workfront] från en delad länk finns i [Åtkomst [!DNL Adobe Workfront] till objekt från en delad länk i [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Konfigurera inställningar {#configure-settings}

1. Skriv följande kommando i ett [!DNL Slack]-meddelandefält:

   `/workfront settings`

   eller

   `/wf settings`

   Alla inställningar är aktiverade som standard.

1. Avmarkera något av följande alternativ om du vill inaktivera inställningarna för Workfront:

   * I området **[!UICONTROL General Settings]** inaktiverar du inställningen **[!UICONTROL When pasting a [!DNL Workfront] URL in a [!DNL Slack] channel, show additional description, due date, or requestor name]** &#x200B; om du inte vill att [!DNL Slack] ska lägga till ytterligare information om dina [!DNL Workfront] -objekt när du delar en URL till objektet i [!UICONTROL Slack].

   * I området **[!UICONTROL Notifications Settings]** inaktiverar du meddelanden som du inte längre vill ta emot från Workfront.\

     Mer information om hur du tar emot [!DNL Workfront] meddelanden i [!DNL Slack] finns i [Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Logga ut från [!DNL Workfront] från [!DNL Slack]

1. Skriv följande kommando i ett [!DNL Slack]-meddelandefält:\
   `/workfront log out`\
   `/wf log out`\
   Du får en bekräftelse på att du har loggats ut från [!DNL Workfront].\
   Du är fortfarande inloggad på [!DNL Workfront] om du har en separat [!DNL Workfront]-instans öppen på en annan webbläsarflik i ett annat program.
