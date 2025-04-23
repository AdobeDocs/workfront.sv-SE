---
title: Dela poster
description: Du kan dela poster med andra för att öka samarbetet.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Dela poster

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Om du vill samarbeta med andra användare kan du dela poster med andra.

Du kan dela en Adobe Workfront Planning-post på följande sätt:

* Kopiera länken till postsidan från webbläsaren när sidan är öppen.

* Kopiera en länk till postens sida när du visar poster i posttypens tabellvy.

* Du kan dela alla poster på en arbetsyta med andra användare genom att dela arbetsytan <span class="preview"> och posttypen.</span>

  Mer information finns i följande artiklar:

   * [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Dela en posttyp](/help/quicksilver/planning/access/share-record-types.md)

  </div>

I den här artikeln beskrivs hur du kan kopiera en länk till en posts sida från en posttyps tabellvy.

## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Contributor eller högre licens </p>
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
   <td>  <p>Visa eller högre behörigheter till en arbetsyta <span class="preview">och posttyp</span> att dela   en post med en länk </p>
   <p>Hantera behörigheter till en arbetsyta <span class="preview">och posttyp</span> för att dela posterna på arbetsytan </p>
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

## Dela postlänkar från posttypstabellvyn

{{step1-to-planning}}

Arbetsytan som du senast öppnade öppnas.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Välj en tabellvy i listrutan **Visa** i tabellens övre högra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Högerklicka på en postrad

   eller

   Håll markören över en posts namn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Kopiera länk**.

   ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)

   Länken kopieras till Urklipp.

1. Klistra in länken i ett e-postmeddelande eller i ett chattfönster om du vill dela den med andra användare. När användarna får länken öppnas postsidan.

   >[!TIP]
   >
   >Fälten på postsidan är samma fält som är tillgängliga i postens tabellvy.


   <!--add there when it will be available: if they have access to this record-->

## Dela alla poster på en arbetsyta genom att dela arbetsytan

Du kan dela alla poster på en arbetsyta när du delar arbetsytan med andra.

Endast användare med behörigheten Hantera för en arbetsyta kan dela den med andra.

Mer information finns i [Dela en arbetsyta](/help/quicksilver/planning/access/share-workspaces.md).


<div class="preview">

## Dela alla poster i en posttyp genom att dela posttypen

I produktionsmiljön ärver poster behörigheter från arbetsytan.

I förhandsgranskningsmiljön ärver poster behörigheter från posttypen.

Som standard ärver posttyper behörigheter från arbetsytan.

Du kan dock göra något av följande:

* Inaktivera ärvda behörigheter från arbetsytan för en posttyp. Detta tar bort högre behörigheter till posterna, men behåller behörigheterna Visa till arbetsytan, posttypen och posterna.
* Bevilja manuellt behörigheter till användare för en posttyp, även om de inte har några behörigheter till arbetsytan. Detta ger dem automatiskt behörigheten Visa på arbetsytan. Detta ger användarna behörighet till posterna.

Endast användare med behörigheten Hantera på en arbetsyta kan dela sina posttyper och poster med andra.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).

</div>
