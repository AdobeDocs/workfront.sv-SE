---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera implementeringsdatum för aktiviteter och ärenden
description: Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i Genomför-datumöversikt.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---


# Uppdatera implementeringsdatum för aktiviteter och ärenden

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Åtkomstkrav

<!--Audited: 01/2024-->

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
   <ul>
   <li><p>Standard för uppgifter</p> </li>
   <li><p>Medarbetare eller högre för problem</p></li>
   </ul>
   <p>eller</p>
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
   <td> <p>Hantera behörigheter för aktiviteten eller problemet</p>
   <p> Du måste ha tilldelats uppgiften eller utgåvan för att kunna uppdatera implementeringsdatumet </p>
    </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   Current:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p>
   <p> You must be assigned to the task or issue to update the commit date </p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Innan du kan redigera implementeringsdatumet för en uppgift eller utgåva måste du tilldelas den uppgift eller utgåva vars implementeringsdatum du måste uppdatera.

## Uppdatera implementeringsdatum för aktiviteter och ärenden


Du kan uppdatera implementeringsdatumet för en uppgift eller ett problem i följande områden i Workfront:

* Avsnittet Information om en uppgift eller ett problem
* Aktivitets- eller utgivningsrubriken

  Din Workfront- eller gruppadministratör måste lägga till implementeringsdatumet i uppgifts- eller utgivningsrubriken i layoutmallen för att kunna visa det från uppgifts- eller utgivningssidan.
Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Uppdateringen av implementeringsdatumet är identisk för uppgifter och utgåvor.

>[!NOTE]
>
>Du kan be din system- eller gruppadministratör att lägga till fältet Genomför datum på panelen Sammanfattning för att göra det enklare att uppdatera det i olika områden av Workfront.
>
>Mer information finns i följande artiklar:
>
>* [Sammanfattningsöversikt](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Anpassa panelen Sammanfattning med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Gå till en aktivitet eller ett problem som du har tilldelats som **ägare**.

   Mer information om hur du tar reda på vem som är aktivitetsägare för ett problem eller en uppgift finns i avsnittet [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Villkorligt och valfritt) Om Workfront- eller gruppadministratören har lagt till implementeringsdatumet i huvud för aktiviteten eller utgåvan klickar du på fältet **Bekräftelsedatum** i huvudet och väljer sedan ett datum i kalendern. Om implementeringsdatumet inte finns i huvudet fortsätter du med följande steg.

   ![Bekräftelsedatum i uppgiftshuvudet](assets/commit-date-task-header.png)

1. Klicka på **Uppgiftsinformation** eller **Ärendeinformation** i den vänstra panelen.
1. Klicka på **Översikt** för att expandera den.
1. Uppdatera fältet **Verkställ datum**.

   ![Redigering av datum för aktivitetens genomförande har markerats på informationssidan](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicka på **Spara ändringar**.

   När du har gjort den här ändringen händer följande:

   * Bekräftelsedatumet och det planerade slutförandedatumet för aktiviteten eller utgåvan är inte längre desamma.

     Istället ändras datumet för implementering och det beräknade slutförandedatumet för aktiviteten eller utgåvan.

     ![Aktivitetens beräknade slutförandedatum i markerade detaljer](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Projektägaren meddelas i ett meddelande från Workfront i appen om att du har föreslagit ett nytt implementeringsdatum för uppgiften eller utgåvan.
   * Projektägaren meddelas i uppdateringsavsnittet att du har föreslagit ett nytt implementeringsdatum och de kan för närvarande uppdatera det planerade slutförandedatumet för aktiviteten eller utgåvan så att det matchar det implementeringsdatum du föreslog.

     ![Meddelande från projektägare i uppdateringsdataström som bekräftar datum påverkar projekttidslinjen](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![Project owner notification in update stream that commit date affects the project timeline](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Mer information om de meddelanden och uppdateringar som utlöses av den här ändringen finns i avsnittet&quot;Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet&quot; i artikeln [Bekräfta datumöversikt](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
