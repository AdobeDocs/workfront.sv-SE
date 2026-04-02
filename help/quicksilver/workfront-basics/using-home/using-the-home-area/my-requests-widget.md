---
product-area: projects
navigation-topic: use-the-home-area
title: Använda widgeten Mina förfrågningar
description: Du kan skicka begäranden i widgeten Mina förfrågningar. Du kan också anpassa widgeten med filter och kolumner.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# Använda widgeten Mina förfrågningar

<!--remove Preview and Production references at Production release April 15, 2026-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>Den här artikeln beskriver den nya widgeten Mina förfrågningar. Du måste ha den nya upplevelsen som begär aktiverad för att kunna se den nya widgeten.
>Du kan aktivera den nya begärandeupplevelsen i området Förfrågningar.

Widgeten Mina förfrågningar visar förfrågningar som du har skickat in. Du kan filtrera förfrågningar, söka efter specifika förfrågningar eller justera kolumnordningen och synligheten. Du kan också skapa en ny begäran från widgeten Mina förfrågningar.

>[!NOTE]
>
>* När widgeten Mina förfrågningar läses in visas upp till 50 förfrågningar. Om du vill visa fler begäranden rullar du nedåt i listan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alla Workfront- eller Workflow-paket</p>
   <p>Alla Workfront Planning-paket som kan användas för att komma åt Workfront Planning-begäranden och skapade objekt</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa eller ge senare åtkomst till objekt som du har taggat i en konversation eller behöver lösa ett godkännande (Projekt, Åtgärder, Problem, Dokument)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] behörigheter eller högre till projekt, uppgifter, problem, dokument där du är taggad i en konversation eller behöver lösa ett godkännande</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en förfrågan

Du kan skapa en begäran direkt från widgeten Mina förfrågningar.

Instruktioner finns i avsnittet [Skapa en begäran](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) i artikeln [Skapa arbetsobjekt och projekt från Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Kopiera en begäran

Du kan kopiera en begäran i widgeten Mina förfrågningar, redigera den och skicka den som en ny begäran.

Instruktioner finns i [Kopiera och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Hantera information i listan över förfrågningar i widgeten Mina förfrågningar

<!--
This is similar to what we document in Enhanced lists, so we will link to that to avoid documentation duplication:
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. (Valfritt) Om du vill hantera hur informationen visas i listan med begäranden skapar eller uppdaterar du följande vyelement för listan:

   * Visa
   * Filter
   * Kolumner

   <div class="preview">

   * Grupp
   * Formatera celler
   * Radhöjd

   </div>

   Mer information om hur du uppdaterar vyelement i listan över förfrågningar finns i [Använda förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!--
 Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.
The filter is saved automatically.
-->

>[!TIP]
>
>Om din organisation har köpt Workfront Planning förutom Adobe Workfront, kommer widgeten Mina förfrågningar att innehålla både Workfront- och Workfront Planning-förfrågningar.
> 
>* Om du bara vill filtrera efter Workfront-begäranden anger du filtret till **Objekttyp** > **Har något av** > **Problem**.
>* Om du bara vill filtrera efter Workfront Planning-begäranden anger du filtret till **Objekttyp** > **Har inga av** > **Problem**.

<!--

Use enhanced lists and other requests articles describe all of these:

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Sökbegäranden

Så här söker du efter specifika förfrågningar i widgeten Mina förfrågningar:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. I sökfältet uppe till höger i widgeten Mina förfrågningar anger du den term som du vill söka efter.

   Förfrågningar som innehåller termen markeras med orange.

1. (Valfritt) Om du vill gå till de markerade förfrågningarna klickar du på upp- eller nedpilarna i sökfältet.

## Gå till ett objekt som skapats av en begäran

Du kan söka efter objekt som har skapats av en begäran i widgeten Mina förfrågningar.

>[!NOTE]
>
>Följande objekt har länkar från listan över förfrågningar i widgeten Mina förfrågningar när du aktiverar den nya upplevelsen av förfrågningar i området Förfrågningar:
>
>* Planering och Workfront-begäranden i ämnesfältet.
>* Planeringsposter som har skapats från planeringsbegäranden i fältet Objekt som har skapats.
>* <span class="preview">Workfront-uppgifter och -problem som konverterats från Workfront-begäranden i fältet Objekt som skapats i förhandsgranskningsmiljön.</span>

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/lines-main-menu.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Om du vill lägga till widgeten **Mina förfrågningar** på hemskärmen. Klicka på **Anpassa** och sök efter **Mina förfrågningar**. Klicka sedan på den för att lägga till den i **Hem**.
1. Leta reda på den begäran som skapade objektet.
1. Klicka på objektnamnet i kolumnen **Skapat objekt** för den begäran.

   Objektets sida öppnas.

   >[!TIP]
   >
   >I produktionsmiljön har bara planeringsposter en länk i fältet **Skapat objekt**.
   >   
   ><span class="preview">I förhandsgranskningsmiljön har Workfront-aktiviteter och -projekt som konverterats från problem samt planeringsposter som skapats från planeringsbegäranden en länk i fältet **Skapat objekt**.</span>
   >



