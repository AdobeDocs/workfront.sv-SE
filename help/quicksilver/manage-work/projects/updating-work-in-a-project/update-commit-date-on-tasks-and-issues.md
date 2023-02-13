---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera implementeringsdatum för aktiviteter och ärenden
description: Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i Genomför-datumöversikt.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Uppdatera implementeringsdatum för aktiviteter och ärenden

Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Åtkomstkrav

<!--drafted for P&P

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
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Redigera åtkomst till uppgifter och ärenden</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteten eller problemet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du tilldelas uppgiften eller utgåvan som du vill uppdatera implementeringsdatumet för.

## Uppdatera implementeringsdatum för aktiviteter och ärenden

Uppdateringen av implementeringsdatumet är identisk för uppgifter och utgåvor.

1. Gå till en uppgift eller ett ärende som du har tilldelats som **Aktivitetsägare**.

   Mer information om hur du tar reda på vem som är aktivitetsägare för ett problem eller en uppgift finns i avsnittet [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Klicka på Arbete på i huvud för aktiviteten eller utgåvan

   eller

   Klicka **Starta aktivitet** eller **Starta utgåva** om knappen Arbeta med den har anpassats i din miljö för att ange att du nu arbetar med arbetsuppgiften.

   För närvarande gäller samma datum för implementering och planerat slutförandedatum för aktiviteten eller utgåvan.

1. (Valfritt) Om du klickade på Starta uppgift eller Starta problem klickar du på **Ångra** i skärmens nedre vänstra hörn. Bekräftelsedatumet har tagits bort.

   Mer information om hur du ersätter knappen Arbeta med knappen Start finns i  [Ersätta knappen Work On It (Arbeta på) med en Start-knapp](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >Alternativet att ångra markeringen för att starta arbetet är inte tillgängligt när du klickar på **Arbeta på den**.

1. Klicka **Uppdateringar** i den vänstra panelen klickar du på **Starta en ny uppdatering** >**Bekräftelsedatum**

   eller

   Klicka **Uppgiftsinformation** eller **Ärendeinformation** i den vänstra panelen dubbelklickar du **Bekräftelsedatum** och välj ett nytt datum i kalendern och klicka sedan på **Spara ändringar**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   Följande saker händer när du har gjort den här ändringen: 

   * Datum för implementering och planerat slutförandedatum är inte längre detsamma.

      Istället ändras datumet för implementering och det beräknade slutförandedatumet för aktiviteten eller utgåvan.

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Ändringarna sparas automatiskt när du väljer ett nytt datum i uppdateringsområdet.
   * Projektägaren får ett meddelande om att du har föreslagit ett nytt implementeringsdatum för uppgiften eller utgåvan och att du för närvarande kan uppdatera det planerade slutförandedatumet för aktiviteten eller utgåvan så att det matchar det implementeringsdatum du föreslog.

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      Mer information om meddelanden och uppdateringar som utlöses av den här ändringen finns i avsnittet [Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) i artikeln [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
