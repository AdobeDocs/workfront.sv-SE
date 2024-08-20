---
title: Ta bort arbetsytor
description: Du kan ta bort arbetsytor när de inte längre är relevanta.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Ta bort arbetsytor

{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet. Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

Du kan ta bort arbetsytor som inte längre är relevanta.

Vi rekommenderar att du återskapar vissa eller alla posttyper, poster, fält och vyer som är kopplade till arbetsytan som du vill ta bort på en annan arbetsyta innan du tar bort den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
<p>Din organisation måste vara registrerad på Workfront Planning i ett tidigt skede </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Att tänka på när du tar bort arbetsytor

* När du tar bort arbetsytor tas även alla posttyper, poster, fält och vyer bort.
* Borttagna arbetsytor och den information de innehåller kan inte återställas.

## Ta bort en arbetsyta

{{step1-to-planning}}

1. (Villkorligt) Om du är Workfront-administratör klickar du på **Arbetsytor som jag är på** för att komma åt arbetsytor som du har skapat, eller **Andra arbetsytor** för att komma åt arbetsytor som andra delar med dig.

1. (Valfritt) Klicka på **Visa alla** om du vill visa ytterligare arbetsytor. Länken **Visa alla** visas bara när du har fler än två rader med arbetsytekort.
1. (Valfritt) Klicka på **Visa färre** om du vill begränsa antalet arbetsytor som visas på skärmen.
1. Gör något av följande om du vill ta bort en arbetsyta:

   * Håll pekaren över arbetsytans kort och klicka sedan på menyn **Mer** ![](assets/more-menu.png) i kortets övre högra hörn
eller
   * Klicka på ett arbetsytekort för att öppna arbetsytan och klicka sedan på menyn **Mer** ![](assets/more-menu.png) till höger om arbetsytans namn.
1. Klicka på **Ta bort**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Skriv **delete** i det angivna utrymmet och klicka sedan på **Ta bort permanent**. Detta är inte skiftlägeskänsligt.

   Arbetsytan tas bort och kan inte återskapas. Alla posttyper, poster, fält och vyer som är kopplade till dem tas också bort. <!--ensure this is right at or before GA-->
