---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Skapa en undergrupp
description: Du kan skapa en undergrupp under en grupp som du hanterar för att ordna användare och projekt och för att tilldela behörigheter i Adobe Workfront. Vanligtvis hanterar gruppadministratörer grupper och undergrupper. De kan använda gruppsidan för att hantera sina grupper och undergrupper på ett och samma ställe.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Skapa en undergrupp

Du kan skapa en undergrupp under en grupp som du hanterar för att ordna användare och projekt och för att tilldela behörigheter i Adobe Workfront.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Vanligtvis hanterar gruppadministratörer grupper och undergrupper. De kan använda gruppsidan för att hantera sina grupper och undergrupper på ett och samma ställe. Mer information om hur grupper och undergrupper fungerar i Workfront finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md) och [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Åtkomstkrav

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

## Lägg till en undergrupp

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Markera den befintliga gruppen eller undergruppen där du vill lägga till en ny undergrupp.
1. Klicka på **Ny undergrupp**.
1. I rutan **Ny undergrupp** som visas skriver du **Gruppnamn** för undergruppen.
1. (Valfritt) Ange någon av följande uppgifter:

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
      <td>Ange en beskrivning för undergruppen. Du kan skriva upp till 512 tecken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Är aktiv</td> 
      <td> <p>(Aktiverat som standard) Aktiverar gruppen i din Workfront-instans.</p> <p>När vanliga användare söker efter en grupp för att bifoga den till ett objekt eller för att dela ett objekt i ett textfält som det som visas nedan, visas endast aktiva grupper i listan.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Om du vill effektivisera detta för dina användare kan du inaktivera alternativet Är aktiv för grupper som inte används för närvarande.</p> <p>Du kan enkelt visa, filtrera och gruppera grupplistan baserat på aktiv eller inaktiv status i det här fältet. Mer information om hur du använder vyer, filter och grupperingar i listor finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Rapportera element: filter, vyer och grupperingar</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gör den här gruppen och dess undergrupper offentliga</td> 
      <td> <p>(Endast tillgängligt om du visar Detaljer för en grupp på den översta nivån, inte för en undergrupp.) Aktivera det här alternativet om du vill tillåta användare i undergruppen med redigeringsanvändaråtkomst (som inte är administratörer för gruppen) att lägga till den här gruppen och dess undergrupper i andra användares användarprofil.</p> <p>För en offentlig grupp kan alla användare (i eller utanför gruppen) som har behörighet att redigera användare lägga till gruppen i profilen för andra användare. De kan inte göra detta för en privat grupp.</p> <p>Du kan bara redigera det här alternativet på den översta överordnade gruppen i en grupphierarki som har mer än en nivå. Alla undergrupper i den överordnade gruppen ärver inställningen.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Du kan inte göra en undergrupp offentlig för sig själv, men du kan göra den till en överordnad grupp på översta nivån offentlig, vilket även gör alla överordnade undergrupper offentliga.</li> 
         <li>En undergrupp som tillhör en offentlig grupp är som standard offentlig, så alla användare med redigeringsåtkomst kan lägga till undergruppen även till andra användare.</li> 
        </ul> </p> <p>Om du behöver information om den åtkomst som krävs för att redigera användare läser du <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Bevilja åtkomst till användare</a>. Mer information om hur du redigerar användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Redigera en användares profil</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företagsledare </td> 
      <td> <p>Du kan utse en användare till affärsledare för en undergrupp som du hanterar. En företagsledare är någon som fattar affärsbeslut för undergruppen. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över företagsledare</a><span>.</span></p> <p>Om personen inte redan är medlem i undergruppen läggs även personens namn till i gruppen om du lägger till personen i det här fältet.</p> <p><b>OBS</b>:  
        <ul> 
         <li>Innan du kan ta bort affärsledaren från en undergrupp måste du ta bort deras namn från fältet Affärsledare.</li> 
         <li>Om du tar bort namnet från fältet Affärsledare förblir användaren medlem i undergruppen såvida du inte tar bort dem från den. Instruktioner om hur du tar bort någon från en grupp finns i avsnittet <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Hantera en grupps medlemskap</a> i artikeln <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Hantera en grupp</a>.</li> 
        </ul> </p> <p>Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över företagsledare</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppmedlemmar och gruppadministratörer</td> 
      <td> 
       <ul> 
        <li> <p>Gruppmedlemmar: Om du vill lägga till användare och grupper i undergruppen börjar du skriva namnet på en befintlig användare eller grupp som du vill lägga till och markerar sedan namnet när det visas.</p> <p>De användare och grupper som du lägger till har åtkomst till alla objekt som delas med gruppen.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Gruppadministratörer: En undergrupp ärver gruppadministratörerna för gruppen ovan, vilket innebär att det är valfritt att ange en användare som gruppadministratör för en undergrupp. Du kan tilldela en gruppmedlem som administratör för gruppen med den nedrullningsbara menyn till höger om användarens namn.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Söka efter personer och grupper i listan</td> 
      <td> Om du behöver hitta en användare eller grupp som redan är tilldelad den här undergruppen kan du skriva namnet här och markera den när den visas.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara.**
