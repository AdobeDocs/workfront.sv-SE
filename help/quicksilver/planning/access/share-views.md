---
title: Visa
description: Du kan dela en vy med andra för att säkerställa samarbete när du använder Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Visa

{{planning-important-intro}}

Du kan dela en vy med andra för att säkerställa samarbete när du arbetar med poster i Adobe Workfront Planning.

Om du ger behörighet till en arbetsyta ger det inte andra användare behörighet till vyerna på posttypssidorna. Du måste tilldela behörigheter till enskilda vyer på en posttypsida för att kunna dela dem med andra användare.

När du delar en vy ger du andra behörighet att komma åt alla element i vyn. Om du till exempel ger dem behörigheten Hantera för en vy kan de ändra grupperingen, filtret, sorteringen eller utseendet på fält.


Du kan dela en vy med följande enheter:

* Workfront
* Workfront-grupper
<!--* Publicly, with users outside Workfront
-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p> Adobe Workfront</p> </td>
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
   eller
   <p>Aktuell: Planera </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td>
   <td> Det finns inga åtkomstkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Behörigheter</p></td>
   <td> <p>Hantera behörigheter till en vy</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/planning/access/access-overview.md">Åtkomstöversikt</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Dela behörigheter till en vy <!--internally-->

Du kan dela vyer som du har skapat eller vyer som du har behörigheten Hantera till <!--with users or groups in Workfront-->.

>[!NOTE]
>
>Systemadministratörer kan inte visa eller dela vyer som de inte själva skapat. De kan bara komma åt eller dela vyer som delas med dem.
>
>Systemadministratörer kan bara ha behörigheten Hantera för en vy.

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill dela och klicka sedan på ett posttypskort.

   Då öppnas posttypssidan.

1. Håll markören över den vy du vill dela på fliken Visa och klicka på **Mer** meny ![](assets/more-menu.png) till höger om vynamnet och klicka sedan på **Dela**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. (Valfritt) Välj bland följande alternativ för att dela vyn:

   * **Endast inbjudna personer har åtkomst**: Du måste ange användare eller grupper som du vill dela vyn med. Det här är standardalternativet.
   * **Alla på arbetsytan kan visa**: Alla användare som har behörighet att visa eller högre på arbetsytor kan komma åt vyn.

1. I **Ge vy åtkomst till** börjar du skriva namnet på en användare eller grupp och klickar sedan på den när den visas i listan.  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Välj någon av följande behörighetsnivåer i listrutan:
   * Visa
   * Hantera

     Mer information om behörighetsnivåer och vilka åtgärder användare kan utföra för varje nivå finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratörer får alltid behörigheten Hantera för vyer som delas med dem.

1. Klicka **Kopiera länk** om du vill kopiera en länk till vyn till Urklipp.
1. Dela den kopierade länken med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt posttypssidan och visa den i den valda vyn.
1. Klicka **Spara**.

   >[!TIP]
   >
   >   Vyer som delas med dig har en personindikator ![](assets/view-shared-with-others-people-icon.png) bredvid visningsikonen. Vyer utan personindikatorn är vyer som du har skapat.



<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-planning}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## Ta bort behörigheter till en vy

{{step1-to-planning}}

1. Öppna arbetsytan vars vy du vill sluta dela och klicka sedan på ett posttypskort. Då öppnas posttypssidan.
1. Håll muspekaren över fliknamnet för den vy du vill ta bort delning från och klicka på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Dela**.
1. Hitta användaren eller gruppen du vill ta bort och klicka sedan på **Ta bort** i listrutan Behörigheter till höger om användarens eller gruppens namn.
1. Klicka **Spara**.
Användaren eller användarna som tillhör gruppen som tagits bort har inte längre åtkomst till vyn. Användarna som har tagits bort från vyn får inget meddelande om att de har förlorat åtkomsten.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-planning}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->