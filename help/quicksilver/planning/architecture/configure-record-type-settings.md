---
title: Konfigurera inställningsområdet för en posttyp
description: Du kan redigera posttyper efter att de har sparats på sidan Inställningar.
hide: true
hidefromtoc: true
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


<!--add better metadata at release:

title: Configure Record Type Settings
description: You can edit record types after they have been saved in the Settings page. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog 

-->

# Konfigurera inställningsområdet för en posttyp

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan konfigurera ytterligare inställningar för en posttyp efter att de har sparats i Adobe Workfront Planning.

Beroende på vilka funktioner du vill definiera för en posttyp kan du konfigurera ytterligare inställningar för den genom att göra något av följande:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Redigera dem

  Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

* Konfigurerar sidan Inställningar för en posttyp.

  I den här artikeln beskrivs hur du kan redigera en posttyp genom att konfigurera sidan Inställningar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Alla Workfront-paket</p></li>
<p>Och</p>
<li><p>Planeringspaket för att skapa kopplingsbara posttyper</p></li>
<li><p>Planning Plus-paket för att skapa centraliserade posttyper</p></li>
</ul>
<p>Eller:</p>
<ul><li><p>Ett Workflow and Planning Prime- eller Ultimate-paket</p> </li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av din kontoansvarige på Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> 

-->

## Konfigurera posttypsinformation på sidan Inställningar

Du kan definiera funktioner för olika arbetsytor för en posttyp genom att konfigurera information på sidan Inställningar.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill redigera,

   Arbetsytans sida öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll muspekaren över kortet för en posttyp och klicka på menyn **Mer** ![Mer](assets/more-menu.png) i det övre högra hörnet av posttypskortet och klicka sedan på **Inställningar**
eller
   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Inställningar**.

   <!--update screen shot at release-->

   ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card.png)

1. Avsnittet **Inställningar för arbetsytan mellan arbetsytor** är markerat som standard.
1. Aktivera eller inaktivera någon av följande inställningar:

   * **Tillåt att den här posttypen läggs till i andra arbetsytor** för att ange att det här är en global posttyp
   * **Tillåt anslutning till den här posttypen i andra arbetsytor** för att ange att det här är en kopplingsbar posttyp.

   Inställningarna är inaktiverade som standard.

   Mer information finns i [Konfigurera funktioner för arbetsytan över flera arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)