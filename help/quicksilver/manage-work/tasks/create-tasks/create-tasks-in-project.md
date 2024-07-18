---
product-area: projects
navigation-topic: create-tasks
title: Skapa uppgifter i ett projekt
description: Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# Skapa uppgifter i ett projekt

<!-- Audited: 1/2024 -->

Du kan bara skapa uppgifter i ett projekt efter att du har skapat projektet.

När du har skapat ett projekt kanske du vill lägga till uppgifter och ändra dem för att ordna projektplanen. Mer information om hur du skapar ett projekt finns i [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

Mer information om hur du skapar personliga uppgifter som inte finns i ett projekt finns i avsnittet [Skapa en personlig uppgift](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task) i artikeln [Skapa arbetsobjekt från startdelen](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

I den här artikeln beskrivs hur du skapar åtgärder från grunden. Du kan också skapa uppgifter på följande sätt:

* Genom att kopiera eller duplicera befintliga uppgifter. Mer information finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Genom att flytta uppgifter från ett projekt till ett annat. Mer information finns i [Flytta aktiviteter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-licens</p> </td> 
   <td><p>Aktuell: Arbete eller högre</p> 
   eller
   <p>Nytt: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter till projektet med möjlighet att lägga till uppgifter eller högre</p> <p>När du skapar en uppgift får du automatiskt behörigheten Hantera för uppgiften</p> <p> Mer information om aktivitetsbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Dela en uppgift </a>. </p> <p>Mer information om hur du begär ytterligare behörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa uppgifter i ett projekt

1. Gå till det projekt där du vill skapa en uppgift.
1. Klicka på **Åtgärder** i den vänstra panelen.
1. (Villkorligt) Om du visar uppgiftslistan i en flexibel vy klickar du på ikonen **Listvy** ![](assets/list-view-in-agile-view-for-tasks.png) i det övre högra hörnet för att visa uppgiftslistan.
1. (Valfritt) Klicka på ikonen **Planeringsläge** ![](assets/nwe-plan-mode-icon-task-list.png) och välj **Manuell sparning**. Välj sedan antingen **Standard** eller **Tidslinjeplanering**. Detta inaktiverar alternativet **Spara automatiskt** som är aktiverat som standard.

   ![Välj Spara manuellt](assets/manual-save-option.png)

   >[!TIP]
   >
   >Du kan ångra ändringarna när du väljer Spara manuellt.

1. Skapa en ny uppgift genom att göra något av följande:

   * Klicka på **Ny aktivitet** överst i uppgiftslistan.
   * Klicka på **Lägg till fler aktiviteter** längst ned i uppgiftslistan.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Villkorligt) Om du klickade på **Ny aktivitet** gör du följande:

   1. Ange något av fälten i den begränsade listan med fält i rutan **Ny uppgift** och klicka sedan på **Skapa uppgift** om du snabbt vill skapa en uppgift.

      eller

      Om du vill uppdatera alla fält för uppgiften klickar du på **Fler alternativ** för att öppna rutan **Skapa uppgift** .

      ![](assets/nwe-create-task-small-screen-350x272.png)

      Rutan **Skapa uppgift** öppnas.

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

   1. (Villkorlig och valfri) Om du vill att aktiviteten ska vara återkommande uppdaterar du fältet **Återkommande frekvens**. Mer information om hur du skapar återkommande aktiviteter finns i [Skapa återkommande aktiviteter](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Valfritt) Klicka på **Dokument** i den vänstra panelen för att bifoga ett dokument till den nya aktiviteten och klicka sedan på **Lägg till eller länka filer** för att lägga till ett dokument till uppgiften från datorn, en annan tjänst eller för att länka dokument och mappar från datorn eller en annan tjänst.

1. (Villkorligt) Om du klickade på **Lägg till fler uppgifter** i steg 5 börjar du ange aktivitetsinformationen med hjälp av redigering online och trycker sedan på Retur.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Vi rekommenderar att du använder det här alternativet särskilt när du lägger till flera uppgifter i listan.

   ![](assets/add-more-tasks-inline.png)

1. (Villkorligt) Gör något av följande:

   * Om du klickade på **Ny aktivitet** i steg 5 klickar du på **Skapa aktivitet** för att spara ändringarna och lägga till den nya aktiviteten i projektet.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Om du klickade på **Lägg till fler uppgifter** i steg 5 gör du följande:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Klicka var som helst i webbläsaren för att skicka ändringarna eller tryck på Retur.
      1. (Valfritt) I uppgiftslistan markerar du den nyligen skapade aktiviteten och klickar sedan på **Indrag**.

         Detta gör den nya uppgiften till en underordnad uppgift eller underuppgift till den föregående uppgiften.

         Mer information om underordnade uppgifter finns i [Skapa underaktiviteter](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Villkorligt) Om du inaktiverade alternativet **Spara automatiskt** efter att du tryckt på **Lägg till fler uppgifter** kan du göra följande:

         * Klicka på **Ångra** när du vill ångra den senaste ändringen eller **Avbryt** om du vill ångra alla ändringar du har gjort i uppgiftslistan.
         * Om du tidigare klickade på **Ångra** klickar du på **Gör om** för att tillämpa den senaste ändringen som du avbröt.
         * Klicka på **Spara** om du vill spara ändringarna i uppgiftslistan.
