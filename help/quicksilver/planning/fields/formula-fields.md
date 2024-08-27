---
title: Översikt över formelfält
description: I Adobe Workfront Planning kan du skapa formelfält där funktioner och befintliga fält används för att beräkna ett nytt anpassat värde.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Översikt över formelfält

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

Du kan skapa anpassade fält i Adobe Workfront Planning genom att referera till befintliga fält och koppla dem i ett formeltypsfält.

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur befintliga värden ska beräknas.

Mer information finns i avsnittet Formel i artikeln [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
   <td> 
<p>Alla </p> 
<p>Mer information om vad som ingår i varje Workfront Planning-plan finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfornt planining</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Överväganden om formelfält

* Formelfält refererar till fält som tillhör samma posttyp.
* Du kan bara referera till fält från andra posttyper när du kopplar en annan posttyp till den som du skapar ett formelfält för.
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

## Formler som stöds

Adobe Workfront Planning-formelfält har stöd för alla uttryck från Workfront beräkningsfält. Mer information finns i [Översikt över beräknade datauttryck](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Dessutom har vi stöd för följande uttryck för formelfält i Workfront Planning:

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
