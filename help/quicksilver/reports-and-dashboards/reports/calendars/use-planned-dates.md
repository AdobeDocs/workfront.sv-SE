---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Använd planerade datum i en kalenderrapport
description: En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda fältet Planerat datum i en kalenderrapport för uppgifter, utgåvor och projekt.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: 78cfafe4c9a0fb846533c04da392a09dc1dbc9f1
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Använd [!UICONTROL Planned Dates] i en kalenderrapport

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

En kalenderrapport är en dynamisk rapport som ger en visuell representation av ditt arbete. Du kan använda [!UICONTROL Planned Date] fält i en kalenderrapport för följande objekt:

* Uppgifter
* Problem
* Projekt

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards] och [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Manage] åtkomst till kalenderrapporten</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ställ in artikelgruppen i produktion

Du kan välja hur du vill att gruppen med objekt ska visas i din kalender.

{{step1-to-calendars}}

1. Markera den kalender som du vill lägga till en ny grupp med objekt i.
eller
Klicka på **[!UICONTROL + New Calendar]** och ange kalendernamnet.

   >[!NOTE]
   >
   >Du måste ha behörighet att redigera till rapporter, instrumentpaneler och kalendrar på åtkomstnivån för att skapa en kalenderrapport.

1. Klicka på **[!UICONTROL Add to Calendar]** till vänster och sedan på **[!UICONTROL Add advanced items]**.

1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Ange ett namn för gruppen med objekt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Välj en färg för gruppen med objekt. Alla objekt visas i den valda färgen i kalenderrapporten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Välj <strong>[!UICONTROL Planned dates]</strong>. Mer information om planerade datum finns i </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Översikt över projektets planerade startdatum</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Översikt över aktivitetens planerade startdatum</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Översikt över aktivitetens planerade slutförandedatum</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Ange projektplanerat slutförandedatum</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Visa i kalendern</strong></td>
      <td><p>Välj hur du vill att datumen ska visas:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: I kalendern visas objektet på ett enda datum.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: I kalendern visas objektet på ett enda datum.</li>
        <li><strong>[!UICONTROL Duration] (från början till slut)</strong>: I kalendern visas objektet över ett antal dagar.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>Kalendern växlar automatiskt till faktiska datum när de är tillgängliga. <br>Välj <strong>[!UICONTROL Yes]</strong> eller <strong>[!UICONTROL No]</strong> om du vill växla till faktiska datum när det är tillgängligt. Mer information om faktiska datum finns i</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Översikt över projektets faktiska startdatum </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Översikt över projektets faktiska slutförandedatum </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Fortsätt till följande avsnitt.

## Lägga till objekt i gruppen med objekt i produktion

När du har ställt in hur du vill att objekten ska visas måste du lägga till de objekt som du vill se i kalendern i grupperingen.

1. I avsnittet **[!UICONTROL What would you like to add to the calendar?]** väljer du

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Klicka på **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]** eller **[!UICONTROL Add Issues]**, beroende på vilken objekttyp du lägger till i kalendern.
   ![Välj objekt för kalendern](assets/field-name.png)

1. I listrutan börjar du skriva fältnamnet och väljer sedan fältkällan för objektet som du vill visa i kalendern (till exempel **[!UICONTROL Late Tasks]**).
1. Ange en villkorssats för kalendergrupperingen.

   ![Villkorssats](assets/condition-statement-calendar.png)

   Mer information om hur du ställer in villkor finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Valfritt) Ange ytterligare objekt för kalendergrupperingen genom att upprepa steg 1-4.
1. I fältet **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** väljer du hur objekten i den här kalendergruppen ska märkas i kalendern.

   >[!NOTE]
   >
   >Om standardetikettalternativen inte är tillgängliga för ett visst objekt visas objektnamnet i stället. Om etiketten [!UICONTROL Parent Task] till exempel är markerad och det inte finns någon överordnad aktivitet kopplad till objektet, visar [!DNL Adobe Workfront] objektnamnet som du visar i kalendern.

1. Klicka på **[!UICONTROL Save]**.

<!--

## Set up the group of items in Preview

You can choose how you want the group of items to display on your calendar.

{{step1-to-calendars}}

1. Select the calendar you want to add a new group of items to.
   Or
   Click **[!UICONTROL + New Calendar]** and enter the calendar name.

   >[!NOTE]
   >
   >You must have Edit access to Reports, Dashboards, and Calendars in your access level to create a calendar report.

1. On the left, click **[!UICONTROL Add to Calendar]**, then click **[!UICONTROL Add advanced items]**.

1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Type a name for the group of items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Select a color for the group of items. All items display in the selected color on the calendar report.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Planned dates]</strong>. For more information on planned dates, see </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overview of the project Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>On the calendar, show</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>The calendar automatically switches to actual dates when they are available. <br>Choose <strong>[!UICONTROL Yes]</strong> or <strong>[!UICONTROL No]</strong> to switch to actual dates when available. For more information on Actual Dates, see</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overview of the project Actual Start Date </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

## Add objects to the group of items in Preview

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, or **[!UICONTROL Add Issues]**, depending on the object type you are adding to the calendar.
   ![Select object for calendar](assets/field-name.png)

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.

   ![Condition statement](assets/condition-statement-calendar.png)

   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

1. Click **[!UICONTROL Save]**. 

-->