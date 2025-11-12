---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Beräknade anpassade fält kontra beräknade kolumner
description: Om du vill samla flera fält i Adobe Workfront och visa det sammanlagda värdet i ett nytt fält kan du skapa ett beräknat anpassat fält i ett anpassat formulär eller en beräknad kolumn i en vy.
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 0%

---

# Beräknade anpassade fält kontra beräknade kolumner

Om du vill samla flera fält i Adobe Workfront och visa det sammanlagda värdet i ett nytt fält kan du skapa följande:

* Ett beräknat anpassat fält i ett anpassat formulär\
  Mer information om hur du lägger till ett beräknat anpassat fält i ett anpassat formulär finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* En beräknad kolumn i en vy\
  Mer information om hur du använder beräkningar i en vy finns i avsnittet [Använd textläge i vyer](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) i artikeln [Översikt över vanliga användningsområden för textläge](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Även om du använder textläge för att skapa både beräknade fält och beräknade kolumner skiljer sig syntaxen för att skapa dem åt. Läs artiklarna ovan om du vill veta mer om hur du skapar beräknade fält och beräknade kolumner. Mer information om de olika syntaxerna som används i beräknade datamängder, t.ex. beräknade anpassade fält och kolumner, finns i avsnittet [Syntax för beräknade anpassade fält kontra beräknade anpassade kolumner](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) i den här artikeln.

Du kan använda samma beräkningar i båda beräkningsfälten samt i en beräknad kolumn. Beroende på vad du vill göra med beräkningarna kan det dock vara bra att bygga en jämfört med en annan.

## Syntax för beräknade anpassade fält kontra beräknade anpassade kolumner

Även om funktionerna du använder är desamma kan syntaxen för att skapa ett uttryck i ett beräknat anpassat fält skilja sig från den för att skapa en beräknad anpassad kolumn.

Exempel:

* I ett anpassat fält, i ett anpassat formulär för uppgifter, använder du följande för att generera namnet på det överordnade projektet för den uppgift där det anpassade formuläret är kopplat:

  `{project}.{name}`

* I en anpassad kolumn i en rapport använder du följande för att lägga till en anpassad kolumn för projektnamn i en aktivitetsrapport:

  `valuefield=project:name`

  eller

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >Samma syntax gäller för alla rapportelement i textläge där beräkningsuttryck används: vyer, filter, grupperingar och uppmaningar.

Skillnaderna mellan de två syntaxerna är:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Beräknat eget fält</strong></td>
   <td><strong>Element för beräknad anpassad rapportering</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Använd namnet på fälten så som de visas i Workfront-gränssnittet.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Exempel på fältnamn som används i ett beräknat anpassat fält: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Använd namnet på objekten eller fälten så som de visas i Workfront-databasen. Namnen på objekt och fält stavas med gemener eller med kameler, om de är sammansatta namn. </p> <p>En inventering av alla objekt och fält i Workfront som de visas i databasen finns i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Exempel på fältnamn som används i ett beräknat anpassat rapportelement: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Omge fältnamn inom parentes eller klammerparentes</td> 
   <td> <p>Omslut inte fältnamn inom parenteser eller parenteser när du använder dem på en <code>valuefield </code>rad.</p> <p>Omslut fältnamn inom klammerparentes när du använder dem på en <code>valueexpression</code>-rad.</p> </td> 
  </tr> 
  <tr> 
   <td>Avgränsa fälten med punkter</td> 
   <td> <p>Separera fälten med kolon när du använder dem på en <code>valuefield</code>rad.</p> <p>Separera fälten med punkter när du använder dem på en <code>valueexpression</code>rad.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om syntaxen som du måste använda i en beräknad anpassad kolumn finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## När beräknade anpassade fält ska användas

* När du vill gruppera aggregerade resultat i en rapport eller vill visa den här informationen i ett diagram
* När du vill samla in data utöver den aggregering som beräknas i fältet
* När du inte är orolig för att data ska vara aktuella, eftersom data inte uppdateras och kan ändras över tid

## Åtgärder som utlöser uppdateringen av ett beräknat anpassat fält

* På ett objekts huvudsida klickar du på ikonen Mer ![Mer](assets/more-icon.png) och sedan på **Beräkna om uttryck**

* Redigera flera objekt gruppvis när **Beräkna om anpassade uttryck** är aktiverat.
* Redigera flera objekt gruppvis när du klickar på **Beräkna om uttryck** på menyn Mer i en lista med objekt.
* Redigera ett anpassat formulär när **Uppdatera tidigare beräkningar** är aktiverat för det beräknade anpassade fältet.

Mer information finns i [Redigera information i anpassade formulärfält](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## När beräknade kolumner ska användas i en vy

* När ni vill att realtidsdata ska vara tillgängliga i en rapport.

  Beräknade vyer är alltid aktuella eftersom beräkningen görs när rapporten körs eller vyn används.

* När du inte har några planer på att gruppera aggregerade resultat eller använda den här informationen i ett diagram.
* När du inte planerar att aggregera data utöver den aggregering som beräknas i kolumnen (data kan bara aggregeras en gång).
* När du vill att beräkningen ska innehålla en referens till det aktuella datumet med jokertecknen $$TODAY eller $$NOW.

  >[!TIP]
  >
  >Använd inte den här referensen i beräknade anpassade fält eftersom de bara beräknas om när det kopplade objektet redigeras. Den här typen av beräkningar blir inaktuella.

## Exempel på beräknade anpassade fält och kolumner

Exempel på beräknade anpassade fält finns i [Beräknade anpassade data i rapporter](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Exempel på beräknade anpassade kolumner i vyer finns i följande artiklar:

* [Översikt över vanliga användningsområden för textläge](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Anpassad vy, filter och gruppering av exempel: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
