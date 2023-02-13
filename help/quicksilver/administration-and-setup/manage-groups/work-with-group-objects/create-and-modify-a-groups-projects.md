---
user-type: administrator
product-area: system-administration;user-management
keywords: grupp,projekt
navigation-topic: work-with-a-groups-objects
title: Skapa och ändra en grupps projekt
description: När du visar en grupp som du hanterar i området Grupper kan du skapa, redigera export, kopiera och ta bort gruppens projekt.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Skapa och ändra en grupps projekt

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med dess projekt på följande sätt:

* Skapa ett nytt projekt för gruppen
* Redigera, exportera, kopiera eller ta bort ett projekt

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td >Workfront</a>*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</a>*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <ul> 
     <li> <p>Projektet måste vara associerat med gruppen eller någon av dess undergrupper. </p> <p>Mer information om hur du tilldelar en grupp till ett projekt finns i <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Hantera information i projektöversiktsområdet</a>.</p> </li> 
     <li> <p>Du måste också ha behörighet att redigera projektet, antingen för att du skapade det eller för att det delades med dig.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </li> 
    </ul> <p><b>ANMÄRKNING</b>: När du skapar ett projekt från en gruppsida tilldelas projektet till den gruppen. Detta skiljer sig från att skapa ett projekt i andra Workfront-områden, där systemet tilldelar projektet till hemgruppen för den användare som skapar det (projektägaren).</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Visa, arbeta med och skapa projekt för din grupp från området Grupper

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på namnet på gruppen som du vill skapa, visa eller arbeta med projekt för.
1. Klicka på i den vänstra panelen **Projekt** ![](assets/projects-in-main-menu.png) om du vill visa en lista över projekt som är associerade med gruppen.

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Arbeta med ett projekt</p> </td> 
      <td> <p>Markera projektet och använd sedan verktygsfältsknapparna för att redigera <img src="assets/edit-icon.png">, dela <img src="assets/share-icon.png">eller ta bort <img src="assets/delete.png">.</p> <p>Mer information om dessa aktiviteter finns i <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">Hantera projekt</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Skapa ett nytt projekt för gruppen</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>Klicka <strong>Nytt projekt</strong>väljer du sedan ett alternativ i listrutan för att ange hur du vill skapa det. </p> <p>Mer information finns i avsnittet <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">Olika sätt att skapa projekt</a> i artikeln <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Skapa ett projekt</a>.</p> </li> 
        <li value="2">Ange ett namn för projektet och konfigurera det enligt anvisningarna i <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Redigera projekt</a>.</li> 
       </ol> <p> Projektinställningar som har angetts för gruppen påverkar alla projekt som du skapar i området Grupper. Mer information finns i <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">Konfigurera projektinställningar för en grupp</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera listan med projekt</td> 
      <td>Klicka på ikonen Exportera <img src="assets/export.png"> i verktygsfältet ovanför listan.</td> 
     </tr> 
    </tbody> 
   </table>
