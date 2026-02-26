---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]
description: Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: e6f61cdde9e8ad14a9226de4cc61fbcdcb6f839b
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Ta emot [!DNL Adobe Workfront] meddelanden i [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

När du har installerat [!DNL Adobe Workfront for Slack] kan du få [!DNL Workfront] meddelanden i [!DNL Slack].\
Mer information om hur du installerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Du kan aktivera ett visst antal [!UICONTROL notifications] som visas i meddelandebubblan i [!DNL Workfront] -gränssnittet och som också ska levereras i [!DNL Slack].

E-postmeddelanden fungerar oberoende av [!DNL Workfront]-gränssnittsmeddelanden. Du eller din [!DNL Workfront]-administratör kan inaktivera e-postmeddelanden, medan gränssnittsmeddelanden inte kan inaktiveras i [!DNL Workfront].\
Du kan dock inaktivera [!DNL Workfront]-meddelanden som du kan ta emot i [!DNL Slack] om du bara vill fokusera på dessa meddelanden inuti [!DNL Workfront]-gränssnittet.

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

Innan du kan ta emot [!DNL Workfront] meddelanden i [!DNL Slack] måste du

* Konfigurera [!DNL Workfront for Slack]\
   Instruktioner om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Konfigurera [!DNL Workfront] meddelanden för [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Villkorligt) När [!DNL Workfront] har lagts till i din [!DNL Slack]-instans loggar du in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om inloggning på [!DNL Workfront] från [!DNL Slack] finns i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront settings`

   eller

   `/wf settings`

1. Alla meddelanden är aktiverade som standard.\
   Inaktivera något av följande meddelanden:

   * [!UICONTROL I'm assigned to a new task or issue]
   * [!UICONTROL My team is assigned to a new task or issue]
   * [!UICONTROL I receive a new approval or access request]

     >[!NOTE]
     >
     >Godkännanden avser godkännanden av äldre dokument. Enhetliga dokumentgodkännanden stöds för närvarande inte i [!DNL Slack]. Mer information om de olika godkännandesystemen i Workfront finns i [Tillgänglig funktion för dokumentgodkännanden](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).


   * [!UICONTROL Someone includes me on a directed update]
   * [!UICONTROL Someone comments on a thread I'm in]
   * [!UICONTROL An update is made to a task, issue or project I am subscribed to]
   * [!UICONTROL Someone comments on one of my work items]
   * [!UICONTROL Someone comments on my help request]

   De ändringar du gör i alternativen för [!UICONTROL notifications] börjar gälla omedelbart.\
   De meddelanden du har aktiverat levereras i [!DNL Workfront] [!DNL Slack]-kanalen. När du inaktiverar meddelanden här inaktiveras de bara för [!DNL Slack], inte för gränssnittet [!DNL Workfront]. Du fortsätter att ta emot dem i meddelandebubblan [!DNL Workfront] i det övre högra hörnet av gränssnittet.

## Hantera [!DNL Workfront] meddelanden från [!DNL Slack]

Du kan ta emot och svara på [!DNL Workfront] meddelanden från [!DNL Slack].

Du kan inaktivera e-postmeddelanden för meddelanden som du aktiverar i [!DNL Slack], så att du inte får dubbla meddelanden.\
Mer information om hur du konfigurerar e-postmeddelanden finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Om du aktiverar eller inaktiverar [!DNL Workfront] meddelanden i [!DNL Slack] påverkas inte de meddelanden du får i gränssnittet [!DNL Workfront].\
Meddelanden i gränssnittet [!DNL Workfront] kan inte inaktiveras.

Så här hanterar du [!DNL Workfront]-meddelanden för [!DNL Slack]:

1. Logga in på [!UICONTROL Slack].
1. Logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Kontrollera att dina [!DNL Workfront]-meddelanden för [!DNL Slack] är aktiverade.\
   Mer information om vilka [!DNL Workfront]-meddelanden som kan konfigureras att även skickas till [!DNL Slack] finns i [Konfigurera [!DNL Workfront] meddelanden för [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Gå till **[!DNL Workfront]**-kanalen för att hitta dina [!DNL Workfront]-meddelanden.
1. (Villkorligt och valfritt) Gör något av följande:

   * Klicka på **[!UICONTROL Work on it]** om du vill acceptera att arbeta med en uppgift.

   * (Villkorligt och valfritt) Klicka på **[!UICONTROL Reply in [!DNL Workfront]]** om du vill svara på en kommentar, skriva ditt svar och klicka på **[!UICONTROL Reply]**.

   * (Villkorligt och valfritt) Klicka på **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** för att godkänna eller avvisa en aktivitet, ett problem eller ett projekt som väntar på ditt godkännande.

   * (Villkorligt och valfritt) Klicka på **[!UICONTROL Approve]**, **[!UICONTROL Changes]** eller **[!UICONTROL Reject]** om du vill godkänna, godkänna med ändringar eller avvisa ett dokument.

     Du kan också föra musen över dokumentets miniatyrbild och klicka på förstoringsglaset för att visa en större förhandsvisning av dokumentet innan du godkänner det.\
      Endast de godkända Slack [filtyperna](https://api.slack.com/types/file) kan förhandsgranskas.

   * (Villkorligt och valfritt) Klicka på **[!UICONTROL Grant]** eller **[!UICONTROL Ignore]** för att bevilja eller ignorera begäran om mer åtkomst från en annan användare.\

     Du får en bekräftelse på att din åtgärd har slutförts i [!DNL Workfront] för varje beslut du fattar i dina meddelanden.
