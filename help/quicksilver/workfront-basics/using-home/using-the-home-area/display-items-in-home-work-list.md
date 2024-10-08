---
product-area: projects
navigation-topic: use-the-home-area
title: Visa objekt i [!UICONTROL Work List] i hemområdet
description: '[!UICONTROL Work List] i området [!UICONTROL Home] visar alla arbetsobjekt som har tilldelats dig. Du kan styra vilka objekt som ska visas i [!UICONTROL Work List] genom att använda filter och genom att gruppera och sortera arbetsobjekten.'
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: d614d5cbded1de6fd899a47495a6e058f9eaf3cf
workflow-type: tm+mt
source-wordcount: '1564'
ht-degree: 0%

---

# Visa objekt i [!UICONTROL Work List] i området [!UICONTROL Home]

<!-- Audited: 1/2024 -->


[!UICONTROL Work List] i området [!UICONTROL Home] visar alla arbetsobjekt som har tilldelats dig. Du kan styra vilka objekt som ska visas i [!UICONTROL Work List] genom att använda filter och genom att gruppera och sortera arbetsobjekten.

>[!NOTE]
>
>* När du konverterar ett problem till en uppgift eller ett projekt tas problemet bort från startdelen för den användare som är tilldelad problemet.
>
>* När du konverterar en uppgift till ett projekt tas uppgiften bort och tas bort från hemområdet för användaren som tilldelats uppgiften.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> <p>Nytt:</p><ul><li>[!UICONTROL Contributor] endast för godkännanden</li> <li>[!UICONTROL Standard] eller högre för alla andra objekt</li> <p>eller</p> 
  </ul><p>Aktuell:</p><ul><li>[!UICONTROL Review] endast för godkännanden</li> <li>[!UICONTROL Work] eller högre för alla andra objekt</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL View] eller högre tillgång till projekt, uppgifter, ärenden och dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Contribute behörigheter eller högre för de uppgifter och problem du behöver arbeta med</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrera [!UICONTROL Work List]

Du kan filtrera objekt i [!UICONTROL Work List] om du bara vill visa vissa typer av objekt. Du kan till exempel filtrera [!UICONTROL Work List] så att endast utgåvor eller förfrågningar visas.

