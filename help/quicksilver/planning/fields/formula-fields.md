---
title: Översikt över formelfält
description: I Adobe Workfront Planning kan du skapa formelfält där funktioner och befintliga fält används för att beräkna ett nytt anpassat värde.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Översikt över formelfält

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan skapa anpassade fält i Adobe Workfront Planning genom att referera till befintliga fält och koppla dem i ett formeltypsfält.

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur befintliga värden ska beräknas.

Mer information finns i avsnittet Formel i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td>   <p>Hantera behörigheter till en arbetsyta <span class="preview">och posttyp</span> </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>I produktionsmiljön måste alla användare, inklusive systemadministratörer, tilldelas en layoutmall som innehåller Planning.</p>
<p><span class="preview">I förhandsvisningsmiljön har standardanvändare och systemadministratörer Planering aktiverat som standard.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överväganden om formelfält

* Formelfält refererar till fält som tillhör samma posttyp.
* Du kan bara referera till fält från andra posttyper när du kopplar en annan posttyp till den som du skapar ett formelfält för.
* &lt;span class-&quot;preview&quot;>Referens till anslutna posttyper eller deras sökfält i en formel beror på dina behörigheter till de anslutna posttyperna. Om du inte har behörighet att visa posttypen kan du inte referera till deras fält i en formel. </span>
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
