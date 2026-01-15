---
title: Konfigurera inställningsområdet för en posttyp
description: Förutom att redigera en posttyp i rutan Redigera posttyp kan du även redigera posttyper på sidan Inställningar.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---


# Konfigurera inställningsområdet för en posttyp

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan konfigurera ytterligare inställningar för en posttyp efter att de har sparats i Adobe Workfront Planning.

Beroende på vilka funktioner du vill definiera för en posttyp kan du konfigurera ytterligare inställningar genom att göra något av följande:

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
<p>Alla Workfront- och Planning-paket</p>
<p>Alla arbetsflödes- och planeringspaket</p>

<p><b>ANMÄRKNING</b></p>

<p>Så här konfigurerar du kopplingsbara posttyper:</p>

<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
eller
<li><p>Alla arbetsflödespaket och ett Planning Prime- eller Ultimate-paket</p></li></ul>

<p>Så här konfigurerar du globala posttyper:</p>

<ul> 
<li><p>Alla Workfront-paket och ett Planning Plus-paket</p></li>
eller
<li><p>Alla arbetsflödespaket och ett Planning Prime- eller Ultimate-paket</p></li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
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

     ![Fler menyalternativ från posttypskort](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     eller

   * Klicka på ett posttypskort för att öppna posttypssidan, klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn och klicka sedan på **Inställningar**.

   <!--update screen shot at prod??-->

   ![Inställningar för arbetsytan mellan arbetsytor på sidan Inställningar](assets/settings-page-cross-workspace-settings.png)

1. Avsnittet **Inställningar för arbetsytan mellan arbetsytor** är markerat som standard.
1. Aktivera eller inaktivera någon av följande inställningar:

   * **Tillåt att den här posttypen läggs till i andra arbetsytor** för att ange att det här är en global posttyp
   * **Tillåt anslutning till den här posttypen i andra arbetsytor** för att ange att det här är en kopplingsbar posttyp.

   Inställningarna är inaktiverade som standard.

   Mer information finns i [Konfigurera funktioner för arbetsytan över flera arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)