---
title: Ange ett anpassat villkor som standard för projekt
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Om ett projekts villkorstyp är inställd på Status i stället för Manuell, visar Adobe Workfront automatiskt ett av tre inbyggda standardvillkor i projektet (På mål, Vid risk eller I problem) när det fortskrider, vilket förklaras i Översikt över Projektvillkor och Villkorstyp.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Ange ett anpassat villkor som standard för projekt

Om ett projekts villkorstyp är inställd på Status i stället för Manuell, visar Adobe Workfront automatiskt ett av tre inbyggda standardvillkor i projektet (Vid mål, Vid risk eller I problem) allt eftersom det fortskrider, vilket förklaras i [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Du kan ange anpassade villkor som standardvillkor i stället för att använda dessa tre inbyggda standardvillkor. Du kan till exempel ändra standardvillkoret På mål så att det visas som Spärra/knip i alla projekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ange ett anpassat villkor som standardvillkor för alla projekt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Projektinställningar** > **Villkor**.

1. Klicka på **Projekt** -fliken.
1. Klicka **Ange standardvillkor**.
1. I listrutan bredvid det standardvillkor som du vill ändra klickar du i stället på det anpassade villkor som du vill använda.
1. Upprepa föregående steg för alla andra standardvillkor som du vill ändra.
1. Klicka **Spara**.

Mer information om hur du anger ett anpassat villkor som standardvillkor för uppgifter och problem finns i [Ange ett anpassat villkor som standard för uppgifter och ärenden](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Mer information om hur du konfigurerar ett projekt så att användare kan uppdatera villkoret manuellt finns i [Uppdatera villkor för aktiviteter och ärenden](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Mer information om anpassade villkor finns i [Anpassade villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
