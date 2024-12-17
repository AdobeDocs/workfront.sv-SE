---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Konfigurera inställningar för aktiviteter och problem i hela systemet
description: Du kan konfigurera systemomfattande inställningar för uppgifter och problem. Dessa inställningar påverkar hur dina användare skapar uppgifter och problem i Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 0%

---

# Konfigurera inställningar för uppgifter och problem i hela systemet

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

Som [!DNL Adobe Workfront]-administratör kan du konfigurera systemomfattande inställningar för uppgifter och problem. De här inställningarna påverkar hur dina användare skapar uppgifter och problem i [!DNL Workfront].

Inställningarna för uppgifter och utgåvor är som standard låsta och gruppadministratörer kan inte ändra dem på gruppnivån om du inte låser upp dem för alla grupper i hela systemet. Mer information finns i avsnittet [Lås uppgifter och utgivningsinställningar för grupper](#lock-task-and-issue-preferences-for-groups) i den här artikeln.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera inställningar för aktiviteter och ärenden för alla i [!DNL Workfront]

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** >**[!UICONTROL Tasks & Issues]i den vänstra panelen.**

1. På den sida som visas fortsätter du med något av de sex avsnitten nedan för att konfigurera inställningar för [!UICONTROL New Task Defaults], [!UICONTROL Issues], [!UICONTROL Deletion], [!UICONTROL Actual Dates] och [!UICONTROL Access]:

   * [[!UICONTROL New Task Defaults]](#new-task-defaults)
   * [[!UICONTROL Issues]](#issues)
   * [[!UICONTROL Deletion]](#deletion)

   <!--* <span class="preview">[Move](#move)</span>-->

   * [[!UICONTROL Actual Dates]](#actual-dates)
   * [[!UICONTROL Delegation]](#delegation)
   * [[!UICONTROL Access]](#access)

<!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
-->



### [!UICONTROL New Task Defaults] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Start Date]</td> 
    <td> <p>Bestämmer standardstartdatumet för nya uppgifter för projektledare. Startdatumet för nya aktiviteter kan antingen vara det planerade startdatumet för projektet eller den dag då aktiviteten skapas.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Bestämmer relationen mellan antalet resurser (och deras allokeringsprocent) och varaktigheten eller den totala ansträngningen för aktiviteten. Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Typer av aktivitetsvaraktighet och varaktighet</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>Beräknar planerade och faktiska intäktsuppskattningar för en aktivitet. När <strong>[!UICONTROL Revenue Type]</strong> är inställt på <strong>[!UICONTROL Not Billable]</strong> genereras ingen intäktsuppskattning för aktiviteten av planerade timmar och registrerade timmar, och arbetet med aktiviteten bidrar inte till intäkten på projektnivå.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>Beräknar planerade och faktiska kostnadsuppskattningar för en aktivitet. När värdet är <strong>[!UICONTROL No Cost]</strong> genereras ingen planerad eller faktisk kostnadsuppskattning för aktiviteten av planerade timmar och registrerade timmar, och arbetet med aktiviteten bidrar inte till projektnivåkostnaderna.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problem {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object changes]</td> 
    <td> <p>När någon konverterar ett problem till ett projekt eller en uppgift blir både det ursprungliga problemet och det konverterade projektet eller den konverterade aktiviteten objekt som löses. Med den här inställningen kan du korrelera upplösningen för det ursprungliga problemet med upplösningen för dess objekt som kan lösas. Mer information om hur du löser objekt finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a>.</p> <p>För att den här inställningen ska ha någon effekt måste du välja alternativet <strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>.</p> 
      <ul> 
      <li>När den här inställningen är aktiverad kan du skapa anpassade statusvärden med samma nyckel för både utgåvor, projekt och uppgifter. När projektet eller aktiviteten (som ett upplösningsbart objekt) blir en anpassad status, återspeglas ändringen även i problemets status. Statusnyckeln måste vara densamma för utleverans- och projekt- eller aktivitetsstatus.</li> 
      <li>När den här inställningen är inaktiverad ställs objektstatus automatiskt in på standardstatus i stället för de anpassade. Mer information om standardstatusvärdena finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Öppna listan över status för systemproblem</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a task]</td> 
    <td> <p>Inställningarna i det här avsnittet avgör vad som händer under konverteringsprocessen från problem till uppgift:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>: När du konverterar ett problem förblir det synligt som ett problem tills det är klart. Status för problemet ändras automatiskt till [!UICONTROL Closed] när aktiviteten slutförs. När detta är avmarkerat tas problemet bort.</p> <p><b>OBS</b>:  <p>Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till utgåvor</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett problem </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the task]</strong>: Ger den primära kontakten (den som skapat utgåvan) Visa åtkomst till uppgiften för att granska den, hålla dig informerad om hur den fortlöper och göra kommentarer i uppdateringsavsnittet för uppgiften.</li> 
      <li> <p><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Användare som konverterar problemet kan ändra dessa alternativ under konverteringen av ett problem till en aktivitet.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a project]</td> 
    <td> <p>Inställningarna i det här avsnittet avgör vad som händer under konverteringsprocessen från problem till projekt:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the project]</strong>: När du konverterar problemet förblir det synligt som ett problem tills projektet är klart. Status för problemet ändras automatiskt till [!UICONTROL Closed] när projektet slutförs. När detta är avmarkerat tas problemet bort. </p> <p><b>OBS</b>:  <p>Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Bevilja åtkomst till utgåvor</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett problem </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the project]</strong>: Ger den primära kontakten (den som skapat problemet) Visa åtkomst till projektet för att granska det, hålla dig informerad om projektets förlopp och kommentera uppdateringsavsnittet i projektet.</li> 
      <li><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Användare som konverterar problemet kan ändra de listade alternativen under konverteringen av en utgåva till ett projekt.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Deletion] {#deletion}

**[!UICONTROL Allow users to delete tasks & issues with logged hours]**: Gör att du kan avgöra om du tillåter att uppgifter eller problem tas bort där timmar loggas. Det här alternativet är markerat som standard.

>[!TIP]
>
>Den här inställningen gäller även för att ta bort projekt som har uppgifter eller problem med timmar som är inloggade. Den här inställningen gäller inte för att ta bort projekt där tiden loggas direkt för projektet.

* När det är markerat får du en informativ varning när du tar bort en uppgift eller ett problem. Varningen påminner dig om att om aktiviteten eller problemet har loggat timmar kommer de antingen att flyttas till projektet eller tas bort. Du kan konfigurera om timmarna ska tas bort eller flyttas till projektet i området [!UICONTROL Timesheet & Hours Preferences] i [!UICONTROL Setup]. När du har bekräftat att du har sett varningen tas uppgiften eller problemet bort. Mer information om hur du konfigurerar inställningar för tidrapport och timmar finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >När du tar bort ett projekt med uppgifter och ärenden som har loggade timmar, tas de loggade timmarna bort eller så bevaras de enligt inställningarna i området [!UICONTROL Timesheet & Hours Preferences] i [!UICONTROL Setup]. Varningsmeddelandet visas inte när du tar bort ett projekt.

* När du avmarkerar det här alternativet får du en varning när du tar bort en uppgift eller ett problem med loggade timmar, eller när du tar bort ett projekt med timmar som loggats för dess uppgifter eller problem. Varningen anger att administratören inte tillåter att uppgifter eller problem med loggade timmar tas bort. Det går inte att ta bort aktiviteter, utgåvor eller projekt som har timmar loggade för uppgifter och utgåvor.

<!--*****also replace the & with "and" in the Deletion section

<div class="preview">

### Move

**[!UICONTROL Allow users to move tasks and issues with logged hours]**: Lets you determine whether you allow the move of tasks or issues where hours are logged. This option is selected by default.

* When it is selected, you can move tasks and issues that have time logged. The hours also move with the tasks or issues. 

* When you deselect this option, you receive a prohibitive warning when you move a task or issue with logged hours. The warning specifies that the administrator does not allow for tasks or issues with logged hours to be moved. The tasks or issues that have hours logged cannot be moved. 

</div>

-->

### [!UICONTROL Actual Dates] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue goes from "New" to "In Progress," set the Actual Start Date to]</td> 
    <td> <p>Välj ett av följande alternativ för när det faktiska startdatumet registreras i [!DNL Workfront] när en uppgift eller ett problem går från <strong>[!UICONTROL New]</strong> till <strong>[!UICONTROL In Progress]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Det faktiska startdatumet är inställt på det aktuella datumet.</li> 
      <li><strong>[!UICONTROL The Planned Start Date]:</strong> Det faktiska startdatumet är inställt på det planerade startdatumet för aktiviteten eller utgåvan.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue is completed, set the Actual Completion Date to]</td> 
    <td> <p>Välj ett av följande alternativ för när det faktiska slutförandedatumet registreras i [!DNL Workfront] när en uppgift eller ett problem har slutförts:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Det faktiska slutförandedatumet är inställt på det aktuella datumet.</li> 
      <li> <p><strong>[!UICONTROL The Planned Completion Date]:</strong> Det faktiska slutförandedatumet är inställt på det planerade slutförandedatumet för aktiviteten eller utgåvan.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegering

Om du aktiverar inställningen **[!UICONTROL Allow users to delegate their tasks & issues]** kan alla användare tillfälligt delegera sitt arbete till andra.

När den här inställningen är aktiverad kan användarna se följande:

* Länken [!UICONTROL **Delegera**] i deras [!UICONTROL My Work]-, [!UICONTROL My Tasks]- eller [!UICONTROL My Issues]-widgetar i området [!UICONTROL Home]. De kan delegera uppgifter och utgivningstilldelningar därifrån.

  >[!NOTE]
  >
  >  Länken [!UICONTROL **Delegera godkännanden**] är alltid aktiverad i området [!UICONTROL Home].

* En indikation på att en aktivitet eller ett problem har delegerats till en annan användare i området [!UICONTROL Assignments and delegations] i huvud för aktiviteten eller problemet.
* En indikation på att en uppgift eller ett problem har delegerats till en annan användare i deras [!UICONTROL My Work]-widget i [!UICONTROL Home].

  Om du inaktiverar inställningen [!UICONTROL Allow users to delegate their tasks & issues] kommer delegeringarna som är schemalagda att stoppas och de delegerade användarna får ett e-postmeddelande om att delegeringen har stoppats.

Mer information om hur du delegerar arbete till andra finns i följande artiklar:

* [Delegera arbetsöversikt](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delegera uppgifter och ärenden](../../../manage-work/delegate-work/how-to-delegate-work.md)


<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Access] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to a task]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Definierar standardbehörigheten som en användare har för den uppgift han/hon är tilldelad till. Mer information om aktivitetsbehörigheter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Definierar standardbehörigheten som en användare har för det projekt som han/hon har en uppgift tilldelad till. Mer information om projektbehörigheter finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to an issue]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Definierar standardbehörigheten som en användare har för den uppgift han/hon är tilldelad till. Mer information om aktivitetsbehörigheter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Definierar standardbehörigheten som en användare har för det projekt som han/hon har en uppgift tilldelad till. Mer information om projektbehörigheter finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone submits a request]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to the issue]</strong>: Definierar standardbehörigheten som en användare har på en begäran som de har skickat. Mer information finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett problem </a>.</li> 
      <li> <p><strong>[!UICONTROL People from the same company will inherit the same permissions for all requests]</strong>: Tillåter användare att se begäranden som andra användare från samma företag skickar. De har samma behörigheter för de begäranden som de själva har skickat.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Klicka på **[!UICONTROL Save]**.

