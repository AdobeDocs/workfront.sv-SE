---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]
description: Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

När du har installerat [!DNL Adobe Workfront for Slack]kan du få [!DNL Workfront] meddelanden i [!DNL Slack].\
Mer information om installation [!DNL Workfront for Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Du kan aktivera ett visst antal [!UICONTROL notifications] som visas i meddelandebubblan i [!DNL Workfront] -gränssnitt, som också ska levereras i [!DNL Slack].

E-postmeddelanden fungerar oberoende av [!DNL Workfront] gränssnittsmeddelanden. Du eller [!DNL Workfront] administratören kan inaktivera e-postmeddelanden, medan gränssnittsmeddelanden inte kan inaktiveras i [!DNL Workfront].\
Du kan dock inaktivera [!DNL Workfront] meddelanden som du kan få i [!DNL Slack]om du bara vill fokusera på meddelandena i [!DNL Workfront] gränssnitt.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.\

## Förutsättningar

Innan du kan ta emot [!DNL Workfront] meddelanden i [!DNL Slack]måste du

* Konfigurera [!DNL Workfront for Slack]\
   Instruktioner om konfigurering [!DNL Workfront for Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Konfigurera [!DNL Workfront] meddelanden om [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Villkorligt) Efter [!DNL Workfront] har lagts till i [!DNL Slack] instans, logga in [!DNL Workfront] från [!DNL Slack].\
   Mer information om inloggning [!DNL Workfront] från [!DNL Slack], se [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront settings`

   eller

   `/wf settings`

1. Alla meddelanden är aktiverade som standard.\
   Inaktivera något av följande meddelanden:

   * [!UICONTROL I'm assigned to a new task or issue]
   * [!UICONTROL My team is assigned to a new task or issue]
   * [!UICONTROL I receive a new approval or access request]
   * [!UICONTROL Someone includes me on a directed update]
   * [!UICONTROL Someone comments on a thread I'm in]
   * [!UICONTROL An update is made to a task, issue or project I am subscribed to]
   * [!UICONTROL Someone comments on one of my work items]
   * [!UICONTROL Someone comments on my help request]

   De ändringar du gör i [!UICONTROL notifications] aktiveras omedelbart.\
   De meddelanden du har aktiverat visas i [!DNL Workfront] [!DNL Slack] kanal. När du inaktiverar meddelanden här inaktiveras de bara för [!DNL Slack]och inte för [!DNL Workfront] gränssnitt. Du får dem även i fortsättningen i [!DNL Workfront] meddelanden bubblar i det övre högra hörnet av gränssnittet.

## Hantera [!DNL Workfront] meddelanden från [!DNL Slack]

Du kan ta emot och svara på [!DNL Workfront] meddelanden från [!DNL Slack].

Du kan inaktivera e-postmeddelanden för meddelanden som du aktiverar i [!DNL Slack], för att vara säker på att du inte får dubbla meddelanden.\
Mer information om hur du konfigurerar e-postmeddelanden finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Aktivera eller inaktivera [!DNL Workfront] meddelanden i [!DNL Slack] påverkar inte meddelanden som du får i dialogrutan [!DNL Workfront] gränssnitt.\
Meddelanden inuti [!DNL Workfront] gränssnittet kan inte inaktiveras.

Hantera dina [!DNL Workfront] meddelanden om [!DNL Slack]:

1. Logga in på [!UICONTROL Slack].
1. Logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Se till att [!DNL Workfront] meddelanden om [!DNL Slack] är aktiverade.\
   Mer information om [!DNL Workfront] meddelanden kan konfigureras att även skickas till [!DNL Slack], se [Konfigurera [!DNL Workfront] meddelanden om [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Gå till **[!DNL Workfront]** för att hitta [!DNL Workfront] meddelanden.
1. (Villkorligt och valfritt) Gör något av följande:

   * Klicka **[!UICONTROL Work on it]** för att acceptera att arbeta med en uppgift.

   * (Villkorligt och valfritt) Klicka **[!UICONTROL Reply in [!DNL Workfront]]** om du vill svara på en kommentar skriver du ditt svar och klickar på **[!UICONTROL Reply]**.

   * (Villkorligt och valfritt) Klicka **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** för att godkänna eller avvisa en aktivitet, ett problem eller ett projekt som väntar på ditt godkännande.

   * (Villkorligt och valfritt) Klicka **[!UICONTROL Approve]**, **[!UICONTROL Changes]**, eller **[!UICONTROL Reject]**, för att godkänna, godkänna med ändringar eller avvisa ett dokument.

      Du kan också föra musen över dokumentets miniatyrbild och klicka på förstoringsglaset för att visa en större förhandsvisning av dokumentet innan du godkänner det.\
      Endast godkänd Slack [filtyper](https://api.slack.com/types/file) kan förhandsgranskas.

   * (Villkorligt och valfritt) Klicka **[!UICONTROL Grant]** eller **[!UICONTROL Ignore]** för att bevilja eller ignorera begäran om mer åtkomst från en annan användare.\

      Du får en bekräftelse på att åtgärden har slutförts i [!DNL Workfront]för varje beslut du fattar i dina meddelanden.
