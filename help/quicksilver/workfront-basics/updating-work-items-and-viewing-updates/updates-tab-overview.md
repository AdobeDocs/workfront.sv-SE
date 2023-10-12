---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över uppdateringsavsnittet
description: I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Översikt över uppdateringsavsnittet

<!--take "Beta" references out when we remove the beta-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>\
<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">Information om det aktuella releaseschemat finns i [Versionsöversikt för fjärde kvartalet 2023](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Beroende på vilken miljö och vilka objekt du har tillgång till kommentarfunktionerna från kan du se olika funktioner i uppdateringsavsnittet.
>
>Mer information om den nya kommentarsfunktionen och dess tillgänglighet finns på [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Den nya kommentarsupplevelsen är bara tillgänglig för uppdateringsavsnittet och är inte tillgänglig för följande områden:
>
> * Startsida
> * Panelen Sammanfattning i listor
> * Sammanfattningspanelen i tidrapporter

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old note, removed with August 2023: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the new commenting experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.

-->

## Översikt över uppdateringsavsnittet

* I uppdateringsavsnittet för ett objekt visas upp till 200 av de senaste uppdateringarna under de senaste 90 dagarna.

  ![](assets/updates-tab-before-unified-experience-for-issues.png)

* Uppdateringsavsnittet visas för följande objekt:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td> 
      <ul> 
      <li>Dokument</li> 
      <li>Mål</li> 
      <li>Problem</li> 
      <li>Iterationer</li> 
      <li>Projekt</li> 
      <li>Program</li> 
      <li>Portfolio</li> 
      </ul> </td> 
    <td> 
      <ul> 
      <li>Artiklar*</li> 
      <li>Uppgifter</li> 
      <li>Mallar</li> 
      <li>Malluppgifter</li> 
      <li>Tidrapporter</li> 
      <li>Användare</li>
      <li>Kort ombord</li>
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *Artiklar är uppgifter. All information som rör uppgifter är också tillgänglig för artiklar.

Informationen i uppdateringsavsnittet är organiserad på olika sätt beroende på vilken miljö du kommer åt den från.


### Översikt över aktuellt uppdateringsavsnitt

<!--October 26 - replace current with legacy-->

* I det aktuella uppdateringsavsnittet visas följande information:

   * **Användaruppdateringar**: Synpunkter från användare och svar på dessa kommentarer.
   * **Systemuppdateringar**: Informationsmeddelanden som Workfront skapar för att spela in vissa händelser i ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Följande objekt registrerar inte systemuppdateringar:

   * Team
   * Mall
   * Malluppgift

### Översikt över uppdateringsavsnittet i den nya kommentarsfunktionen

Information om vilka funktioner som är tillgängliga för den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--update screen shot and maybe save it under a new name??? with the August 17 release - also make sure you have some people tagged, similar to what we show in the old UI-->

<span class="preview">![](assets/updates-tab-after-unified-experience-for-tasks.png)</span>

* I uppdateringsavsnittet visas information på följande flikar i den nya kommentarsfunktionen:

   * **Kommentar**: Visar kommentarer från användare och svar på dessa kommentarer. Mer information om hur du uppdaterar objekt i den nya kommentarsfunktionen finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).
   * **Systemaktivitet**: Visar systemuppdateringar som är informationsmeddelanden som Workfront skapar för att registrera vissa händelser för ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

      * Följande objekt saknar fliken Systemaktivitet:

         * Team
         * Mall
         * Malluppgift
         * Ad hoc-kort

* För närvarande kan du lägga till kommentarer och svara på uppdateringar med hjälp av den nya kommentarsfunktionen för följande objekt:


   * Projekt
   * Uppgifter (och artiklar)
   * Problem
   * Dokument
   * Mål

  >[!NOTE]
  >
  >Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * Kort ombord

  >[!NOTE]
  >
  > Du kan lägga till och visa uppdateringar för kort i kortområdet när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).


  <span class="preview">

   * Mallar
   * Malluppgifter
   * Tidrapporter
   * Användare
   * Portfolio
   * Program

  >[!NOTE]
  >
  >    Du kan inte visa den nya kommentarsfunktionen för iterationer.

  </span>

<!--hidden in August 2023 and replaced by the list above: 

  <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>Goals</p>
        <li>Cards in the Boards area*</li>
          This is the only experience for goals and cards.
        </li> 
        <li>Projects</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>Issues</li> 
        <li>Tasks</li>
        <li>Documents</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

  *You can add and view updates to cards in the Board areas when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md). 
  -->



## Uppdateringar som också visas på objekt med högre rankning