## Lås uppgifter och utgivningsinställningar för grupper {#lock-task-and-issue-preferences-for-groups}

Om grupper i organisationen behöver en uppgift eller en utgåva som har konfigurerats på olika sätt för sina unika arbetsflöden, kan du låsa upp inställningen för alla grupper i organisationen så att de kan konfigurera den på egen hand. När en inställning är olåst och gruppadministratören ändrar den påverkas de uppgifter eller problem som är kopplade till gruppen av inställningen på gruppnivå i stället för inställningen på systemnivå.

Mer information om hur en gruppadministratör konfigurerar uppgifter och utgåvor för en grupp finns i [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>När en [!DNL Workfront]-administratör har låst upp en inställning på systemnivå kan alla gruppadministratörer konfigurera den och sedan låsa den för att se till att alla i gruppen och undergrupperna nedan använder samma konfiguration. Detta är parallellt med möjligheten för en [!DNL Workfront]-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och [Lås eller lås upp ett projekt, en aktivitet eller en utgåva för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Så här låser eller låser du upp en uppgift eller en utgåva så att grupper kan konfigurera den:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Tasks & Issues]**.

1. Gör något av följande:

   * Om du vill att administratörer för grupper under gruppen ska kunna konfigurera en inställning för sina grupper, låser du upp den ![](assets/unlock-toggle-button.png).
   * Om du vill att din grupp och alla grupper under den ska använda din konfiguration för en inställning kontrollerar du att den är låst (detta är standardinställningen).

     >[!IMPORTANT]
     >
     >Vi rekommenderar att du kommunicerar med administratörer och användare i grupper i hela systemet för att säkerställa att alla behov beaktas när du konfigurerar en låst inställning. När du låser den ärvs konfigurationen för den av alla grupper i systemet. Om inställningen har låsts upp under en viss tid ersätter konfigurationen de som gruppadministratörer kan ha gjort.

1. Klicka på **[!UICONTROL Save]**.
