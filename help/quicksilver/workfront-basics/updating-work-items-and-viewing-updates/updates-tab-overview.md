---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över uppdateringsavsnittet
description: I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# Översikt över uppdateringsavsnittet

<!--take "Beta" references out when we remove the beta-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

>[!NOTE]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Mer information om de nya kommentarfunktionerna finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Du kan komma åt den nya funktionen för följande objekt:
> * Problem, projekt, uppgifter och dokument.
>
>     Detta är tillgängligt när du aktiverar den nya kommentarsfunktionen.
>
>     Den här funktionen är bara tillgänglig för uppdateringsavsnittet och är inte tillgänglig för följande områden:
>
>     * Startsida
>     * Panelen Sammanfattning i listor
>     * Sammanfattningspanelen i tidrapporter
>
> * Mål, kort i området för anslagstavlor
>
>   Den nya kommentarsupplevelsen är den enda upplevelsen för mål och kort. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för användning av Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Du kan lägga till och visa uppdateringar för kort i kortområdet när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.

## Översikt över uppdateringsavsnittet

Informationen i uppdateringsavsnittet är organiserad på olika sätt beroende på vilken miljö du kommer åt den från.

### Översikt över aktuellt uppdateringsavsnitt

<!--October 26 - replace current with legacy-->

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
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *Artiklar är uppgifter. All information som rör uppgifter är också tillgänglig för artiklar.

* I det aktuella uppdateringsavsnittet visas följande information:

   * **Användaruppdateringar**: Synpunkter från användare och svar på dessa kommentarer.
   * **Systemuppdateringar**: Informationsmeddelanden som Workfront skapar för att spela in vissa händelser i ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Följande objekt registrerar inte systemuppdateringar:

   * Team
   * Mall
   * Malluppgift

### Översikt över uppdateringsavsnittet i den nya kommentarsfunktionen

Information om vilka funktioner som är tillgängliga för den nya kommentarsfunktionen och för vilka objekt finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--update screen shot and maybe save it under a new name??? with the August 17 release-->

![](assets/updates-tab-after-unified-experience-for-issues.png)

* I uppdateringsavsnittet visas information på följande flikar i den nya kommentarsfunktionen:

   * **Kommentar**: Visar kommentarer från användare och svar på dessa kommentarer. Mer information om hur du uppdaterar objekt i den nya kommentarsfunktionen finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).
   * **Systemaktivitet**: Visar systemuppdateringar som är informationsmeddelanden som Workfront skapar för att registrera vissa händelser för ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* För närvarande kan du lägga till kommentarer och svara på uppdateringar med hjälp av den nya kommentarsfunktionen för följande objekt:

<!--replace the table with this list on August 17: 

    * Projects
    * Tasks (and stories)
    * Issues
    * Documents

    <span class="preview">
    
    * Templates
    * Template Tasks
    * Timesheets
    * Users
    * Portfolios
    * Programs
    
    >[!NOTE]
    >
    >    You cannot display the new commenting experience for iterations. 

    </span>
  
  -->

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>Mål</p>
        <li>Kort i området för anslagstavlor*</li>
          Det här är den enda upplevelsen för mål och kort.
        </li> 
        <li>Projekt</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>Problem</li> 
        <li>Uppgifter</li>
        <li>Dokument</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

*Du kan lägga till och visa uppdateringar av kort i styrelsegena när du aktiverar avsnitten Kommentarer och Systemaktivitet på ett kort. Mer information finns i [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

<!--enable this when we release the new update stream to ALL other objects and only if Anna's bug was fixed to include this: 

* The following objects don't have a System Activity tab:

  * Team
  * Template
  * Template Task
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

Du kan inte uppdatera team. Uppdateringsavsnittet för team fylls i av uppdateringar som anges för följande objekt:

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

<!--might need to update this note when the new commenting experience will be the only experience; also - how will this affect the areas that will keep the old experience, like Iterations?-->

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