>[!NOTE]
>
>Filteralternativen lagras i webbläsaren. Om du konsekvent använder samma webbläsare på samma dator (och inte rensar platsdata) ändras inte de valda filtren. Om du byter webbläsare eller dator återställs standardalternativet, vilket innebär att alla filter är avmarkerade.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på listrutan **[!UICONTROL Filter]** ![](assets/filter-nwepng.png). Om du har markerat några filter visas antalet markerade filter i stället för ikonen.
1. Välj bland följande filteralternativ för att ange vilken typ av objekt du vill visa:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Visar och markerar alla objekt. Detta omfattar uppgifter, ärenden, godkännanden, personliga uppgifter samt slutförda uppgifter och ärenden. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Working On]</strong></td> 
      <td> <p>Visar endast aktiviteter som du arbetar med. Detta är uppgifter som tilldelats dig och som du har klickat på knappen [!UICONTROL Work On It] för.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast aktiviteter som är klara att startas. Båda följande programsatser måste vara sanna:</p> 
        <ul> 
         <li> <p>Aktiviteterna och deras föräldrar har inga föregående aktiviteter eller uppgiftsbegränsningar som hindrar dem från att arbeta.</p> </li> 
         <li> <p>Alla föregående aktiviteter har slutförts.</p> </li> 
         <li> <p>[!UICONTROL Planned Start Date] av aktiviteterna har passerat eller upp till två veckor framåt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks: Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast aktiviteter som inte är klara att starta än. Någon av följande programsatser måste vara true:</p> 
        <ul> 
         <li> <p>Aktiviteterna och deras överordnade kan ha föregångare eller uppgiftsbegränsningar som förhindrar att de bearbetas.</p> </li> 
         <li> <p>Aktiviteterna har en [!UICONTROL Planned Start Date] som är mer än två veckor i framtiden.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Working On]</strong></td> 
      <td> <p>Visar endast problem som du arbetar med aktivt. Det här är ärenden som du har tilldelats och som du har klickat på knappen [!UICONTROL Work On It] för.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues: Requested]</strong></td> 
      <td>Visar endast problem som du har tilldelats men som du inte har klickat på knappen [!UICONTROL Work On It] för.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personligt</strong></td> 
      <td>Visar endast personliga uppgifter. Detta är uppgifter som du skapar som en [!UICONTROL To Do]-uppgift, vilket beskrivs i avsnittet <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Skapa en personlig uppgift</a> i artikeln <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Skapa arbetsobjekt från [!UICONTROL Home]-området</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast godkännanden som tilldelats eller delegerats till dig och godkännanden som du har skickat in. Godkännanden omfattar godkännanden av arbetsobjekt (projekt, uppgifter och utgåvor) och godkännanden av dokument, korrektur, åtkomstbegäranden och tidrapporter. Mer information om godkännanden finns i följande artiklar:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Visa godkännanden</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Arbetsgodkännanden</a> </p> </li> 
        </ul> 
        <p>Obs! Godkännanden som du har skickat och där du också är en av godkännarna räknas två gånger.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated by me]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast arbetsobjekt som du har delegerat till en annan användare.</p> 
        <p>Mer information om delegering av uppgifter finns i <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delegera uppgifter och ärenden till en annan användare</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated: Delegated to me]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast arbetsobjekt som tillfälligt har delegerats till dig av en annan användare.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>Visar endast slutförda uppgifter, ärenden och personliga uppgifter. Slutfört arbete visas för de senaste två veckorna och grupperas i arbetslistan efter den vecka då det slutfördes. Godkännanden inkluderas inte.</p> <p>Slutförda arbeten är dolda i [!UICONTROL Work List] om du inte väljer det här filtret.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filteralternativen är baserade på objekt (uppgifter, ärenden, godkännanden, personliga uppgifter).
   >* Aktiviteter och ärenden filtreras ytterligare efter deras tillstånd i relation till vår beredskap att arbeta med dem ([!UICONTROL Working On], [!UICONTROL Ready to Start], [!UICONTROL Not Ready] för aktiviteter samt [!UICONTROL Working On] och [!UICONTROL Requested] för problem). Du kan välja att visa uppgifter eller problem i ett visst läge eller klicka på Åtgärder eller Problem för att välja och visa alla lägen.
   >* Det finns ett separat filter för slutförda objekt och det innehåller både uppgifter och problem. Detta inkluderar inte godkännanden. Filtret [!UICONTROL Completed] innehåller personliga uppgifter.
   >* Du kan välja att bara visa ett läge åt gången. Du kan till exempel bara visa [!UICONTROL Working On] uppgifter och bara [!UICONTROL Requested] problem. Du kan också markera flera lägen samtidigt.
   >* Du kan inte använda filter för objekt som har tilldelats ett team, och teamtilldelningar ingår inte i objekt som har tilldelats direkt till dig.


