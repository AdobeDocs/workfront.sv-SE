---
title: Redigera posttyper
description: Du kan redigera posttyper när de har sparats. Posttyperna är objekttyperna för Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---


# Redigera posttyper

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. Du kan redigera utseendet på posttyper som du eller någon annan har skapat. Mer information om hur du skapar posttyper för Workfront Planning finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
   <td>   <p>Hantera behörigheter till en arbetsyta och en posttyp </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Endast systemadministratörer kan aktivera posttyper för anslutning från andra arbetsytor</p> </td> 
  </tr>

</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera posttyper

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera,

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Redigera**
eller
   * <span class="preview">Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Redigera**. </span>

   <span class="preview">![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)</span>

1. I rutan **Redigera posttyp** öppnas fliken **Utseende** som standard.

   ![Redigera flik för posttypsrutans utseende ](assets/edit-record-type-box-appearance-tab.png)

   Uppdatera följande information på fliken **Utseende**:

   * Redigera posttypens namn om det behövs. <!--did they add a field label for this?-->
   * **Beskrivning**: Redigera eller lägg till en beskrivning för posttypen med mer information om den.
   * Redigera färg och form för ikonen som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar posttypen. Det här är färgen på ikonen för posttyp.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

   <!--old info: 
   1. (Conditional) If you are a system administrator, click the **Advanced settings** tab in the **Edit record type** box. 
      ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
   1. (Conditional) Update the following information in the **Advanced settings** tab: 
      * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
      * Choose from which workspaces the record type can be accessed. Choose from the following options:
         * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
         * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.-->


1. (Valfritt och villkorligt) Om du är systemadministratör klickar du på **Avancerade inställningar** och uppdaterar följande information i avsnittet **Arbetsytans funktioner**: <!--the info here is duplicated in the Create record types article-->
   * Aktivera inställningen **Tillåt anslutning till den här posttypen i andra arbetsytor**: Detta gör att arbetsytehanterare kan ansluta till den här posttypen från andra arbetsytor.\
     Du kan ange vilka arbetsytor som den här posttypen kan anslutas från. Du kan göra den tillgänglig för alla arbetsytor eller ange specifika arbetsytor där du kan importera den.
Mer information finns i [Konfigurera funktioner för arbetsytan över flera arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Fliken Redigera posttypsruta för avancerade inställningar](assets/edit-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types:
      1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
         * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
               You can designate specific users who can add this record type to other workspaces. 
         * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
               You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
         For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  
         ******** replace screen shot below **********
         ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
      -->

1. Klicka på **Spara**.

   Posttypkortet på arbetsytan visar en anslutningsikon ![Anslut från andra arbetsytor-ikon](assets/connect-from-other-workspaces-icon.png) i det övre högra hörnet för att ange att posten nu är tillgänglig från andra arbetsytor.

1. (Valfritt) Klicka på posttypskortet i arbetsytan för att öppna posttypens sida och byt sedan namn på posttypen i rubriken.

1. (Valfritt) Om du vill redigera en annan posttyp expanderar du den nedåtriktade pilen till höger om ett posttypsnamn, söker efter en posttyp och markerar den när den visas i listan.

   ![Listrutan Posttyp på posttypssidan med sökrutan](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
