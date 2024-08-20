---
title: Redigera posttyper
description: Du kan redigera posttyper när de har sparats. Posttyperna är objekttyperna för Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Redigera posttyper

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. Du kan redigera utseendet på posttyper som du eller någon annan har skapat. Mer information om hur du skapar posttyper för Workfront Planning finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>Om du vill ansluta posttyper för Adobe Workfront Planning till Experience Manager Assets måste du ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Endast systemadministratörer kan aktivera posttyper för anslutning från andra arbetsytor</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Workfront- eller gruppadministratören måste lägga till planeringsområdet i layoutmallen. Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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