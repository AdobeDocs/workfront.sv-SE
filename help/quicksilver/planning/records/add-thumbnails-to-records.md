---
title: Lägga till en miniatyrbild i en post
description: Du kan redigera postinformation i Adobe Workfront Planning och associera varje post med enskilda miniatyrbilder för att göra dem lätta att känna igen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---


# Lägga till en miniatyrbild i en post

{{planning-important-intro}}

Du kan associera poster med unika miniatyrbilder i Adobe Workfront Planning för att göra dem lätta att känna igen.

Du måste skapa posttyper innan du kan börja skapa och redigera poster.
Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Åtkomstkrav

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td><p> Standard </p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta </p>  
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

<!--OLD:


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
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td>  <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfornt documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Att tänka på när du spelar in miniatyrbilder

Om du vill skilja mellan posterna i en tabellvy kan du koppla en unik miniatyrbild till varje post.

Tänk på följande:

* En miniatyrbild är unik för en post och gäller inte för alla poster av samma typ.
* Du kan bara lägga till bildfiler som miniatyrer.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Du kan lägga till en miniatyrbild till enskilda poster i tabellvyn eller från postens sida eller förhandsvisningsruta.
* Workfront laddar automatiskt upp en miniatyrbild varje gång du skapar en post. Du kan ändra den här bilden senare.
* Miniatyrbilder tillhör postinformationen och visas i områden där posterna visas. Miniatyrbilder visas till exempel tillsammans med postinformation i följande områden:

   * Det primära fältet för en post i tabellvyn
   * Postfältet i tidslinjevyn.
   * Postens förhandsgranskning och sida med information.

## Lägga till en miniatyrbild i en post

Du kan lägga till en miniatyrbild på följande sätt:

* [Lägga till en miniatyrbild till en post från tabellvyn](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Lägga till en miniatyrbild till en post från informationssidan](#add-a-thumbnail-to-a-record-from-the-details-page)

### Lägga till en miniatyrbild till en post från tabellvyn

{{step1-to-planning}}

1. Klicka på arbetsytan för vars poster du vill lägga till miniatyrbilder och klicka sedan på posttypskortet.

   Då öppnas posttypssidan.
1. Välj en tabellvy i listrutan **Visa**. Alla poster av den typ som du har markerat visas i en tabell.
1. Håll markören över informationen för det primära fältet, klicka på menyn **Mer** ![](assets/more-menu.png) och sedan på **Miniatyrbild**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Det primära fältet är det fält som visas i den första kolumnen i en tabellvy. Det primära fältet är alltid fryst och kan inte döljas eller flyttas. Alternativet Miniatyrbilder är inte tillgängligt på menyn Mer när det primära fältet är ett formelfält.

   Fliken **Överför** öppnas som standard i rutan **Spela in miniatyrbild**.

   Mer information om hur du överför miniatyrbilden finns i avsnittet [Lägg till en miniatyrbild till en post från informationssidan](#add-a-thumbnail-to-a-record-from-the-details-page) i den här artikeln, med början från steg 6. <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Lägga till en miniatyrbild till en post från informationssidan

{{step1-to-planning}}

1. Klicka på arbetsytan för vars poster du vill lägga till miniatyrbilder och klicka sedan på posttypskortet.

   Då öppnas posttypssidan.
1. Öppna en post genom att klicka på den i valfri vy.

   Förhandsvisningsrutan med information visas.
1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![](assets/open-details-in-a-new-tab-icon.png) i det övre högra hörnet.

   Postens informationssida öppnas.
1. Håll pekaren över miniatyrbilden eller ikonen ![](assets/record-thumbnail-icon-on-details-page.png) och klicka sedan på menyn **Mer** ![](assets/more-menu.png) > **Redigera miniatyrbild**.

   Fliken **Överför** öppnas som standard i rutan **Spela in miniatyrbild**.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Dra och släpp en fil som du vill lägga till som miniatyrbild

   eller

   Klicka på **Bläddra bland bilder** och bläddra sedan efter en bildfil som du vill lägga till. Filen måste sparas på datorn.

1. (Valfritt) När bilden har överförts i rutan **Spela in miniatyrbild** använder du storleksförändringsverktyget för att beskära och ändra storlek på bilden.
1. (Valfritt) Klicka på ikonen **Överför ny bild** ![](assets/upload-new-image-icon.png) om du vill överföra en annan bild.
1. (Valfritt) Klicka på fliken **Galleri** och sedan på en bild. Det går inte att ändra bildgalleriet.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Valfritt) Om du vill ta bort miniatyrbilden innan den sparas klickar du på ikonen **Ta bort** ![](assets/remove-image-icon.png) till höger om bilden.

1. Klicka på **Använd bild** om du vill lägga till bilden som en miniatyrbild.
Då stängs rutan **Spela in miniatyrbild**.
Miniatyrbilden visas i områden i Workfront Planning där posten visas.

   >[!TIP]
   >
   >   Du måste aktivera fältet Miniatyrbilder i tabellvyn om du vill visa miniatyrbilder i den här vyn. Det är inaktiverat som standard.

1. (Valfritt) Om du vill ta bort miniatyrbilden när den har sparats klickar du på en post i valfri vy för att öppna informationssidan, håller pekaren över miniatyrbilden och klickar på **Mer**-menyn ![](assets/more-menu.png)> **Ta bort**-ikonen ![](assets/remove-image-icon.png) . Miniatyrbilden tas bort.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->