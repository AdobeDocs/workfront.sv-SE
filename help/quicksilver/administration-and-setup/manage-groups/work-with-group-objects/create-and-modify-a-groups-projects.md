---
user-type: administrator
product-area: system-administration;user-management
keywords: grupp,projekt
navigation-topic: work-with-a-groups-objects
title: Skapa och ändra en grupps projekt
description: När du visar en grupp som du hanterar i området Grupper kan du skapa, redigera export, kopiera och ta bort gruppens projekt.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Skapa och ändra en grupps projekt

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med dess projekt på följande sätt:

* Skapa ett nytt projekt för gruppen
* Redigera, exportera, kopiera eller ta bort ett projekt

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
  <tr> 
   <td>Objektbehörigheter</td>
   <td> 
    <ul> 
     <li> <p>Projektet måste vara associerat med gruppen eller någon av dess undergrupper. </p> <p>Mer information om hur du tilldelar en grupp till ett projekt finns i <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Hantera information i projektöversiktsområdet</a>.</p> </li> 
     <li> <p>Du måste också ha behörighet att redigera projektet, antingen för att du skapade det eller för att det delades med dig.</p></li> 
    </ul>
    <p><b>Obs!</b> När du skapar ett projekt från en gruppsida tilldelas projektet till den gruppen. Detta skiljer sig från att skapa ett projekt i andra Workfront-områden, där systemet tilldelar projektet till hemgruppen för den användare som skapar det (projektägaren).</p> </td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa, arbeta med och skapa projekt för din grupp från området Grupper

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen som du vill skapa, visa eller arbeta med projekt för.
1. Klicka på **Projekt** ![Projekt på huvudmenyn](assets/projects-in-main-menu.png) i den vänstra panelen om du vill visa en lista över de projekt som är associerade med gruppen.

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Arbeta med ett projekt</p> </td> 
      <td> <p>Markera projektet och använd sedan verktygsfältsknapparna för att redigera <img src="assets/edit-icon.png">, dela <img src="assets/share-icon.png"> eller ta bort det <img src="assets/delete.png">.</p> <p>Mer information om de här aktiviteterna finns i <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">Hantera projekt: artikelindex</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Skapa ett nytt projekt för gruppen</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicka på <strong>Nytt projekt</strong> och välj sedan ett alternativ i listrutan för att ange hur du vill skapa det. </p> <p>Mer information finns i avsnittet <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">Olika sätt att skapa projekt</a> i artikeln <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Skapa ett projekt</a>.</p> </li> 
        <li value="2">Ange ett namn för projektet och konfigurera det, så som beskrivs i <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Redigera projekt</a>.</li> 
       </ol> <p> Projektinställningar som har angetts för gruppen påverkar alla projekt som du skapar i området Grupper. Mer information finns i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">Konfigurera projektinställningar för en grupp</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera listan med projekt</td> 
      <td>Klicka på ikonen Exportera <img src="assets/export.png"> i verktygsfältet ovanför listan.</td> 
     </tr> 
    </tbody> 
   </table>
