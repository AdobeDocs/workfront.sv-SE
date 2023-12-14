---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över uppdateringsavsnittet
description: I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 7b920a139689efe6c33f3a4bc495e5c5f270ebf4
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Översikt över uppdateringsavsnittet

<!--take "legacy" and "new commnenting" references out when we remove the legacy - Jan 2024???-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - Jan 2024???-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. </span>

<span class="preview">Information om det aktuella releaseschemat finns i [Första utgåvan, kvartal 2024, översikt](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>


>[!IMPORTANT]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Beroende på vilka objekt du har tillgång till kommentarfunktionerna för kan du se följande funktionalitet för uppdateringsavsnittet:
>* Den nya upplevelsen
>* Den gamla upplevelsen
>* Det nya och gamla gränssnittet
>
>Den här artikeln innehåller information om de nya och äldre versionerna av uppdateringsavsnittet.
>
>Mer information om den nya kommentarsfunktionen och dess tillgänglighet finns på [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Den nya kommentarsupplevelsen är bara tillgänglig för uppdateringsavsnittet för Workfront-objekt och är inte tillgänglig när du öppnar objekt från följande områden:
>
> * Startsida
> * Panelen Sammanfattning i listor
> * Sammanfattningspanelen i tidrapporter

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->


## Översikt över uppdateringsavsnittet

I uppdateringsavsnittet för ett objekt visas systemuppdateringar och upp till 200 av de senaste uppdateringarna som användare har gjort under de senaste 90 dagarna.

<span class="preview">![](assets/updates-tab-after-unified-experience-for-issues.png)</span>

Beroende på vilka objekt du har tillgång till kommentarfunktionerna för kan du hitta följande i uppdateringsavsnittet:

* Både den nya och gamla kommentarsfunktionen för följande objekt:

   * Projekt
   * Uppgift (här ingår artiklar)
   * Problem
   * Dokument

     >[!TIP]
     >
     >Använd alternativet Ny kommentering för att visa den nya kommentarsfunktionen (när du aktiverar den) eller den gamla kommentarsfunktionen (när du inaktiverar den). Den nya kommentarsfunktionen är standard. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Bara den nya kommentarsfunktionen för objekten som listas nedan. Det finns inget alternativ för att aktivera den gamla kommentarfunktionen för dessa objekt:

   * Mål

     >[!NOTE]
     >
     >Du måste ha ytterligare en licens för Adobe Workfront Goals för att få tillgång till det här området av Workfront. Mer information finns i [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * Kort ombord
   * Team
   * Mall
   * Malluppgift
   * Tidrapport
   * Program
   * Portfolio
   * Användare

* Endast den äldre kommentarsfunktionen för följande objekt:

   * Iterationer

     Det finns inget alternativ för att aktivera den nya kommentarfunktionen för iterationer.

### Översikt över uppdateringsavsnittet i den nya kommentarsfunktionen

<span class="preview">![](assets/updates-tab-after-unified-experience-for-tasks.png)</span>

>[!NOTE]
>
>Den nya kommentarsfunktionen är inte tillgänglig för upprepningar.


* I uppdateringsavsnittet visas information på följande flikar i den nya kommentarsfunktionen:


   * **Kommentar**: Visar kommentarer från användare och svar på dessa kommentarer. Använd fliken Kommentarer för att lägga till nya kommentarer eller svara på befintliga kommentarer. Mer information om hur du uppdaterar objekt i den nya kommentarsfunktionen finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).
   * **Systemaktivitet**: Visar systemuppdateringar som är informationsmeddelanden som Workfront skapar för att registrera vissa händelser för ett objekt. Till exempel hämtas ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Följande objekt saknar fliken Systemaktivitet:

   * Team
   * Mall
   * Malluppgift
   * Ad hoc-kort


### Översikt över det äldre uppdateringsavsnittet

<!--when we remove legacy, make this section an "Iterations-only" section-->

![](assets/updates-tab-before-unified-experience-for-tasks.png)

I avsnittet med äldre uppdateringar visas följande information:

* **Användaruppdateringar**: Synpunkter från användare och svar på dessa kommentarer.
* **Systemuppdateringar**: Informationsmeddelanden som Workfront skapar för att spela in vissa händelser i ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Följande objekt registrerar inte systemuppdateringar:

* Team
* Mall
* Malluppgift
* Iterationer


## Uppdateringar som också visas på objekt med högre rankning

Kommentarer, svar eller systemuppdateringar för vissa objekt visas också i uppdateringsavsnittet för objekt med högre rankning.

När du till exempel lägger till en uppdatering för en uppgift visas uppdateringen i uppdateringsavsnittet för uppgiften och i uppdateringsavsnittet för projektet som innehåller uppgiften.

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
   <td><p>Användare, team</p>
   <p><b>ANMÄRKNING</b></p>
   <p>Tidrapportkommentarer visas i uppdateringsavsnittet för den användare som gör kommentaren och uppdateringsavsnittet i sin hemgrupp.</p>
   </td> 
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
   <td>Resultat</td> 
   <td>Mål</td> 
  </tr> 
  <tr> 
   <td>Aktivitet</td> 
   <td>Mål</td> 
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

Tänk på följande när du visar uppdateringar för användare och team:

* Du kan inte lägga till nya kommentarer i uppdateringsavsnittet i ett team.

* Du kan lägga till ett svar på en uppdatering som du visar i ett team. Svaret visas i teamets uppdateringsavsnitt samt i uppdateringsavsnittet för det objekt det tillhör.

* Uppdateringsavsnittet för team fylls i av uppdateringar som anges för följande objekt:

   * Användare
   * Tidrapporter*
   * Artiklar
   * Iterationer*

  *Dessa finns inte för den nya kommentarsfunktionen.

* I uppdateringsavsnittet för användare och team kan du visa de uppdateringar som har gjorts under de senaste 90 dagarna.

  Om du vill se alla uppdateringar som gjorts för en användare eller ett team, utöver 90-dagarsgränsen, kan du skapa en rapport för anteckningar. Rapporten ska inte ha något tidsfilter som visar alla uppdateringar som gjorts för användare eller team. Mer information finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Begränsningar när du skriver kommentarer för en annan användares räkning

Adobe Workfront-administratörer och gruppadministratörer kan logga in som andra användare och utföra åtgärder i Workfront som att skriva kommentarer.

Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Tänk på följande när du loggar in som en annan användare och lägger till kommentarer:

* Alla kommentarer som görs för en annan användares räkning anges i kommentaren.

* En gruppadministratör kan kommentera för en annan persons räkning, men kan inte ta bort kommentaren. Det är bara en Adobe Workfront-administratör som kan ta bort en kommentar som de har gjort för en annan användares räkning.

* En Workfront- eller gruppadministratör kan bara redigera en kommentar som de har lagt till för en annan användares räkning när de loggar ut som användare och sedan loggar in som sig själva. De kan inte ta bort en kommentar för en annan användares räkning.

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
