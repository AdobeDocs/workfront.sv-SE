---
title: Ange ett anpassat villkor som standard för projekt
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Om ett projekts villkorstyp är inställd på Status i stället för Manuell, visar Adobe Workfront automatiskt ett av tre inbyggda standardvillkor i projektet (På mål, Vid risk eller I problem) när det fortskrider, vilket förklaras i Översikt över Projektvillkor och Villkorstyp.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Ange ett anpassat villkor som standard för projekt

Om ett projekts villkorstyp är inställd på Status i stället för Manuell, visar Adobe Workfront automatiskt ett av tre inbyggda standardvillkor i projektet (På mål, Vid risk eller I problem) när det fortskrider, vilket förklaras i [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Villkor i projekthuvudet och detaljer](assets/condition-of-project-0825.png)

Du kan ange anpassade villkor som standardvillkor i stället för att använda dessa tre inbyggda standardvillkor. Du kan till exempel ändra standardvillkoret På mål så att det visas som Spärra/knip i alla projekt.

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
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ange ett anpassat villkor som standardvillkor för alla projekt:

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Villkor**.

1. Klicka på fliken **Projekt**.
1. Klicka på **Ange standardvillkor**.
1. Klicka på det anpassade villkor som du vill använda i stället i listrutan för standardvillkoret som du vill ändra.
1. Upprepa föregående steg för alla andra standardvillkor som du vill ändra.
1. Klicka på **Spara**.

Mer information om hur du anger ett anpassat villkor som standardvillkor för uppgifter och problem finns i [Ange ett anpassat villkor som standard för uppgifter och problem](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Mer information om hur du konfigurerar ett projekt så att användare kan uppdatera villkoret manuellt finns i [Uppdatera villkor för aktiviteter och problem](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
