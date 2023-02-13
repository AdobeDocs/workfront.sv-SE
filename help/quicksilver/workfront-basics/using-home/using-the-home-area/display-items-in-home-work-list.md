---
product-area: projects
navigation-topic: use-the-home-area
title: Visa objekt i [!UICONTROL Work List] i hemområdet
description: The [!UICONTROL Work List] i [!UICONTROL Home] visas alla arbetsobjekt som har tilldelats dig. Du kan styra vilka objekt som visas i [!UICONTROL Work] Lista enligt beskrivning nedan.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1350'
ht-degree: 0%

---

# Visa objekt i [!UICONTROL Work List] i hemområdet

The [!UICONTROL Work List] i [!UICONTROL Home] visas alla arbetsobjekt som har tilldelats dig. Du kan styra vilka objekt som visas i [!UICONTROL Work] Lista enligt beskrivning nedan.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Review] endast för godkännanden</p> <p>[!UICONTROL Work] eller högre för alla andra objekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] eller högre tillgång till projekt, uppgifter, ärenden och dokument</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Contribute-behörigheter eller högre för de uppgifter och ärenden du behöver arbeta med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Filtrera [!UICONTROL Work List]

Du kan filtrera objekt i [!UICONTROL Work List] om du bara vill visa vissa typer av objekt. Du kan till exempel filtrera [!UICONTROL Work List] om du bara vill visa problem eller förfrågningar.

>[!NOTE]
>
>Filteralternativen lagras i webbläsaren. Om du konsekvent använder samma webbläsare på samma dator (och inte rensar platsdata) ändras inte de valda filtren. Om du byter webbläsare eller dator återställs standardalternativet som är inaktiverat för alla filter.

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) nedrullningsbar meny.
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
      <td role="rowheader"><strong>[!UICONTROL Tasks Working On]</strong></td> 
      <td> <p>Visar endast aktiviteter som du arbetar med. Det här är uppgifter som tilldelats dig och som du har klickat på [!UICONTROL Work On It] -knappen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast aktiviteter som är klara att startas. Båda följande programsatser måste vara sanna:</p> 
        <ul> 
         <li> <p>Aktiviteterna och deras föräldrar har inga föregående aktiviteter eller uppgiftsbegränsningar som hindrar dem från att arbeta.</p> </li> 
         <li> <p>The [!UICONTROL Planned Start Date] tidigare eller upp till två veckor framåt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>Visar endast aktiviteter som inte är klara att starta än. Någon av följande programsatser måste vara true:</p> 
        <ul> 
         <li> <p>Aktiviteterna och deras överordnade kan ha föregångare eller uppgiftsbegränsningar som förhindrar att de bearbetas.</p> </li> 
         <li> <p>Uppgifterna har en [!UICONTROL Planned Start Date] det är mer än två veckor i framtiden.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Working On]</strong></td> 
      <td> <p>Visar endast problem som du arbetar med. Det här är ärenden som tilldelats dig och som du har klickat på [!UICONTROL Work On It] -knappen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Requested]</strong></td> 
      <td>Visar endast problem som du har tilldelats men som du inte har klickat på [!UICONTROL Work On It] -knappen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personligt</strong></td> 
      <td>Visar endast personliga uppgifter. Det här är uppgifter som du skapar som [!UICONTROL To Do] uppgift, enligt beskrivningen i avsnittet <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Skapa en personlig uppgift</a> i artikeln <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Skapa arbetsobjekt från [!UICONTROL Home] area</a>.</td> 
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
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>Visar endast slutförda uppgifter, ärenden och personliga uppgifter. Slutfört arbete visas för de senaste två veckorna och grupperas i arbetslistan efter den vecka då det slutfördes. Godkännanden inkluderas inte.</p> <p>Slutfört arbete är dolt i [!UICONTROL Work List] om du inte markerar det här filtret.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filteralternativen är baserade på objekt (uppgifter, ärenden, godkännanden, personliga uppgifter).
   >* Uppgifter och ärenden filtreras vidare efter deras tillstånd i relation till vår beredskap att arbeta med dem ([!UICONTROL Working On], [!UICONTROL Ready to Start], [!UICONTROL Not Ready] för uppgifter, och [!UICONTROL Working On] och [!UICONTROL Requested] för problem). Du kan välja att visa uppgifter eller problem i ett visst läge eller klicka på Åtgärder eller Problem för att välja och visa alla lägen.
   >* Det finns ett separat filter för slutförda objekt och det innehåller både uppgifter och problem. Detta inkluderar inte godkännanden. The [!UICONTROL Completed] filtret innehåller personliga uppgifter.
   >* Du kan bara välja ett läge åt gången. Du kan till exempel bara visa [!UICONTROL Working On] uppgifter och endast [!UICONTROL Requested] problem.
   >* Du kan inte använda filter för objekt som har tilldelats ett team och de ingår inte i objekt som har tilldelats direkt till dig.



