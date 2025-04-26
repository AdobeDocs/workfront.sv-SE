---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Sök efter [!DNL Adobe Workfront] objekt från [!DNL Slack]
description: Du kan söka efter [!DNL Adobe Workfront] objekt från [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] appen som är installerad.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Sök efter [!DNL Adobe Workfront] objekt från [!DNL Slack]

Du kan söka efter [!DNL Adobe Workfront] objekt från [!DNL Slack] om appen [!DNL Workfront] har installerats på din instans av [!DNL Slack].

Mer information om hur du konfigurerar [!DNL Workfront] med [!DNL Slack] finns i [Konfigurera [!DNL Adobe Workfront] för [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.\

## Förutsättningar

Innan du kan söka efter [!DNL Workfront] objekt från [!DNL Slack] måste du

* Konfigurera [!DNL Workfront] för [!DNL Slack]\
   Instruktioner om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Sök efter [!DNL Workfront] objekt från [!DNL Slack]:

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].\
   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Börja skriva något av följande kommandon i meddelandefältet från valfri kanal:

   `/workfront search <keyword>`

   eller

   `/wf search <keyword>`

   >[!NOTE]
   >
   >Kommandon är skiftlägeskänsliga. Nyckelordet är inte skiftlägeskänsligt och måste anges utan hakparenteser eller citattecken.

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

1. Klicka på namnet på ett objekt för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