1. (Valfritt) Ordna [!UICONTROL Work List] ytterligare, enligt beskrivningen i avsnittet [Gruppera och sortera efter datum, projekt och prioritet](#group-and-sort-by-date-project-and-priority) i den här artikeln.

## Gruppera och sortera efter [!UICONTROL Date], [!UICONTROL Project] och [!UICONTROL Priority]

Du kan gruppera och sortera [!UICONTROL Work List] efter [!UICONTROL Planned Completion Date], [!UICONTROL Commit Date], [!UICONTROL Project] eller [!UICONTROL My Priority]. Det alternativ du väljer avgör hur objekt grupperas i [!UICONTROL Work List].

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på listrutan **[!UICONTROL Group by]** ![Gruppera efter](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> Objekten visas i följande grupperingar i [!UICONTROL Work List], beroende på deras [!UICONTROL Planned Completion Date] (antalet objekt i varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL No Planned Completion Date]</p> </li> 
        <li> <p>[!UICONTROL This Week]</p> <p>Den här grupperingen utökas som standard.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], följt av olika [!UICONTROL Planned Completion Dates] (flera grupperingar)</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Start]</strong></td> 
      <td> <p>Objekten visas i följande grupperingar i [!UICONTROL Work List], beroende på deras [!UICONTROL Planned Start Date] (antalet objekt i varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>Den här grupperingen utökas som standard.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], följt av olika [!UICONTROL Planned Start Dates] (flera grupperingar)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>Objekten visas i följande grupperingar i [!UICONTROL Work List] (antalet objekt i varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Objekten grupperas efter projekt och projekten visas i bokstavsordning i [!UICONTROL Work List]. (Antalet objekt i varje gruppering visas inom parentes bredvid rubriktiteln.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>Objekten visas i den ordning du väljer. Mer information finns i <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Prioritera arbete i [!UICONTROL Home] området </a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>Standardsorteringen är stigande. Om du ändrar sorteringen till fallande sparas de valda sorteringsalternativen i webbläsaren. Om du konsekvent använder samma webbläsare på samma dator (och inte rensar platsdata) ändras inte sorteringen, men om du byter webbläsare eller datorer ändras sorteringen till standardsorteringen.

## Visa sena artiklar

[!DNL Adobe Workfront] använder följande datum för att avgöra om arbetsförfrågningar är sena:

* **Uppgifter**: [!UICONTROL Planned Completion Date]
* **Problem**: [!UICONTROL Planned Completion Date]
* **Dokument**: [!UICONTROL Submitted date]
* **Tidrapporter**: [!UICONTROL Submitted date]
* **Godkännanden**: [!UICONTROL Submitted date]
* **Korrektur för godkännanden**: [!UICONTROL Proof deadline]

## Sök i [!UICONTROL Work List]

När du söker i [!UICONTROL Work List] returneras alla objekt som du har tilldelats i sökningen (även objekt som inte är inlästa på skärmen). Om alternativet [!UICONTROL Show complete] har valts returneras även alla objekt som du har markerat som slutförda under de senaste två veckorna.

Dessutom genomsöks bara namnen på arbetsobjekten (informationen i arbetsposten genomsöks inte och inte heller namnen på de projekt där arbetsposten finns).

Så här söker du efter [!UICONTROL Work List]:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Valfritt) Filtrera och gruppera [!UICONTROL Work List] enligt beskrivningen i [Filtrera [!UICONTROL Work List]](#filter-the-work-list) och [Gruppera och sortera efter datum, projekt och prioritet](#group-and-sort-by-date-project-and-priority).

1. (Valfritt) Om du söker efter ett arbetsobjekt som redan är färdigt måste du konfigurera [!UICONTROL Work List] så att det visar de slutförda objekten innan du söker.

1. Klicka på sökikonen ![Sök](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Börja skriva namnet på det objektnamn du söker efter.\
   [!UICONTROL Work List] filtreras automatiskt så att objekt med ett matchande namn inkluderas.

## Ändra storlek på arbetslistan

Du kan ändra storleken på [!UICONTROL Work List] så att den förbrukar var som helst mellan ungefär en fjärdedel av startområdet och ungefär hälften av [!UICONTROL Home] -området.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. För musen över den högra kanten av [!UICONTROL Work List] och dra sedan åt vänster eller höger tills arbetslistan har önskad storlek.

## Komprimera och expandera grupperingar

Objekt i [!UICONTROL Work List] visas i grupperingar. Du kan komprimera och expandera grupperingar för att styra hur mycket information som visas på sidan vid en viss tidpunkt.

Du kan komprimera och expandera grupperingar inom [!UICONTROL Work List] för att bättre kontrollera vilken information som visas.\
Som standard utökas grupperingen [!UICONTROL This Week] och alla andra grupperingar komprimeras. Alla ändringar du gör sparas nästa gång du öppnar området Hem.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på pilen **[!UICONTROL Expand]** eller **[!UICONTROL Collapse]** bredvid de grupperingar du vill expandera eller komprimera.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   eller\
   Om du vill expandera eller komprimera alla grupperingar samtidigt klickar du på **[!UICONTROL Expand]**- eller **[!UICONTROL Collapse]**-pilen bredvid en gruppering samtidigt som du håller ned [!UICONTROL Shift].
