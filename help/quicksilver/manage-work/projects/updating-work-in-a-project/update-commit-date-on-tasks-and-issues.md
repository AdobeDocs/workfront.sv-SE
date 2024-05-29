---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera implementeringsdatum för aktiviteter och ärenden
description: Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i Genomför-datumöversikt.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 44073ea242803e28ca00c82811ae2865747d11c3
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Uppdatera implementeringsdatum för aktiviteter och ärenden

{{highlighted-preview}}

Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Åtkomstkrav

<!--Audited: 01/2024-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
   För de nya licenserna:
   <ul>
   <li><p>Standard för uppgifter</p> </li>
   <li><p>Medarbetare eller högre för problem</p></li>
   </ul>
   För aktuella licenser:
<ul>
   <li><p>Arbeta eller högre för uppgifter</p></li> 
   <li><p>Begär eller högre för problem</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och ärenden</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteten eller problemet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Innan du kan redigera implementeringsdatumet för en uppgift eller utgåva måste du tilldelas den uppgift eller utgåva vars implementeringsdatum du måste uppdatera.

## Uppdatera implementeringsdatum för aktiviteter och ärenden


Du kan uppdatera implementeringsdatumet för en uppgift eller ett problem i följande områden i Workfront:

* Avsnittet Information om en uppgift eller ett problem
<!--
* <span class="preview">The task or issue header
   Your Workfront or group administrator must add the Commit Date to the task or issue header of your layout template to view it from the task or issue page. </span>
   For information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). -->

Uppdateringen av implementeringsdatumet är identisk för uppgifter och utgåvor.

>[!NOTE]
>
>Du kan be din system- eller gruppadministratör att lägga till fältet Genomför datum på panelen Sammanfattning för att göra det enklare att uppdatera det i olika områden av Workfront.
>
>Mer information finns i följande artiklar:
>
>* [Sammanfattning](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Anpassa hem och sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Gå till en uppgift eller ett ärende som du har tilldelats som **Ägare**.

   Mer information om hur du tar reda på vem som är aktivitetsägare för ett problem eller en uppgift finns i avsnittet [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--1. <span class="preview">(Conditional and optional) If your Workfront or group administrator added the Commit Date to your task or issue header, click the **Commit Date** field in the header, then select a date from the calendar. If the Commit Date is not in the header, proceed with the following steps. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>-->

1. Klicka **Uppgiftsinformation** eller **Ärendeinformation** till vänster.
1. Klicka **Ökning** för att utöka den.
1. Uppdatera **Bekräftelsedatum** fält.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicka **Spara ändringar**.

   När du har gjort den här ändringen händer följande: 

   * Bekräftelsedatumet och det planerade slutförandedatumet för aktiviteten eller utgåvan är inte längre desamma.

     Istället ändras datumet för implementering och det beräknade slutförandedatumet för aktiviteten eller utgåvan.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Projektägaren meddelas i ett meddelande från Workfront i appen om att du har föreslagit ett nytt implementeringsdatum för uppgiften eller utgåvan.
   <!--* The Project Owner is notified in the Updates section that you have suggested a new Commit Date and they can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. This functionality is not supported in the new commenting experience. For information, see [The new commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). -->

   <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

   Mer information om de meddelanden och uppdateringar som utlöses av den här ändringen finns i avsnittet&quot;Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet&quot; i artikeln [Genomför datumöversikt](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->