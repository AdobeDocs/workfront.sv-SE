---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över fliken Uppdateringar
description: På fliken Uppdateringar visas upp till 200 av de senaste uppdateringarna som har gjorts under de senaste 90 dagarna.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Översikt över fliken Uppdateringar

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

På fliken Uppdateringar visas upp till 200 av de senaste uppdateringarna som har gjorts under de senaste 90 dagarna.

Du kan kommentera och svara på uppdateringar för följande objekt:

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
     <li>Artiklar</li> 
     <li>Uppgifter</li> 
     <li>Mallar</li> 
     <li>Malluppgifter</li> 
     <li>Tidrapporter</li> 
     <li>Användare</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdateringar som också visas på objekt med högre rankning

Som framgår av följande tabell visas även svar på uppdateringar av vissa objekt på fliken Uppdateringar för objekt med högre rankning.

När du till exempel lägger till en uppdatering för en uppgift visas uppdateringen på fliken Uppdateringar för uppgiften och på fliken Uppdateringar för projektet som innehåller uppgiften.

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

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Begränsningar för fliken Uppdateringar

### Begränsningar för användare och team

Du kan inte uppdatera team. Fliken Uppdateringar för team fylls i av uppdateringar som anges för följande objekt:

* Användare
* Tidrapporter
* Artiklar
* Iterationer

På fliken Uppdateringar för användare och team kan du visa de uppdateringar som har gjorts under de senaste 90 dagarna.

Om du vill se alla uppdateringar som gjorts för en användare eller ett team, utöver 90-dagarsgränsen, kan du skapa en rapport för anteckningar. Rapporten ska inte ha något tidsfilter som visar alla uppdateringar som gjorts för användare eller team. Mer information finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Begränsningar när du skriver kommentarer för en annan användares räkning

Adobe Workfront-administratörer och gruppadministratörer kan logga in som andra användare och utföra åtgärder i Workfront som att skriva kommentarer. (Mer information finns i [Logga in som en annan användare](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Alla kommentarer som görs för en annan användares räkning anges i kommentaren.

En gruppadministratör kan kommentera för en annan persons räkning, men kan inte ta bort kommentaren. Det är bara en Adobe Workfront-administratör som kan ta bort en kommentar som de har gjort för en annan användares räkning.

## Visa systemuppdateringar för arbetsobjekt med journalpostrapporten

Journalanmälningsrapporten innehåller systemuppdateringar från uppdateringsområdet för projekt, uppgifter och utgåvor.

I rapporten kan du se:

* Hur många statusändringar som har gjorts
* När en uppgift eller ett problem togs bort
* Hur värden i viktiga anpassade fält ändrades under ett projekt
* Vilka viktiga datum som har ändrats under ett projekt
* Om prioritet ändras under ett projekt
* Om ägaren till ett projekt har ändrats

Mer information finns i [Rapport om uppdateringsområdet](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
