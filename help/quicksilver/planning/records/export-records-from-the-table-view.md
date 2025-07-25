---
title: Exportera poster från tabellvyn
description: Du kan exportera poster och deras information från tabellvyn till en CSV- eller Excel-fil.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Exportera poster från tabellvyn

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan exportera poster och deras information från tabellvyn till en Excel- eller CSV-fil i Adobe Workfront Planning.

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
   <td><p> Ljus eller högre </p>
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
   <td>   <p>Visa eller högre behörigheter i en vy</p>  
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportera poster från tabellvyn

Tänk på följande när du exporterar tabellvyn:

* Den information som exporteras till en Excel-fil bevarar de filter, grupperingar och sorteringar som används i tabellvyn i Workfront Planning. Grupperingar visas inte i CSV-filen.

* Miniatyrbilder och anpassade radfärger stöds inte i exporterade filer.

* Endast fält som är synliga i Workfront-gränssnittet exporteras. Dolda fält exporteras inte.

Så här exporterar du information från tabellvyn eller en posttyp:

1. Gå till en posttypssida och klicka på en tabellvyflik.
1. Gör något av följande:

   * Håll muspekaren över namnet på tabellvyfliken och klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) till höger om vynamnet. Klicka sedan på **Exportera**.

   ![Mer meny i en vy](assets/view-more-menu-with-duplicate-option.png)

   * Klicka på **Dela** > **Exportera den aktuella vyn**. Det här alternativet är bara tillgängligt när du visar tabellvyn.

   ![Dela-knappen med posttyp och visningsdelningsalternativ](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Välj något av följande format:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Du kan inte exportera information från tabellvyn när du visar en annan vy på skärmen. Du måste visa den tabellvy som du vill exportera för att kunna komma åt alternativet Exportera på Mer-menyn.

   Filen hämtas till datorn.

1. (Valfritt) Gå till hämtningsmappen på datorn och leta reda på den hämtade filen.

   Namnet på den exporterade filen har följande format:

   `Name of the view - name of the record type`

   En tabellvy för posttypen Campaigns genererar till exempel filen `Table view - Campaigns`.

   Filen innehåller följande information:

   * Kolumnrubrikerna markeras med svart i Excel-filen
   * Alla fält som är synliga i Workfront-gränssnittet, sorterade och filtrerade efter samma villkor
   * Grupperingar bevaras i Excel-filen

   Du kan nu dela de exporterade filerna med andra eller bifoga dem till valfri kommunikation.

</div>
