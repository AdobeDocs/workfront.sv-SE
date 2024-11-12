---
product-area: reporting
navigation-topic: text-mode-reporting
title: Redigera en vy i textläge
description: 'OBS! Lägg till ett avsnitt i den här artikeln: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Utkast till det här området i översiktsartikeln om textläge)'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Redigera en vy i textläge

<!--Audited: 01/2024-->

<!--
<add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Du kan redigera en vy i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa vyer.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard </p>
   <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera vyer i en rapport</p> <p>Hantera behörigheter till en vy för att redigera den</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.
Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar använda textläge i en rapport eller lista bör du alltid kontrollera att du känner till Workfront textläge.

Mer information finns i:

* [Textläge - översikt](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Anpassad vy, filter och gruppering av exempel: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Redigera textläge i en vy

Att redigera en vy i textläge är identiskt för rapporter och listor. Åtkomsten till vyn från en rapport eller från en lista skiljer sig åt.

>[!TIP]
>
>Vi rekommenderar att du skapar så mycket som möjligt av vyn i standardläge och sedan konverterar den till textläge för att redigera den.

Mer information om hur du skapar vyer finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gör något av följande:

   1. Gå till rapporten och klicka sedan på **Rapportåtgärder** > **Redigera** > **Kolumner (vy)** för att få åtkomst till vyn från en rapport.
   1. Om du vill få åtkomst till vyn från en lista går du till listan och från listrutan **Visa** håller du musen över den vy du vill ändra och klickar på ikonen **Redigera** ![](assets/edit-icon.png) .

      Vyverktyget öppnas.

1. Markera en kolumn i vyn.

   eller

   Välj fliken **Kolumner (Visa)** i rapportverktyget och markera sedan en kolumn.

   >[!TIP]
   >
   >Om du vill redigera en vy i textläge måste du redigera en kolumn i taget.

1. Klicka på **Växla till textläge** i det övre högra hörnet av verktyget och klicka sedan på **Redigera textläge**.

   >[!NOTE]
   >
   >När du redigerar en kolumn i textläge lägger Workfront till kodraden `textmode=true` i kolumnen. Detta anger att kolumnen ändras i textläge.

   Följande tabell visar nyckelraderna i en textlägesvy:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Exempelrad</th> 
      <th>Beskrivning</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><ol><tr><tr><ol><tr><tr><tr><tr><tr><tr><tr><tr><tr><tr><div class="example" data-mc-autonum="<b>Example: </b>"><code><strong>valuefield</strong>=</cod></p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
        
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p> <p>For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.</p> </td> 
     </tr> 
      
      <td><code><strong>valueformat=</strong></code> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
      
      <td> <p><code><strong>valueexpression=</strong></code> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist: </p> 
        
        <li value="1"> <p>If you want to display a field in a column in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li> 
        <li value="3"> <p>For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p> <p>Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see <span help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a></span>.</p> <p>For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
      
      <td> <p><code><strong>descriptionkey=</strong></code> / <code><strong>description=</strong></code> </p> </td> 
      <td> <p>This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
      
      <td><code><strong>namekey=</code> / <code><strong>name=</strong></code> </td> 
      <td> <p>This line defines the column label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the column name you can change this value to: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p> <p>To change the column name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
      
      <td><code><strong>displayname =</strong></code> </td> 
      <td> <p>You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
      
      <td><code><strong>querysort=</strong> </code></td> 
      <td>This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td> 
     </tr> 
      
      <td><code><strong>width=</strong></code> </td> 
      <td> <p>This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p> <p>When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p> </td> 
     </tr> 
      
      <td><code><strong>usewidths=true</strong></code> </td> 
      <td> <p>You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p> </td> 
     </tr> 
      
      <td><code><strong>makeFieldEditable=</strong></code> </td> 
      <td> <p>This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true</strong>, the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valuefield=</strong> </code></td> 
      <td> <p>Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p> <p> For example, you can insert <code>link.valuefield=priority</code> in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valueformat=</strong> </code></td> 
      <td> <p>Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p> <p>Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are<code> link.valuefield</code> and <code>link.valueformat</code>. </p> </td> 
     </tr> 
      
      <td><code><strong>aggregator.function=</strong></code> </td> 
      <td> <p>This refers to how the values of each column are summarized. There are multiple lines that start with <code>aggregator.</code> and they all refer to the aggregator that summarizes the results of the column. </p> <p>As a general rule, the <code>aggregator.</code> lines match those of the column object. </p> 
       
        <span class="autonumber"><span><b>Example: </b></span></span> 
        <p>The Planned&nbsp;Hours column in a task report summarized by Sum may look like the following: </p>

   <div>
         <code>textmode=true</code>
         <code>valuefield=workRequired</code>
         <code>valueformat=compound</code>
         <code>aggregator.function=SUM</code>
         <code>aggregator.valuefield=workRequired</code>
         <code>aggregator.displayformat=minutesAsHoursString</code>
         <code>aggregator.valueformat=compound</code>
         <code>namekey=workRequired</code>
         <code>shortview=false</code> 
        </div> 
       </div>

   <div>
      <code>aggregator. </code> rader kan innehålla <code>valuefield </code> eller <code>valueexpression</code>.
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Använd** om du vill spara ändringarna och fortsätta redigera vyn.
1. Klicka på **Spara + stäng** för att spara rapporten.

   eller

   Klicka på **Spara vy** för att spara vyn i en lista.
