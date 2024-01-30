---
title: Lägga till miniatyrbilder i poster
description: Du kan redigera postinformation i Adobe Maestro och associera varje post med enskilda miniatyrbilder för att göra dem lätta att känna igen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Lägga till miniatyrbilder i poster

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan associera poster med unika miniatyrbilder i Adobe Maestro för att göra dem lätta att känna igen.

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
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
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
   <td> <p>Det finns inga åtkomstkontroller för Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Contribute eller högre behörighet till en arbetsyta </p>  
   <p>Contribute eller högre behörigheter till tabellvyn </p> 
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Din Workfront- eller gruppadministratör måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>


## Att tänka på när du spelar in miniatyrbilder

Om du vill skilja mellan posterna i en tabellvy kan du koppla en unik miniatyrbild till varje post.

Tänk på följande:

* Du kan bara lägga till bildfiler som miniatyrer.
* Du kan lägga till en miniatyrbild till enskilda poster i tabellvyn.
* Du kan inte lägga till postminiatyrer från postens informationssida eller i tidslinjevyn.
* Miniatyrbilden visas alltid till vänster om det primära fältet för varje post, oavsett vilken fälttyp det är.

  Fält som är enkelradig text, siffror eller formler kan definieras som primära fält.
Mer information finns i [Hantera tabellvyn](/help/quicksilver/maestro/views/manage-the-table-view.md).

<!--above: when you know exactly what type of files are allowed, add the exact extensions above-->

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
1. Klicka på Fält i tabellvyns övre högra hörn.
1. Välj **Miniatyrbild** för att visa miniatyrbilden. Detta är som standard avmarkerat.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   Miniatyrbilden visas till vänster om det primära fältvärdet.
1. (Valfritt) Om du vill ta bort miniatyrbilden håller du pekaren över det primära fältet och klickar på knappen **Mer** meny ![](assets/more-menu.png)> **Miniatyrbild** > **Ta bort** icon ![](assets/remove-image-icon.png)och sedan klicka **Spara ändringar**.
