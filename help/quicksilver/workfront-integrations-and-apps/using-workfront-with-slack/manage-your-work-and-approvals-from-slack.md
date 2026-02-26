---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Hantera ditt material och godkännanden från Slack
description: Du kan öppna din hemarbetslista, granska och godkänna att arbeta med uppgifter och ärenden samt granska eller fatta beslut om godkännanden direkt från Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: e6f61cdde9e8ad14a9226de4cc61fbcdcb6f839b
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# Hantera ditt arbete och dina godkännanden från [!DNL Slack]

När du har installerat [!DNL Adobe Workfront for Slack] kan du göra följande:

* Åtkomstlistor för dina [!UICONTROL Home]-objekt från [!DNL Slack]
* Granska och godkänn att arbeta med uppgifter och ärenden från [!DNL Slack]
* Granska och fatta beslut om godkännanden från [!DNL Slack]

Mer information om hur du konfigurerar [!DNL Workfront] med [!DNL Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

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

## Förutsättningar

Innan du kan hantera ditt arbete och dina godkännanden från [!DNL Slack] måste du

* Konfigurera [!DNL Workfront for Slack]\
  Instruktioner om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Hantera ditt arbete från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront home`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan starta kommandot med `/wf` i stället för `/workfront`.

   De knappar som du kan använda för att komma åt listor över dina uppgifter, utgåvor och godkännanden visas. Om du klickar på någon av knapparna visas de första 20 objekten i varje lista i [!DNL Slack].

1. (Valfritt) Klicka på **[!UICONTROL Tasks]** om du vill visa alla dina uppgifter.

   Mer information om hur du hanterar uppgifter i [!DNL Slack] finns i [Hantera dina uppgifter från  [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Valfritt) Klicka på **[!UICONTROL Issues]** om du vill visa alla utgåvor.

   Mer information om hur du hanterar problem i [!DNL Slack] finns i [Hantera dina problem från  [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Valfritt) Klicka på **[!UICONTROL Approvals]** om du vill visa alla godkännanden som väntar på ditt beslut.\
   Mer information om hur du hanterar dina godkännanden i [!DNL Slack] finns i [Hantera dina godkännanden från [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Hantera dina uppgifter från [!DNL Slack] {#manage-your-tasks-from-slack}

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home` och klicka sedan på **[!UICONTROL Tasks]**

   eller

   `/workfront tasks`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan starta kommandot med `/wf` i stället för `/workfront`.

   De första 20 uppgifterna i listan visas.

1. Klicka på **[!UICONTROL +`<remaining number>`mer]** om du vill visa ytterligare uppgifter.
1. Titta på följande information om dina arbetsobjekt:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project Name]** eller **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** av arbetsobjektet.
   * **[!DNL Assigned By Name]**: Det här är namnet på den användare som tilldelade uppgiften till dig.
   * **[!UICONTROL Status]**

1. (Valfritt) Klicka på namnet på ett objekt för att öppna det i Workfront på en separat webbläsarflik.
1. (Valfritt) Välj en ny status i fältet **[!UICONTROL Status]**.
1. (Valfritt) Klicka på **[!UICONTROL Log Time]** och välj sedan ett **[!UICONTROL Hour Type]**- och timbelopp för att logga tiden på objektet.

   >[!NOTE]
   >
   >* Du kan bara logga timmar i steg om en hel eller en halvtimme, upp till 12 timmar och 30 minuter.
   >* Timmarna du loggar har ett anmälningsdatum idag. Du kan inte logga tid för ett tidigare eller framtida datum från [!DNL Slack].

   Du får en bekräftelse på att tiden har loggats.

1. (Valfritt) Klicka på **[!UICONTROL Work on it]** om du vill acceptera att arbeta med en uppgift. Knappen [!UICONTROL Work on it] försvinner.

## Hantera dina problem från [!DNL Slack] {#manage-your-issues-from-slack}

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i [Logga in på [!DNL Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home` och klicka sedan på **[!UICONTROL Issues]**

   eller

   `/workfront issues`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan starta kommandot med `/wf` i stället för `/workfront`.

   De första 20 utgåvorna i din listvisning.

1. Klicka på **[!UICONTROL + remaining `<number>`mer]** om du vill visa fler objekt.
1. Titta på följande information om dina arbetsobjekt:

   * **[!UICONTROL Name]**
   * Namn på **[!UICONTROL Project]** eller överordnat objekt
   * **[!UICONTROL Due on]** Datum: Detta är det planerade slutförandedatumet för arbetsobjektet.
   * **[!DNL Requested by]** Namn: Detta är den primära kontakten (för problem) eller användaren som tilldelades (för uppgifter).

1. (Valfritt) Klicka på problemets namn för att öppna det i Workfront på en separat webbläsarflik.
1. (Valfritt) Klicka på **[!DNL Work on it]** för att börja arbeta med problem som du inte har godkänt än.

   Knappen [!UICONTROL Work on it] försvinner.

## Hantera dina godkännanden från [!DNL Slack] {#manage-your-approvals-from-slack}

Godkännanden avser godkännanden av äldre dokument. Enhetliga dokumentgodkännanden stöds för närvarande inte i [!DNL Microsoft Teams]. Mer information om de olika godkännandesystemen i Workfront finns i [Tillgänglig funktion för dokumentgodkännanden](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront home` och klicka sedan på **[!UICONTROL Approvals]**

   eller

   `/workfront approvals`

   >[!NOTE]
   >
   >* Kommandon är skiftlägeskänsliga.
   >* Du kan starta kommandot med `/wf` i stället för `/workfront`.

   De första 20 objekten i din **[!UICONTROL Approvals]**-lista visas. Ytterligare information om objekten visas också, t.ex. namnet på den användare som begärde det eller namnet på det projekt som objektet tillhör.

1. Klicka på **[!UICONTROL + remaining `<number>`mer]** om du vill visa fler objekt.

1. Överväg att hantera godkännanden för följande objekt:

   * **Projekt**

     Klicka på **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** för att acceptera eller ignorera statusändringen för ett projekt.

   * **Uppgifter**

     Klicka på **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** om du vill acceptera eller ignorera statusändringen för en aktivitet.

   * **Problem**

     Klicka på **[!UICONTROL Approve]** eller **[!DNL Reject]** om du vill acceptera eller ignorera statusändringen för ett problem.

   * **Dokument**

     Klicka på **[!UICONTROL Approve]** för att godkänna ett dokument, **[!UICONTROL Reject]** för att avvisa det eller **[!UICONTROL Changes]** för att ange att du godkänner det, men att dokumentet behöver ändras ytterligare.\
     (Valfritt) För musen över dokumentminiatyrbilden för att klicka på förstoringsglaset och förhandsgranska dokumentet.

   * **Korrektur** &#x200B; Klicka på korrekturnamnet för att öppna det i [!DNL Workfront] på en separat flik och hantera godkännandet.
   * **Åtkomstbegäranden**

     Klicka på **[!UICONTROL Grant Access]** om du vill ge utökade behörigheter till det begärda objektet eller på **[!UICONTROL Ignore]** om du vill ignorera begäran om utökad åtkomst.

1. (Valfritt) Klicka på namnet på objektet som skickats för godkännande för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