1. (Valfritt) Ordna [!UICONTROL Work List], enligt beskrivningen i avsnittet [Gruppera och sortera efter datum, projekt och prioritet](#group-and-sort-by-date-project-and-priority) i den här artikeln.

## Gruppera och sortera efter [!UICONTROL Date], [!UICONTROL Project]och [!UICONTROL Priority]

Du kan gruppera och sortera [!UICONTROL Work List] av [!UICONTROL Planned Completion Date], [!UICONTROL Commit Date], [!UICONTROL Project], eller [!UICONTROL My Priority]. Det alternativ du väljer avgör hur objekten grupperas i [!UICONTROL Work List].

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL Group by]** nedrullningsbar meny.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> Objekten visas i följande grupperingar i [!UICONTROL Work List], beroende på deras [!UICONTROL Planned Completion Date] (antalet objekt inom varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
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
      <td> <p>Objekten visas i följande grupperingar i [!UICONTROL Work List], beroende på deras [!UICONTROL Planned Start Date] (antalet objekt inom varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>Den här grupperingen utökas som standard.</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned], följt av olika [!UICONTROL Planned Start Dates] (flera grupperingar)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>Objekten visas i följande grupperingar i [!UICONTROL Work List] (antalet objekt inom varje gruppering visas inom parentes bredvid rubriktiteln):</p> 
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
      <td>Objekten visas i den ordning du väljer. Mer information finns i <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Prioritera arbetet i [!UICONTROL Home] area</a>.</td> 
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
* **Bevis på godkännanden**: [!UICONTROL Proof deadline]

## Sök i [!UICONTROL Work List]

När du söker i [!UICONTROL Work List]returneras alla objekt som du har tilldelats i sökningen (även objekt som inte är inlästa på skärmen). Om [!UICONTROL Show complete] om du väljer det här alternativet returneras alla objekt som du har markerat som slutförda under de senaste två veckorna.

Dessutom genomsöks bara namnen på arbetsobjekten (informationen i arbetsposten genomsöks inte, inte heller namnen på de projekt där arbetsposten finns).

Om du vill söka i [!UICONTROL Work List]:

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Valfritt) Filtrera [!UICONTROL Work List], enligt beskrivningen i [Filtrera [!UICONTROL Work List]](#filter-the-work-list) och [Gruppera och sortera efter datum, projekt och prioritet](#group-and-sort-by-date-project-and-priority).

1. (Valfritt) Om du söker efter en arbetsuppgift som redan är klar måste du konfigurera [!UICONTROL Work List] om du vill visa slutförda objekt innan du söker.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Börja skriva namnet på det objektnamn du söker efter.\
   The [!UICONTROL Work List] filtreras automatiskt så att objekt med ett matchande namn tas med.

## Ändra storlek på arbetslistan

Du kan ändra storleken på [!UICONTROL Work List] så att den förbrukar var som helst mellan cirka en fjärdedel av hemsidan och cirka hälften av [!UICONTROL Home] område.

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Muspekaren över den högra kanten av [!UICONTROL Work List]drar du åt vänster eller höger tills arbetslistan har önskad storlek.

## Komprimera och expandera grupperingar

Objekt i [!UICONTROL Work List] visas i grupperingar. Du kan komprimera och expandera grupperingar för att styra hur mycket information som visas på sidan vid en viss tidpunkt.

Du kan komprimera och expandera grupperingar i [!UICONTROL Work List] för att bättre kontrollera vilken information som visas.\
Som standard är [!UICONTROL This Week] grupperingen expanderas och alla andra grupperingar komprimeras. Alla ändringar du gör sparas nästa gång du öppnar området Hem.

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. Klicka på **[!UICONTROL Expand]** eller **[!UICONTROL Collapse]** pilen bredvid de grupperingar du vill expandera eller komprimera.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   eller\
   Om du vill expandera eller komprimera alla grupperingar samtidigt klickar du på **[!UICONTROL Expand]** eller **[!UICONTROL Collapse]** pilen bredvid en gruppering medan du håller ned [!UICONTROL Shift] nyckel.
