---
title: Redigera posttyper
description: Du kan redigera posttyper när de har sparats. Posttyperna är objekttyperna för Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Redigera posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. Du kan redigera utseendet på posttyper som du eller någon annan har skapat. Mer information om hur du skapar posttyper för Workfront Planning finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <td>   <p>Hantera behörigheter till en arbetsyta <span class="preview">och posttyp</span> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Endast systemadministratörer kan aktivera posttyper för anslutning från andra arbetsytor</p> </td> 
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


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Redigera posttyper

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera,

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Redigera**
eller
   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Redigera**.

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

1. I rutan **Redigera posttyp** öppnas fliken **Utseende** som standard.

   ![Redigera flik för posttypsrutans utseende ](assets/edit-record-type-box-appearance-tab.png)

   Uppdatera följande information på fliken **Utseende**:

   * Redigera posttypens namn om det behövs. <!--did they add a field label for this?-->
   * **Beskrivning**: Redigera eller lägg till en beskrivning för posttypen med mer information om den.
   * Redigera färg och form för ikonen som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar posttypen. Det här är färgen på ikonen för posttyp.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

1. (Villkorligt) Om du är systemadministratör klickar du på fliken **Avancerade inställningar** i rutan **Redigera posttyp** . <!--the info here is duplicated in the Create record types article-->

   ![Fliken Redigera posttypsruta för avancerade inställningar](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Villkorligt) Uppdatera följande information på fliken **Avancerade inställningar**:

   * Aktivera inställningen **Anslut från en annan arbetsyta**. När det här alternativet är aktiverat är posttypen tillgänglig och kan anslutas från andra arbetsytor.
   * Välj från vilka arbetsytor som posttypen kan nås. Välj bland följande alternativ:

      * **Systemomfattande**: Användare kan ansluta till den här posttypen från alla arbetsytor där de har behörighet att hantera.
      * **Specifika arbetsytor**: Lägg till namnen på arbetsytorna där arbetsytehanterare kan ansluta till den här posttypen.

1. Klicka på **Spara**.

   Posttypkortet på arbetsytan visar en anslutningsikon ![Anslut från andra arbetsytor-ikon](assets/connect-from-other-workspaces-icon.png) i det övre högra hörnet för att ange att posten nu är tillgänglig från andra arbetsytor.

1. (Valfritt) Klicka på posttypskortet i arbetsytan för att öppna posttypens sida och byt sedan namn på posttypen i rubriken.

1. (Valfritt) Om du vill redigera en annan posttyp expanderar du den nedåtriktade pilen till höger om ett posttypsnamn, söker efter en posttyp och markerar den när den visas i listan.

   ![Listrutan Posttyp på posttypssidan med sökrutan](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
