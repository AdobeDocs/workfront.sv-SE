---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visa aktivitetsloggen för Jira
description: Som  [!DNL Jira] administratör kan du visa de undantag och fel som inträffar under synkroniseringen eller skapandet av biljetterna mellan [!DNL Adobe Workfront] och [!DNL Jira] i en aktivitetslogg.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Visa [!UICONTROL [!DNL Jira] Activity Log]

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen kommer integreringen av Workfront för Jira inte att vara tillgänglig efter **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Jira.
>
>Åtta färdiga mallar för automatisering och integrering av Workfront för Jira kommer att vara tillgängliga i augusti för att hjälpa till att replikera vanliga arbetsflöden och snabba upp implementeringen. Mallarna är helt anpassningsbara för att uppfylla specifika affärsbehov och kan utökas i takt med att behoven utvecklas.
> 
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration Module för Jira finns i [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

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
