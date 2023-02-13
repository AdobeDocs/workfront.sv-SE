---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]
description: Integrera [!DNL Adobe Workfront] med [!DNL Slack] ger dig åtkomst [!DNL Workfront] från Slack, eller utföra vissa åtgärder i [!DNL Workfront] med ett snedstreck. Integreringen kan användas från alla [!DNL Slack] miljö, inklusive [!DNL Slack] mobilapp.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%

---

# Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]

Integrera [!DNL Adobe Workfront] med [!DNL Slack] ger dig åtkomst [!DNL Workfront] från [!DNL Slack]eller utför vissa åtgärder i [!DNL Workfront] med ett snedstreck. Integreringen kan användas från alla [!DNL Slack] miljö, inklusive [!DNL Slack] mobilapp.

Du eller [!DNL Slack] administratören måste installera [!DNL Workfront] i din [!DNL Slack] innan du kan använda [!DNL Workfront] från [!DNL Slack]. Mer information finns i [Konfigurera Adobe Workfront för Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Om snedstreckskommandon {#about-slash-commands}

När du använder [!DNL Slack]skriver du meddelanden i ett meddelandefält. När du börjar ett meddelande med ett snedstreck blir det ett kommando och fungerar annorlunda än ett enkelt meddelande. Kommandot anger [!DNL Slack] för att utföra en åtgärd.

Du kan komma åt [!DNL Workfront] instans från [!DNL Slack] genom att skriva ett snedstreck [!DNL Slack] kanal.

Kom ihåg följande när du använder ett snedstreck i [!DNL Slack] för åtkomst [!DNL Workfront]:

* Snedstreckskommandon är skiftlägeskänsliga.
* Kommandona för [!DNL Workfront] är bara synliga för dig, oavsett vilken kanal du skriver in dem i.
* Kommandot ska alltid börja med `/workfront` eller `/wf`, följt av ett mellanslag och namnet på en åtgärd som du vill utföra i [!DNL Workfront].

   Detta anger att kommandot är avsett för [!DNL Workfront] app. Kommandona för [!DNL Workfront] fungerar bara när du redan har konfigurerat [!DNL Workfront] appen med [!DNL Slack] -instans.

En lista över alla kommandon som du kan köra från Slack för [!DNL Workfront], se [Åtkomst [!DNL Workfront] från ett snedstreck [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Logga in på [!DNL Workfront] från [!DNL Slack] {#log-in-to-workfront-from-slack}

När du skriver ett kommando i meddelandefältet i Slack blir du ombedd att logga in på [!DNL Workfront] först.\
En fullständig lista över [!DNL Workfront] kommandon från [!DNL Slack], se [Åtkomst [!DNL Workfront] från ett snedstreck [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) i den här artikeln.

Logga in på [!DNL Workfront] från [!DNL Slack]:

1. Logga in på [!DNL Slack] -instans.
1. Skriv något av följande kommandon från valfri kanal:\
   `/workfront log in`

   eller

   `/wf log in`

1. Klicka på [!DNL Workfront] **[!UICONTROL Log In]** länk som visas i svaret.\
   En ny flik öppnas med fält för [!DNL Workfront] autentiseringsuppgifter.

1. Följ instruktionerna för att logga in på [!DNL Workfront] med Förbättrad autentisering, OAuth 2.0 eller en SAML-URL (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* När du uppmanas att ange värddatorn för din [!DNL Workfront] konto, skriv in det i följande format: *ditt företag&#39;sDomain.my.workfront.com*. Företagets domän är vanligtvis namnet på ditt företag.
   >* Förbättrad autentisering är inte tillgängligt förrän en [!DNL Workfront] administratören aktiverar det för den här integreringen.



   Konfigurationssidan för [!DNL Workfront] meddelanden i [!DNL Slack] öppnas.

1. (Valfritt) Inaktivera [!DNL Workfront] meddelanden som du inte vill ta emot i [!DNL Slack].

   Mer information om konfiguration [!DNL Workfront] inställningar för [!DNL Slack], se [Konfigurera inställningar](#configure-settings-configure-settings) avsnitt i den här artikeln

1. Navigera tillbaka till [!DNL Slack] kanal.

   Du är inloggad på [!DNL Workfront] från [!DNL Slack] -instans.

## Åtkomst [!DNL Workfront] från [!DNL Slack]

* [Om snedstreckskommandon](#about-slash-commands-about-slash-commands)
* [Åtkomst [!DNL Workfront] från en delad länk i [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Åtkomst [!DNL Workfront] från ett snedstreck [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se [Logga in på [!DNL Workfront] från [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront help`

   eller

   `/wf help`

1. Välj bland följande kommandon:

   * `/wf home`

      Visar knappar som du kan använda för att få åtkomst till listor med uppgifter, utgåvor och godkännanden. Om du klickar på någon av knapparna visas de första 20 objekten i varje lista i [!DNL Slack].

      ![](assets/slack-home-buttons-350x80.png)

      Mer information om hur du hanterar [!DNL Workfront] arbetsobjekt från [!DNL Slack], se [Hantera ditt arbete och godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Inkludera namnet på uppgiften så som den kommer att visas i [!DNL Workfront] gränssnitt.

      Lägger till en uppgift i [!DNL Workfront].

      Mer information om hur du lägger till uppgifter i [!DNL Workfront] från Slack, se&quot;Skapa uppgifter från [!DNL Slack]&quot; i [Skapa uppgifter och ärenden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Inkludera namnet på utgåvan så som det kommer att visas i [!DNL Workfront] gränssnitt.

      Lägger till en utgåva i [!DNL Workfront]

      Mer information om hur du lägger till problem i [!DNL Workfront] från [!DNL Slack], se&quot;Skapa problem från [!DNL Slack]&quot; i [Skapa uppgifter och ärenden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Visar en lista över [!DNL Workfront] Favoriter.

      Mer information om hur du får åtkomst till dina favoriter från [!DNL Slack], se [Åtkomst till [!UICONTROL Favorites] Lista från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) i [Åtkomst till dina favoriter och senaste objekt från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `/wf recent`

      Visar en lista över de senast använda objekten i [!DNL Workfront].

      Mer information om hur du får åtkomst till dina senaste objekt från [!DNL Slack], se [Åtkomst till [!UICONTROL Recent Items] Lista från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] och [!UICONTROL recent items from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `wf tasks`

      Visar en lista över dina uppgifter.

      Mer information om hur du hanterar uppgifter från [!DNL Slack], se&quot;Hantera dina uppgifter från [!DNL Slack]&quot; i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Visar en lista över dina problem.

      Mer information om hur du hanterar problem från [!DNL Slack], se&quot;Hantera dina problem från [!DNL Slack]&quot; i [Hantera ditt arbete och dina godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Visar dina [!DNL Workfront] godkännanden.\

      Mer information om hur du hanterar godkännanden från [!DNL Slack], se&quot;Hantera dina godkännanden från [!DNL Slack]&quot; i [Hantera ditt arbete och godkännanden från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

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

         Mer information om sökning i [!DNL Slack], se [Sök efter [!DNL Adobe Workfront] objekt från Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Loggar in dig på [!DNL Workfront] från [!DNL Slack].

   * `/wf log out `

      Loggar ut dig från [!DNL Workfront] från [!DNL Slack]. Du förblir inloggad på [!DNL Workfront] om du har ett separat [!DNL Workfront] -instansen öppnas i en annan webbläsarflik i ett annat program.
   * `/wf settings`

      Ger dig åtkomst att konfigurera [!DNL Workfront] inställningar i [!DNL Slack].

      Mer information om konfiguration [!DNL Workfront] inställningar i Slack, se [Konfigurera inställningar](#configure-settings-configure-settings).

   * `/wf help`
Visar en fullständig lista med kommandon för [!DNL Workfront].


   * `Visit Workfront Help`: Öppnar [!UICONTROL Slack] i [!DNL Workfront] Hjälpwebbplats på en ny flik i webbläsaren.


1. (Valfritt) Om du vill ta bort ett kommando för du musen över det övre högra hörnet av det Slack-meddelande som innehåller kommandot och klickar på &#x200B;**[!UICONTROL Show message actions]** och sedan klicka **[!UICONTROL Delete message]**.

1. (Valfritt och villkorligt) Klicka på **[!UICONTROL Delete]** för att bekräfta att du vill ta bort det här meddelandet.

### Åtkomst [!DNL Workfront] från en delad länk i [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Du kan komma åt [!DNL Workfront] objekt från en länk till de objekt som delas med dig i [!DNL Slack].

Mer information om åtkomst [!DNL Workfront] från en delad länk, se [Åtkomst [!DNL Adobe Workfront] objekt från en delad länk i [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Konfigurera inställningar {#configure-settings}

1. Innanför en [!DNL Slack] meddelandefält, skriv följande kommando:

   `/workfront settings`

   eller

   `/wf settings`

   ![](assets/slack-configuring-settings-350x302.png)

   Alla inställningar är aktiverade som standard.

1. Avmarkera något av följande alternativ om du vill inaktivera inställningarna för Workfront:

   * I **[!UICONTROL General Settings]** område, inaktivera **[!UICONTROL When pasting a [!DNL Workfront] URL in a [!DNL Slack] channel, show additional description, due date, or requestor name]**&#x200B; om du inte vill [!DNL Slack] om du vill lägga till ytterligare information om [!DNL Workfront] objekt när du delar en URL till objektet i [!UICONTROL Slack].

   * I **[!UICONTROL Notifications Settings]** kan du inaktivera meddelanden som du inte längre vill ta emot från Workfront.\

      För information om mottagande [!DNL Workfront] meddelanden i [!DNL Slack], se [Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Logga ut från [!DNL Workfront] från [!DNL Slack]

1. Innanför en [!DNL Slack] meddelandefält, skriv följande kommando:\
   `/workfront log out` eller\
   `/wf log out`\
   Du får en bekräftelse på att du har loggats ut från [!DNL Workfront].\
   Du förblir inloggad på [!DNL Workfront] om du har ett separat [!DNL Workfront] -instansen öppnas i en annan webbläsarflik i ett annat program.
