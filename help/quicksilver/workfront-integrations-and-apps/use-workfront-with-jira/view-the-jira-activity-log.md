---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visa aktivitetsloggen för Jira
description: Som  [!DNL Jira] administratör kan du visa de undantag och fel som inträffar under synkroniseringen eller skapandet av biljetterna mellan [!DNL Adobe Workfront] och [!DNL Jira] i en aktivitetslogg.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 1%

---

# Visa [!UICONTROL [!DNL Jira] Activity Log]

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen kommer integreringen av Workfront för Jira inte att vara tillgänglig efter **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Jira.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration Module för Jira finns i [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Som [!DNL Jira]-administratör kan du visa de undantag och fel som inträffar under synkroniseringen eller skapandet av biljetterna mellan [!DNL Adobe Workfront] och [!DNL Jira] i en [!UICONTROL Activity Log].

Du kan se upp till 500 objekt i aktivitetsloggen, och de listas med början från de senaste.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira-åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt: Vi rekommenderar att du skapar separata systemadministratörskonton i Jira och Workfront för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira] måste du

* Installera [!DNL Workfront for Jira]

  Instruktioner om hur du installerar [!DNL Workfront for Jira] finns i [Installera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Öppna [!UICONTROL [!DNL Jira] Activity Log]:

1. Logga in på Jira som systemadministratör.
1. Klicka på **[!UICONTROL Settings]** i huvudmenyn för [!DNL Jira].
1. Klicka på **[!UICONTROL Add-ons]** och sedan på **[!UICONTROL Manage add-ons]**.

1. Expandera tillägget **[!DNL Workfront]**.
1. Klicka på **[!UICONTROL Configure]**.
1. Logga in på [!DNL Workfront] som systemadministratör.
1. Klicka på fliken **[!UICONTROL Activity Log]**.  

   Visa information om undantag och fel som inträffade när objekt skapades eller när fält synkroniserades mellan de två programmen.

   Loggen innehåller följande fält:

   * Datum för förekomsten
   * Namnet på användaren i Jira
   * Jirasnummer
   * En kort beskrivning av felet.
