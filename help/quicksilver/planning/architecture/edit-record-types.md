---
title: Redigera posttyper
description: Du kan redigera posttyper när de har sparats. Posttyperna är objekttyperna för Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---


# Redigera posttyper

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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
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
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Redigera posttyper

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera,

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Redigera**
eller
   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Redigera**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. I rutan **Redigera posttyp** öppnas fliken **Utseende** som standard.

   ![](assets/edit-record-type-box-appearance-tab.png)

   Uppdatera följande information på fliken **Utseende**:

   * Redigera posttypens namn om det behövs. <!--did they add a field label for this?-->
   * **Beskrivning**: Redigera eller lägg till en beskrivning för posttypen med mer information om den.
   * Redigera färg och form för ikonen som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar posttypen. Det här är färgen på ikonen för posttyp.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

1. (Villkorligt) Om du är systemadministratör klickar du på fliken **Avancerade inställningar** i rutan **Redigera posttyp** .

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Villkorligt) Som systemadministratör uppdaterar du följande information på fliken **Avancerade inställningar**:

   * **Anslut från andra arbetsytor**: Välj det här alternativet om du vill tillåta användare att ansluta till den här posttypen från andra arbetsytor. Detta är som standard avmarkerat.
   * **Systemomfattande**: Välj det här alternativet om du vill tillåta användare att ansluta till den här posten från alla arbetsytor i systemet.
   * **Specifika arbetsytor**: Välj det här alternativet om du vill begränsa de arbetsytor som användare kan ansluta till den här posttypen från. Utöka sedan listrutan och välj de arbetsytor som du vill att användarna ska ansluta till den här posttypen från. Du kan börja skriva namnet på en arbetsyta och markera den när den visas i listan.

1. Klicka på **Spara**.

   Posttypkortet på arbetsytan visar en anslutningsikon ![](assets/connect-from-other-workspaces-icon.png) i det övre högra hörnet för att ange att posten nu är tillgänglig från andra arbetsytor.

1. (Valfritt) Klicka på posttypskortet i arbetsytan för att öppna posttypens sida och byt sedan namn på posttypen i rubriken.

1. (Valfritt) Om du vill redigera en annan posttyp expanderar du den nedåtriktade pilen till höger om ett posttypsnamn, söker efter en posttyp och markerar den när den visas i listan.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)