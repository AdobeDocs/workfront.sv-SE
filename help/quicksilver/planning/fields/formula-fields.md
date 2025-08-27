---
title: Översikt över formelfält
description: I Adobe Workfront Planning kan du skapa formelfält där funktioner och befintliga fält används för att beräkna ett nytt anpassat värde.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7288c6fb0f5d45758e0a82b8d1283e1f43ae94e6
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Översikt över formelfält

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan skapa anpassade fält i Adobe Workfront Planning genom att referera till befintliga fält och koppla dem i ett formeltypsfält.

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur befintliga värden ska beräknas.

Mer information finns i avsnittet Formel i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

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
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr>

</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Överväganden om formelfält

* Formelfält refererar till fält som tillhör samma posttyp.
* Du kan bara referera till fält från andra posttyper när du kopplar en annan posttyp till den som du skapar ett formelfält för.
* Hur du refererar till anslutna posttyper eller deras sökfält i en formel beror på dina behörigheter till de anslutna posttyperna. Om du inte har behörighet att visa posttypen kan du inte referera till deras fält i en formel.
* Du kan inte ändra fälttypen för ett formelfält när du har sparat det.
* Du kan uppdatera beräkningen av ett formelfält när du har sparat det och resultatet av beräkningen uppdateras automatiskt för alla poster av samma typ.
* Du måste lägga till de fält som du refererar till i formler när de visas i Workfront Planning-gränssnittet.
* Du kan bara referera till fält som visas i tabellvyn för en posttyp eller på sidan med postinformation.
* Du kan definiera formatet för värdet i en formelberäkning genom att välja bland följande formatalternativ:

   * Text
   * Nummer
   * Procent
   * Valuta
   * Taggar
   * Datum

  Mer information finns i avsnittet Formel i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).
* Du kan referera till formelfält i nya formler. När värdet uppdateras i ett fält som det refereras till i ett formelfält, uppdateras alla efterföljande fält som refererar till det fältet eller formelfälten som innehåller det fältet automatiskt.


<!--

<div class="preview">

## Limitations of formula fields

* You can add a maximum of 20 formula fields for one record type. 

   Formula lookup fields added from connected record types do not count against this limit. 

* The formula expression cannot exceed 50,000 characters. 

* Formula fields might display as `#ERROR!` in the following cases:
   * When a field used in a formula is deleted.
   * When a field used in an aggregated lookup field displays as `#ERROR!`. 
   
      For example, if you display a lookup field that contains aggregated lookup formula fields and one of the referenced formula fields  displays as `#ERROR!`. 
   *  When a formula value cannot be displayed in the selected format. 
   
      For example, if I select Number for the Format of a formula field, and the fields used in the formula are text fields that display only non-numeric text values, the formula result will display as `#ERROR!`, because it cannot parse the text into a number.
 
 </div>
 
 -->

## Formler som stöds

Adobe Workfront Planning-formelfält har stöd för de flesta uttryck från Workfront beräkningsfält.

>[!NOTE]
>
>Följande Workfront-uttryck stöds inte för Workfront Planning-formelfält:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* VÄXLA
>* FORMAT

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

En fullständig lista över Workfront-uttryck finns i [Översikt över beräknade datauttryck](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Dessutom stöder vi följande uttryck för formelfält för Workfront Planning. Följande uttryck stöds inte för Workfront-uttryck:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uttryck</th> 
   <th>Förklaring och exempel</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Returnerar sammanfogad sträng med avgränsare.</p> <p>Uttrycket formateras på följande sätt:

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Returnerar en array med unika värden.</p> <p>Uttrycket formateras på följande sätt:

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Returnerar ID för en post. Varje post har ett unikt ID.</p> <p>Uttrycket formateras på följande sätt:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Returnerar data från JSON med angiven JSONPath. Om JSONPath inte finns i JSON returneras ett tomt resultat. </p> <p>Uttrycket formateras på följande sätt:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Anger tidszonen för ett datum och en tid till en viss tidszon.</p> <p>Uttrycket formateras på följande sätt:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>VECKOFYEAR</strong> </td> 
   <td> <p>Returnerar veckonumret i ett år. Du kan också ange vilken dag veckan börjar på (använd 1 för söndag eller 2 för måndag). Om det utelämnas startar veckor som standard på söndag.</p> <p>Uttrycket formateras på följande sätt:

<code>VECKOFYEAR(date,2)</code>
eller
<code>VECKOFYEAR(date)</code>
</p>
   </td></tr>

</table>
