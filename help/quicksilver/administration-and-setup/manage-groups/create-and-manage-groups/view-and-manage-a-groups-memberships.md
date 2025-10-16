---
user-type: administrator
product-area: system-administration;user-management
keywords: lägg till,användare,grupp,lägg till,annan,tilldela,administratör,ta bort,användare,visa,roller,medlemmar,exportera,medlemskap,data
navigation-topic: create-and-manage-groups
title: Visa och hantera medlemskap i en grupp
description: Som Adobe Workfront-administratör kan du visa, lägga till, ta bort, exportera, aktivera och inaktivera medlemmar i alla grupper som du hanterar. Du kan också redigera deras profiler, lägga till uppdateringar i deras profiler och tilldela dem som ytterligare gruppadministratörer för gruppen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Visa och hantera medlemskap i en grupp

Som Adobe Workfront-administratör kan du visa, lägga till, ta bort, exportera, aktivera och inaktivera medlemmar i alla grupper som du hanterar. Du kan också redigera deras profiler, lägga till uppdateringar i deras profiler och tilldela dem som ytterligare gruppadministratörer för gruppen.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

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

## Visa och hantera medlemskap i en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** i den vänstra panelen.

   I den lista som visas kan Workfront-administratörer se alla grupper och undergrupper. Gruppadministratörer kan bara se de grupper och undergrupper som de administrerar.

1. Klicka på namnet på gruppen som du vill redigera.
1. Gör något av följande på sidan som visas när **Gruppmedlemmar** är markerat på den vänstra menyn:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lägg till en användare i gruppen</td> 
      <td> 
       <ol> 
        <li>Klicka på <strong>Lägg till medlemmar</strong> <img src="assets/add-icon-plus-in-circle.png">, börja skriva användarens namn och markera det när det visas.</li>
        <li> <p>Upprepa detta för alla andra användare som du vill lägga till.</p> <p>Du kan klicka på krysset till höger om ett namn om du inte vill lägga till användaren.</p> </li>
        <li>Klicka på <strong>Klar</strong> när du är klar.</li>
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort en användare från gruppen</td> 
      <td> 
       <ol> 
        <li>Markera ett eller flera användarnamn och klicka sedan på <strong>Ta bort medlem</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li> <p>Klicka på <strong>Ta bort</strong> i varningsmeddelandet som visas.</p> <p>Du kan hitta en användare som du vill ta bort från listan genom att klicka på <strong>Sök efter personer och grupper i listan</strong>, skriva deras namn i rutan och sedan klicka på namnet när det visas.</p> <p><b>OBS</b>:  
          <ul> 
           <li>Om den här gruppen är hemgruppen för en användare som du vill ta bort måste du först tilldela en annan hemgrupp i användarens profil. Mer information finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Översikt över hemgrupper</a> och <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</li> 
           <li>Om gruppen bara har en gruppadministratör och du behöver ta bort honom eller henne från gruppen, måste du tilldela en annan gruppadministratör till gruppen först.</li> 
           <li>En användare kan tillhöra både en undergrupp och den överordnade gruppen. När du tar bort någon från en undergrupp förblir de en del av den överordnade gruppen. När du tar bort dem från den överordnade gruppen förblir de på samma sätt en del av undergruppen. Om du inte vill att en användare ska ha den åtkomst som är tillåten för den överordnade gruppen, måste du ta bort användaren både från undergrupperna och den överordnade gruppen, om de listas på båda platserna individuellt.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redigera en användares profilinformation</td> 
      <td> 
       <ol> 
        <li>Markera ett eller flera användarnamn och klicka sedan på <strong>Redigera</strong> <img src="assets/edit-icon.png">.</li> 
        <li> <p>Ändra användarens profilinformation.</p> <p>Mer information om de ändringar du kan göra finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera data för användarmedlemskap</td> 
      <td> 
       <ol> 
        <li>Markera ett eller flera användarnamn och klicka sedan på <strong>Exportera</strong> <img src="assets/export.png">.</li> 
        <li> <p>Exportera data som en PDF-, Excel- eller tabbavgränsad fil.</p> <p>Mer information om att exportera data finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportera data</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa och redigera medlemmarnas grupproller</td> 
      <td> <p>I kolumnen <strong>Grupproll</strong> visas varje medlems roll. Som gruppadministratör kan du dubbelklicka på en medlems roll för att ändra den.</p> <p>För medlemmar i gruppen som inte är gruppadministratörer går det inte att redigera den här kolumnen.</p> <p>Gruppadministratörer visas alltid överst i listan.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skicka en kommentar till gruppmedlemmar</td> 
      <td> 
       <ol> 
        <li>Markera minst en gruppmedlem och klicka sedan på <strong>Skicka uppdatering till användare</strong> i verktygsfältet.</li> 
        <li><p>Skriv den kommentar du vill skicka till användarna och till uppdateringsområdet för deras användarprofiler.</p>
        <p>Mer information finns i <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Skicka direktmeddelanden till andra användare</a>.</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivera en användare i Workfront</td> 
      <td>Markera en eller flera inaktiva användare och klicka sedan på <strong>Aktivera användare</strong> för att aktivera dem i Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inaktivera en användare i Workfront</td> 
      <td>Markera en eller flera aktiva användare och klicka sedan på <strong>Inaktivera användare</strong><img src="assets/deactivate-user.png"> för att inaktivera dem i Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sortera efter kolumn</td> 
      <td>Klicka på rubriken för en kolumn för att sortera listan efter innehållet i den kolumnen.</td> 
     </tr> 
    </tbody> 
   </table>
