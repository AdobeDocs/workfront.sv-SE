---
product-area: projects
navigation-topic: create-tasks
title: Skapa uppgifter i ett projekt
description: Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 0aed653b9e5f0123e6b4d6e494aaff563ae1a72d
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Skapa uppgifter i ett projekt

<!-- Audited: 1/2024 -->

Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.

När du har skapat ett projekt kanske du vill lägga till uppgifter och ändra dem för att ordna projektplanen. Mer information om hur du skapar ett projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

Mer information om hur du skapar personliga uppgifter som inte finns i ett projekt finns i [Skapa en personlig uppgift](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task) i artikeln [Skapa arbetsobjekt från startdelen](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

I den här artikeln beskrivs hur du skapar åtgärder från grunden. Du kan också skapa uppgifter på följande sätt:

* Genom att kopiera eller duplicera befintliga uppgifter. Mer information finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Genom att flytta uppgifter från ett projekt till ett annat. Mer information finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Åtkomstkrav

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-licens*</p> </td> 
   <td><p>Aktuell: Arbete eller högre</p> 
   eller
   <p>Nytt: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till uppgifter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Bevilja åtkomst till uppgifter</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter till projektet med möjlighet att lägga till uppgifter eller högre</p> <p>När du skapar en uppgift får du automatiskt behörigheten Hantera för uppgiften</p> <p> Mer information om aktivitetsbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Dela en uppgift </a>. </p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa uppgifter i ett projekt

1. Gå till det projekt där du vill skapa en uppgift.
1. Klicka **Uppgifter** till vänster.
1. (Villkorligt) Om du visar uppgiftslistan i en flexibel vy klickar du på **Listvy** icon ![](assets/list-view-in-agile-view-for-tasks.png) i det övre högra hörnet för att visa uppgiftslistan.
1. (Valfritt) Klicka på **Planläge** icon ![](assets/nwe-plan-mode-icon-task-list.png) och markera **Spara manuellt** väljer du antingen **Standard** eller **Planering av tidslinje**. Detta inaktiverar **Spara automatiskt** som aktiveras som standard.

   ![Välj Spara manuellt](assets/manual-save-option.png)

   >[!TIP]
   >
   >Du kan ångra ändringarna när du väljer Spara manuellt.

1. Skapa en ny uppgift genom att göra något av följande:

   * Klicka **Ny uppgift** högst upp i uppgiftslistan.
   * Klicka **Lägg till fler aktiviteter** längst ned i uppgiftslistan.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Villkorligt) Om du klickade **Ny uppgift** gör följande:

   1. Ange något av fälten i den begränsade listan med fält i **Ny uppgift** och klicka sedan på **Skapa uppgift** om du snabbt vill skapa en uppgift.

      eller

      Om du vill uppdatera alla fält för uppgiften klickar du på **Fler alternativ** för att öppna **Skapa uppgift** box.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      The **Skapa uppgift** öppnas.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Beroende på hur din Workfront-administratör konfigurerar vår layoutmall kan fälten i rutan Skapa uppgift visa olika fält i din miljö. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Ange information för följande områden i den vänstra panelen i rutan Skapa uppgift:

      * Aktivitetsnamn
      * Ökning
      * Uppdrag
      * Anpassad Forms
      * Ekonomi
      * Inställningar

        Mer information om hur du definierar alla uppgiftsrelaterade fält i en uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Villkorligt och valfritt) Om du vill att uppgiften ska vara återkommande uppdaterar du **Återkommande frekvens** fält. Mer information om hur du skapar återkommande uppgifter finns i [Skapa återkommande uppgifter](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Valfritt) Klicka på **Dokument** i den vänstra panelen för att bifoga ett dokument till den nya uppgiften och klicka sedan på **Lägga till eller länka filer** om du vill lägga till ett dokument till uppgiften från datorn, en annan tjänst eller länka dokument och mappar från datorn eller en annan tjänst.

1. (Villkorligt) Om du klickade **Lägg till fler aktiviteter** i steg 5 börjar du att ange uppgiftsinformationen med hjälp av redigering online och trycker sedan på Retur.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Vi rekommenderar att du använder det här alternativet särskilt när du lägger till flera uppgifter i listan.

   ![](assets/ctp4-350x26.png)

1. (Villkorligt) Gör något av följande:

   * Om du klickade **Ny uppgift** i steg 5 klickar du på **Skapa uppgift** för att spara ändringarna och lägga till den nya uppgiften i projektet.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Om du klickade **Lägg till fler aktiviteter** I steg 5 gör du följande:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Klicka var som helst i webbläsaren för att skicka ändringarna eller tryck på Retur.
      1. (Valfritt) Markera den nyligen skapade uppgiften i uppgiftslistan och klicka sedan på **Indrag**.

         Detta gör den nya uppgiften till en underordnad uppgift eller underuppgift till den föregående uppgiften.

         Mer information om underordnade uppgifter finns i [Översikt över uppgifter](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (Villkorligt) Om du har inaktiverat **Spara automatiskt** efter att ha tryckt **Lägg till fler aktiviteter** kan du göra följande:

         * Klicka **Ångra** när som helst för att ångra den senaste ändringen, eller **Avbryt** om du vill ångra alla ändringar du har gjort i uppgiftslistan.
         * Om du tidigare klickat **Ångra**, klicka **Gör om** för att återanvända den senaste ändringen du avbröt.
         * Klicka **Spara** om du vill spara ändringarna i uppgiftslistan.
