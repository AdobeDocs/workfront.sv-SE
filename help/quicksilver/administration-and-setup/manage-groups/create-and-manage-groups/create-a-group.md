---
user-type: administrator
product-area: system-administration;user-management
keywords: skapa,grupp,undergrupp,ny
navigation-topic: create-and-manage-groups
title: Skapa en grupp
description: Som Adobe Workfront-administratör kan du skapa grupper för att ordna användare och projekt och för att tilldela behörigheter i Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 0%

---

# Skapa en grupp

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Som Adobe Workfront-administratör kan du skapa grupper för att ordna användare och projekt och för att tilldela behörigheter i Workfront. Mer information finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Varje undergrupp behöver minst en gruppadministratör. Gruppadministratörer kan använda gruppsidan för att hantera sina grupper på ett och samma ställe.

Om du är gruppadministratör eller Workfront-administratör kan du även skapa undergrupper under en grupp. Instruktioner finns i [Skapa en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Skapa en grupp på den översta nivån från grunden

I de här stegen beskrivs hur du skapar en ny grupp från grunden. Mer information om hur du skapar en grupp eller undergrupp genom att kopiera en befintlig finns i [Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) i den här artikeln.

Du måste vara Workfront-administratör för att kunna skapa en högnivågrupp.

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Ovanför listan med grupper klickar du på **Ny grupp**.

   >[!TIP]
   >
   >Längst ned i listan med grupper kan du även klicka på **Lägg till fler grupper** för att lägga till en grupp på raden och sedan klicka på **Retur** när du är klar med att lägga till gruppinformationen.

1. Ange ett namn för gruppen i rutan **Ny grupp** som visas.
1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gruppnamn</td> 
      <td>Ändra namnet på gruppen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för gruppen. Du kan skriva upp till 512 tecken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>(Aktiverat som standard) Aktiverar gruppen i din Workfront-instans.</p> <p>När vanliga användare söker efter en grupp för att bifoga den till ett objekt eller för att dela ett objekt i ett textfält som det som visas nedan, visas endast aktiva grupper i listan.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om du vill effektivisera detta för dina användare kan du inaktivera alternativet Är aktiv för grupper som inte används för närvarande.</p> <p>Du kan enkelt visa, filtrera och gruppera grupplistan baserat på aktiv eller inaktiv status i det här fältet. Mer information om hur du använder vyer, filter och grupperingar i listor finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Rapportera element: filter, vyer och grupperingar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gör den här gruppen och dess undergrupper offentliga</td> 
      <td> <p>(Endast tillgängligt om du visar Detaljer för en grupp på den översta nivån, inte för en undergrupp.) Aktivera det här alternativet om du vill tillåta användare i gruppen med redigeringsanvändaråtkomst (som inte är administratörer för gruppen) att lägga till den här gruppen och dess undergrupper i andra användares användarprofil.</p> <p>För en offentlig grupp kan alla användare (i eller utanför gruppen) som har behörighet att redigera användare lägga till gruppen i profilen för andra användare. De kan inte göra detta för en privat grupp.</p> <p>Du kan bara redigera det här alternativet på den översta överordnade gruppen i en grupphierarki som har mer än en nivå. Alla undergrupper i den överordnade gruppen ärver inställningen.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Du kan inte göra en undergrupp offentlig för sig själv, men du kan göra den överordnade gruppen på den översta nivån offentlig, vilket även gör alla överordnade undergrupper offentliga.</li> 
         <li>En undergrupp som tillhör en offentlig grupp är som standard offentlig, så alla användare med redigeringsåtkomst kan lägga till undergruppen även till andra användare.</li> 
        </ul> </p> <p>Om du behöver information om den åtkomst som krävs för att redigera användare läser du <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>. Mer information om hur du redigerar användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företagsledare </td> 
      <td> <p>Du kan utse en användare till affärsledare för en grupp som du hanterar. En företagsledare är någon som fattar affärsbeslut för gruppen. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Översikt över företagsledare</a><span>.</span></p> <p>Om personen inte redan är medlem i gruppen läggs även namnet till i gruppen när namnet läggs till i det här fältet.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Innan du kan ta bort affärsledaren från en grupp måste du ta bort deras namn från fältet Affärsledare.</li> 
         <li>Om du tar bort namnet från fältet Affärsledare förblir användaren medlem i gruppen om du inte tar bort dem från den. Instruktioner om hur du tar bort någon från en grupp finns i avsnittet <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Hantera en grupps medlemskap</a> i artikeln <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Hantera en grupp</a>.</li> 
        </ul> </p> <p>Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Översikt över företagsledare</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppmedlemmar och gruppadministratörer</td> 
      <td>
        <p>Om du vill lägga till gruppmedlemmar börjar du skriva namnet på en befintlig användare eller grupp som du vill lägga till och markerar sedan namnet när det visas.</p> 
        <p>Användare och grupper som du lägger till har åtkomst till alla objekt som delas med gruppen.</p>
        <p>En grupp på den översta nivån måste ha minst en gruppadministratör. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Söka efter personer och grupper i listan</td> 
      <td> Om du behöver hitta en användare eller grupp som redan är tilldelad den här gruppen kan du skriva namnet här och markera den när den visas.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skapa grupp**.

## Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Som Workfront-administratör kan du skapa en ny toppnivågrupp genom att kopiera en befintlig grupp eller undergrupp.

Tänk på följande när du vill göra detta:

* Alla medlemmar och undergrupper som tillhör den befintliga gruppen kopieras till den nya översta gruppen.
* Medlemmarna i den kopierade gruppen behåller de tilldelningar de hade i den ursprungliga gruppen. Gruppadministratörerna för den ursprungliga gruppen anges därför också som gruppadministratörer i den kopierade gruppen.

Så här skapar du en ny grupp på den översta nivån genom att kopiera en grupp eller undergrupp:

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Markera gruppen som du vill kopiera och klicka sedan på ikonen Kopiera ![](assets/copy-icon.png).
1. Skriv ett **gruppnamn** för den kopierade gruppen i rutan **Kopiera grupp**.

1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gruppnamn</td> 
      <td>Ändra namnet på gruppen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för gruppen. Du kan skriva upp till 512 tecken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>(Aktiverat som standard) Aktiverar gruppen i din Workfront-instans.</p> <p>När vanliga användare söker efter en grupp för att bifoga den till ett objekt eller för att dela ett objekt i ett textfält som det som visas nedan, visas endast aktiva grupper i listan.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om du vill effektivisera detta för dina användare kan du inaktivera alternativet Är aktiv för grupper som inte används för närvarande.</p> <p>Du kan enkelt visa, filtrera och gruppera grupplistan baserat på aktiv eller inaktiv status i det här fältet. Mer information om hur du använder vyer, filter och grupperingar i listor finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Rapportera element: filter, vyer och grupperingar</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gör den här gruppen och dess undergrupper offentliga</td> 
      <td> <p>(Endast tillgängligt om du visar Detaljer för en grupp på den översta nivån, inte för en undergrupp.) Aktivera det här alternativet om du vill tillåta användare i gruppen med redigeringsanvändaråtkomst (som inte är administratörer för gruppen) att lägga till den här gruppen och dess undergrupper i andra användares användarprofil.</p> <p>För en offentlig grupp kan alla användare (i eller utanför gruppen) som har behörighet att redigera användare lägga till gruppen i profilen för andra användare. De kan inte göra detta för en privat grupp.</p> <p>Du kan bara redigera det här alternativet på den översta överordnade gruppen i en grupphierarki som har mer än en nivå. Alla undergrupper i den överordnade gruppen ärver inställningen.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Du kan inte göra en undergrupp offentlig för sig själv, men du kan göra den till en överordnad grupp på översta nivån offentlig, vilket även gör alla överordnade undergrupper offentliga.</li> 
         <li>En undergrupp som tillhör en offentlig grupp är som standard offentlig, så alla användare med redigeringsåtkomst kan lägga till undergruppen även till andra användare.</li> 
        </ul> </p> <p>Om du behöver information om den åtkomst som krävs för att redigera användare läser du <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Bevilja åtkomst till användare</a>. Mer information om hur du redigerar användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Redigera en användares profil</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företagsledare </td> 
      <td> <p>Du kan utse en användare till affärsledare för en grupp som du hanterar. En företagsledare är någon som fattar affärsbeslut för gruppen. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över företagsledare</a><span>.</span></p> <p>Om personen inte redan är medlem i gruppen läggs även namnet till i gruppen när namnet läggs till i det här fältet.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Innan du kan ta bort affärsledaren från en grupp måste du ta bort deras namn från fältet Affärsledare.</li> 
         <li>Om du tar bort namnet från fältet Affärsledare förblir användaren medlem i gruppen om du inte tar bort dem från den. Instruktioner om hur du tar bort någon från en grupp finns i avsnittet <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Hantera en grupps medlemskap</a> i artikeln <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Hantera en grupp</a>.</li> 
        </ul> </p> <p>Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över företagsledare</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppmedlemmar och gruppadministratörer</td> 
      <td> 
       <ul> 
        <li> <p>Gruppmedlemmar: Om du vill lägga till användare och grupper i gruppen börjar du skriva namnet på en befintlig användare eller grupp som du vill lägga till och markerar sedan namnet när det visas.</p> <p>De användare och grupper som du lägger till har åtkomst till alla objekt som delas med gruppen.</p> </li> 
        <li> <p>Gruppadministratörer: Alla gruppadministratörer i den ursprungliga gruppen anges också som gruppadministratörer i den kopierade gruppen. Du kan tilldela en gruppmedlem som administratör för gruppen med den nedrullningsbara menyn till höger om användarens namn.</p> <p>En grupp på den översta nivån måste ha minst en gruppadministratör.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Söka efter personer och grupper i listan</td> 
      <td> Om du behöver hitta en användare eller grupp som redan är tilldelad den här gruppen kan du skriva namnet här och markera den när den visas.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Om den ursprungliga gruppen har undergrupper läggs undergrupperna till i den nya gruppen och deras namn är som standard&quot;Det ursprungliga undergruppsnamnet (Kopiera)&quot;.
   >* Du kan ta bort användare och undergrupper från den ursprungliga gruppen genom att klicka på X till höger om användarens eller undergruppens namn.

1. Klicka på **Skapa grupp**.
