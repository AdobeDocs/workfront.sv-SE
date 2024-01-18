---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera implementeringsdatum för aktiviteter och ärenden
description: Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i Genomför-datumöversikt.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Uppdatera implementeringsdatum för aktiviteter och ärenden

Du kan uppdatera implementeringsdatumet för en uppgift eller ett ärende som du har tilldelats manuellt. Mer information om implementeringsdatum i Adobe Workfront finns i [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Åtkomstkrav

<!--Audited: 01/2024-->

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

Innan du börjar måste du tilldelas uppgiften eller utgåvan som du vill uppdatera implementeringsdatumet för.

## Uppdatera implementeringsdatum för aktiviteter och ärenden

Uppdateringen av implementeringsdatumet är identisk för uppgifter och utgåvor.

1. Gå till en uppgift eller ett ärende som du har tilldelats som **Ägare**.

   Mer information om hur du tar reda på vem som är aktivitetsägare för ett problem eller en uppgift finns i avsnittet [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Klicka **Uppgiftsinformation** eller **Ärendeinformation** till vänster.
1. Klicka **Ökning** för att utöka den.
1. Uppdatera **Bekräftelsedatum** fält.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicka **Spara ändringar**.

   När du har gjort den här ändringen händer följande: 

   * Bekräftelsedatumet och det planerade slutförandedatumet för aktiviteten eller utgåvan är inte längre desamma.

     Istället ändras datumet för implementering och det beräknade slutförandedatumet för aktiviteten eller utgåvan.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Om du använder det gamla uppdateringsområdet får projektägaren ett meddelande om att du har föreslagit ett nytt implementeringsdatum för aktiviteten eller utgåvan och kan för närvarande uppdatera det planerade slutförandedatumet för aktiviteten eller utgåvan så att det matchar det implementeringsdatum du föreslog. Den här funktionen stöds inte i den nya kommenteringsfunktionen. Mer information finns i [Den nya kommentarsfunktionen](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Mer information om meddelanden och uppdateringar som utlöses av den här ändringen finns i avsnittet [Meddelanden och uppdateringar som utlöses av ändring av implementeringsdatumet](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) i artikeln [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
