---
title: Ta bort poster
description: Du kan ta bort poster som du eller någon annan användare har skapat. Du kan inte återställa borttagna poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---


# Ta bort poster

{{planning-important-intro}}

Du kan ta bort poster som inte längre är relevanta i Adobe Workfront Planning.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute eller högre behörighet till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p> </td> 
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

OLD

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
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront license*</p>
   </td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning </p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Att tänka på när du tar bort poster

* Du kan ta bort poster som du eller någon annan användare har skapat.
* Du kan inte återställa borttagna poster. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Om de borttagna posterna är länkade till andra poster tas de länkade posterna inte bort, men informationen från den borttagna posten tas också bort.
* Du kan inte ta bort flera poster samtidigt. <!--this will probably change-->
* Du kan inte ta bort poster från tidslinjevyn.

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
   * Håll markören över namnet på en post i tabellvyn, klicka på menyn **Mer** ![](assets/more-menu.png) och sedan på **Visa**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Postsidan öppnas.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om postnamnet, klicka sedan på **Ta bort** och sedan på **Ta bort** igen för att bekräfta.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Posten tas bort och kan inte återställas.

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
   * Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Ta bort**

     ![](assets/contextual-menu-for-record-row.png)

   * Klicka på ikonen **Öppna detaljer** ![](assets/open-details-icon-in-table-name-field.png) för att öppna rutan med postens detaljerade information, och klicka på **Mer** ![](assets/more-menu.png) till höger om postnamnet och sedan på **Ta bort**.

   Posten tas bort och kan inte återställas.

1. (Valfritt) Använd följande kortkommandon för att ångra eller göra om borttagning av en post:

   * CTRL + Z ( ⌘ + Z för Mac) för att ångra en ändring
   * CTRL + Skift + Z ( ⌘ + Skift + Z för Mac) för att göra om en ändring
