---
title: Visa och hantera information om en grupp
description: Du kan visa och redigera sidan Gruppinformation för en grupp eller undergrupp som du hanterar.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Visa och hantera information om en grupp

Du kan visa och redigera sidan Gruppinformation för en grupp eller undergrupp som du hanterar. Den här sidan innehåller:

* En beskrivning av gruppen
* Namn på företagsledare och gruppadministratörer
* Ett alternativ som gör att du kan göra gruppen och dess undergrupper offentliga eller privata

Mer information om andra sätt att hantera en grupp finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Mer information om hur du kan inaktivera eller återaktivera en grupp finns i [Inaktivera eller återaktivera en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och hantera information om en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på den grupp på den översta nivån som du vill redigera.
1. Om du vill inaktivera eller återaktivera gruppen
1. Klicka på **Gruppinformation** på den vänstra menyn och gör sedan något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td> <p>Du kan skriva upp till 512 tecken.</p> <p>Om fältet är tomt klickar du på <strong>Lägg till</strong> för att ange en beskrivning.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>(Aktiverat som standard) Aktiverar gruppen i din Workfront-instans.</p> <p>När vanliga användare söker efter en grupp för att bifoga den till ett objekt eller för att dela ett objekt i ett textfält som det som visas nedan, visas endast aktiva grupper i listan.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om du vill effektivisera detta för dina användare kan du inaktivera alternativet Är aktiv för grupper som inte används för närvarande.</p> <p>Du kan enkelt visa, filtrera och gruppera grupplistan baserat på aktiv eller inaktiv status i det här fältet. Mer information om hur du använder vyer, filter och grupperingar i listor finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Rapportera element: filter, vyer och grupperingar</a>.</p> <p>Mer information om inaktiva grupper finns i avsnittet <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Att tänka på för inaktiva grupper</a> i artikeln <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Ta bort eller inaktivera ett anpassat formulär</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupptillgänglighet</td> 
      <td> <p>(Endast tillgängligt om du visar Information för en grupp, inte en undergrupp.) Aktivera eller inaktivera alternativet <strong>Gör gruppen och undergrupperna privata</strong>.</p> <p>För en offentlig grupp kan alla användare (i eller utanför gruppen) som har behörighet att redigera användare lägga till gruppen i profilen för andra användare. De kan inte göra detta för en privat grupp.</p> <p>Du kan bara redigera det här alternativet på den översta överordnade gruppen i en grupphierarki som har mer än en nivå. Alla undergrupper i den överordnade gruppen ärver inställningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppintressenter</td> 
      <td> 
       <ul> 
        <li><strong>Gruppadministratörer</strong>: Lägg till eller ta bort användare med en planeringslicens som gruppadministratörer för gruppen. Börja skriva namnet på en användare och klicka sedan på namnet när det visas i listrutan.</li> 
        <li><strong>Affärsledare</strong>: Gör något av följande:
         <ul>
          <li>Om du ännu inte har tilldelat någon affärsledare för gruppen klickar du på <strong>Lägg till</strong>, börjar skriva namnet på användaren som du vill tilldela och klickar sedan på personens namn när det visas.</li>
          <li>Om gruppen redan har en affärsledare och du vill ändra den dubbelklickar du på namnet på den befintliga affärsledaren. Ta bort namnet, börja skriva namnet på den användare som du vill tilldela och klicka sedan på personens namn när det visas.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lägg till anpassat formulär</td> 
      <td>Om din åtkomstnivå tillåter dig att hantera anpassade formulär lägger du till ett anpassat formulär i gruppen. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Anpassade formulär</a>.</td> 
     </tr> 
    </tbody> 
   </table>
