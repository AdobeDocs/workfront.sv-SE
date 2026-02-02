---
product-area: projects
navigation-topic: manage-tasks
title: Associera milstolpar med uppgifter
description: Du kan associera milstolpar med uppgifter för att ange när du når viktiga steg i projektets livstid. Du måste associera en milstolpe-bana med ett projekt innan du kan associera milstolpar med uppgifter i projektet.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Koppla milstolpar till uppgifter

<!--Audited: 01/2024-->

Du kan associera milstolpar med uppgifter för att ange när du når viktiga steg i projektets livstid.

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
   <p>Arbeta eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgiften</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Innan du kan associera en milstolpe med en uppgift måste följande finnas:

* Workfront-administratören måste skapa en milstolpe-sökväg enligt beskrivningen i [Skapa en milstolpe-sökväg](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Du måste associera en milstolpe-sökväg till ett projekt.

  Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Om du vill associera en milstolpe-sökväg med ett projekt måste projektet ha statusen Planering eller Aktuell.

  >[!TIP]
  >
  >För att få bästa möjliga överblick över hur milstolparna i dina projekt utvecklas i vyn Milstolpe bör du skapa överordnade uppgifter och associera dem med varje större fas i projektet. Koppla sedan dessa överordnade uppgifter till var och en av milstolparna i milstolpen.

## Koppla en milstolpe till en uppgift

När en milstolpe-sökväg har associerats med ett projekt kan uppgifter tilldelas en milstolpe.

1. Gå till en aktivitet och klicka sedan på ikonen **Mer** ![Mer](assets/more-icon.png) till höger om aktivitetsnamnet och sedan på **Redigera** .

   Aktiviteter och milstolpar har en :1-relation. Du kan inte koppla samma milstolpe till flera uppgifter. Varje aktivitet kan länkas till en enskild milstolpe, eller varje milstolpe kan mappas till en aktivitet.

1. Klicka på **Inställningar** och välj sedan en milstolpe i fältet **Milstolpe** för aktiviteten.
1. Klicka på **Spara**.
1. (Valfritt) Lägg till kolumnen **Statusikoner** i en lista över uppgifter för att identifiera vilka aktiviteter som har milstolpar. Diamantindikatorn för milstolpe visas i kolumnen Statusikoner.

   Mer information finns i [Skapa eller redigera vyer i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![Statusikoner](assets/amwt3.png)

1. (Valfritt) Gå till en lista med projekt och markera vyn **Milstolpe** för att identifiera förloppet för dina milstolpeuppgifter.

   ![Vyprojektlista för milstolpe](assets/milestone-view-project-list.png)
