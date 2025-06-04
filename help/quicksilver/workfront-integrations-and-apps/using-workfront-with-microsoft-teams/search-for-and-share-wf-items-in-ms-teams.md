---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Sök efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]
description: Du kan söka efter [!DNL Workfront] objekt i alla [!DNL Adobe WorkfrontWorkfront] kanaler i [!DNL Microsoft Teams] och dela objekten med medlemmar i dina team.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 71d83723-daea-4b7b-8e5b-cfcf414611fe
source-git-commit: 372b7566fa5eb38703905b22ff43d49a76bcb400
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Sök efter och dela [!DNL Adobe Workfront] objekt i [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>När Microsoft går över till New Teams-klienten är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. Vi håller på att utveckla en ny version av Microsoft Teams-integreringen som är helt kompatibel med nya Teams-klienten och som är tillgänglig före 1 juli för att säkerställa en smidig övergång.
>
>Instruktioner om hur du hämtar och installerar integreringen i New Teams-klienten blir tillgänglig när integreringen har släppts.

Du kan söka efter [!DNL Workfront] objekt i valfri [!DNL Adobe Workfront]-kanal i [!DNL Microsoft Teams] och dela dessa objekt med medlemmar i dina team.

* [Förutsättningar för att dela  [!DNL Workfront] objekt i [!DNL Microsoft Teams]](#prerequisites-for-sharing-workfront-items-in-microsoft-teams-prerequisites-for-sharing-workfront-items-in-microsoft-teams)
* [Sök efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams]](#search-for-and-share-adobe-workfront-items-in-microsoft-teams)

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

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Krav för delning av [!DNL Workfront] objekt i [!DNL Microsoft Teams] {#prerequisites-for-sharing-workfront-items-in-microsoft-teams}

Du kan söka efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams] om följande villkor uppfylls:

* En teamägare har installerat och konfigurerat [!DNL Workfront for Microsoft Teams] för ditt team.
* Du är inloggad på [!DNL Workfront] från [!UICONTROL Microsoft Teams].

Information om hur du installerar [!UICONTROL Workfront for Microsoft Teams] och loggar in på [!UICONTROL Workfront] från [!DNL Microsoft Teams] finns i [Installera Adobe Workfront för Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

>[!NOTE]
>
>[!DNL Microsoft Teams] stöder inte längre [!DNL Internet Explorer]. Om du vill använda [!DNL Adobe Workfront for Microsoft Teams integration] måste du använda en annan webbläsare än [!DNL Internet Explorer].


## Sök efter och dela [!DNL Workfront] objekt i [!DNL Microsoft Teams] {#search-for-and-share-workfront-items-in-microsoft-teams}

Du kan söka efter följande [!DNL Workfront] objekt från en [!DNL Microsoft Teams]-kanal:

* Projekt
* Uppgifter

  >[!NOTE]
  >
  >Du kan inte söka efter personliga uppgifter.

* Problem

När du har hittat de objekt du sökte efter kan du dela dem med andra användare i [!DNL Microsoft Teams].

Så här söker du efter ett [!DNL Workfront]-objekt från [!DNL Microsoft Teams] och delar det med andra:

1. Gå till en chattkanal i [!DNL Microsoft Teams] och klicka på ikonen **[!DNL Workfront]** .
1. Sök efter objektet [!DNL Workfront] genom att göra något av följande:

   * Klicka på ikonen [!DNL Workfront] under konversationsfältet.\

     ![ms_teams_workfront_pin_icon_highlight.png](assets/ms-teams-workfront-pinned-icon-highlight-350x69.png)\
      Beroende på dina inställningar kan den här ikonen visas under ikonen **[!UICONTROL More]** i stället.\
      ![more_icon.png](assets/more-icon-52x34.png)\
      Rutan **[!UICONTROL Search]** visas som standard.

   * Skriv *@[!DNL Workfront]* från valfri kanal, välj Workfront och sedan **[!UICONTROL Search].**

     ![ms_teams_search_from_command.png](assets/ms-teams-search-from-command-350x74.png)

1. I rutan [!UICONTROL search] börjar du skriva namnet eller referensnumret för ett projekt, en uppgift eller ett problem och klickar på det när det visas i listan.\
   ![ms_teams_searching_for_items.png](assets/ms-teams-searching-for-items-350x359.png)\
   Detta lägger till ett kort med objektet [!DNL Workfront] i chattfältet. Viss information om artikeln finns på kortet, inklusive namnet på artikeln, det överordnade objektet, status, prioritet, procent färdigt.

1. (Valfritt) Lägg till en kommentar under kortet [!DNL Workfront] och klicka sedan på **[!UICONTROL Send]** eller tryck på Retur.\
   Detta skickar meddelandet inklusive objektet [!DNL Workfront] till din kanal.\
   Alla medlemmar i kanalen kan se det här meddelandet, inklusive informationen på kortet [!DNL Workfront].

1. Klicka på **[!UICONTROL View in Workfront]** om du vill visa objektet i [!DNL Workfront].\
   Endast användare som har en [!DNL Workfront]-licens kan visa ett objekt i [!DNL Workfront].
