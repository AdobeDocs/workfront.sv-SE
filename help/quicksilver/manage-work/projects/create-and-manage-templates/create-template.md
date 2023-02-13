---
product-area: templates
navigation-topic: templates-navigation-topic
title: Skapa en projektmall
description: Du kan skapa och ta bort mallar i området Mallar. När du skapar en ny mall kan du ange informationen för alla uppgifter och all information för dina framtida projektinställningar. Den här informationen överförs sedan till projektet när du skapar det från mallen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Skapa en projektmall

Du kan skapa och ta bort mallar i området Mallar. När du skapar en ny mall kan du ange informationen för alla uppgifter och all information för dina framtida projektinställningar. Den här informationen överförs sedan till projektet när du skapar det från mallen.

Du kan skapa en ny mall på följande sätt:

* Från början, enligt beskrivningen i den här artikeln.
* Från befintliga projekt genom att spara ett projekt som en mall.

   Mer information om hur du skapar mallar från befintliga projekt finns i [Spara ett projekt som en mall](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Genom att kopiera den från en annan mall.

   Mer information om hur du kopierar en befintlig mall finns i [Kopiera en projektmall](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Om du är Workfront-administratör kan du skapa mallar genom att importera utkast. Mer information finns i [Konfigurera en plan](../../../administration-and-setup/blueprints/configure-template-package.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Systemadministratör för import av mallar från utkast</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Som standard har du behörigheten Hantera för de mallar du skapar</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en mall

1. Från **Huvudmeny** ![](assets/main-menu-icon.png) klicka **Mallar**.

1. Klicka **Ny mall**.

   Mallen är namnlös.

   ![Ny mall](assets/create-template-nwe-2022-350x102.png)

1. Ange ett namn för den nya mallen i mallhuvudet och tryck sedan på **Retur.**
1. Klicka på **Malluppgifter** i den vänstra panelen.
1. Klicka **Börja lägga till malluppgifter**.

   eller

   Klicka **Ny mallaktivitet** för att börja lägga till uppgifter i mallen.

   Att lägga till malluppgifter i en mall är detsamma som att lägga till uppgifter i ett projekt.

   Mer information om hur du lägger till uppgifter i ett projekt finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Du kan inte lägga till återkommande uppgifter i en mall.

1. (Valfritt) Klicka på **Gantt-schema** i det övre högra hörnet av uppgiftslistan för att visa en visuell representation av mallens uppgiftslista.

   >[!TIP]
   >
   >Du kan inte redigera aktiviteter direkt från det här Gantt-diagrammet.

1. Om du vill lägga till information i den nya mallen klickar du på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Redigera**.

   Mer information om hur du redigerar en mall finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Klicka **Spara ändringar**.
1. (Valfritt) Om du vill lägga till fler objekt i mallen kan du läsa avsnittet [Lägga till ytterligare objekt i en mall](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) i artikeln [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Mallinställningar som bestäms av gruppassociationen

Om en projektmall är associerad med en grupp (eller om den saknas) påverkar det hur inställningar för projekt, uppgift och problem bestämmer vissa inställningar i mallen. Mer information finns i avsnittet [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
