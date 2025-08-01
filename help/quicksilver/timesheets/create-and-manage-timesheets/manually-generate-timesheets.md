---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generera tidrapporter manuellt
description: Om du vill aktivera ändringar som du har gjort i tidrapportprofilerna så att de återspeglar de aktuella tidrapporterna, måste du först ta bort de befintliga tidrapporterna och sedan generera nya manuellt. Du kan generera tidrapporter manuellt från tidrapporterna eller diagnostikområdet i installationsprogrammet, vilket förklaras i den här artikeln.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: c9df676467007a84920073fe06bc3c73b18a89ae
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Generera tidrapporter manuellt

Om du vill aktivera ändringar som du har gjort i tidrapportprofilerna så att de återspeglar de aktuella tidrapporterna, måste du först ta bort de befintliga tidrapporterna och sedan generera nya manuellt. Du kan generera tidrapporter manuellt från tidrapporterna eller diagnostikområdet i installationsprogrammet, vilket förklaras i den här artikeln.

Instruktioner om hur du tar bort tidrapporter finns i [Ta bort tidrapporter i Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront-administratör eller, om du arbetar med tidrapportprofiler för en grupp, du måste vara gruppadministratör (eller Workfront-administratör). Mer information finns i <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a>.</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överväganden om manuellt genererade tidrapporter

När du genererar tidrapporter manuellt:

* De genereras enligt de tidrapportprofiler som är kopplade till dina användare. Användare som inte har associerade tidrapportprofiler får inga tidrapporter.
* Endast den aktuella tidrapporten och den som följer genereras. Workfront genererar inte två tidrapporter för samma period. Om du redan har en tidrapport för den aktuella tidsramen, kommer en annan inte att genereras när du använder den manuella processen för att generera tidrapporter.

## Generera tidrapporter manuellt från tidrapporter och timmar

Du kan generera tidrapporter på systemnivå eller gruppnivå manuellt från området Tidrapporter och timmar i installationsprogrammet.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Om du genererar tidrapporter som används i hela systemet klickar du på **Tidrapporter och timmar.**

   eller

   Om du genererar tidrapporter som används av en viss grupp klickar du på **Grupper** och sedan på gruppens namn.

1. Klicka på **Tidrapportprofiler**.
1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png) för tidrapportprofiler på systemnivå eller **Mer** för grupptidrapportprofiler överst i listan över tidrapportprofiler och klicka sedan på **Generera tidrapporter**.

   Nya tidrapporter skapas för upp till två tidsperioder för användare som är kopplade till tidrapportprofiler.

## Generera tidrapporter på systemnivå manuellt från diagnostikområdet

Du kan generera tidrapporter på systemnivå manuellt från området Diagnostik i installationsprogrammet.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Expandera **System** och klicka sedan på **Diagnostik**.

1. Klicka på **Kör diagnostik**.
1. Klicka på **Generera tidrapporter**.
