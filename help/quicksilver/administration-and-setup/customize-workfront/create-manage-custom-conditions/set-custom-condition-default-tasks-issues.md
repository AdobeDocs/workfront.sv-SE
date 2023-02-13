---
title: Ange ett anpassat villkor som standard för uppgifter och ärenden
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: När en användare klickar på Arbeta med det eller lägger till en uppdateringskommentar till en ny uppgift som de har tilldelats (utan att manuellt ange ett villkor för uppgiften), visar Adobe Workfront standardvillkoret för uppgifter, som har konfigurerats i installationsprogrammet. Detsamma gäller för problem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Ange ett anpassat villkor som standard för uppgifter och ärenden

När en användare klickar på Arbeta med det eller lägger till en uppdateringskommentar till en ny uppgift som de har tilldelats (utan att manuellt ange ett villkor för uppgiften), visar Adobe Workfront standardvillkoret för uppgifter, som har konfigurerats i installationsprogrammet. Detsamma gäller för problem.

Workfront använder det inbyggda villkoret Going Smoothly som standardvillkor för uppgifter och, separat, för problem. Som Workfront-administratör kan du ändra standardvillkoret för båda dessa objekttyper till ett anpassat villkor som du har skapat.

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

## Ange ett anpassat villkor som standardvillkor för uppgifter eller för ärenden:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Projektinställningar** > **Villkor**.

1. Klicka på **Uppgifter** eller **Problem** -fliken.

1. Klicka **Ange standardvillkor**.
1. I listrutan klickar du på det anpassade villkor som du vill använda som standardvillkor för uppgifter (eller ärenden).
1. Klicka **Spara**.

>[!NOTE]
>
>* En användare som har tilldelats en uppgift eller ett problem, eller som har behörigheten Hantera, kan ändra dess villkor manuellt. Mer information finns i [Uppdatera villkor för aktiviteter och ärenden](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* De tre standardvillkoren för uppgifter och ärenden som ingår i Workfront är att fungera smidigt, vissa bekymmer och viktiga vägspärrar. Du kan inte dölja eller ta bort dessa villkor, men du kan ändra deras namn och färger. Du kan också skapa nya som du vill använda i stället, vilket beskrivs i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>


Mer information om hur du konfigurerar ett anpassat villkor som standardvillkor för projekt finns i [Ange ett anpassat villkor som standard för projekt](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Mer information om anpassade villkor finns i [Anpassade villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
