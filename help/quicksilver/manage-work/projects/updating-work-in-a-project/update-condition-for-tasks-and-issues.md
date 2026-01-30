---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera villkor för aktiviteter och ärenden
description: Villkoret för en aktivitet eller ett problem är en flagga som anger hur den ska gå. Detta skiljer sig från arbetsobjektets status, som anger det aktuella utvecklingssteget för objektet.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Uppdatera villkor för aktiviteter och ärenden

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Villkoret för en aktivitet eller ett problem är en flagga som anger hur den ska gå. Detta skiljer sig från arbetsobjektets status, som anger det aktuella utvecklingssteget för objektet.

Du kan ställa in villkoret för en uppgift eller ett problem antingen automatiskt eller manuellt.

Villkorsvärdena som vi hänvisar till i den här artikeln är som standard tillgängliga i Workfront. Din Adobe Workfront-administratör kan skapa anpassade villkor för din miljö, vilket beskrivs i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Åtkomstkrav {#access-requirements}

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
   <td> 
   <ul><li><p>Standard för uppgifter</p></li>
   <li><p>Medarbetare eller högre för problem</p></li></ul>
  <p>eller</p>
   <ul><li><p>Arbeta eller högre för uppgifter</p></li>
   <li><p>Begär eller högre för problem</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomst till projekt</p> <p>Redigera åtkomst till uppgifter och ärenden </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller öka behörigheter för aktiviteter och ärenden för att visa deras villkor</p>
   <p>Contribute-behörigheter för uppgifter och ärenden för att uppdatera villkoret</p>
  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>
   Current:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Contribute permissions on tasks and issues to update the Condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Du måste tilldelas en aktivitet eller ett problem för att kunna uppdatera dess villkor manuellt.

## Leta reda på villkoret för uppgifter och problem

Villkor visas som en flagga som är kopplad till uppgifter eller problem. De kan även kopplas till ett tal som kan visas i rapporter i stället för etiketten. Mer information om hur du associerar villkor med tal finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Du hittar villkoren för åtgärder och problem i följande områden av Workfront:

* Sidan Detaljer visas när en Workfront- eller gruppadministratör har lagt till den i layoutmallen. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* Rubriken för en uppgift eller ett problem, efter att en Workfront- eller gruppadministratör har lagt till den i layoutmallen. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* Panelen Sammanfattning visas när en Workfront- eller gruppadministratör har lagt till den i layoutmallen. Mer information finns i [Anpassa panelen Sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Rapporter och listor när du visar fältet Villkor i en vy eller gruppering.

  >[!NOTE]
  >
  >När ordet &quot;villkor&quot; visas i fältet Fältnamn i en journalpostrapport, visar detta att villkoret för ett objekt har uppdaterats. När fältet Villkor spåras i journalposter visar värdena för Nytt och Gammalt nummer numret som är associerat med villkoret i stället för dess namn. Om ett villkor ursprungligen inte är definierat för en aktivitet eller ett problem och du senare uppdaterar det, kommer journalposten som hämtar uppdateringen att visa värdet för Gammalt nummer i villkorsfältet som -2 147 483 648.

## Uppdatera villkoret automatiskt genom att uppdatera statusen

När du har tilldelats en aktivitet eller ett problem och klickar på **Arbeta med den** , Starta aktivitet eller Starta problem, eller uppdatera dess status, ändras aktivitetens eller problemets villkor automatiskt till det standardvillkor som är kopplat till **Går smidigt**.

Mer information om hur du använder ett anpassat villkor som standardvillkor finns i artiklarna [Ange ett anpassat villkor som standard för uppgifter och problem](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) och [Ange ett anpassat villkor som standard för projekt](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Mer information om hur du ändrar aktivitetsstatus finns i [Uppdatera aktivitetsstatus](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Mer information om hur du ändrar utgivningsstatus finns i [Uppdatera utgivningsstatus](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Mer information om hur du ställer in knappen Arbeta på den till en Start-aktivitet eller Starta problem finns i [Ersätt Arbeta på den med en Start-knapp](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Uppdatera villkoret manuellt

Du måste tilldelas en uppgift eller ett ärende eller ha behörigheten Hantera för att kunna ställa in villkoret på den.

Du kan uppdatera villkoret för en uppgift eller ett problem manuellt i en rapport eller en utgivningslista när du visar fältet Villkor i vyn.

>[!NOTE]
>
>Du kan be system- eller gruppadministratören att lägga till villkorsfältet på sammanfattningspanelen eller huvud- eller utleveranssidorna eller informationssidorna.
>
>Mer information finns i följande artiklar:
>
>* [Sammanfattningsöversikt](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Anpassa panelen Sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Du kan uppdatera villkoret för uppgifter och problem manuellt i olika områden av Workfront. I följande avsnitt beskrivs hur du manuellt kan uppdatera villkor för uppgifter och problem.

### Uppdatera villkoret för en aktivitet eller ett problem i huvud för aktiviteten eller problemet

1. (Villkorligt) Om Workfront- eller gruppadministratören har lagt till fältet Villkor i huvud för aktiviteten eller problemet i layoutmallen klickar du på fältet **Villkor** i sidhuvudet och väljer bland följande alternativ:
   * Går smidigt
   * Vissa bekymmer
   * Större vägspärrar

   ![Villkor i uppgiftshuvudet](assets/condition-in-task-header-0925.png)

<!--1. Click Enter to save the Condition.-->

### Uppdatera villkoret för en aktivitet eller ett problem i avsnittet med information om aktiviteten eller problemet

1. (Villkorligt) Om Workfront- eller gruppadministratören har lagt till villkorsfältet i informationsavsnittet för en uppgift eller ett problem i layoutmallen klickar du på **Information** i den vänstra panelen, sedan på **Aktivitetsvillkor** eller **Utfärdandevillkor** och väljer något av följande alternativ:
   * Går smidigt
   * Vissa bekymmer
   * Större vägspärrar
1. Klicka på **Spara ändringar**. Aktivitets- eller utgivningsvillkoret uppdateras.

### Uppdatera villkoret för en aktivitet eller ett problem i en rapport eller lista

1. Gå till en lista över uppgifter eller problem som du har behörighet att hantera. Kontrollera att fältet **Villkor** visas i listvyn.

1. Uppdatera **villkoret** för problemet eller aktiviteten genom att dubbelklicka på det befintliga villkoret och välja ett nytt värde i listrutan.

   ![Villkorsvärden i uppgiftslistan](assets/condition-values-in-task-list-0925.png)

   >[!NOTE]
   >
   >Villkoren kan anpassas efter din miljö, så du kan hitta fler än tre alternativ för Villkor i din miljö. Namnen på villkoren kan skilja sig från namnen ovan. Mer information om hur du anpassar villkor i Workfront finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Tryck på **Enter** på tangentbordet eller klicka utanför fältet Villkor för att spara den nya aktiviteten eller villkoret för problemet.

   >[!NOTE]
   >
   >I standardvillkorsvyn är fältet **Villkor** en typ av fält som inte kan redigeras infogat. När du lägger till fältet **Villkor** separat i en vy går det att redigera det. Mer information om redigering finns i [Redigera objekt i en lista i Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


