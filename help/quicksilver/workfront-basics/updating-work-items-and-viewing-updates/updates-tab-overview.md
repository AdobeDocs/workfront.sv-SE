---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Översikt över uppdateringsavsnittet
description: I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Översikt över uppdateringsavsnittet

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

>[!NOTE]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>
>Mer information om de nya kommentarfunktionerna finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Du kommer åt den nya funktionen för följande objekt:
> * Problem när du aktiverar kommenteringsfunktionen Beta.
   >
   >     Den här funktionen är bara tillgänglig för uppdateringsavsnittet av utgåvor och är inte tillgänglig för följande områden:
   >
   >     * Startsida
   >     * Panelen Sammanfattning i listor
   >     * Sammanfattningspanelen i tidrapporter
>
> * Mål

   >
   >   Den nya kommentarsfunktionen är standardinställningen för målen. Du måste ha ytterligare en licens för att få tillgång till Workfront Goals. Mer information finns i [Krav för användning av Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Mer information om att kommentera mål finns i [Hantera målkommentarer i Adobe Workfront-mål](../../workfront-goals/goal-management/manage-goal-comments.md).


I uppdateringsavsnittet för ett objekt visas kommentarer som användare gör på objektet eller systemuppdateringar som spårar ändringar i objektet.

## Översikt över uppdateringsavsnittet

Informationen i uppdateringsavsnittet är organiserad på olika sätt beroende på vilken miljö du kommer åt den från.

### Översikt över aktuellt uppdateringsavsnitt

I uppdateringsavsnittet för ett objekt visas upp till 200 av de senaste uppdateringarna under de senaste 90 dagarna.

![](assets/updates-tab-before-unified-experience-for-issues.png)

I det aktuella uppdateringsavsnittet visas följande information:

* Synpunkter från användare och svar på dessa kommentarer.
* Systemuppdateringar är informationsmeddelanden som Workfront skapar för att registrera vissa händelser för ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Uppdateringsavsnittet visas för följande objekt:

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

### Översikt över uppdateringsavsnittet i betakommentarsfunktionen

![](assets/updates-tab-after-unified-experience-for-issues.png)

I uppdateringsavsnittet visas information på följande flikar i den nya kommentarsfunktionen:

* **Kommentarer**: Visar kommentarer som gjorts av användare och svar på dessa kommentarer. Information om hur du uppdaterar objekt i den nya kommentarsfunktionen finns i [Uppdatera arbete](../updating-work-items-and-viewing-updates/update-work.md).
* **Systemaktivitet**: Visar systemuppdateringar som är informationsmeddelanden som Workfront skapar för att registrera vissa händelser för ett objekt. Du kan t.ex. fånga in ändringar i status, namn eller anpassade fält med systemuppdateringar. Din Workfront- eller gruppadministratör kan aktivera systemuppdateringar för dina objekt. Mer information finns i [Konfigurera systemuppdateringar](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

För närvarande kan du göra kommentarer och svara på uppdateringar med hjälp av betakommentarsfunktionen för följande objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><p>Mål</p>
     <p>Det här är standardupplevelsen för mål</p>
     </li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li>Problem</li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdateringar som också visas på objekt med högre rankning

Som framgår av följande tabell visas även svar på uppdateringar av vissa objekt i uppdateringsavsnittet för objekt med högre rankning.

När du till exempel lägger till en uppdatering för en uppgift visas uppdateringen i uppdateringsavsnittet för uppgiften och i uppdateringsavsnittet för projektet som innehåller uppgiften.

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
> Det går inte att svara på systemuppdateringar i den nya kommenteringsfunktionen Beta. Mer information finns i [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

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
