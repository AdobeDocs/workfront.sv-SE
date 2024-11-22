---
title: Återställ borttagna poster
description: Du kan återställa borttagna poster från området Senast borttagna i Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---


# Återställ borttagna poster

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan återställa borttagna poster från området Senast borttagna i Adobe Workfront Planning.

Mer information om hur du tar bort poster finns i [Ta bort poster](/help/quicksilver/planning/records/delete-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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

## Att tänka på när du återställer borttagna poster

* Poster lagras i behållaren för nyligen borttagna poster i 30 dagar. Efter 30 dagar tas posterna bort permanent från Workfront Planning.
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort. Om du återställer de borttagna posterna återställs informationen från de anslutna posterna.
* Du kan återställa flera poster samtidigt.
* När posterna tas bort lagras följande information i behållaren Senast borttagna:
   * **Namn**: Detta är informationen i postens primära fält. Mer information om primära postfält finns i [Översikt över primära fält](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Borttaget datum**: Tid och datum då posten togs bort.
   * **Tid i nyligen borttagna**: Tid sedan posten togs bort. Poster som har tagits bort mer än 30 dagar före det aktuella datumet visas inte i behållaren Senast borttagna.
   * **Borttagen av**: Namnet på den användare som tog bort posten.

## Återställ borttagna poster

1. Gå till posttypssidan där du har tagit bort poster.
1. Klicka på ikonen **Ångra** ![](assets/undo-icon.png) i det övre högra hörnet av en posttypssidvy och klicka sedan på **Senast borttagen**.

   Rutan **Nyligen borttagen** visas.

   ![](assets/recently-deleted-box.png)

1. Markera de poster som du vill ta bort och klicka sedan på **Återställ** > **Återställ**. Du kan markera flera poster.

   Om återställningen lyckades får du ett meddelande om att åtgärden lyckades längst ned på skärmen.
1. Gå till tabellvyn och granska de återställda posterna.
