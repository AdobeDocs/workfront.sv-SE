---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Lägga till ett diagram i en rapport
description: Du kan förbättra dina rapporter genom att lägga till ett diagram. Du kan lägga till diagram i befintliga rapporter eller i rapporter som du skapar.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# Lägga till ett diagram i en rapport

<!--Audited: 01/2024-->

Du kan förbättra dina rapporter genom att lägga till ett diagram. Du kan lägga till diagram i befintliga rapporter eller i rapporter som du skapar.

Innan du lägger till ett diagram i en rapport bör du skapa en vy och en gruppering för rapporten.

Du kan inte lägga till diagram i de flesta rapporter om du inte först grupperar informationen i rapporten. Det enda diagram som kan läggas till utan gruppering är ett mätardiagram.

Mer information om vyer finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>Aktuell: Planera </p>
   eller
   <p>Nytt: Standard</p> </td> 
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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Lägga till ett diagram i en rapport

1. Gå till en befintlig rapport eller skapa en ny rapport. Mer information om hur du skapar en ny rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Villkorligt) Om du går till en befintlig rapport klickar du på **Rapportåtgärder** > **Redigera**.

1. Se till att **Kolumner (vy)** har uppdaterats för att visa den information som du vill diagramma i rapporten.

   Mer information om hur du skapar eller ändrar rapportens vy finns i [Skapa eller redigera vyer i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Klicka på **Grupperingar** och lägga till en gruppering.

   >[!TIP]
   >
   >* Du kan bara lägga till ett diagram i en rapport när rapportresultaten grupperas.
   >* Grupperingar i textläge stöds inte i diagram. Mer information om grupperingar i textläge finns i [Redigera textläge i en gruppering](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Om du lägger till en enda gruppering som representerar ett mätvärde, visas alla diagram utom ett cirkeldiagram som gruppering med samma färg.

   Mer information om hur du skapar grupperingar finns i [Skapa grupperingar i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Välj **Diagram** -fliken.
1. Klicka på en diagramtyp för att markera den.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Välj bland följande diagramtyper:

   * [Kolumndiagram](#column-chart)
   * [Stapeldiagram](#bar-chart)
   * [Cirkeldiagram](#pie-chart)
   * [Linjediagram](#line-chart)
   * [Mätdiagram](#gauge-chart)
   * [Bubbeldiagram](#bubble-chart)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

### Kolumndiagram {#column-chart}

Lägga till en **Kolumn** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel och hur du vill att informationen ska sammanfattas.
1. I **Nedre (X) axel** markerar du den gruppering som du vill ta med i diagrammet.
1. (Valfritt) Välj **Egna färger** om du vill tilldela dina önskade färger till varje kolumn.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.
1. (Valfritt) **Gruppera kolumner**: Välj det här alternativet om du vill definiera hur du vill att kolumnerna ska grupperas.\
   Välj bland följande alternativ:

   * Klicka på något av följande alternativ för att välja hur de grupperade kolumnerna ska visas:

      * **Sida vid sida**
      * **Skiktat**
      * **Staplad till 100 %**

   * Välj den gruppering som du vill ta med i diagrammet från **Gruppera data efter** listruta.
   * (Valfritt) Välj **Egna färger** om du vill anpassa kolumnernas färger.\
     Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Kombinationsdiagram** om du vill inkludera ytterligare ett värde i diagrammet, samt hur du vill att informationen ska sammanfattas.\
   Tänk på följande alternativ:

   * **Rita på sekundär axel**: Välj det här alternativet om du vill rita data till höger om diagrammet.
   * **Diagramtyp**: Välj om du vill att det här extra värdet ska visas som en rad eller som en tredje kolumn.\
     ![](assets/qs-column-chart-350x163.png)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

### Stapeldiagram {#bar-chart}

Lägga till en **Liggande** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Nedre (X) axel** markerar du de värden som du vill ta med på X-axeln i diagrammet samt hur du vill att informationen ska sammanfattas.
1. I **Vänster (Y) axel** markerar du den gruppering som du vill ta med i diagrammet.
1. (Valfritt) Välj **Egna färger** om du vill anpassa fältens färger.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.
1. (Valfritt) Välj **Gruppfält** för att definiera hur du vill att staplarna ska grupperas.\
   Välj bland följande alternativ:

   * Klicka på något av följande alternativ för att välja hur de grupperade fälten ska visas:

      * **Sida vid sida**
      * **Skiktat**
      * **Staplad till 100 %**

   * Välj hur du vill gruppera informationen i diagrammet från **Gruppera data efter** listruta.
   * (Valfritt) Välj **Egna färger** om du vill anpassa färgerna i kolumnerna.\
     Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Kombinationsdiagram** om du vill inkludera ytterligare ett värde i diagrammet, samt hur du vill att informationen ska sammanfattas.\
   ![](assets/qs-bar-chart-350x167.png)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

>[!IMPORTANT]
>
>Begränsa stapeldiagram till 23 eller färre staplar, eftersom stapeldiagram som innehåller fler än 23 staplar inte visar alla stapeletiketter korrekt.

### Cirkeldiagram {#pie-chart}

Lägga till en **Cirkel** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Värden** markerar du de värden som du vill ska visas i rapporten samt hur du vill att de ska sammanfattas.\
   I **Bröllop** markerar du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av diagrammets segment.

1. (Valfritt) Välj **Egna färger** om du vill anpassa färgerna för sektorerna i diagrammet.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Visa i 3D** om du vill visa diagrammet i en tredimensionell vy.
1. I **Visa resultat som** väljer du hur du vill att resultaten ska visas i diagrammet. Tänk på följande alternativ:

   * **Procent**: Diagramresultatet visas i procent.
   * **Nummer**: Diagramresultatet visas som ett tal.\
     ![](assets/qs-pie-chart-350x171.png)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

### Linjediagram {#line-chart}

Lägga till en **Linje** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel och hur du vill att informationen ska sammanfattas.
1. I **Nedre (X) axel** markerar du den gruppering som du vill ta med i diagrammet.
1. (Valfritt) Välj en färg för att anpassa linjens färg.
1. (Valfritt) Välj **Gruppera rader**, om du vill välja ytterligare en gruppering för diagrammet.\
   (Valfritt) Välj **Egna färger** om du vill anpassa färgerna för den nya grupperingen.\
   Mer information om hur du anpassar diagramfärger finns i [Anpassa diagramfärger](#customize-chart-colors).

1. (Valfritt) Välj **Kombinationsdiagram** för att kombinera raderna med ett extra värde.\
   Tänk på följande alternativ:

   * Välj det värde som du vill inkludera i diagrammet samt hur du vill att informationen ska sammanfattas.
   * Välj **Rita på sekundär axel** för att rita data till höger om diagrammet.\
     ![](assets/qs-line-chart-350x172.png)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

### Mätdiagram {#gauge-chart}

A **Mätare** visar antalet poster som uppfyller vissa villkor i ett mätformat. Indikatorn för mätaren pekar på antalet poster som uppfyller de villkor som valts i vyn och rapportgrupperingen. Ingen rapportgruppering krävs för att konfigurera ett mätdiagram.

Lägga till en **Mätare** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Värden** markerar du de värden som du vill ska visas i rapporten samt hur du vill att de ska sammanfattas. Om du väljer **Antal poster**, är de värden som visas objektet i rapporten.

1. I **Indikatorer** markerar du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av indikatorraden i diagrammet.\
   Om du har en gruppering som innehåller två objekt visas två indikatorer i diagrammet.\
   Om du t.ex. har en gruppering av projektstatus och det finns två projektstatusvärden (Aktuell och Väntande), innehåller mätdiagrammet två mätningsindikatorer. De pekar på antalet projekt som har den statusen.\
   (Valfritt) Välj **Totalt** i **Indikatorer** fält för att visa det totala antalet markerade objekt i **Värden** fält.

1. I **Värdeintervall** anger du värdeintervall och färg för dessa värden som ska visas i mätardiagrammet.
1. (Valfritt) Klicka på **Lägg till ett annat värdeintervall** om du vill lägga till ytterligare värdeintervall i diagrammet.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Klicka **Spara + Stäng** för att spara diagrammet och rapporten.

### Bubbeldiagram {#bubble-chart}

Du kan visa upp till tre fält för ett objekt i en **Bubbla** diagram. Det innebär att du kan visa upp till fyra datapunkter i ett bubbeldiagram. Varje entitet med tre associerade fält visas som en cirkel som uttrycker två av fälten inom dess plats inom X- och Y-axlarna. Det tredje fältet representeras av cirkelns storlek.

Lägga till en **Bubbla** till rapporten:

1. Börja lägga till ett diagram i rapporten enligt beskrivningen i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).
1. I **Vänster (Y) axel** markerar du de värden som du vill ta med på diagrammets Y-axel. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas.
1. I **Nedre (X) axelfält** markerar du de värden som du vill ta med på X-axeln i diagrammet. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas.

   >[!NOTE]
   >
   >Se till att du har minst en kolumn som är summerad för att fältet ska vara aktivt.\
   >Mer information om hur du sammanfattar informationen i en rapportkolumn finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. I **Bubbelstorlek** markerar du de värden som du vill representera med storleken på bubblorna i diagrammet. Värdena kommer från rapportvyn. Ange hur du vill att informationen ska sammanfattas.

   >[!NOTE]
   >
   >Se till att du har minst en kolumn som är summerad för att fältet ska vara aktivt.\
   >Mer information om hur du sammanfattar informationen i en rapportkolumn finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. I **Bubblor** markerar du den gruppering som du vill ta med i diagrammet. Grupperingen representeras av placeringen av bubblorna i diagrammet.
1. I **Bubbelfärg** markerar du det fält som du vill ska representeras av bubblornas färger.

   ![](assets/qs-bubble-chart-350x103.png)


   The **Bubbelfärg** kan vara en gruppering som du definierar i rapporten, men den är bara tillgänglig när du väljer **Namn** kolumn för rapportens objekt i **Bubblor** fält.

   Om du till exempel har valt **Aktivitetsnamn** i en uppgiftsrapport kan du lägga till **Aktivitetsstatus** som **Bubbelfärg** fält.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Men om du har valt **Aktivitetsstatus** för **Bubblor** fält kan du inte välja **Bubbelfärg** fält. Du kan inte heller välja **Projektnamn** för **Bubbelfärg** fält, även när du markerar **Aktivitetsnamn** för **Bubbla** fält.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)


1. Klicka **Spara + Stäng** om du vill spara ändringarna i gränssnittsverktyget.

## Exportera ett diagram

Du kan exportera ett diagram till en PDF-fil.

Så här exporterar du ett diagram:

1. Klicka **Exportera** om du vill exportera diagrammet till .pdf.\
   En pdf-fil laddas ned till datorn.

1. Öppna PDF-filen.\
   Den exporterade filen innehåller följande information:

   * En bild av diagrammet.
   * En titel som är rapportens namn.
   * Ett unikt filnamn som är rapportens namn.
   * En sidfot med datum och tid då rapporten exporterades och sidnumret.

## Anpassa diagramfärger {#customize-chart-colors}

Du kan låta Workfront välja färgerna för elementen i diagrammet eller anpassa dem medan du lägger till ett diagram i rapporterna. Om diagrammet innehåller en enda gruppering som representerar ett mått, t.ex. en uppgiftsrapport som visar antalet uppgifter grupperade efter faktiskt slutförandedatum, visas varje resultat i grupperingen i samma färg.

Du kan bara välja en färg för fält som visas i rapportvyn. Du kan välja flera färger - en för varje alternativ - för fält som visas i rapportens gruppering.

>[!IMPORTANT]
>
>För datumfält kan du bara välja en färg för diagramelementen.

Så här anpassar du diagramfärger:

1. Gå till **Diagram** i Report Builder.
1. Välj en diagramtyp som du vill lägga till i rapporten.\
   Mer information om hur du lägger till ett diagram i rapporten finns i [Lägga till ett diagram i en rapport](#add-a-chart-to-a-report).

1. Klicka **Egna färger** när fältet är tillgängligt.\
   Dialogrutan Egna färger visas.\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >Du kan associera anpassade färger med fält som du kan gruppera efter och med vissa fält som kan visas i en vy, inklusive anpassade fält. De anpassade fälten eller anpassade alternativen för fälten som du väljer i dialogrutan Egen färg är skiftlägeskänsliga.

1. Välj något av följande alternativ:

   * **Använd en färg**: Alla element i diagrammet visas i den valda färgen.

      1. Börja skriva namnet på ett alternativ i det markerade fältet och välj sedan en färg. Det här alternativet visas i den valda färgen i diagrammet.
      1. (Valfritt) Ange ett hexadecimalt färgvärde för färgen i stället för att välja ett av de tillgängliga färgproven\
         eller\
         Klicka på färgväljaren som visas när du har klickat på den hexadecimala koden och välj en annan färg.

   * **Lägg till färg**: Fortsätt lägga till anpassade färger för alla andra möjliga alternativ för det markerade fältet.
   * **Ta bort alla**: Välj det här alternativet om du vill ta bort alla färger och alternativ i fältet som markerats ovan.
   * **Avancerade alternativ**: Välj bland följande alternativ:

      * **Inget värde**: Markera det här fältet och en egen färg för att visa den kolumn i diagrammet som grupperar &quot;inget värde&quot;-objekt. Det här är objekt som inte kan grupperas efter något av alternativen i det fält som är markerat i din gruppering.
      * **Alla andra värden**: Markera det här fältet och en egen färg för att visa alla andra diagramelement vars alternativ inte är markerade ovan.

        >[!NOTE]
        >
        >De färger som du har använt senast visas högst upp i dialogrutan Egna färger. När du för musen över en färg som nyligen har använts visas namnet på det fält som är associerat med den.

1. Klicka på&quot;x&quot; i det övre högra hörnet av dialogrutan Egna färger för att stänga dialogrutan Egna färger. Färgerna som du har valt sparas automatiskt.
1. Klicka **Spara + Stäng** för att spara diagrammet och köra rapporten.

## Ta bort ett diagram från en rapport

Så här tar du bort ett diagram från en rapport:

1. Öppna **Diagram** i Report Builder.
1. För musen över ikonen för den diagramtyp du har valt och en x-knapp visas i ikonens övre högra hörn.
1. Klicka på &quot;x&quot; för att ta bort diagrammet.
1. Klicka **Spara + Stäng**.

## Begränsningar när du arbetar med diagram

Tänk på följande begränsningar när du arbetar med diagram:

* The **Förhandsgranska diagram** -avsnittet till höger om Report Builder innehåller inga faktiska data från din rapport. Du måste spara diagrammet och visa det från **Diagram** om du vill visa diagrammet med dina data.

* Vissa diagramelement kan inte redigeras:

   * Du kan inte ändra teckensnittstypen eller storleken på värdena för varje element.
   * Du kan inte ändra namn på axlarna i diagrammet.

* Det går inte att redigera teckenförklaringen.
* När du använder beräkningsfält för dina grupperingar kan du inte klicka på diagramelementen.
* Det största antalet datapunkter som du kan visa i ett diagram är fyra i ett bubbeldiagram. Alla andra diagramtyper visar två eller högst tre datapunkter.
