---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera villkor för aktiviteter och ärenden
description: Villkoret för en aktivitet eller ett problem är en flagga som anger hur den ska gå. Detta skiljer sig från arbetsobjektets status, som anger det aktuella utvecklingssteget för objektet.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Uppdatera villkor för aktiviteter och ärenden

Villkoret för en aktivitet eller ett problem är en flagga som anger hur den ska gå. Detta skiljer sig från arbetsobjektets status, som anger det aktuella utvecklingssteget för objektet.

Du kan ställa in villkoret för en uppgift eller ett problem antingen automatiskt eller manuellt.

Adobe Workfront-administratören kan skapa anpassade villkor för din miljö enligt beskrivningen i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Åtkomstkrav {#access-requirements}

<!--drafted for P&P:

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
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td> <p>Arbeta eller högre för uppgifter</p>
   <p>Begär eller högre för problem</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomst till projekt</p> <p>Redigera åtkomst till uppgifter och ärenden </p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller öka behörigheter för aktiviteter och ärenden för att visa deras villkor</p>
   <p>Hantera behörigheter för aktiviteter och problem för att uppdatera villkoret</p>
    <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Leta reda på villkoret för uppgifter och problem

Villkor visas som en flagga som är kopplad till uppgifter eller problem. De kan även kopplas till ett tal som kan visas i rapporter i stället för etiketten. Mer information om hur du associerar villkor med tal finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Du hittar villkoren för uppgifter och problem i följande områden:

* Området Uppgift och Utleverans av uppdateringar, i en uppdatering, när du har tilldelats uppgiften eller utgåvan.
* Rapporter och listor när du visar fältet Villkor i en vy eller gruppering.

>[!NOTE]
>
>När ordet &quot;villkor&quot; visas i fältet Fältnamn i en journalpostrapport, visar detta att villkoret för ett objekt har uppdaterats. När fältet Villkor spåras i journalposter visar värdena för Nytt och Gammalt nummer numret som är associerat med villkoret i stället för dess namn. Om ett villkor ursprungligen inte är definierat för en aktivitet eller ett problem och du senare uppdaterar det, kommer journalposten som hämtar uppdateringen att visa värdet för Gammalt nummer i villkorsfältet som -2 147 483 648.

## Uppdatera villkoret automatiskt genom att uppdatera statusen

När du har tilldelats en uppgift eller ett ärende och du klickar på **Arbeta på den** , Starta aktivitet eller Starta problem, eller uppdatera status för aktiviteten, så ändras villkoret automatiskt till standardvillkoret som är associerat med **Går smidigt**.

Mer information om hur du använder ett anpassat villkor som standardvillkor finns i artiklarna  [Ange ett anpassat villkor som standard för uppgifter och ärenden](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) och [Ange ett anpassat villkor som standard för projekt](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Mer information om hur du ändrar aktivitetsstatus finns i [Uppdatera aktivitetsstatus](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Mer information om hur du ändrar utgivningsstatus finns i [Uppdatera utleveransstatus](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Mer information om hur du ställer in knappen Work On It (Arbeta på den) på knappen Start Task (Starta aktivitet) eller Start Issue (Starta problem) finns i [Ersätta knappen Work On It (Arbeta på) med en Start-knapp](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Uppdatera villkoret manuellt

Du måste tilldelas en uppgift eller ett ärende eller ha behörigheten Hantera för att kunna ställa in villkoret på den.

Uppdateringen av villkoret för en aktivitet eller ett problem skiljer sig åt beroende på om du har tilldelats den eller inte:

* Du kan uppdatera villkoret på fliken Uppdateringar eller i en lista med uppgifter eller problem om du har tilldelats dem.
* Du kan bara uppdatera villkoret i en lista med uppgifter eller problem om du inte har tilldelats dem, men har behörighet att hantera dem. I det här fallet kan du inte uppdatera villkoret på fliken Uppdatera för uppgiften eller problemet.

Så här ställer du in villkoret för en aktivitet eller ett problem manuellt:

1. Gå till en uppgift eller ett ärende som du har tilldelats och som du vill ange villkoret för.

   eller

   Gå till en lista över uppgifter eller problem som du har behörigheten Hantera för, men som inte har tilldelats till dig.

1. Ändra villkoret för problemet eller aktiviteten enligt följande:

   * Om du har tilldelats uppgiften eller utgåvan och har behörigheten Hantera, går du till **Uppdateringar** flik, klicka **Starta en ny uppdatering** väljer du **Villkor** som bäst återspeglar aktivitetens förlopp, ange orsaken till ändringen av villkoret i dialogrutan **Starta en ny uppdatering** område (valfritt) och klicka sedan på **Uppdatera**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >Villkoren kan anpassas efter din miljö, så du kan hitta fler än tre alternativ för Villkor i din miljö. Namnen på villkoren kan skilja sig från namnen ovan. Mer information om hur du anpassar villkor i Workfront finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
