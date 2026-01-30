---
product-area: projects;templates
navigation-topic: manage-projects
title: Spara ett projekt som en mall
description: Spara ett projekt som en mallSpara som mall på projektnivå, så att användarna ser det i användargränssnittet. Det finns en annan artikel där den här länken är mer detaljerad (steg för steg).
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Spara ett projekt som en mall

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<!--
<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

Om du bestämmer dig för att ett projekt ska inträffa igen någon gång i framtiden kan du skapa en mall från det befintliga projektet. Sedan kan du använda mallen igen för att skapa framtida projekt som kan innehålla liknande information eller som kan dela samma tidslinje eller tilldelningar med det befintliga projektet.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt </p> <p>Du får behörigheten Hantera för mallen när du har sparat projektet som en mall</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p>
   Or 
   <p>Current: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> /td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Spara ett projekt som en mall

<!--
Saving a project as a template differs in the Production and the Preview environments. 

### Save a project as a template in the Production environment


1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/more-icon.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td>Use the drop-down list to select any custom forms to attach to the template. If any custom forms have already been associated with the project, all of the data fields from those custom forms are displayed.<br>You can include up to 10 custom forms on a single template.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Manage Forms** to remove or reorder the forms. For information about how to remove and reorder custom forms on the template, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![Save as template first step](assets/save-as-template-first-step-350x159.png)

1. Click **Next Step.**
1. In the **Options** section, select the checkbox beside any information you want to clear from the template.

   ![Save as template options step](assets/save-as-template-options-step-350x109.png)

1. Click **Next Step.**
1. In the **Exclude** section, select any tasks that you want to exclude from the project.

   ![Save as template exclude](assets/save-as-template-exclude-350x205.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates and can either be attached to an existing project or used to create a new one.


<div class="preview">

### Save a project as a template in the Preview environment

-->

1. Gå till det projekt som du vill spara som en mall.
1. Klicka på ikonen **Mer** meny ![Mer](assets/qs-more-icon-on-an-object.png) till höger om projektnamnet i sidhuvudet och sedan på **Spara som mall**.
1. I avsnittet **Spara som mall** anger du följande information för mallen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mallnamn</td> 
      <td>Ange ett namn för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för mallen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ja</strong>: Andra användare kan hitta mallen och bifoga den till projekt.</p> </li> 
        <li><strong>Nej</strong>: Andra användare kan inte hitta mallen och kan inte bifoga den till projekt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Använd listrutan för att välja anpassade formulär som ska bifogas mallen. Om några anpassade formulär redan har associerats med projektet visas alla datafält från dessa anpassade formulär.<br>Du kan inkludera upp till 10 anpassade formulär i en enda mall.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Egen Forms** i den vänstra panelen för att ta bort eller ändra ordningen på formulären.

   Om du vill ändra ordningen på formulären drar och släpper du dem i rätt ordning.
Om du vill ta bort ett formulär markerar du det och klickar sedan på **Ta bort**. Klicka på **Avbryt** om du vill ta bort de markerade formulären.

   ![Anpassade formulärområden i rutan Spara som mall](assets/custom-forms-ara-in-save-as-template-box.png)

1. Uppdatera information i de bifogade anpassade formulären, om det behövs. Informationen överförs till mallen.

1. Klicka på **Alternativ** i den vänstra panelen och markera sedan kryssrutan bredvid information som du vill överföra till mallen. Avmarkerade objekt överförs inte till mallen. Alla alternativ är som standard avmarkerade.

   ![Alternativ i rutan Spara som mall](assets/options-area-in-save-as-template-box.png)

1. Klicka på **Uteslut** i den vänstra panelen och välj sedan de uppgifter som du vill utesluta från projektet. Alla åtgärder avmarkeras som standard.

   ![Uteslut område i rutan Spara som mall](assets/exclude-area-save-as-template-box.png)

1. Klicka på **Slutför och spara mall** i skärmens övre högra hörn.

   Mallen visas nu i listan med tillgängliga mallar och kan antingen bifogas till ett befintligt projekt eller användas för att skapa ett nytt.

