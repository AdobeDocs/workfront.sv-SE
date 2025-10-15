---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Skapa uppgifter och ärenden från Slack
description: När du har installerat och konfigurerat  [!DNL Adobe Workfront]  för Slack kan du skapa uppgifter och problem från Slack och associera dem med projekt i Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Skapa aktiviteter och ärenden från [!DNL Slack]

När du har installerat och konfigurerat [!DNL Adobe Workfront for Slack] kan du skapa uppgifter och problem från [!DNL Slack] och associera dem med projekt i [!DNL Workfront].

Mer information om hur du konfigurerar [!DNL Workfront] med [!DNL Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Du måste ha åtkomst för att skapa aktiviteter och problem på din åtkomstnivå och du måste ha [!UICONTROL Contribute] behörigheter för det projekt som du associerar dem med.

Mer information om åtkomstnivåer finns i [Översikt över åtkomstnivåer](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Mer information om behörigheter för objekt finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/se/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.\

## Förutsättningar

Innan du kan skapa aktiviteter och ärenden från [!DNL Slack] måste du

* Konfigurera [!DNL Workfront] för Slack\
   Instruktioner om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Skapa aktiviteter från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på Workfront från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Du kan starta kommandot med `/wf` i stället för `/workfront`.
   >  
   >Uppgiftsnamnet måste anges så som det kommer att visas i gränssnittet [!DNL Workfront], utan hakparenteser eller citattecken.

1. (Valfritt) Börja skriva namnet på ett projekt som du vill associera den nya uppgiften med och markera den när den visas i listan.\
   Du får en bekräftelse som anger att uppgiften har lagts till i det valda projektet.
1. (Valfritt) Klicka på uppgiftens namn i bekräftelsemeddelandet för att öppna den i [!DNL Workfront] på en ny webbläsarflik.

## Skapa problem från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva följande kommando i meddelandefältet från valfri kanal:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Du kan starta kommandot med &#39;/wf&#39; i stället för &#39;/workfront&#39;. \
   >Problemnamnet måste anges så som det kommer att visas i gränssnittet [!DNL Workfront], utan hakparenteser eller citattecken.

1. (Valfritt) Börja skriva namnet på ett projekt som du vill associera det nya problemet med och markera det när det visas i listan.\
   Du får en bekräftelse som anger att problemet har lagts till i det valda projektet.
1. (Valfritt) Klicka på namnet på problemet i bekräftelsemeddelandet för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
