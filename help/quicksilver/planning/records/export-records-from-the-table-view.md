---
title: Exportera poster från tabellvyn
description: Du kan exportera poster och deras information från tabellvyn till en CSV- eller Excel-fil.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Exportera poster från tabellvyn

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan exportera poster och deras information från tabellvyn till en Excel- eller CSV-fil i Adobe Workfront Planning.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
eller
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Ljus eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Visa eller högre behörigheter på en arbetsyta och en posttyp</p>   
   <p>Visa eller högre behörigheter i en vy</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>
</td>
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Light or higher </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


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
