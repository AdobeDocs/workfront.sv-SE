---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Hantera ditt arbete och godkännanden från Slack
description: Du kan komma åt din hemarbetslista, granska och godkänna att arbeta med uppgifter och ärenden samt granska eller fatta beslut om godkännanden direkt från Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Hantera ditt arbete och godkännanden från [!DNL Slack]

När du har installerat [!DNL Adobe Workfront for Slack]kan du göra följande:

* Åtkomstlistor till [!UICONTROL Home] objekt från [!DNL Slack]
* Granska och acceptera att arbeta med uppgifter och ärenden från [!DNL Slack]
* Granska och fatta beslut om godkännanden från [!DNL Slack]

Mer information om konfiguration [!DNL Workfront] med [!DNL Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan hantera ditt arbete och dina godkännanden från [!DNL Slack]måste du

* Konfigurera [!DNL Workfront for Slack]\
   Instruktioner om konfigurering [!DNL Workfront for Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Hantera ditt arbete från [!DNL Slack]

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront home`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan börja ditt kommando med `/wf` i stället för `/workfront`.


   De knappar som du kan använda för att komma åt listor över dina uppgifter, utgåvor och godkännanden visas. Om du klickar på någon av knapparna visas de första 20 objekten i varje lista i [!DNL Slack].

1. (Valfritt) Klicka på **[!UICONTROL Tasks]** för att visa alla dina uppgifter.

   Mer information om hur du hanterar uppgifter i [!DNL Slack], se [Hantera dina uppgifter från [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Valfritt) Klicka på **[!UICONTROL Issues]** för att visa alla dina problem.

   Mer information om hur du hanterar problem i [!DNL Slack], se [Hantera dina problem från [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Valfritt) Klicka på **[!UICONTROL Approvals]** för att visa alla godkännanden som väntar på ditt beslut.\
   Mer information om hur du hanterar godkännanden i [!DNL Slack], se [Hantera era godkännanden från [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Hantera dina uppgifter från [!DNL Slack] {#manage-your-tasks-from-slack}

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home`och sedan klicka **[!UICONTROL Tasks]**

   eller

   `/workfront tasks`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan börja ditt kommando med `/wf` i stället för `/workfront`.


   De första 20 uppgifterna i listan visas.

1. Klicka **[!UICONTROL +`<remaining number>`mer]** om du vill visa ytterligare uppgifter.
1. Titta på följande information om dina arbetsobjekt:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project Name]** eller **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** av arbetsuppgiften.
   * **[!DNL Assigned By Name]**: det här är namnet på den användare som tilldelade uppgiften till dig.
   * **[!UICONTROL Status]**

1. (Valfritt) Klicka på namnet på ett objekt för att öppna det i Workfront på en separat webbläsarflik.
1. (Valfritt) I dialogrutan **[!UICONTROL Status]** väljer du en ny status.
1. (Valfritt) Klicka på **[!UICONTROL Log Time]** väljer du en **[!UICONTROL Hour Type]** och ett timbelopp för att logga tiden på artikeln.

   >[!NOTE]
   >
   >* Du kan bara logga timmar i steg om en hel eller en halvtimme, upp till 12 timmar och 30 minuter.
   >* Timmarna du loggar har ett anmälningsdatum idag. Du kan inte logga tid för ett tidigare eller framtida datum från [!DNL Slack].


   Du får en bekräftelse på att tiden har loggats.

1. (Valfritt) Klicka på **[!UICONTROL Work on it]** för att acceptera att arbeta med en uppgift. The [!UICONTROL Work on it] försvinner.

## Hantera dina problem från [!DNL Slack] {#manage-your-issues-from-slack}

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se [Loggar in på [!DNL Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home`och sedan klicka **[!UICONTROL Issues]**

   eller

   `/workfront issues`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan börja ditt kommando med `/wf` i stället för `/workfront`.


   De första 20 utgåvorna i din listvisning.

1. Klicka **[!UICONTROL + remaining `<number>`mer]** om du vill visa ytterligare objekt.
1. Titta på följande information om dina arbetsobjekt:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project]** Namn eller namn på överordnat objekt
   * **[!UICONTROL Due on]** Datum: Det här är det planerade slutförandedatumet för arbetsobjektet.
   * **[!DNL Requested by]** Namn: Det här är den primära kontakten (för problem) eller användaren som tilldelade (för uppgifter).

1. (Valfritt) Klicka på problemets namn för att öppna det i Workfront på en separat webbläsarflik.
1. (Valfritt) Klicka på **[!DNL Work on it]** för att börja arbeta med frågor som du inte har godkänt än.

   The [!UICONTROL Work on it] försvinner.

## Hantera era godkännanden från [!DNL Slack] {#manage-your-approvals-from-slack}

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home`och sedan klicka **[!UICONTROL Approvals]**

   eller

   `/workfront approvals`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan börja ditt kommando med `/wf` i stället för `/workfront`.


   De första 20 objekten på **[!UICONTROL Approvals]** listvisning. Ytterligare information om objekten visas också, t.ex. namnet på den användare som begärde det eller namnet på det projekt som objektet tillhör.

1. Klicka **[!UICONTROL + remaining `<number>`mer]** om du vill visa ytterligare objekt.

1. Överväg att hantera godkännanden för följande objekt:

   * **Projekt**

      Klicka **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** om du vill acceptera eller ignorera statusändringen för ett projekt.

   * **Uppgifter**

      Klicka **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** om du vill acceptera eller ignorera statusändringen för en uppgift.

   * **Problem**

      Klicka **[!UICONTROL Approve]** eller **[!DNL Reject]** om du vill acceptera eller ignorera statusändringen för ett problem.

   * **Dokument**

      Klicka **[!UICONTROL Approve]** för att godkänna ett dokument, **[!UICONTROL Reject]** för att avvisa det, eller **[!UICONTROL Changes]** för att ange att du godkänner det, men att dokumentet behöver ändras ytterligare.\
      (Valfritt) För musen över dokumentminiatyrbilden för att klicka på förstoringsglaset och förhandsgranska dokumentet.

   * **Korrektur**&#x200B; Klicka på korrekturnamnet för att öppna det i [!DNL Workfront] på en separat flik och hantera godkännandet.
   * **Åtkomstbegäranden**

      Klicka **[!UICONTROL Grant Access]** för att ge utökade behörigheter till det begärda objektet, eller **[!UICONTROL Ignore]** för att ignorera begäran om mer åtkomst.

1. (Valfritt) Klicka på namnet på objektet som skickats för godkännande för att öppna det i [!DNL Workfront] på en ny flik i webbläsaren.
