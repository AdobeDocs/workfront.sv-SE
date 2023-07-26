---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Lägga till en avsnittsbrytning i ett anpassat formulär med det äldre formulärverktyget
description: Du kan gruppera anpassade fält och widgetar i ett anpassat formulär i avsnitt med rubriker. Detta är användbart för att ge en välordnad upplevelse till användare som fyller i formuläret. Om du dessutom behöver begränsa åtkomsten till vissa anpassade fält och widgetar för vissa användare, kan du placera dem i ett avsnitt och sedan ge åtkomst till avsnittet till endast dessa användare.
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# Lägga till en avsnittsbrytning i ett anpassat formulär med det äldre formulärverktyget

Du kan gruppera anpassade fält och widgetar i ett anpassat formulär i avsnitt med rubriker. Detta är användbart för att ge en välordnad upplevelse till användare som fyller i formuläret. Om du dessutom behöver begränsa åtkomsten till vissa anpassade fält och widgetar för vissa användare, kan du placera dem i ett avsnitt och sedan ge åtkomst till avsnittet till endast dessa användare.

Om du till exempel behöver spåra känslig information som bara systemadministratörer ska kunna visa eller redigera, kan du skapa en avsnittsbrytning med enbart administratör och placera de känsliga fälten i det avsnittet.

De åtkomstinställningar som du väljer för ett avsnitt är direkt knutna till de behörigheter som användare har på det Workfront-objekt där det anpassade formuläret bifogas. Du kan dölja eller visa ett avsnitt baserat på om användaren har åtkomst till att visa, bidra till eller hantera objektet. Du kan också ange ett avsnitt som Endast administratör så att bara användare med en systemadministratörsåtkomstnivå kan komma åt det.

Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Skapa och konfigurera åtkomst för ett avsnitt i ett anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Lägga till anpassade fält och widgetar i formuläret, enligt beskrivningen i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. När du fortfarande skapar eller redigerar det anpassade formuläret, på **Lägg till ett fält** flik, klicka **Avsnittsbrytning**.

   ![](assets/click-section-break.jpg)

1. På **Fältinställningar** konfigurerar du önskade alternativ för avsnittet:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför avsnittet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv text om du vill förklara för användarna vad avsnittet är till för. Detta visas under avsnittets etikett i det anpassade formuläret.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lägg till logik</td> 
      <td>Använd visningslogik för att ange om avsnittet ska visas i formuläret, baserat på de val som användare gör i anpassade fält med flera val när de fyller i formuläret. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Lägga till visningslogik och hoppa över logik i ett anpassat formulär</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ge åtkomst</p> </td> 
      <td> <p> Markera de behörigheter som användare behöver för ett objekt där det anpassade formuläret är kopplat för att visa det här avsnittet och redigera fältvärdena. 
       <p>Följande behörigheter är tillgängliga under <b>Användare med denna åtkomst till objektet kan visa fältvärden</b>:</p> 
         <ul>  
          <li><p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en uppgift, ett problem eller en användare):</p> 
          <p>Tillåter användare att bidra till objektet om det är ett projekt, en uppgift eller ett problem.</p>
          <p>Tillåter användare att redigera profilen eller äger profilbehörigheten till objektet om det är en användare.</p></li> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
        <p>Följande behörigheter är tillgängliga under <b>Användare med den här åtkomsten till objektet kan redigera fältvärden</b>: </p> 
         <ul> 
          <li> <p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en uppgift, ett problem eller en användare):</p> 
           <p>Om objektet är ett projekt, en uppgift eller ett problem, ger den här behörigheten användarna möjlighet att bidra till objektet</p>
          <p>Om objektet är en användare, ger den här behörigheten användare behörighet att redigera profilen eller äga profilbehörigheten till objektet.</p> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
       </ul> 
       <p>Mer information om objektbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> 
       <p><b>ANMÄRKNING</b>:  
       <ul> 
       <li> <p>Användare som saknar de behörigheter som du anger här kan inte se anpassade fält och widgetar i avsnittet. </p> <p>Detta gäller även om du visar fältets värden i rapporter eller använder dem i beräknade fält i textlägesrapporter.</p> </li> 
       <li> <p>Om du kopplar flera objekttyper till formuläret kan du ändra de visnings- och redigeringsbehörigheter som är tillgängliga i de här stegen. Mer information finns i <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter i ett anpassat formulär</a> i den här artikeln.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dra eller lägg till minst ett anpassat fält eller en widget till det nya avsnittet.

   Detta krävs innan du sparar avsnittet.

1. Klicka **Klar**.

   >[!TIP]
   >
   >Klicka **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

1. Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fylla i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Behörigheten för begränsad redigering för anpassade formuläravsnittsbrytningar är bara tillgänglig för objekttyperna Projekt, Aktivitet, Utgåva och Användare.

Om du lägger till en annan objekttyp i formuläret (Portfolio, Program, Dokument, Företag, Faktureringspost, Iteration, Expense eller Grupp) i ett anpassat formulär med en avsnittsbrytning som är konfigurerad med behörigheten Begränsad redigering, uppmanas du att växla till behörigheten Redigera, som är kompatibel med både den objekttypen och de befintliga objekttyperna i formuläret.

>[!INFO]
>
>**Exempel:** I ett anpassat formulär som är associerat med projektobjekttypen konfigureras en avsnittsbrytning med behörigheten Begränsad redigering.
>
>Du lägger till objekttypen Portfolio i formuläret, vilket innebär att behörighetsalternativet Begränsad redigering inte längre är tillgängligt för avsnittsbrytningen i formuläret.
>
>Ett meddelande på skärmen uppmanar dig att växla till behörigheten Redigera, som är det mest lika alternativet för Begränsad redigering, och som är kompatibelt med både objekttypen och objekttypen Portfolio.
