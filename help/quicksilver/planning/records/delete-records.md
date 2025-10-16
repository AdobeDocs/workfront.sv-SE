---
title: Ta bort poster
description: Du kan ta bort poster som du eller någon annan användare har skapat.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Ta bort poster

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Du kan ta bort poster som inte längre är relevanta i Adobe Workfront Planning. Du kan återställa borttagna poster i 30 dagar efter att de tagits bort. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

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
<p>Alla Workfront- och Planning-paket</p> <p>Alla arbetsflöden och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Contribute eller högre behörighet för en arbetsyta och en posttyp  </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller någon annan användare har skapat.
* Du kan återställa borttagna poster som du eller andra har tagit bort.
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort.
* Du kan inte ta bort poster från tidslinjen eller kalendervyer.

## Ta bort poster

Du kan ta bort en post från följande områden:

* [Från postens sida](#delete-a-record-from-the-records-page)
* [Från tabellvyn för en posttyp](#delete-a-record-from-the-record-type-table-view)

### Ta bort en post från postens sida

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. Gör något av följande:

   * Klicka på en posts namn i en tabellvy.
   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![Mer](assets/more-menu.png) och klicka sedan på **Visa**

     ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Postsidan öppnas.

1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om postnamnet, klicka sedan på **Ta bort** och sedan på **Ta bort** igen för att bekräfta.

   ![Fler menyalternativ från postinformationssidan](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Posten tas bort.
1. (Valfritt) Gå till tabellvyn på postsidan och klicka på ikonen **Ångra** ![Ångra &#x200B;](assets/undo-icon.png) i det övre högra hörnet av vyn. Klicka sedan på **Senast borttagen** för att återställa de borttagna posterna.

Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).

### Ta bort en post från posttyptabellvyn

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill ta bort.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Välj en tabellvy på den nedrullningsbara menyn **Visa** i tabellens övre vänstra hörn. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Gör något av följande:

   * Högerklicka på en postrad och klicka sedan på **Ta bort**.
   * Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Ta bort**.

     ![Sammanhangsbaserad meny för postrad](assets/contextual-menu-for-record-row.png)

   * Klicka på ikonen **Öppna detaljer** ![Öppna detaljikonen i tabellnamnsfältet](assets/open-details-icon-in-table-name-field.png) för att öppna rutan med postens detaljerade information. Klicka sedan på **Mer** ![Mer-menyn](assets/more-menu.png) till höger om postnamnet och sedan på **Ta bort**.

   Posten tas bort.

1. (Valfritt) Gör något av följande om du vill ångra eller göra om borttagning av en post:

   * Klicka på ikonen **Ångra** ![Ångra &#x200B;](assets/undo-icon.png) och sedan på **Senast borttagen** för att återställa de borttagna posterna. Mer information om hur du återställer borttagna poster finns i [Återställa borttagna poster](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Använd följande kortkommandon för att ångra eller göra om borttagning av en post:

      * CTRL + Z (⌘ + Z för Mac) för att ångra borttagning av en post
      * CTRL + Skift + Z (⌘ + Skift + Z för Mac) för att ta bort post igen




