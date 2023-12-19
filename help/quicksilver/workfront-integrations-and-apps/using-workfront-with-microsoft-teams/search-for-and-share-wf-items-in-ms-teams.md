---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Söka efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]
description: Du kan söka efter [!DNL Workfront] objekt i [!DNL Adobe WorkfrontWorkfront] kanal in [!DNL Microsoft Teams] och dela dessa med teammedlemmar.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 71d83723-daea-4b7b-8e5b-cfcf414611fe
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Söka efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]

>[!NOTE]
>
>Integreringen av Adobe Workfront för Microsoft Teams stöds för närvarande bara för den klassiska Microsoft Teams.

Du kan söka efter [!DNL Workfront] objekt i [!DNL Adobe Workfront] kanal in [!DNL Microsoft Teams] och dela dessa med teammedlemmar.

* [Förutsättningar för delning [!DNL Workfront] objekt i [!DNL Microsoft Teams]](#prerequisites-for-sharing-workfront-items-in-microsoft-teams-prerequisites-for-sharing-workfront-items-in-microsoft-teams)
* [Söka efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams]](#search-for-and-share-adobe-workfront-items-in-microsoft-teams)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Förutsättningar för delning [!DNL Workfront] objekt i [!DNL Microsoft Teams] {#prerequisites-for-sharing-workfront-items-in-microsoft-teams}

Du kan söka efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams] om följande villkor är uppfyllda:

* En teamägare har installerat och konfigurerat [!DNL Workfront for Microsoft Teams] för ert team.
* Du är inloggad [!DNL Workfront] från [!UICONTROL Microsoft Teams].

Mer information om installation [!UICONTROL Workfront for Microsoft Teams] och logga in på [!UICONTROL Workfront] från [!DNL Microsoft Teams], se [Installera Adobe Workfront för Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Använd [!DNL Adobe Workfront for Microsoft Teams integration]måste du använda en annan webbläsare än [!DNL Internet Explorer].


## Söka efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams] {#search-for-and-share-workfront-items-in-microsoft-teams}

Du kan söka efter följande [!DNL Workfront] objekt från en [!DNL Microsoft Teams] kanal:

* Projekt
* Uppgifter

  >[!NOTE]
  >
  >Du kan inte söka efter personliga uppgifter.

* Problem

När du har hittat de objekt du sökte efter kan du dela dem med andra användare i [!DNL Microsoft Teams].

Om du vill söka efter en [!DNL Workfront] objekt från [!DNL Microsoft Teams] och dela det med andra:

1. I [!DNL Microsoft Teams], går till valfri chattkanal och klickar på **[!DNL Workfront]** -ikon.
1. Sök efter [!DNL Workfront] gör något av följande:

   * Klicka på [!DNL Workfront] -ikon under konversationsfältet.\

     ![ms_teams_workfront_pin_icon_highlight.png](assets/ms-teams-workfront-pinned-icon-highlight-350x69.png)\
      Ikonen kan visas under **[!UICONTROL More]** i stället.\
      ![more_icon.png](assets/more-icon-52x34.png)\
      The **[!UICONTROL Search]** visas som standard.

   * Typ *@[!DNL Workfront]* från valfri kanal väljer du Workfront och väljer sedan **[!UICONTROL Search].**

     ![ms_teams_search_from_command.png](assets/ms-teams-search-from-command-350x74.png)

1. I [!UICONTROL search] Ange ett namn eller referensnummer för ett projekt, en uppgift eller ett ärende och klicka på det när det visas i listan.\
   ![ms_teams_searching_for_items.png](assets/ms-teams-searching-for-items-350x359.png)\
   Detta lägger till ett kort med [!DNL Workfront] objekt i chattfältet. Viss information om artikeln finns på kortet, inklusive namnet på artikeln, det överordnade objektet, status, prioritet, procent färdigt.

1. (Valfritt) Lägg till en kommentar under [!DNL Workfront] kort och klicka sedan på **[!UICONTROL Send]** eller tryck på Enter.\
   Detta skickar meddelandet inklusive [!DNL Workfront] till din kanal.\
   Alla medlemmar i kanalen kan se det här meddelandet, inklusive informationen på [!DNL Workfront] kort.

1. Klicka **[!UICONTROL View in Workfront]** för att visa objektet i [!DNL Workfront].\
   Endast användare som har [!DNL Workfront] licensen kan visa ett objekt i [!DNL Workfront].
