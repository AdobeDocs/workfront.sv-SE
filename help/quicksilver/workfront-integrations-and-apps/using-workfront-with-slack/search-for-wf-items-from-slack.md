---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Sök efter [!DNL Adobe Workfront] objekt från [!DNL Slack]
description: Du kan söka efter [!DNL Adobe Workfront] objekt från [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] app installerad.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Sök efter [!DNL Adobe Workfront] objekt från [!DNL Slack]

Du kan söka efter [!DNL Adobe Workfront] objekt från [!DNL Slack]om din instans av [!DNL Slack] har haft [!DNL Workfront] app installerad.

Mer information om konfiguration [!DNL Workfront] med [!DNL Slack], se [Konfigurera [!DNL Adobe Workfront] for [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

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

Innan du kan söka efter [!DNL Workfront] objekt från [!DNL Slack]måste du

* Konfigurera [!DNL Workfront] for [!DNL Slack]\
   Instruktioner om konfigurering [!DNL Workfront for Slack], se [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Sök efter [!DNL Workfront] objekt från [!DNL Slack]:

1. Logga in på [!DNL Slack] instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack], se&quot;Logga in på [!DNL Workfront] från [!DNL Slack]&quot; i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront search <keyword>`

   eller

   `/wf search <keyword>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Nyckelordet är inte skiftlägeskänsligt och måste anges utan hakparenteser eller citattecken.\
   >![slack_search_result_select_object_box.png](assets/slack-search-result-select-object-box-350x30.png)   >

1. I fältet som visas väljer du en objekttyp bland följande:

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
   * Anteckning

      Du kan bara markera en objekttyp åt gången.\
      En lista med objekt som matchar sökvillkoren visas.

1. Klicka på namnet på ett objekt för att öppna det i [!DNL Workfront] på en ny flik i webbläsaren.
