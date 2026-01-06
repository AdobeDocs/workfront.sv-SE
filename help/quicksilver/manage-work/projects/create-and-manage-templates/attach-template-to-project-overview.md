---
content-type: overview
product-area: templates
keywords: överskrivning,fält,överskriven
navigation-topic: templates-navigation-topic
title: Översikt över att bifoga en mall till ett projekt
description: När du bifogar en mall till ett befintligt projekt ändrar du en del av informationen i projektet enligt mallen. En del av informationen i projektet ändras inte.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Översikt över att bifoga en mall till ett projekt

När du bifogar en mall till ett befintligt projekt ändrar du en del av informationen i projektet enligt mallen. En del av informationen i projektet ändras inte.

Mer information om hur du bifogar en mall till ett projekt finns i [Koppla en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Att tänka på när du lägger till mallar i projekt

Tänk på följande när du lägger till mallar i projekt:

* Du kan bara bifoga aktiva mallar till projekt.
* Du kan bara bifoga en mall till ett projekt när projektet har statusen Fullständigt, Inaktuellt eller Väntar på godkännande om Adobe Workfront-administratören eller en gruppadministratör har aktiverat den här funktionen i området Projektinställningar. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Såvida du inte utesluter att specifika malluppgifter läggs till i den bifogade processen, läggs alla malluppgifter till i det befintliga projektet.
* De flesta mallinställningar läggs till i projektet. Vissa projektinställningar bevaras. Mer information finns i avsnittet [Förstå ändringar i projektfält när du bifogar en mall](#understand-changes-to-project-fields-when-attaching-a-template) i den här artikeln.

## Förstå ändringar i projektfält när en mall bifogas {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Att bifoga en mall till ett projekt är inte detsamma som att skapa ett projekt från en mall. När du skapar ett projekt från en mall överförs alla mallfält till det nya projektet. När du bifogar en mall ändras inte vissa av de befintliga projektfälten.

Vissa mallinställningar överförs automatiskt till projektet, såvida du inte särskilt markerar att de inte ska tas med vid mallbifogningsprocessen. När du markerar dem som uteslutna bevaras projektfältets värden.

Alla projektfält är dock inte tillgängliga för hantering när en mall bifogas till ett projekt. Mer information finns i [Koppla en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

I följande tabell beskrivs standardinställningen för vad som händer med projektfält när du kopplar en mall och vilka fält som du kan hantera under bilageprocessen för att åsidosätta standardbeteendet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Fält</td> 
   <td>Vad händer när en mall bifogas som standard</td> 
   <td>Möjlighet att hantera fältuppdateringarna i bilageprocessen </td> 
  </tr> 
  <tr> 
   <td>Beskrivning</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Överfört från mall, om fältet är tomt i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Prioritet</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Villkorstyp</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schemaläge</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planerade datum</td> 
   <td>Kan ändras baserat på de tillagda uppgifterna</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Faktiska datum</td> 
   <td>Kan ändras baserat på de tillagda uppgifterna</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupp</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Företag</td> 
   <td>Överfört från mall, om fältet är tomt i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planerade timmar</td> 
   <td>Kan ändras baserat på de tillagda uppgifterna</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektägare</td> 
   <td>Överfört från mall, om fältet är tomt i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektsponsorer</td> 
   <td>Överfört från mall, om fältet är tomt i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resurshanteraren</td> 
   <td>Tillagd i listan över befintliga resurshanterare i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Anpassad Forms</td> 
   <td>Har lagts till i projektet, förutom formulär som redan finns i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Valuta</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planerad förmån</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Faktisk förmån</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sökväg för milstolpe</td> 
   <td>Överfört från mall, om fältet är tomt i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Slutförandeläge</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Läge för slutförande av sammanfattning</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uppdateringstyp</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schema</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Användningstid av</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resursutjämningsläge</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risk (projektfält)</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resursgrupper</td> 
   <td>Tillagd i listan över befintliga resurspooler i projektet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Timtyper</td> 
   <td> <p>Om du avmarkerar alternativet under bilageprocessen ändras inte inställningen Timtyper i projektet. </p> <p>Om du väljer det här alternativet överförs mallinställningen till projektet. Om filtreringen för timtyp är inställd på Ja både i projektet och i mallen läggs timtyperna från mallen till i typerna i projektet.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Påminnelsemeddelanden</td> 
   <td> <p>Lades till i listan över befintliga påminnelser för projektet. </p> <p>Om du avmarkerar alternativet under bilageprocessen ändras inte påminnelsemeddelandena för projektet. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Standardprocess för godkännande av uppgift</td> 
   <td>Projektinformationen bevaras</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Anpassad Forms för aktivitetsstandard</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Arbetsinsats</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Tillåt användare att lägga till interna utgåvor</span> </td> 
   <td><span>Projektinformation bevaras</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Alla inställningar</td> 
   <td>Mallinställningar skriver över projektinställningarna</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uppgifter</td> 
   <td>Lades till längst ned i uppgiftslistan, utöver befintliga projektuppgifter</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>Tillagt i projektet, utöver befintliga projektdokument</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risker (objekt i området Risker i projektet)</td> 
   <td>Som läggs till i projektet, utöver befintliga projektrisker </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Godkännandeprocess</td> 
   <td>Överförd från mall</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Faktureringstaxor</td> 
   <td> <p>Överfört från mallen utöver de befintliga faktureringspriserna för projektet. </p> <p>Om det finns olika hastigheter för samma jobbroll för både projektet och mallen ändras inte hastigheten på projektet. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Faktureringsposter</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Utgifter</td> 
   <td>Överfört från mallen utöver befintliga utgifter för projektet</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ekonomisk information</td> 
   <td> <p>När detta väljs i bilageprocessen överförs eller läggs följande fält till i projektet: </p> 
    <ul> 
     <li> <p>Fast kostnad</p> <p>När alternativet är markerat beräknas den uppdaterade fasta kostnaden för projektet med följande formel:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Fast intäkt</p> <p>När alternativet är markerat beräknas projektets uppdaterade fasta inkomster med följande formel:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Kostnadstyp för uppgifter</p> <p>Överförd från mall</p> </li> 
     <li> <p>Inkomsttyp för uppgifter</p> <p>Överförd från mall</p> </li> 
    </ul> <p>Om det här fältet avmarkeras under bilageprocessen inträffar följande:</p> 
    <ul> 
     <li> <p>Fasta kostnader och fasta intäkter i projektet bevaras.</p> </li> 
     <li> <p>Kostnads- och intäktstyperna för de uppgifter som läggs till från mallen anges till Ingen kostnad och Inte fakturerbar</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Timmar</td> 
   <td>Projektinformationen bevaras</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Köinformation, ämnesgrupper, köämnen, routningsregler</td> 
   <td> <p>Överförd från mall</p> <p>Om du väljer alternativet <strong>Köegenskaper och inställningar för problem</strong> under bilageprocessen skriver köinformationen för mallen över projektets. I det här fallet läggs reglerna för routning, köämnen och ämnesgrupper i mallen till i projektets. <br>Om projektet har konfigurerats som en begärandekö och mallen som du bifogar till projektet inte har ställts in som en begärandekö, tas köinformationen bort om du inte markerar kryssrutan <strong>Köegenskaper och inställningar för problem</strong> . <br>Om du avmarkerar kryssrutan <strong>Köegenskaper och utgivningsinställningar</strong> bevaras alla inställningar för köinställningar för projektet och inga köinställningar från mallen bifogas.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Aktivitetsbegränsningar</td> 
   <td> <p>Överförd från mall </p> <p>Om det här alternativet inte är markerat under bilageprocessen anges aktivitetsbegränsningarna till Så snart som möjligt eller Sent som möjligt, beroende på inställningen Projektschema från. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Föregående aktiviteter</td> 
   <td> <p>Överförd från mall</p> <p>Om du avmarkerar alternativet under bilageprocessen tas alla föregående anslutningar mellan malluppgifterna bort.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delningsalternativ</td> 
   <td> <p>Om du avmarkerar alternativet under bilageprocessen ändras inte projektbehörigheterna.</p> <p>Om det här alternativet väljs under bilageprocessen läggs mallbehörigheterna till eller skrivs över för projektet. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om användare A har behörigheten Visa i projektet, men har behörigheten Hantera i mallen, får användare A åtkomst till projektet när mallen har bifogats.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>



<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->


