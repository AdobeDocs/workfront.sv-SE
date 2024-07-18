---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurera [!DNL Adobe Workfront] för Slack
description: Genom att integrera [!DNL Adobe Workfront]  med Slack kan du få åtkomst till och skapa [!DNL Workfront] arbetsobjekt, godkännanden, favoriter och nyligen använda objekt från Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 1%

---

# Konfigurera [!DNL Adobe Workfront for Slack]

Genom att integrera [!DNL Adobe Workfront] med [!DNL Slack] kan du göra följande:

* Få åtkomst till dina [!DNL Workfront] arbetsobjekt, godkännanden, favoriter, senaste objekt från [!DNL Slack].
* Prenumerera på, godkänn, tilldela arbete från [!DNL Slack].
* Skapa aktiviteter och ärenden från [!DNL Slack].
* Ta emot några [!DNL Workfront] meddelanden i [!DNL Slack].

Beroende på hur din [!DNL Slack]-miljö är konfigurerad kan du installera och konfigurera [!DNL Workfront for Slack] själv, eller så måste [!DNL Workfront] -administratören installera och konfigurera den innan du kan konfigurera den själv.

När du integrerar din [!DNL Slack]-instans med [!DNL Workfront] kan användare använda [!DNL Workfront] när de samarbetar i sina [!DNL Slack]-kanaler. Integrationen kan användas från valfri [!DNL Slack]-miljö, inklusive [!DNL Slack]-mobilappen.

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

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.\

## Krav för att använda [!DNL Workfront] med [!DNL Slack]

* Du måste ha en [!DNL Slack]-instans.
* Systemadministratören för [!DNL Slack] måste tillåta alla [!DNL Slack]-användare att installera [!DNL Workfront for Slack].
* Du måste ha en [!DNL Workfront]-licens för att kunna använda de integrerade funktionerna i [!DNL Workfront].

  >[!NOTE]
  >
  >Användare med en [!DNL Workfront]-licenstyp har åtkomst till [!DNL Workfront] från [!DNL Slack]. De åtgärder du kan utföra från [!DNL Slack] begränsas till din [!DNL Workfront]-licens och dina behörighetsnivåer.

Mer information om hur du hanterar program i [!DNL Slack] finns i [Hantera program för din Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installera [!DNL Workfront for Slack]

Varje [!DNL Slack]-användare måste installera [!DNL Workfront]-appen själv för att kunna använda [!DNL Workfront] från [!DNL Slack].

Du kan installera programmet på följande sätt:

* [Installera  [!DNL Workfront] appen utanför [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installera  [!DNL Workfront] appen i [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installera appen [!DNL Workfront] utanför [!DNL Slack] {#install-the-workfront-app-outside-slack}

Följ stegen nedan för att köra installationsprocessen och auktorisera [!DNL Workfront for Slack] på din [!DNL Slack]-instans.

>[!IMPORTANT]
>
>När en ny version av [!DNL Workfront] för Slack släpps måste du auktorisera appen på nytt för att kunna fortsätta använda den.

1. Leta reda på tillägget [!DNL Adobe Workfront] i [[!DNL Slack] butiken](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klicka på **[!UICONTROL Open in [!DNL Slack]]**.

1. Logga in på arbetsytan genom att ange din [!DNL Slack]-URL och klicka på **[!UICONTROL Continue]**.\

1. Undersök den åtkomst som [!DNL Slack] begär. Om du godkänner den här åtkomsten klickar du på **[!UICONTROL Allow Access]** för att godkänna [!DNL Workfront]-appen.

Du kan nu komma åt [!DNL Workfront] från [!DNL Slack], vilket beskrivs i [Åtkomst [!DNL Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installera appen [!DNL Workfront] i [!DNL Slack] {#install-the-workfront-app-within-slack}

Du kan installera appen [!DNL Workfront] direkt från programmet [!DNL Slack]:

1. Navigera till din [!DNL Slack]-URL.

   Till exempel: *`<YourTeamName>`.slack.com/apps*.

   eller

   Klicka på ikonen **[!UICONTROL Add Apps]** i din [!DNL Slack]-instans.

1. Börja skriva *[!DNL Workfront]* i sökfältet.
1. Tryck på Enter.
1. Välj appen **[!DNL Workfront]**.
1. Klicka på **[!UICONTROL Settings]**.

   Sidan App Directory visas.

1. Klicka på **[!UICONTROL Visit App Site]**.
1. Klicka på **[!UICONTROL Add to [!DNL Slack]]**.
1. Slutför installationen genom att följa stegen.
1. När installationen är klar kan du komma åt [!DNL Workfront] från [!DNL Slack], vilket beskrivs i [[!UICONTROL Access [!DNL Workfront] från [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
