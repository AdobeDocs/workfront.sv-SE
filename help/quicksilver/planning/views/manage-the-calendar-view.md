---
title: Hantera kalendervyn
description: Du kan visa poster och deras fält i en kalendervy. I den här artikeln beskrivs hur du skapar en kalendervy och redigerar eller tar bort en befintlig.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '1624'
ht-degree: 0%

---

# Hantera kalendervyn

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan visa poster och deras fält i en kalendervy från posttypssidan.

Mer information om Adobe Workfront Planning-vyer och hur du hanterar dem finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard för att skapa och ta bort vyer</p>
   <p>Medarbetare eller högre för att uppdatera vyelement</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en vy</p>  
   <p>Visa behörigheter till en vy om du tillfälligt vill ändra visningsinställningarna eller duplicera den</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hantera en kalendervy {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tänk på följande:

* Du kan bara skapa en kalendervy om du har minst två datumfält kopplade till en posttyp. När du har ett eller inga datumfält kopplade till en posttyp är alternativet Kalendervy nedtonat.

  Du kan välja från postdatumfält eller uppslagsdatumfält från anslutna post- eller objekttyper.
* Följande scenarier finns:

   * När både start- och slutdatum saknar värden visas inte posterna i kalendern
   * När start- eller slutdatumet saknar värde visas posten som en endagshändelse
   * När startdatumet är efter slutdatumet visas inte posten i kalendern.

Så här hanterar du en kalendervy:

1. Gå till den posttypssida som du vill visa kalendern för.
1. Skapa en kalendervy enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exempel på kalendervy](assets/calendar-view-example.png)

   Posterna som är associerade med den posttyp som du har valt visas som staplar i en kalender. Färgen på staplarna matchar färgen på postikonen som standard.

1. Navigera i kalendern genom att göra något av följande:

   * Klicka på ikonerna till vänster och höger i kalenderns övre vänstra hörn eller använd den vågräta rullningen för att flytta bakåt och framåt i kalendern.
   * Klicka på **Idag** i det övre högra hörnet om du vill centrera kalendern till dagens datum.
   * Välj något av följande alternativ på den nedrullningsbara menyn för tidsram för att uppdatera tidsstegen:

      * **Månad**: Posterna visas i en månadskalender.

      * **Vecka**: Posterna visas i följande områden:

         * Poster som sträcker sig över flera dagar visas högst upp i kalendern.
         * Poster som varar en dag eller mindre visas i den nedre halvan av kalendervyn. Om du valde att visa timmen för Start- och slutdatum visas posten vid lämplig tidpunkt under dagen då den inträffar.

1. <span class="preview">(Valfritt) Klicka på ikonen **Helskärm** ![Öppna helskärmsikonen](assets/open-full-screen-icon.png) om du vill öppna vyn i helskärmsläge och sedan på ikonen **Avsluta helskärm** ![Avsluta helskärmsikonen](assets/exit-full-screen-icon.png) eller Esc om du vill avsluta helskärmsläget.  </span>

