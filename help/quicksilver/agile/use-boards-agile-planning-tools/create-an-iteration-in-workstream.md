---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Skapa en iteration i en arbetsström
description: En iteration är en angiven tidsrymd som är reserverad för att slutföra arbete. Vissa rörliga team kan kalla en iteration för en fjäder.
author: Jenny
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Skapa en iteration i ett arbetsflöde

>[!IMPORTANT]
>
>Arbetsflöden är bara tillgängliga för en viss kundgrupp.

En iteration är en angiven tidsrymd som är reserverad för att slutföra arbete. Vissa rörliga team kan kalla en iteration för en fjäder.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p>
   </td> 
  </tr>  
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en iteration i ett arbetsflöde

{{step1-to-boards}}

1. Öppna arbetsflödet där du vill lägga till iterationen. Om du vill öppna ett arbetsflöde klickar du på [!UICONTROL **Visa arbetsflöde**].
1. Skapa en iteration på något av följande sätt:

   * Klicka på [!UICONTROL **Skapa iteration**] i iterationsvyn på fliken Kortlista.
   * Klicka på [!UICONTROL **Skapa iteration**] i listvyn på fliken Kortlista.
   * Klicka på [!UICONTROL **Lägg till anslagstavla**] på fliken Ritytor och välj [!UICONTROL **Intervationsprocess**] som ritytema. Öppna sedan iterationspanelen och klicka på [!UICONTROL **Konfigurera iterationer**].

1. Lägg till följande information i dialogrutan Intervallinformation:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>Namnet på iterationen, till exempel "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Iteration length]</strong></td> 
      <td>Längden på iteration, i dagar, veckor eller månader.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>Det datum då iterationen börjar. Slutdatumet anges automatiskt baserat på itereringslängden.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på [!UICONTROL **Spara**].

   Numret visas nu i iterationsvyn för kortlistan och i metriområdet på iterationsytan.

   Mer information om hur du lägger till kort i en iteration finns i [Använd kortlistan](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Redigera en befintlig iteration

1. Om du vill öppna ett arbetsflöde klickar du på [!UICONTROL **Visa arbetsflöde**].
1. Öppna iterationen på något av följande sätt:

   * Klicka på ikonen [!UICONTROL **Iterationsinformation**] ![Iterationsinformation](assets/iteration-details-button.png) i vyn över kortlistan.
   * Klicka på ikonen [!UICONTROL **Iterationsinformation**] ![Iterationsinformation](assets/iteration-details-button.png) i mätområdet högst upp till höger på iterationspanelen.

1. Redigera upprepningen efter behov på panelen [!UICONTROL Iteration Configuration].
1. Utöka [!UICONTROL **iterationsinformationen**] om du vill ändra upprepningsnamnet.

   När en iteration har startats kan du bara ändra iteration och inte datum eller iteration.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Ta bort en iteration

1. Klicka på fliken [!UICONTROL **Kortlista**] i arbetsflödet och öppna itereringsvyn.
1. Klicka på ikonen **Ta bort** ![Ta bort &#x200B;](assets/delete.png) intill iterationen.
1. Klicka på [!UICONTROL **Ta bort upprepning**] i bekräftelsemeddelandet.
