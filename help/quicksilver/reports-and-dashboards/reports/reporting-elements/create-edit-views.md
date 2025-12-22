---
product-area: reporting
navigation-topic: reporting-elements
title: Skapa eller redigera vyer i Adobe Workfront
description: Du kan anpassa vilken typ av information som visas på skärmen med hjälp av vyer. Du kan använda flera typer av vyer i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 0%

---

# Skapa eller redigera vyer i Adobe Workfront

<!-- Audited: 11/2024 -->

Du kan anpassa vilken typ av information som visas på skärmen med hjälp av vyer. Du kan använda flera typer av vyer i Adobe Workfront.

I den här artikeln beskrivs hur du skapar och redigerar standardvyer för listor och rapporter.

Mer information finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</strong></td> 
   <td> 
    <p>Medarbetare eller högre</p>
    <p>Begäran eller senare</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att skapa en vy i en rapport</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att skapa eller redigera en vy i en rapport</p> <p>Hantera behörigheter till en vy för att redigera den</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Skapa eller anpassa en vy

Hur du skapar eller anpassar en vy varierar beroende på om du skapar eller anpassar en standardvy eller en styrelsvy.

### Skapa eller anpassa en standardvy {#create-or-customize-a-standard-view}

Du kan skapa en ny standardvy eller anpassa en befintlig standardvy som du skapade tidigare.

1. Klicka på listrutan **Visa** i en lista där du vill skapa eller anpassa en vy.

1. Klicka på knappen **+ Ny vy** för att skapa en ny vy.
eller
Klicka på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) som visas i muspekaren till höger om en befintlig vy som du vill redigera.
Dialogrutan **Anpassa vy** visas.

1. Gör något av följande i avsnittet **Förhandsvisa kolumn**:

   * Ändra värdet för en kolumn genom att klicka på kolumnrubriken och sedan markera ett nytt fält.
   * Lägg till en kolumn genom att klicka på **Lägg till kolumn**, börja skriva namnet på kolumnen som du vill lägga till och klicka sedan på den när den visas i listrutan.
   * Justera den ordning som kolumnerna visas i genom att dra kolumnrubriken till en ny plats.

   * Klicka på **Sammanfatta den här kolumnen med** i området **Kolumninställningar** och välj hur du vill att data ska visas i kolumnen. Det här alternativet är tillgängligt för följande kolumntyper:
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Datumfält</strong></td> 
           <td><ul>
           <li>Maximal</li>
         <li>Minimum</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Valutafält</strong></td> 
           <td><ul>
           <li>Antal</li>
         <li>Summa</li>
           <li>Genomsnittlig</li>
         <li>Maximal</li>
           <li>Minimum</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Sträng- och booleska fält</strong></td> 
           <td><ul><li>Antal</li></ul>
           <p>Obs! Workfront rekommenderar vanligtvis inte att du sammanfattar ett booleskt fält utifrån antal eftersom värdet alltid är true/false.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du sammanfattar värden för följande fält i grupperingar:
     >   
     > * Alla sifferfält och valutafält utom Faktiska timmar (t.ex. Planerad/Faktisk arbetskostnad, Planerad/Faktisk kostnad, Planerad/Faktisk kostnad, Planerad/Timmar) sammanfattar värdena för enbart underordnade aktiviteter och fristående aktiviteter. De sammanfattar inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
     > * Faktiska timmar sammanfattar värdena för de överordnade och de fristående aktiviteterna. De sammanfattar inte siffrorna för de överordnade aktiviteternas överordnade eller underordnade aktiviteternas överordnade aktiviteter.
     > * Anpassade datafält för tal- och valutavärden sammanfattar alla uppgifter: överordnade, underordnade, överordnade och fristående uppgifter.
     >
     >Mer information om hur du använder grupperingar i en rapport finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Valfritt) Klicka på **Avancerade alternativ** för att ange följande information för kolumnen:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etikett för anpassad kolumn</strong></td> 
           <td><p>Ange en anpassad etikett för kolumnen. Den här etiketten ersätter standardetiketten. Vi rekommenderar att du endast använder UTF-8-tecken för att undvika kompatibilitetsproblem.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Fältformat</strong></td> 
           <td>Välj i vilket format du vill att värdena ska visas för fälten i kolumnen.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Visa den här kolumnen när du arbetar på en instrumentpanel</strong></td> 
           <td><p>Välj det här alternativet om du vill visa den här kolumnen på en kontrollpanel när rapporten visas sida vid sida med en annan rapport. När det här alternativet är avmarkerat visas inte den här kolumnen när du visar rapporten på en kontrollpanel där rapporter visas sida vid sida.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Kolumnregler</strong></td> 
           <td><p>Klicka på <strong>+ Lägg till en regel för den här kolumnen </strong> för att definiera en regel för kolumnen. När du har lagt till en regel kan du definiera fält- och textformat för hur fält som matchar den regeln visas. Klicka på <strong>Lägg till regel</strong> när du har definierat regeln.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Mer information om villkorlig formatering av vyer i rapporter finns i artikeln [Använd villkorsstyrd formatering i textläge](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Villkorligt) Om du klickade på **Avancerade alternativ** klickar du på **Klar**.

1. Klicka på **Spara vy** om du vill skapa en ny vy eller ersätta den aktuella vyn med ändringarna.\
   eller\
   Klicka på **Spara som ny vy** om du vill spara ändringarna som en ny vy.

   >[!TIP]
   >
   >**Spara som ny vy** är det enda tillgängliga alternativet när du anpassar en inbyggd Workfront-vy.

   Åtkomsten styr hur vyn sparas. Om du skapade vyn från början kan du spara ändringarna. Annars uppmanas du att spara en version. Tänk på att de ändringar du gör i vyn påverkar användare som vyn har delats med.

### Skapa eller anpassa en styrelsvy {#create-or-customize-an-agile-view}

Du kan hantera projekt enligt en Agile-metod med hjälp av en styrelse.

Styrelsevyer är bara tillgängliga för listor över uppgifter och frågor i ett projekt.

De är förkonfigurerade, men du kan ändra vissa inställningar för dem.

Mer information om Agile- och Board-vyer finns i artikeln [Hantera ett Agile-projekt i styrelsvyn](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the Agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the Agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the Agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
