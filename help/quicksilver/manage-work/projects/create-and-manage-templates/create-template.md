---
product-area: templates
navigation-topic: templates-navigation-topic
title: Skapa en projektmall
description: Du kan skapa och ta bort mallar under Mallar. När du skapar en ny mall kan du ange informationen för alla uppgifter och för dina framtida projektinställningar. Den här informationen överförs sedan till alla projekt som du skapar från mallen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 46133f435c665dd82d134f18d0b5de4e70bab7d7
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Skapa en projektmall

<!-- Audited: 10/2025 -->

Du kan skapa och ta bort mallar under Mallar. När du skapar en ny mall kan du ange informationen för alla uppgifter och för dina framtida projektinställningar. Den här informationen överförs sedan till alla projekt som du skapar från mallen.

>[!NOTE]
>
>En mall och dess uppgifter har inga faktiska datum, utan snarare en indikation på vilken dag (från när det framtida projektet kan starta) en aktivitet kan starta och vilken dag aktiviteten kan behöva slutföras. När du använder mallar för att skapa framtida projekt får projekten faktiska datum. Mer information finns i [Skapa ett projekt](../create-projects/create-project.md).


Du kan skapa en ny mall på följande sätt:

* Från början, enligt beskrivningen i den här artikeln.
* Från befintliga projekt genom att spara ett projekt som en mall.

  Mer information om hur du skapar mallar från befintliga projekt finns i [Spara ett projekt som en mall](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Genom att kopiera den från en annan mall.

  Mer information om hur du kopierar en befintlig mall finns i [Kopiera en projektmall](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Genom att importera utkast. Du måste vara Workfront-administratör för att kunna importera utkast. Mer information finns i [Konfigurera en plan](../../../administration-and-setup/blueprints/configure-template-package.md).

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
   <td> <p>Standard </p><p>Plan</p> <p>Du måste vara systemadministratör för att kunna importera mallar från utkast</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Som standard har du behörigheten Hantera för de mallar du skapar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa en mall

{{step1-to-templates}}

1. Klicka på **Ny mall**.

   Mallen är namnlös.

   ![Ny mall](assets/create-template-nwe-2022-350x102.png)

1. Ange ett namn för den nya mallen i mallhuvudet och tryck sedan på **Retur.**
1. Klicka på avsnittet **Malluppgifter** i den vänstra panelen.
1. Klicka på **Börja lägga till malluppgifter** om du vill lägga till inline-aktiviteter

   eller

   Klicka på **Ny mallaktivitet** om du vill lägga till aktiviteter i mallen i rutan **Ny mallaktivitet**.

   ![Ny mallaktivitet](assets/new-template-task-box.png)

   <!--<span class="preview">The Create Template Task opens in the new experience.</span>-->

   <!--
   1. <span class="preview">(Conditional) Using the new experience, update information in the following areas in the **Create Template Task** box:</span>
   <div class="preview">
   * Template Task Name
   * Overview
   * Assignments
   * Finance
   * Custom Forms
   * Documents
   * Settings 
   </div>
   1. Click **Save**
   Or (*******remove the 1. from the step below and continue with those steps here*********)
   1. (Optional) Click **Switch back to old experience** at the bottom of the **Create Template Task** box.
   The **New Template Task** opens. (************add screen shot***********)-->

1. Uppdatera information i följande områden i rutan **Ny mallaktivitet**:

   * Översikt
   * Ekonomi
   * Inställningar
   * Uppdrag
   * Anpassad Forms
   * Bifoga dokument

     Att uppdatera information för en malluppgift påminner om att redigera uppgifter i ett projekt. Mer information finns i [Redigera uppgifter](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). <!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >Du kan inte lägga till återkommande uppgifter i en mall.

1. Klicka på något av följande:

   * **Spara mallaktivitet** om du vill spara den aktuella mallaktiviteten och stänger rutan Ny mallaktivitet.
   * **Spara mallaktivitet och starta en annan** om du vill spara den aktuella mallaktiviteten och öppna en annan ny malluppgift om du vill lägga till en annan uppgift.
   * **Avbryt** om du vill stänga rutan utan att spara mallaktiviteten.
1. (Valfritt) När du har lagt till malluppgifterna kan du klicka på ikonen **Gantt-schema** i det övre högra hörnet i uppgiftslistan för att visa en visuell representation av mallens uppgiftslista.

   >[!TIP]
   >
   >Du kan inte redigera aktiviteter direkt från det här Gantt-diagrammet.

1. Om du vill lägga till information i den nya mallen klickar du på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) till vänster om mallnamnet i sidhuvudet och sedan på **Redigera**.

   Mer information om hur du redigerar en mall finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >   Om en projektmall är associerad med en grupp (eller om det inte finns någon grupp) påverkar det hur inställningar för projekt, uppgift och problem bestämmer vissa inställningar i mallen.
   >
   >Mer information finns i avsnittet&quot;Hur inställningar gäller för mallar och malluppgifter&quot; i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Klicka på **Spara**.
1. (Valfritt) Lägg till följande objekt i mallen

   * Dokument
   * Risker
   * Godkännandeprocesser
   * Faktureringstaxor
   * Utgifter
   * Köinformation
   * Ämnesgrupper och Köämnen

1. (Valfritt) Lägg till följande objekt till uppgifterna i mallen:

   * Dokument
   * Utgifter
   * Godkännanden

   Mer information finns i avsnittet Lägg till fler objekt i en mall i artikeln [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




