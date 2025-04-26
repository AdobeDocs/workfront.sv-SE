---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Villkorsoperatorer i beräknade anpassade uttryck
description: Du kan använda villkorsoperatorer eller modifierare när du skapar beräknade anpassade data i Adobe Workfront i textläge.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 0%

---

# Villkorsoperatorer i beräknade anpassade fält

<!-- Audited: 2/2024 -->

Du kan använda villkorsoperatorer eller modifierare när du skapar beräknade anpassade data i Adobe Workfront i textläge. Mer information om hur du använder textläge i Workfront finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Villkorsoperatorer eller modifierare hjälper till att skapa villkorssats genom att koppla befintliga Workfront-fält i satser och generera ett nytt fält. Det vanligaste användningsområdet för villkorsoperatorer är att skapa villkoret för en IF-programsats.

Du kan använda IF-satser i Workfront för att jämföra, formatera och strängsätta fält med data för både rapportering och anpassade datamängder.

Du kan skapa IF-satser för följande Workfront-element:

* Vyer
* Grupperingar
* Beräknade anpassade fält

Mer information om hur du skapar IF-satser finns i Översikt över [ IF-satser ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Exemplen i den här handboken visar hur du använder villkorsoperatorer i beräknade anpassade fält. Du kan även använda dem i beräknade anpassade kolumner eller grupperingar när du följer rätt syntax för beräknade anpassade fält i rapporter.

Mer information om skillnaden i syntax mellan beräknade anpassade fält och beräknade anpassade data i rapporter finns i [Beräknade anpassade fält kontra beräknade kolumner](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

I API-utforskaren hittar du de fält som du vill referera till i dina beräknade anpassade uttryck. Mer information om API-utforskaren finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

Du kan använda följande villkorsmodifierare i Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Villkorsoperator</th> 
   <th>Villkorsoperatorsyntax</th> 
   <th>Definition av villkorsoperator</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Jämn</td> 
   <td>= </td> 
   <td> <p>Använd den här operatorn för att ange att villkoret är uppfyllt när det första fältet i programsatsen är lika med det andra fältet.</p> <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som jämför det planerade slutförandedatumet med det planerade slutförandedatumet för en uppgift: </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Större än </td> 
   <td>&gt; </td> 
   <td>Använd den här operatorn för att ange att villkoret är uppfyllt när det första fältet i programsatsen är större än det andra fältet. <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som jämför det planerade slutförandedatumet med det planerade slutförandedatumet för en uppgift: </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Större än eller lika med </td> 
   <td>&gt;= </td> 
   <td>Använd den här operatorn för att ange att villkoret är uppfyllt när det första fältet i programsatsen är större än eller lika med det andra fältet. <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som jämför det planerade slutförandedatumet med det planerade slutförandedatumet för en uppgift: </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Mindre än </td> 
   <td>&lt; </td> 
   <td>Använd den här operatorn för att ange att villkoret är uppfyllt när  det första fältet i programsatsen är mindre än det andra fältet. <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som jämför det planerade slutförandedatumet med det planerade slutförandedatumet för en uppgift: </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Mindre än eller lika med </td> 
   <td>&lt;= </td> 
   <td>Använd den här operatorn för att ange att villkoret är uppfyllt när  det första fältet i programsatsen är mindre än eller lika med det andra fältet. <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som jämför det planerade slutförandedatumet med det planerade slutförandedatumet för en uppgift: </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Gör inte </td> 
   <td>! </td> 
   <td> <p>Lägg till den här operatorn framför någon av ovanstående operatorer för att negera operatorn. </p> <p>Exempel: </p> 
    <ul> 
     <li>Lika med: = </li> 
     <li>Är inte lika med: != </li> 
    </ul> <p>Om du lägger till den här operatorn framför följande datauttryck läggs en negativ programsats till i uttryck: </p> 
    <ul> 
     <li>INNEHÅLLER </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Mer information om de här datauttrycken och en fullständig lista finns i <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Översikt över beräknade datauttryck</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>eller </td> 
   <td>|| </td> 
   <td> <p>Använd den här operatorn för att ange att villkoret är uppfyllt när uttrycket  hittar antingen det första eller det andra värdet i programsatsen. </p> <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som markerar projekt i aktuell status eller planeringsstatus som"Aktiv": </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> Och </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Använd den här operatorn för att ange att villkoret är uppfyllt när uttrycket  söker efter ett objekt som uppfyller två villkor samtidigt. </p> <p>Använd till exempel följande programsats i ett beräknat anpassat fält för att skapa en IF-programsats som söker efter projekt som har statusen Aktuell och som har villkoret Vid risk och markerar dem som"Mediation behövs". </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
