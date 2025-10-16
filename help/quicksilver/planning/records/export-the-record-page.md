---
title: Exportera postsidan
description: Du kan exportera en posts förhandsgransknings- eller informationssida från Adobe Workfront Planning till en Microsoft Word-fil.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Exportera information för en post

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


Om du vill samarbeta effektivare med andra som kanske inte har ett Workfront-konto kan du exportera en posts informationssida till en Microsoft Word-fil och dela den med dem.

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
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
eller
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Ljus eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Visa eller högre behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning.
   <p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p></div></li></ul>
</td>
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
   <td> <p>Light or higher</p>
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
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Att tänka på när du exporterar information om en post:

* Du kan exportera en posts information till följande filformat:

   * .docx Word
   * PDF

* Du kan bara exportera fliken Detaljer för en posts sida eller förhandsvisningsområde.

* Den exporterade filen bevarar postsidans layout, inklusive miniatyrbilderna och omslagsbilderna.

## Exportera information för en post

{{step1-to-planning}}

1. Klicka på kortet för en arbetsyta.

   Arbetsytan öppnas och posttyperna visas på kort.

1. Klicka på ett posttypskort.
Posttypssidan öppnas och alla poster av den typen visas.

1. Klicka i valfri vy på namnet på en post.

   Postens förhandsvisningsruta öppnas.

1. (Valfritt) Klicka på ikonen **Öppna på ny flik** ![Öppna information på en ny flikikon](assets/open-details-in-a-new-tab-icon.png) för att öppna postens sida.

1. Välj fliken **Detaljer**. Fliken Detaljer ska öppnas som standard.

1. Klicka på **Exportera**-menyn ![Exportikonen på postinformationssidan](assets/export-icon-in-record-details-page.png) antingen i förhandsgranskningen eller på postens sida och klicka sedan på något av följande:

   * **Microsoft Word**
   * **Adobe PDF**

   En Word-fil (.docx) eller en PDF-fil hämtas och sparas på datorn.

   Namnet på den exporterade filen är det primära fältet i posten.

   ![Exporterad ordfil](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Ytterligare information som inte visas på sidan och som bara visas när du har klickat på Visa mer i området med postinformation visas inte i den exporterade PDF-filen. Endast den information som visas på sidan visas i den exporterade filen.


1. (Valfritt) Gå till den hämtade filen, öppna den och redigera den (om det är en Word-fil) eller dela den med andra.

