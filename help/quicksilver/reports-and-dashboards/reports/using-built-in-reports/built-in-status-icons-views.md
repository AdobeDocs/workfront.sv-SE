---
product-area: reporting
navigation-topic: using-built-in-reports
title: Inbyggda statusikoner i vyer
description: Du kan lägga till det inbyggda fältet Statusikoner som en kolumn i vyerna för att förbättra synligheten i viktiga punkter om objekten.
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---

# Inbyggda statusikoner i vyer

<!-- Audited: 11/2024 -->

<!--(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.)-->

Du kan lägga till det inbyggda fältet Statusikoner som en kolumn i vyerna för att förbättra synligheten i viktiga punkter om objekten. Med statusikoner ser du direkt när följande villkor är uppfyllda:

* Ett objekt har bifogade dokument
* Ett objekt är associerat med en godkännandeprocess
* Ett objekt har ytterligare anteckningar kopplade till sig
* En utgift är fakturerbar eller återbetalningsbar
* En uppgift är på en kritisk väg
* En användare tillhör ett företag, ett team eller befinner sig personligen i en annan tidszon

Tänk på följande:

* De flesta indikatorerna i fältet Statusikoner är snabblänkar till det objekt eller det område i objektet som de representerar.

* Om något av objekten som representeras av ikonerna saknas i objektet visas ikonen som representerar det saknade objektet nedtonad i kolumnen Statusikoner i stället för i en färgad bild.

  ![task_status_icons.png](assets/task-status-icons.png)

  Mer information finns i avsnittet [Översikt över statusikoner och flaggor](#overview-of-status-icons-and-flags) i den här artikeln.

* I vissa vyer heter fältet **Statusikoner** **Flaggor** eller **Visa ikoner**.\
  Du kan inte anpassa utseendet på de ikoner som finns i fältet Statusikoner.

* Du kan inte redigera antalet ikoner i fältet Statusikoner.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Medarbetare eller högre</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Begäran eller senare</p></li>
         </ul>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att lägga till kolumner i en rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en befintlig vy</p> <p>Hantera behörigheter för en rapport för att lägga till kolumner i den</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till fältet Statusikoner i en vy

I vissa inbyggda vyer och rapporter finns redan fältet Statusikoner.

Du kan inte lägga till fältet Statusikoner i alla vyer.

Så här lägger du till fältet Statusikoner i en anpassad vy som du bygger från början:

1. Gå till en lista med något av följande objekt:

   * Uppgifter
   * Problem
   * Projekt
   * Malluppgifter
   * Mallar
   * Utgifter
   * Dokument
   * Användare\
     Endast dessa objekt har fältet **Statusikoner** tillgängligt.\
     Mer information om objektlistor finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Välj **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn**.
1. I rutan **Visa i den här kolumnen** börjar du skriva något av följande fältnamn och markerar det sedan när det visas i listan:

   * *Statusikoner*
   * *Flaggor*
   * *Visa ikoner *(endast i dokumentvyer).

   De inbyggda ikonerna visas under något av dessa namn.\
   En mallvy innehåller både fälten **Statusikoner** och **Flaggor**. I det här fallet innehåller de två kolumnerna identiska ikoner.\
   Dokumentvyer innehåller fältet **Visa ikoner**.

1. Klicka på **Spara vy**.
1. (Valfritt) Ange ett nytt namn för vyn och klicka sedan på **Spara vy**.\
   Detta lägger till kolumnen **Statusikoner** i din vy.
1. (Valfritt) För musen över en ikon för att förstå vad den representerar.
1. (Valfritt) Klicka på en ikon om du vill gå till det område som representeras av den.\
   Alla ikoner är inte länkar till objekt.\
   En fullständig lista över attribut för varje ikon finns i avsnittet [Översikt över statusikoner och flaggor](#overview-of-status-icons-and-flags).

## Översikt över statusikoner och flaggor {#overview-of-status-icons-and-flags}

I följande tabell visas alla statusikoner som är tillgängliga i Workfront, vilken typ av objekt som kan kopplas till dem samt vad som händer när du klickar på dem.

Du måste ha behörighet att åtminstone visa objekten för att kunna klicka på några av följande ikoner och komma åt dessa objekt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Statusikon eller flagga</strong> </th> 
   <th><strong>Beskrivning</strong> </th> 
   <th><strong>Objekt</strong> </th> 
   <th>Vid klickning</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">eller <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;"> eller <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> eller <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Anger att projektvillkoret är On Target (green), In Trouble (red) eller At Risk (yellow).<br>Mer information om projektvillkor finns i <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Översikt över projektvillkor och villkorstyp</a>.</td> 
   <td>Projekt</td> 
   <td>Klicka för att öppna aktivitetslistan för projektet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Anger att objektet har anteckningar (uppdateringar) på fliken Uppdateringar.</td> 
   <td> <p>Projekt<br>Uppgifter<br>Problem<br>Mallar<br>Malluppgifter</p> </td> 
   <td> <p>Klicka för att öppna fliken Uppdateringar för objektet. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">eller <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Anger att objektet har bifogade dokument. </td> 
   <td> Projekt<br>Uppgifter<br>Problem<br>Mallar<br>Malluppgifter </td> 
   <td>Klicka för att öppna fliken Dokument i objektet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">eller <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Anger att det finns öppna problem med projektet eller aktiviteten.</td> 
   <td> Projekt<br>aktiviteter </td> 
   <td>Klicka för att öppna objektet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> eller <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Anger att det finns ett godkännande för objektet.</td> 
   <td> Projekt<br>Uppgifter<br>Problem<br>Mallar<br>Malluppgifter </td> 
   <td>Klicka för att öppna objektet. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="utgifter_ikon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>Du kan lägga till en kolumn för utgiftsikonen i vyn om du vill visa den här ikonen. Detta anger att projektet eller aktiviteten har tillhörande utgifter.</p> </td> 
   <td> <p>Projekt</p> <p>Uppgifter</p> </td> 
   <td>Klicka för att öppna fliken Utgifter för projektet eller uppgiften. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Anger att en uppgifts förloppsstatus är något av följande:</p> 
    <ul> 
     <li>I tid (grön fyrkant)</li> 
     <li>Sena (röd cirkel)</li> 
     <li>Risk (blå romb)</li> 
     <li>Bakom (gul triangel)</li> 
    </ul> <p>Mer information om aktiviteternas förloppsstatus finns i <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Översikt över status för aktivitetsstatus</a>.</p> </td> 
   <td>Uppgifter</td> 
   <td>Klicka för att öppna uppgiften. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> eller <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Anger att aktiviteten finns på den kritiska sökvägen. <br>Mer information om aktiviteter på en kritisk sökväg till projektet finns i <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Översikt över projektets kritiska sökväg</a>.</td> 
   <td>Uppgifter</td> 
   <td>Klicka för att öppna uppgiften.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="millestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Anger att aktiviteten är associerad med en milstolpe. Systemadministratören kan anpassa diamantens färg i din miljö.<br>Mer information om milstolpar finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Skapa en milstolpe</a>.</td> 
   <td>Uppgifter</td> 
   <td>Klicka för att öppna uppgiften. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Länk till ett problems källobjekt. Källobjektet för ett problem är det objekt där problemet loggades. En uppgift eller ett projekt kan vara källobjekt för problem. </td> 
   <td>Problem</td> 
   <td>Klicka för att öppna källobjektet (aktiviteten eller projektet) för ett problem. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Anger att det finns ett objekt som åtgärdar problemet. I det här fallet kan du inte slutföra problemet. Den slutförs när det matchande objektet har slutförts. <br>Mer information om hur du löser objekt finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a> .</td> 
   <td>Problem</td> 
   <td>Klicka för att öppna problemets objekt som åtgärdas. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Visa ett dokument.</td> 
   <td>Dokument</td> 
   <td>Klicka för att hämta dokumentet.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Hämta ett dokument.</td> 
   <td>Dokument</td> 
   <td>Klicka för att hämta dokumentet.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Anger dokumenttypen.</td> 
   <td>Dokument</td> 
   <td>Klicka för att hämta dokumentet.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_tillhör_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Anger att användaren är associerad med ett företag. </td> 
   <td>Användare</td> 
   <td>Otillgänglig</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Anger att användaren är associerad med ett team.</td> 
   <td>Användare</td> 
   <td>Klicka för att öppna användarprofilen.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Kortkommando till fliken Allokering för användaren. </td> 
   <td>Användare</td> 
   <td>Klicka för att öppna fliken Allokering för användaren och se vilka arbetsobjekt användaren är tilldelad.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Anger att användaren befinner sig i en annan tidszon än den i systemet.</td> 
   <td>Användare</td> 
   <td>Otillgänglig</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_cost_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Anger att en utgift är fakturerbar.<br>Mer information om utgifter finns i <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Hantera projektutgifter </a>.</td> 
   <td>Utgifter</td> 
   <td>Otillgänglig</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="kostnad_ersättningsbar_ikon.png" style="width: 44;height: 45;"> </td> 
   <td> Anger att en utgift är återbetalningsbar.<br>Mer information om utgifter finns i <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Hantera projektutgifter </a>.</td> 
   <td>Utgifter</td> 
   <td>Otillgänglig</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="replace_cost_icon.png" style="width: 44;height: 43;"></td> 
   <td> Anger att en utgift har återbetalats.<br>Mer information om utgifter finns i <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Hantera projektutgifter </a>.</td> 
   <td>Utgifter</td> 
   <td>Otillgänglig</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
