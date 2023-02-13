---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Skapa uppgifter och ärenden från Slack
description: När du har installerat och konfigurerat [!DNL Adobe Workfront] för Slack kan du skapa uppgifter och ärenden från Slack och associera dem med projekt i Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Skapa uppgifter och ärenden från [!DNL Slack]

När du har installerat och konfigurerat [!DNL Adobe Workfront for Slack]kan du skapa uppgifter och ärenden från [!DNL Slack] och associera dem med projekt i [!DNL Workfront].

Mer information om konfiguration [!DNL Workfront] med [!DNL Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Du måste ha åtkomst till att skapa uppgifter och problem på din åtkomstnivå och du måste ha [!UICONTROL Contribute] behörigheter för det projekt som du associerar dem med.

Mer information om åtkomstnivåer finns i [Översikt över åtkomstnivåer](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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

Innan du kan skapa uppgifter och ärenden från [!DNL Slack]måste du

* Konfigurera [!DNL Workfront] för Slack\
   Instruktioner om konfigurering [!DNL Workfront for Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Skapa uppgifter från [!DNL Slack]

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på Workfront från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Du kan börja ditt kommando med `/wf` i stället för `/workfront`.
   >  
   >Uppgiftsnamnet måste anges så som det kommer att visas i [!DNL Workfront] utan hakparenteser eller citattecken.\
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)

1. (Valfritt) Börja skriva namnet på ett projekt som du vill associera den nya uppgiften med och markera den när den visas i listan.\
   Du får en bekräftelse som anger att uppgiften har lagts till i det valda projektet.
1. (Valfritt) Klicka på uppgiftens namn i bekräftelsemeddelandet för att öppna den i [!DNL Workfront], på en ny flik i webbläsaren.

## Skapa problem från [!DNL Slack]

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Du kan starta kommandot med &#39;/wf&#39; i stället för &#39;/workfront&#39;. \
   >Du måste ange problemnamnet så som det kommer att visas i dialogrutan [!DNL Workfront] utan hakparenteser eller citattecken.\
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)

1. (Valfritt) Börja skriva namnet på ett projekt som du vill associera det nya problemet med och markera det när det visas i listan.\
   Du får en bekräftelse som anger att problemet har lagts till i det valda projektet.
1. (Valfritt) Klicka på namnet på problemet i bekräftelsemeddelandet för att öppna det i [!DNL Workfront], på en ny flik i webbläsaren.
