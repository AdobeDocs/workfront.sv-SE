---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Konfigurera [!DNL Adobe Workfront] för Slack
description: Integrera [!DNL Adobe Workfront] med Slack kan du komma åt och skapa [!DNL Workfront] arbetsobjekt, godkännanden, favoriter, nyligen använda objekt från Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 09b4644a63241fa9e0a213bfa6f1a7e4264a1703
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# Konfigurera [!DNL Adobe Workfront for Slack]

Integrera [!DNL Adobe Workfront] med [!DNL Slack] gör att du kan göra följande:

* Få åtkomst till dina [!DNL Workfront] arbetsobjekt, godkännanden, favoriter, senaste objekt från [!DNL Slack].
* Prenumerera, godkänn, tilldela arbete från [!DNL Slack].
* Skapa uppgifter och ärenden från [!DNL Slack].
* Ta emot några [!DNL Workfront] meddelanden i [!DNL Slack].

Beroende på hur [!DNL Slack] miljön är konfigurerad kan du installera och konfigurera [!DNL Workfront for Slack] dig själv eller [!DNL Workfront] administratören måste installera och konfigurera den innan du kan konfigurera den själv.

När du integrerar [!DNL Slack] instans med [!DNL Workfront] användare kan använda [!DNL Workfront] när de samarbetar inom [!DNL Slack] kanaler. Integreringen kan användas från alla [!DNL Slack] miljö, inklusive [!DNL Slack] mobilapp.

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

## Krav för att använda [!DNL Workfront] med [!DNL Slack]

* Du måste ha en [!DNL Slack] -instans.
* Dina [!DNL Slack] systemadministratören måste tillåta alla [!DNL Slack] användare att installera [!DNL Workfront for Slack].
* Du måste ha en [!DNL Workfront] som kan använda de integrerade funktionerna i [!DNL Workfront].

   >[!NOTE]
   >
   >Användare med [!DNL Workfront] licenstypen kan komma åt [!DNL Workfront] från [!DNL Slack]. De åtgärder du kan utföra från [!DNL Slack] begränsas till [!DNL Workfront] licens- och behörighetsnivåer.

Mer information om hur du hanterar program i [!DNL Slack], se [Hantera program för din arbetsyta.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installera [!DNL Workfront for Slack]

Varje [!DNL Slack] användaren måste installera [!DNL Workfront] appen i sig för att kunna använda [!DNL Workfront] från [!DNL Slack].

Du kan installera programmet på följande sätt:

* [Installera [!DNL Workfront] app utanför [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installera [!DNL Workfront] app inom [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installera [!DNL Workfront] app utanför [!DNL Slack] {#install-the-workfront-app-outside-slack}

Följ stegen nedan för att köra installationsprocessen och auktorisera [!DNL Workfront for Slack] på [!DNL Slack] -instans.

>[!IMPORTANT]
>
>När en ny version av [!DNL Workfront] för att Slack ska kunna släppas måste du återauktorisera appen för att kunna fortsätta använda den.

1. Leta reda på [!DNL Adobe Workfront] tillägg i [[!DNL Slack] store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Klicka på **[!UICONTROL Open in [!DNL Slack]]**.

1. Logga in på arbetsytan genom att ange [!DNL Slack] URL och klicka **[!UICONTROL Continue]**.\
   ![Screen_Shot_2017-10-17_at_8.27.38_AM.png](assets/screen-shot-2017-10-17-at-8.27.38-am-350x432.png)

1. Undersök åtkomsten som [!DNL Slack] begär. Om du godkänner den här åtkomsten klickar du på **[!UICONTROL Allow Access]** för att godkänna [!DNL Workfront] app.

   ![](assets/integrations-access-screen-350x429.png)

Nu kan du komma åt [!DNL Workfront] från [!DNL Slack], enligt beskrivningen i [Åtkomst [!DNL Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installera [!DNL Workfront] app inom [!DNL Slack] {#install-the-workfront-app-within-slack}

Du kan installera [!DNL Workfront] direkt från [!DNL Slack] program:

1. Navigera till [!DNL Slack] URL.

   Till exempel: *`<YourTeamName>`.slack.com/apps*.

   eller

   Klicka på **[!UICONTROL Add Apps]** ikonen i [!DNL Slack] -instans.

   ![add_apps_in_Slack.png](assets/add-apps-in-slack-350x112.png)

1. Börja skriva *[!DNL Workfront]* i sökfältet.
1. Tryck på Enter.
1. Välj **[!DNL Workfront]** app.
1. Klicka på **[!UICONTROL Settings]**.

   Sidan App Directory visas.

1. Klicka på **[!UICONTROL Visit App Site]**.
1. Klicka på **[!UICONTROL Add to [!DNL Slack]]**.
1. Slutför installationen genom att följa stegen.
1. När installationen är klar får du åtkomst [!DNL Workfront] från [!DNL Slack], enligt beskrivningen i [[!UICONTROL Access [!DNL Workfront] från [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
