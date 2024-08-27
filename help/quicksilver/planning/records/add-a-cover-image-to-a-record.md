---
title: Lägga till en omslagsbild till en post
description: Du kan anpassa poster genom att lägga till en omslagsbild på postsidan i Adobe Workfront Planning när du redigerar en post.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---


# Lägga till en omslagsbild till en post

{{planning-important-intro}}

Du kan anpassa poster genom att lägga till en omslagsbild på postsidan i Adobe Workfront Planning när du redigerar en post.

Mer information om hur du redigerar poster finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

Du måste skapa posttyper innan du kan börja skapa och redigera poster.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

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

## Att tänka på när det gäller omslagsbilder för postsidor

Du kan anpassa postens sida genom att lägga till en omslagsbild.

Tänk på följande:

* En omslagsbild är unik för en post och gäller inte för alla poster av samma typ.
* Du kan bara lägga till bildfiler som omslagsbilder.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Du kan lägga till en omslagsbild till enskilda poster från postförhandsvisningen i valfri vy eller från postsidan.
* Du kan inte lägga till omslagsbilder från en postvy.
* Workfront laddar automatiskt upp en omslagsbild varje gång du skapar en post. Du kan ändra den här bilden senare.

## Lägga till en omslagsbild till en post

Du kan anpassa en post genom att lägga till en omslagsbild högst upp i postens förhandsvisning eller sida.

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill anpassa,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.

1. Klicka på en post i en vy av valfri typ

   eller

   Klicka på ikonen **Öppna detaljer** ![](assets/open-details-icon-in-table-name-field.png) i den första kolumnen i tabellvyn.

   Postens förhandsgranskning öppnas i vyn.

   ![](assets/details-box.png)

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> i det övre högra hörnet av postens förhandsgranskning för att öppna postens sida på en ny flik.

   Postsidan öppnas.

   ![](assets/details-page.png)

1. Klicka på **Lägg till omslag** i postens förhandsgranskning eller på sidan.


   eller

   Håll pekaren över en befintlig omslagsbild, klicka på menyn **Mer** ![](assets/more-menu.png) och klicka sedan på **Överför**. <!--check the casing here; I logged a bug for this-->
Rutan **Postomslag** öppnas på fliken **Överför** .

   ![](assets/record-cover-box-for-upload.png)

1. Klicka på **Bläddra bland bilder** och bläddra efter en bild på datorn för att markera och lägga till den.

1. (Valfritt) Om du vill ta bort bilden innan den sparas klickar du på ikonen **Överför ny bild** ![](assets/upload-new-image-icon.png) och överför en ny bild.

1. (Valfritt) Klicka på fliken **Galleri** och sedan på en bild i bildgalleriet. Det går inte att ändra bildgalleriet.

   ![](assets/record-cover-box-for-gallery.png)

1. Klicka på **Använd bild**.

   Bilden överförs högst upp i postens förhandsgranskning eller sida och ändringarna sparas automatiskt.

   ![](assets/record-page-with-cover-image.png)

1. (Valfritt) Hovra över bilden, klicka sedan på menyn **Mer** ![](assets/more-menu.png) i det nedre högra hörnet av omslagsbilden och gör något av följande:

   * Klicka på **Överför** om du vill ersätta omslagsbilden och upprepa steg 6 för att överföra och spara en ny bild.
   * Klicka på **Flytta** och använd verktyget **Flytta** ![](assets/reposition-tool-icon.png) för att centrera omslagsbilden. Klicka sedan på **Spara** när du är klar.
   * Klicka på **Ta bort** för att ta bort omslagsbilden.

   Workfront sparar automatiskt ändringarna.
