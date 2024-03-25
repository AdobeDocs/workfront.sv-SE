---
title: Lägga till miniatyrbilder i poster
description: Du kan redigera postinformation i Adobe Workfront-planeringen och associera varje post med enskilda miniatyrbilder för att göra dem lätta att känna igen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Lägga till miniatyrbilder i poster

{{maestro-important-intro}}

Du kan associera poster med unika miniatyrbilder i Adobe Workfront-planeringen för att göra dem lätta att känna igen.

Du måste skapa posttyper innan du kan börja skapa och redigera poster.
Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

## Åtkomstkrav

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i betaprogrammet för Adobe Workfront-planering. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstkontroller för Workfront-planering </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Contribute eller högre behörighet till en arbetsyta </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td>  <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/maestro/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Att tänka på när du spelar in miniatyrbilder

Om du vill skilja mellan posterna i en tabellvy kan du koppla en unik miniatyrbild till varje post.

Tänk på följande:

* Du kan bara lägga till bildfiler som miniatyrer.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Du kan lägga till en miniatyrbild till enskilda poster i tabellvyn.
* Miniatyrbilder tillhör postinformationen och visas i vyer där posterna visas. Miniatyrbilder visas till exempel tillsammans med postinformation i följande områden:

   * Det primära fältet för en post i tabellvyn
   * Postfältet i tidslinjevyn.
* Du kan inte lägga till postminiatyrer från postens informationssida eller i tidslinjevyn.
* Miniatyrbilder visas inte på postens informationssida.

## Lägga till en miniatyrbild i en post

{{step1-to-maestro}}

1. Välj den arbetsyta vars poster du vill lägga till miniatyrbilder för och klicka sedan på posttypskortet.

   Då öppnas posttypssidan.
1. Välj en tabellvy på menyn **Visa** listruta. Alla poster av den typ som du har markerat visas i en tabell.
1. Håll markören över informationen i det primära fältet och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Miniatyrbild**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Det primära fältet är det fält som visas i den första kolumnen i en tabellvy. Det primära fältet är alltid fryst och kan inte döljas eller flyttas.

   The **Spela in miniatyrbild** öppnas.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. I **Överför** dra och släpp en fil som du vill lägga till som miniatyrbild eller klicka på **Välj att överföra** och bläddra sedan efter en bildfil att lägga till. Filen måste sparas på datorn.
1. (Valfritt) Använd storleksförändringsverktyget för att beskära och ändra storlek på bilden.
1. Klicka **Använd bild** om du vill lägga till bilden som en miniatyrbild.
Detta stänger **Spela in miniatyrbild** box.
1. (Villkorligt) Om du har minst Contribute-behörighet till tabellvyn klickar du på **Fält** i tabellvyns övre högra hörn.
1. Välj **Miniatyrbild** för att visa miniatyrbilden. Detta är som standard avmarkerat.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   Miniatyrbilden visas till vänster om det primära fältvärdet.
1. (Valfritt och villkorligt) Om du inte har Contribute eller högre behörighet för vyn väljer du en ny vy i **Visa** eller skapa en vy.
1. (Valfritt) Om du vill ta bort miniatyrbilden håller du pekaren över det primära fältet och klickar på knappen **Mer** meny ![](assets/more-menu.png)> **Miniatyrbild** > **Ta bort** icon ![](assets/remove-image-icon.png)och sedan klicka **Spara ändringar**.