Kommentarer eller svar på uppdateringar av vissa objekt visas också i uppdateringsavsnittet för objekt med högre rankning.

När du till exempel lägger till en uppdatering för en uppgift visas uppdateringen i uppdateringsavsnittet för uppgiften och i uppdateringsavsnittet för projektet som innehåller uppgiften.

>[!NOTE]
>
>När du aktiverar den nya kommentarsfunktionen visas kommentarer på följande objekt med högre rankning:
>
>* Problem
>* Projekt
>* Uppgifter
>
>Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

I följande tabell visas de objekt vars kommentarer också visas på de objekt som ligger högst upp i listan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objekt där den ursprungliga uppdateringen lades till</strong> </th> 
   <th> <p><strong>Objekt med högre rankning där den ursprungliga uppdateringen också visas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Problem</td> 
   <td>Projekt</td> 
  </tr> 
  <tr> 
   <td>Uppgift</td> 
   <td>Projekt</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Program, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Dokument </td> 
   <td>Objekt där dokumentet är bifogat, Projekt </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td>Team</td> 
  </tr> 
  <tr> 
   <td>Tidrapport</td> 
   <td>Användare, team</td> 
  </tr> 
  <tr> 
   <td>Malluppgift</td> 
   <td>Mall</td> 
  </tr> 
  <tr> 
   <td>Artikel</td> 
   <td>Iteration, Team</td> 
  </tr> 
  <tr> 
   <td>Upprepning</td> 
   <td>Team</td> 
  </tr>

<tr> 
   <td>Mål</td> 
   <td>Resultat, aktivitet</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Svar som lagts till i systemuppdateringar sammanfogas inte med det överordnade objektet. Endast direkta svar på ett underordnat objekt och svar som lagts till i befintliga uppdateringar läggs ihop med överordnade objekt.
>
>Mer information om objekthierarkin i Adobe Workfront finns i [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> Det går inte att svara på systemuppdateringar i den nya kommentarsfunktionen. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## Begränsningar i uppdateringsavsnittet

Det finns vissa begränsningar i uppdateringsavsnittet för ett team och när du anger uppdateringar för andra användares räkning.

### Begränsningar för användare och team

Du kan inte lägga till nya kommentarer i uppdateringsavsnittet i ett team.

<span class="preview">Du kan lägga till ett svar på en uppdatering som du visar i ett team. Svaret visas i teamets uppdateringsavsnitt samt i uppdateringsavsnittet för det objekt det tillhör. </span>

Uppdateringsavsnittet för team fylls i av uppdateringar som anges för följande objekt:

* Användare
* Tidrapporter
* Artiklar
* Iterationer

I uppdateringsavsnittet för användare och team kan du visa de uppdateringar som har gjorts under de senaste 90 dagarna.

Om du vill se alla uppdateringar som gjorts för en användare eller ett team, utöver 90-dagarsgränsen, kan du skapa en rapport för anteckningar. Rapporten ska inte ha något tidsfilter som visar alla uppdateringar som gjorts för användare eller team. Mer information finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Begränsningar när du skriver kommentarer för en annan användares räkning

Adobe Workfront-administratörer och gruppadministratörer kan logga in som andra användare och utföra åtgärder i Workfront som att skriva kommentarer.

Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Alla kommentarer som görs för en annan användares räkning anges i kommentaren.

<!--remove the note below when we release this back to the new commenting-->

>[!NOTE]
>
>När du använder den nya kommentarsfunktionen läggs kommentaren till som den användare som loggade in som en annan användare och det finns inget som tyder på att han/hon lägger till en kommentar för någon annans räkning.
>
>Om en Workfront-administratör till exempel loggar in som en annan användare är den användare som är associerad med kommentaren Workfront-administratören. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


En gruppadministratör kan kommentera för en annan persons räkning, men kan inte ta bort kommentaren. Det är bara en Adobe Workfront-administratör som kan ta bort en kommentar som de har gjort för en annan användares räkning.

## Visa systemuppdateringar för arbetsobjekt med journalpostrapporten

Journalanmälningsrapporten innehåller systemuppdateringar från uppdateringsområdet för projekt, uppgifter och utgåvor.

I rapporten kan du se:

* Hur många statusändringar som har gjorts
* När en uppgift eller ett problem har tagits bort
* Hur värden i viktiga anpassade fält ändrades under ett projekt
* Vilka viktiga datum som har ändrats under ett projekt
* Om prioritet ändras under ett projekt
* Om ägaren till ett projekt har ändrats

Mer information finns i [Rapport om uppdateringsområdet](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
