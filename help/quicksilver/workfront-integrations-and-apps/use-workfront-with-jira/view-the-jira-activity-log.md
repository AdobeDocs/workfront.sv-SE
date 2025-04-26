---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visa aktivitetsloggen för Jira
description: Som  [!DNL Jira] administratör kan du visa de undantag och fel som inträffar under synkroniseringen eller skapandet av biljetterna mellan [!DNL Adobe Workfront] och [!DNL Jira] i en aktivitetslogg.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Visa [!UICONTROL [!DNL Jira] Activity Log]

Som [!DNL Jira]-administratör kan du visa de undantag och fel som inträffar under synkroniseringen eller skapandet av biljetterna mellan [!DNL Adobe Workfront] och [!DNL Jira] i en [!UICONTROL Activity Log].

Du kan se upp till 500 objekt i aktivitetsloggen, och de listas med början från de senaste.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över licenser för Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p>Viktigt! Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

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
1. Välj fliken **[!UICONTROL Activity Log]**.

   Visa information om undantag och fel som inträffade när objekt skapades eller när fält synkroniserades mellan de två programmen.

   Loggen innehåller följande fält:

   * Datum för förekomsten
   * Namnet på användaren i Jira
   * Jirasnummer
   * En kort beskrivning av felet.
