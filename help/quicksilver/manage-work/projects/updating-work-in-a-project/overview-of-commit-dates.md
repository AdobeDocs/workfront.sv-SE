---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Genomför datumöversikt
description: Bekräftelsedatum är det datum som en användare tilldelat uppgiften eller ett problem förbinder sig att slutföra uppgiften eller problemet. Detta skiljer sig från det planerade slutförandedatumet eftersom det är en mer realistisk uppskattning av det slutförandedatum som anges av användaren som är ansvarig för arbetet.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Genomför datumöversikt

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Bekräftelsedatum är det datum som en användare tilldelat uppgiften eller ett problem förbinder sig att slutföra uppgiften eller problemet. Detta skiljer sig från det planerade slutförandedatumet för en uppgift eller ett problem eftersom det är en mer realistisk uppskattning av det slutförandedatum som bara anges av den användare som ansvarar för arbetet.

Information om det planerade slutförandedatumet finns i [Översikt över den planerade slutförandetiden](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Genomför datumöversikt

Tänk på följande när du arbetar med implementeringsdatum:

* Endast aktiviteter och ärenden har ett implementeringsdatum.
* Bekräftelsedatum anges inte automatiskt av Adobe Workfront. När du skapar en uppgift eller ett problem finns det inget tilldelat implementeringsdatum.
* Om du är tilldelad en uppgift eller ett ärende kan du ange implementeringsdatum genom att göra något av följande:

   * Låt Workfront ställa in Genomför-datum så att det matchar det befintliga planerade slutförandedatumet för uppgiften eller problemet genom att klicka på Arbeta på den, Starta utgåva eller Starta uppgift för uppgiften eller problemet. Mer information finns i [Ersätt knappen Arbeta med med knappen Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Ange datumet för implementering manuellt enligt när du tror att uppgiften eller utgåvan kommer att slutföras. Detta är din uppskattning och ditt åtagande, som tilldelad, till projektledaren att du kommer att ha uppgiften eller problemet slutfört ett visst datum. Mer information finns i [Uppdatera implementeringsdatum för aktiviteter och problem](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

>[!NOTE]
>
>Du måste vara aktivitetsägare för en aktivitet för att kunna ändra implementeringsdatumet. Följande användare kan inte ändra implementeringsdatumet för en uppgift:
>
>* Projektägare
>* Projektsponsorer
>* Resurshanteraren
>* Systemadministratör
>* Annan tilldelad person för uppgiften
>* Alla andra användare med behörigheter för uppgiften
>
>Mer information om aktivitetsägaren finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Leta reda på implementeringsdatumet för uppgifter och problem

Information om implementeringsdatum för uppgifter och problem finns i följande områden i Workfront:

* Sidan Information
* Panelen Sammanfattning när en Workfront- eller gruppadministratör har lagt till den i layoutmallen. Mer information finns i [Anpassa panelen Sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Rubriken för en uppgift eller ett problem efter att en Workfront- eller gruppadministratör har lagt till den i layoutmallen. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet {#notifications-and-updates-triggered-by-changing-the-commit-date}

När en tilldelad uppgift eller utleverans manuellt ändrar ett implementeringsdatum till ett annat datum än det som anges av projektägaren finns det ett antal meddelanden och uppdateringar som informerar projektägaren och andra användare om den här ändringen.

>[!NOTE]
>
>Ändringar som görs i implementeringsdatumet ändrar inte automatiskt planerade datum, och ändringar som görs i planerade datum ändrar inte automatiskt implementeringsdatumet.

Om du ställer in implementeringsdatumet manuellt för en aktivitet eller ett problem utlöses följande ändringar:

* Ändringen Genomför datum fylls i i systemaktiviteten och på flikarna Alla i uppdateringsavsnittet för uppgiften eller utgåvan.

  ![Bekräfta meddelande om datumändring](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  Ändringen Genomför datum visas under Uppdateringar för aktiviteten eller problemet när Workfront-administratören aktiverar den här uppdateringen i området Uppdateringsfeeds i installationsprogrammet. Mer information finns i [Systemspårade uppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Om en projektägare inte vill godkänna ändringen rekommenderar vi att han/hon kommenterar tillbaka till användaren och föreslår ett nytt datum med hjälp av fliken Kommentarer i uppdateringsavsnittet, ber honom/henne att ändra datumet för implementeringen till det ursprungliga planerade datumet eller välja ett nytt datum.

  Om en projektägare godkänner ändringen kan de manuellt justera det planerade slutförandedatumet så att det matchar det implementeringsdatum som erbjuds av användaren som är tilldelad objektet genom att redigera uppgiften eller utgåvan.

  Du måste ha behörighet att hantera uppgiften eller problemet för att kunna redigera den.

  >[!TIP]
  >
  >Du kan be din system- eller gruppadministratör att lägga till fältet Genomför datum på panelen Sammanfattning eller huvudet för att göra det enklare att uppdatera.
  >
  >Mer information finns i följande artiklar:
  >
  >* [Sammanfattningsöversikt](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [Anpassa panelen Sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [Anpassa objektrubriker med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![Project owner notification update stream about commit date change](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* Aktivitetens eller utställningens beräknade slutförandedatum anges till samma datum eftersom aktiviteten nu har en mer korrekt indikation på när den troligen kommer att slutföras.

  Mer information finns i [Översikt över planerat slutförandedatum för projekt, uppgifter och problem](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![Aktiviteten beräknade slutförandedatum i detaljer markerade](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* Projektägaren meddelas i området Meddelanden om att en aktivitet eller ett ärende har ändrats.

  ![Bekräfta meddelande om datumändring](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >Meddelandet om att implementeringsdatumet har ändrats skickas endast till projektägaren när Workfront-administratören aktiverar visningen av implementeringsdatumet i området Uppdateringsfeeds i installationsprogrammet. Mer information finns i [Systemspårade uppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar ett arbetsobjekt finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Information om hur du uppdaterar implementeringsdatum för aktiviteter och problem finns i [Uppdatera implementeringsdatum för aktiviteter och problem](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