1. Uppdatera följande vyelement enligt beskrivningen i underavsnitten nedan:
   * [Filter](#add-filters)
   * [Inställningar](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Lägg till filter

Du kan minska mängden information som visas på skärmen genom att använda filter.

Tänk på följande när du arbetar med filter i kalendervyn:

<!-- this list is almost identical to the one for the table view - update both-->

* De filter du skapar för en kalendervy fungerar oberoende av filtren i andra vyer som används för samma posttyp.

* Filtren är unika för den vy du väljer. Två kalendervyer av samma posttyp kan ha olika filter.

* Två användare som tittar på samma kalendervy ser samma filter som används för närvarande.

* Du kan inte namnge filtren som du skapar för en kalendervy.

* När du tar bort filter tas de bort från alla som använder samma posttyp som du och som visar samma vy som du.

* Du kan filtrera efter anslutna postfält eller uppslagsfält.

* Du kan filtrera efter uppslagsfält som visar flera värden.

Så här lägger du till ett filter i en kalendervy:

1. Skapa en kalendervy för en posttypsida, enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Markera en kalendervy och klicka sedan på **Filter** i tabellens övre högra hörn.
1. Klicka på **Lägg till villkor** och lägg till följande information:

   * **Markera ett fält** som du vill filtrera efter <!-- the tip below might change-->

   * **Välj ett alternativ** (eller en filtermodifierare) för att definiera vilken typ av villkor fältet måste uppfylla

     Tabellen nedan visar tillgängliga modifierare för varje typ av fält.

     <table>
        <thead>
        <tr>
            <th><b>Fälttyp</b></th>
            <th><b>Modifierare</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Enkelrad, Stycke, Formel </td>
            <td><p>Innehåller</p>
            <p>Innehåller inte</p>
            <p>Är</p>
            <p>Är inte</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr><td>Enkelval</td>
            <td><p>Är</p>
            <p>Är inte</p>
            <p>Är något av</p>
            <p>Är inget av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Flera val, personer</td>
            <td><p>Har någon av</p>
            <p>Har alla</p>
            <p>Är exakt</p>
            <p>Har ingen av</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Antal, Procentandel, Valuta</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Är tom</p>
            <p>Är inte tom</p></td>
        </tr>
        <tr>
            <td>Datum</td>
            <td><p>Är</p>
            <p>Är inte</p>
            <p>Är efter</p>
            <p>Är före</p>
            <p>Är mellan</p><p>Är inte mellan</p>
            <p>Är tom</p><p>Är inte tom</p></td>
        </tr>

     <tr>
            <td>Kryssruta</td>
            <td><p>Är</p>
        </tr>
        </tbody>
        </table>

   * Välj ett värde för det markerade fältet.

   ![Filtrera gränssnittstabellvy](assets/filter-ui-table-view.png)

   Det finns ingen gräns för hur många filtreringsvillkor du kan lägga till.

1. (Valfritt) Klicka på **Lägg till villkor** om du vill lägga till ytterligare ett filtreringsalternativ och upprepa stegen ovan. Antalet filter som används visas till vänster om filterikonen.
1. Klicka på följande operatorer för att ange hur filtervillkoren ska kopplas och användas:

   * **AND**: Alla angivna villkor måste uppfyllas.
   * **OR**: Alla angivna villkor måste vara uppfyllda. Det här är standardalternativet.

   1. (Valfritt) Lägg till ytterligare **AND**- eller **OR**-operatorer mellan flera villkorsgrupperingar.

      ![Filter med flera nivåer i vyer](assets/multi-tiered-filters-in-views.png)

   Postlistan filtreras automatiskt.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Valfritt) Klicka på ikonen **x** för att ta bort ett filtervillkor.
1. (Valfritt) Klicka på **Filter** för att stänga filterrutan. <!--right now you cannot "clear all" for filters, but this might come later-->

### Redigera inställningar för kalendervyn

Uppdatera inställningarna för kalendervyn för att ange vad och hur information visas i vyn.

1. Skapa en kalendervy för en posttyp enligt beskrivningen i artikeln [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicka på **Inställningar**.
1. Klicka på **Datum och tid** i den vänstra panelen och välj sedan ett **Startdatum** och ett **slutdatum** som ska visas i kalendern. Du kan välja standarddatum för start och slut eller välja ett tillgängligt datumfält.

   De staplar som representerar posterna börjar på det datum som du anger som startdatum och slutar på det datum som motsvarar slutdatumet.

   >[!NOTE]
   >
   >* Poster som inte har några värden för start- eller slutdatum eller som har ett startdatum efter slutdatumet visas inte i kalendervyn.
   >
   >* Om du visar ytterligare poster med alternativet Uppdelning är start- och slutdatumen huvudpostens. Du kan inte välja start- och slutdatum för de anslutna posterna i det här området.

1. Klicka på **Stapelformat** i den vänstra panelen för att ange vilken information du vill visa i postfälten.

   Postens primära fält (eller rubrik), enligt postens tabellvy, är markerat som standard.
   <!--adjust this when the primary field is released??-->

1. (Valfritt och villkorligt) Om du har lagt till miniatyrbilder till poster markerar du alternativet **Miniatyrbild** för att visa den bild som är associerad med posterna i deras postfält.

   >[!NOTE]
   >
   >    Du måste lägga till miniatyrbilder i tabellvyn innan du kan visa dem i kalendervyn. Mer information finns i [Lägga till en miniatyrbild i en post](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Klicka på **Lägg till fält**, klicka i rutan **Sök fält** och klicka på det fält som du vill lägga till.

   >[!TIP]
   >
   >   * Du måste skapa fälten innan du kan lägga till dem i postfälten.
   > 
   >   * Du måste ha minst ett fält markerat. **Namn** är markerat som standard.
   >
   >   * Du kan lägga till upp till fem fält.

   En förhandsvisning av hur fälten kommer att se ut i kalendern visas till höger.

   ![Stolpstilsavsnittet i inställningarna för kalendervyn](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. Klicka på **Färg** i den vänstra panelen om du vill anpassa färgerna för posterna i kalendern.

   ![Färgpanelen i inställningarna för kalendervyn](assets/color-panel-on-calendar-view-settings.png)

1. I avsnittet **Ange postfärg till** väljer du bland följande alternativ för att ange en färg för posterna:

   * **Posttyp**: Färgen på postfälten i kalendern matchar färgen på den posttyp du valde. Det här är standardalternativet.
   * **Fältvärden**: Färgen på posterna matchar färgen i ett fält som du anger.
   * **Ingen**: Posterna visas i ett vitt fält.

1. (Villkorligt) Om du valde **Fältvärden** för postfärgerna väljer du ett fält i listrutan **Matcha postfärgen till**.

   ![Listrutan Fältväljare för kalendervyn](assets/field-selector-drop-down-menu-calendar-view.png)

   Endast fält med färgkodade alternativ visas i listrutan.

   Flervalsfält eller envalsfält kan t.ex. ha färgkodade alternativ.

   Om du inte har något fält med färgkodade alternativ för den valda posttypen är det här alternativet nedtonat.


1. Klicka på **Spara**.

   Posterna visas i kalendervyn med de specifikationer som du har valt.