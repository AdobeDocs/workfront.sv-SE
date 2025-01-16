---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Lägga till ett diagram i en rapport
description: Du kan förbättra dina rapporter genom att lägga till ett diagram. Du kan lägga till diagram i befintliga rapporter eller i rapporter som du skapar.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '2734'
ht-degree: 0%

---

# Lägga till ett diagram i en rapport

<!--Audited: 11/2024-->

Du kan förbättra dina rapporter genom att lägga till ett diagram. Du kan lägga till diagram i befintliga rapporter eller i rapporter som du skapar.

Innan du lägger till ett diagram i en rapport bör du skapa en vy och en gruppering för rapporten.

Du kan inte lägga till diagram i de flesta rapporter om du inte först grupperar informationen i rapporten. Det enda diagram som kan läggas till utan gruppering är ett mätardiagram.

Mer information om vyer finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Mer information om grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Om rapporten innehåller för många objekt skapas inget diagram. I det här fallet måste du också lägga till ett filter i rapporten för att minska antalet resultat i rapporten.

Mer information om filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägga till ett diagram i en rapport

1. Gå till en befintlig rapport eller skapa en ny rapport. Mer information om hur du skapar en ny rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. (Villkorligt) Om du gick till en befintlig rapport klickar du på **Rapportera åtgärder** > **Redigera**.

