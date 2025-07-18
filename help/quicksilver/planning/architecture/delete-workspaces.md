---
title: Ta bort arbetsytor
description: Du kan ta bort arbetsytor när de inte längre är relevanta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---


# Ta bort arbetsytor

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

I Adobe Workfront Planning är arbetsytorna centraliserade platser där team kan planera arbetet. Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

Du kan ta bort arbetsytor som inte längre är relevanta.

Vi rekommenderar att du återskapar vissa eller alla posttyper, poster, fält och vyer som är kopplade till arbetsytan som du vill ta bort på en annan arbetsyta innan du tar bort den.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du tar bort arbetsytor

* När du tar bort arbetsytor tas även alla posttyper, poster, fält och vyer bort.
* Borttagna arbetsytor och den information de innehåller kan inte återställas.

## Ta bort en arbetsyta

{{step1-to-planning}}

1. (Villkorligt) Om du är Workfront-administratör klickar du på **Arbetsytor som jag är på** för att komma åt arbetsytor som du har skapat, eller **Andra arbetsytor** för att komma åt arbetsytor som andra delar med dig.

1. (Valfritt) Klicka på **Visa alla** om du vill visa ytterligare arbetsytor. Länken **Visa alla** visas bara när du har fler än två rader med arbetsytekort.
1. (Valfritt) Klicka på **Visa färre** om du vill begränsa antalet arbetsytor som visas på skärmen.
1. Gör något av följande om du vill ta bort en arbetsyta:

   * Håll pekaren över arbetsytans kort och klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) i kortets övre högra hörn
eller
   * Klicka på ett arbetsytekort för att öppna arbetsytan och klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) till höger om arbetsytans namn.
1. Klicka på **Ta bort**.

   ![Bekräftelse av borttagning av arbetsyta permanent](assets/permanently-delete-workspace-confirmation.png)

1. Skriv **delete** i det angivna utrymmet och klicka sedan på **Ta bort permanent**. Detta är inte skiftlägeskänsligt.

   Arbetsytan tas bort och kan inte återskapas. Alla posttyper, poster, fält och vyer som är kopplade till dem tas också bort. <!--ensure this is right at or before GA-->