1. Kontrollera att fliken **Kolumner (Visa)** har uppdaterats för att visa den information som du vill att diagrammet ska innehålla i rapporten.

   Mer information om hur du skapar eller ändrar rapportvyn finns i [Skapa eller redigera vyer i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Klicka på fliken **Grupperingar** och lägg till en gruppering.

   >[!TIP]
   >
   >* Du kan bara lägga till ett diagram i en rapport när rapportresultaten grupperas.
   >* Grupperingar i textläge stöds inte i diagram. Mer information om grupperingar i textläge finns i [Redigera en gruppering i textläge](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Om du lägger till en enda gruppering som representerar ett mätvärde, visas alla diagram utom ett cirkeldiagram som gruppering med samma färg.

   Mer information om hur du skapar grupperingar finns i [Skapa grupperingar i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Välj fliken **Diagram**.

1. Klicka på en diagramtyp för att markera den.\
   ![Val av diagramtyp](assets/unshimmed-report-builder-chart.png)

1. Välj bland följande diagramtyper:

   * [Kolumndiagram](#column-chart)
   * [Stapeldiagram](#bar-chart)
   * [Cirkeldiagram](#pie-chart)
   * [Linjediagram](#line-chart)
   * [Mätdiagram](#gauge-chart)
   * [Bubbeldiagram](#bubble-chart)

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

### Kolumndiagram {#column-chart}

Så här lägger du till ett **kolumndiagram** i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel. Välj sedan hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**.

1. (Valfritt) Klicka på **Egna färger** om du vill tilldela önskade färger till var och en av kolumnerna.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. I fältet **Underaxel (X)** väljer du den gruppering som du vill ta med i diagrammet.

1. (Valfritt) Klicka på **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.

1. (Valfritt) **Gruppera kolumner**: Välj det här alternativet om du vill definiera hur du vill att kolumnerna ska grupperas.\
   Välj bland följande alternativ:

   * Klicka på något av följande alternativ för att välja hur de grupperade kolumnerna ska visas:

      * **Sida vid sida**
      * **Staplad**
      * **Staplad till 100 %**

   * Välj den gruppering som du vill ta med i diagrammet i listrutan **Gruppera data efter**.
   * (Valfritt) Klicka på **Egna färger** om du vill anpassa färgerna i kolumnerna.\
     Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Klicka på **Kombinationsdiagram** om du vill inkludera ett ytterligare värde i diagrammet, samt hur du vill att informationen ska sammanfattas.\
   Tänk på följande alternativ:

   * **Rita på sekundär axel**: Välj det här alternativet om du vill rita data till höger om diagrammet.
   * **Diagramtyp**: Välj om du vill att det här extra värdet ska visas som en rad eller en tredje kolumn.

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

### Stapeldiagram {#bar-chart}

Så här lägger du till ett **liggande**-diagram i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Nederkant (X) axel** markerar du de värden som du vill inkludera på diagrammets X-axel och väljer sedan hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**.

1. (Valfritt) Klicka på **Egna färger** om du vill anpassa fältens färger.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. I fältet **Vänster (Y) axel** markerar du den gruppering som du vill ta med i diagrammet.

1. (Valfritt) Klicka på **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.

1. (Valfritt) Klicka på **Grupperingsfält** för att definiera hur du vill att staplarna ska grupperas.\
   Välj bland följande alternativ:

   * Klicka på något av följande alternativ för att välja hur de grupperade fälten ska visas:

      * **Sida vid sida**
      * **Staplad**
      * **Staplad till 100 %**

   * Välj hur du vill gruppera informationen i diagrammet från den nedrullningsbara menyn **Gruppera data efter**.
   * (Valfritt) Klicka på **Egna färger** om du vill anpassa färgerna i kolumnerna.\
     Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Klicka på **Kombinationsdiagram** om du vill inkludera ett ytterligare värde i diagrammet, samt hur du vill att informationen ska sammanfattas.

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

>[!IMPORTANT]
>
>Begränsa stapeldiagram till 23 eller färre staplar, eftersom stapeldiagram som innehåller fler än 23 staplar inte visar alla stapeletiketter korrekt.

### Cirkeldiagram {#pie-chart}

Så här lägger du till ett **cirkeldiagram** i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Värden** markerar du de värden som du vill ska visas i rapporten och väljer sedan hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**.\
   I fältet **Bröllop** väljer du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av diagrammets segment.

1. (Valfritt) Klicka på **Egna färger** om du vill anpassa färgerna i sektorerna i diagrammet.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Klicka på **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.

1. I fältet **Visa resultat som** väljer du hur du vill att resultaten ska visas i diagrammet. Tänk på följande alternativ:

   * **Procent**: Diagramresultatet visas i procent.
   * **Nummer**: Diagramresultatet visas som ett tal.

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

### Linjediagram {#line-chart}

Så här lägger du till ett **Line**-diagram i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel. Välj sedan hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**.

1. I fältet **Underaxel (X)** väljer du den gruppering som du vill ta med i diagrammet.

1. (Valfritt) Klicka på **Gruppera rader** om du vill välja ytterligare en gruppering för diagrammet.\
   (Valfritt) Klicka på **Egna färger** om du vill anpassa färgerna för den nya grupperingen.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Klicka på **Kombinationsdiagram** om du vill kombinera raderna med ett ytterligare värde.\
   Tänk på följande alternativ:

   * Välj det värde som du vill inkludera i diagrammet samt hur du vill att informationen ska sammanfattas.
   * Klicka på fältet **Rita på sekundär axel** för att rita data till höger om diagrammet.

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

### Mätdiagram {#gauge-chart}

Ett **Mätardiagram** visar antalet poster som uppfyller vissa villkor i ett mätformat. Indikatorn för mätaren pekar på antalet poster som uppfyller de villkor som valts i vyn och rapportgrupperingen. Ingen rapportgruppering krävs för att konfigurera ett mätdiagram.

Så här lägger du till ett **Gage**-diagram i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Värden** markerar du de värden som du vill ska visas i rapporten och väljer sedan hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**. Om du väljer **Antal poster** är de värden som visas rapportens objekt.

1. I fältet **Indikatorer** väljer du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av indikatorraden i diagrammet.\
   Om du har en gruppering som innehåller två objekt visas två indikatorer i diagrammet.\
   Om du t.ex. har en gruppering av projektstatus och det finns två projektstatusvärden (Aktuell och Väntande), innehåller mätdiagrammet två mätningsindikatorer. De pekar på antalet projekt som har den statusen.\
   (Valfritt) Välj **Totalt** i fältet **Indikatorer** om du vill visa det totala antalet markerade objekt i fältet **Värden**.

1. (Valfritt) Klicka på **Lägg till ett annat värdeintervall** om du vill lägga till ett värdeintervall i diagrammet.

1. (Valfritt) I fältet **Värdeintervall** anger du värdeintervallet och färgen som ska representera dessa värden som ska visas i mätardiagrammet.

1. Klicka på **Spara + stäng** för att spara diagrammet och rapporten.

### Bubbeldiagram {#bubble-chart}

Du kan visa upp till tre fält för ett objekt i ett **bubbeldiagram**. Det innebär att du kan visa upp till fyra datapunkter i ett bubbeldiagram. Varje entitet med tre associerade fält visas som en cirkel som uttrycker två av fälten inom dess plats inom X- och Y-axlarna. Det tredje fältet representeras av cirkelns storlek.

Så här lägger du till ett **bubbeldiagram** i rapporten:

1. Börja lägga till ett diagram i rapporten, enligt beskrivningen i [Lägg till ett diagram i en rapport](#add-a-chart-to-a-report).

1. I fältet **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas i fältet **Sammanfattad av**.

1. I fältet **Underaxel (X)** markerar du de värden som du vill ta med på diagrammets X-axel. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas.

   >[!NOTE]
   >
   >Se till att du har minst en kolumn som är summerad för att fältet ska vara aktivt.\
   >Mer information om att sammanfatta informationen i en rapportkolumn finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. I fältet **Bubbelstorlek** väljer du de värden som du vill representera med storleken på bubblorna i diagrammet. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas.

   >[!NOTE]
   >
   >Se till att du har minst en kolumn som är summerad för att fältet ska vara aktivt.\
   >Mer information om att sammanfatta informationen i en rapportkolumn finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. I fältet **Bubbles** markerar du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av placeringen av bubblorna i diagrammet.

1. I fältet **Bubbelfärg** markerar du det fält som du vill ska representeras av bubblornas färger.

   **Bubbelfärg** kan vara en gruppering som du definierar i rapporten, men alternativet är bara tillgängligt om du väljer en gruppering i fältet **Bubbles** som innehåller **Name** för ett överordnat objekt i förhållande till rapportens objekt, till exempel **Projektnamn** för en aktivitetsrapport eller **Programnamn** för en projektrapport.

   Om du till exempel har valt **Projektnamn** i en aktivitetsrapport kan du lägga till **Aktivitetsstatus** som **Bubbelfärg**-fält.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Om du däremot valde **Aktivitetsstatus** för fältet **Bubbles** kan du inte välja ett **Bubbelfärg** -fält. Du kan inte heller välja **Projektnamn** för fältet **Bubbelfärg**, även om du väljer **Projektnamn** för fältet **Bubbles** .

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)

1. Klicka på **Spara + Stäng** för att spara ändringarna i gränssnittsverktyget.

## Anpassa diagramfärger {#customize-chart-colors}

Du kan låta Workfront välja färgerna för elementen i diagrammet eller anpassa dem medan du lägger till ett diagram i rapporterna. Om diagrammet innehåller en enda gruppering som representerar ett mått, t.ex. en uppgiftsrapport som visar antalet uppgifter grupperade efter faktiskt slutförandedatum, visas varje resultat i grupperingen i samma färg.

Du kan bara välja en färg för fält som visas i rapportvyn. Du kan välja flera färger - en för varje alternativ - för fält som visas i rapportens gruppering.

>[!IMPORTANT]
>
>För datumfält kan du bara välja en färg för diagramelementen.

Så här anpassar du diagramfärger:

1. Gå till fliken **Diagram** i Report Builder när du skapar en rapport.

1. Välj en diagramtyp som du vill lägga till i rapporten.\
   Mer information om hur du lägger till ett diagram i rapporten finns i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).

1. Klicka på **Egna färger** när det här fältet är tillgängligt.\
   Dialogrutan Egna färger visas.\
   ![](assets/unshimmed-custom-colors-in-charts.png)

   >[!NOTE]
   >
   >Du kan associera anpassade färger med fält som du kan gruppera efter och med vissa fält som kan visas i en vy, inklusive anpassade fält. De anpassade fälten eller anpassade alternativen för fälten som du väljer i dialogrutan Egen färg är skiftlägeskänsliga.

1. Välj något av följande alternativ:

   * **Använd en färg**: Alla element i diagrammet visas i den valda färgen.
   * **Lägg till färg**: Lägg till en anpassad färg för ett möjligt värde för det valda fältet.
   * **Ta bort alla**: Välj det här alternativet om du vill ta bort alla fältvärden och färger som anges ovan.
   * **Inget värde**: Markera det här fältet och en anpassad färg för att visa diagramkolumnen som grupperar&quot;inget värde&quot;-objekt. Det här är objekt som inte kan grupperas efter något av alternativen i det fält som är markerat i din gruppering.
   * **Alla andra värden**: Markera det här fältet och en anpassad färg om du vill visa alla andra diagramelement vars alternativ inte definieras ovan.

     >[!NOTE]
     >
     >De senast redigerade färgerna visas till höger om knappen **Egna färger** . När du för musen över en färg visas namnet på det fält som är associerat med den. Du kan också klicka på en färg om du vill redigera den utan att öppna **Anpassade färger** igen.

1. Välj en färg:
Klicka inuti färgväljaren för att välja en färg.
ELLER
Ange ett hexadecimalt färgvärde för färgen.

1. Klicka var som helst utanför dialogrutan Egna färger för att stänga den. Färgerna som du har valt sparas automatiskt.

1. Klicka på **Spara + stäng** för att spara diagrammet och köra rapporten.

## Exportera ett diagram

Du kan exportera ett diagram till en PDF-fil.

Så här exporterar du ett diagram:

1. Klicka på **Exportera** på diagramfliken i en rapport om du vill exportera diagrammet till .pdf.\
   En pdf-fil laddas ned till datorn.

1. Öppna PDF-filen.\
   Den exporterade filen innehåller följande information:

   * En bild av diagrammet.
   * En titel som är rapportens namn.
   * Ett unikt filnamn som baseras på rapportens namn.
   * En sidfot med datum och tid då rapporten exporterades och sidnumret.

## Ta bort ett diagram från en rapport

Så här tar du bort ett diagram från en rapport:

1. Öppna fliken **Diagram** i Report Builder.

1. Klicka på x-knappen till höger om diagramtyperna för att ta bort diagrammet.

1. Klicka på **Spara + Stäng**.

## Begränsningar när du arbetar med diagram

Tänk på följande begränsningar när du arbetar med diagram:

* Avsnittet **Förhandsgranska diagram** till höger om rapportverktyget innehåller inga faktiska data från din rapport. Du måste spara diagrammet och visa det på fliken **Diagram** för att kunna se diagrammet med dina data.

* Vissa diagramelement kan inte redigeras:

   * Du kan inte ändra teckensnittstypen eller storleken på värdena för varje element.
   * Du kan inte ändra namn på axlarna i diagrammet.

* Det går inte att redigera teckenförklaringen.
* När du använder beräkningsfält för dina grupperingar kan du inte klicka på diagramelementen.
* Det största antalet datapunkter som du kan visa i ett diagram är fyra i ett bubbeldiagram. Alla andra diagramtyper visar två eller högst tre datapunkter.
