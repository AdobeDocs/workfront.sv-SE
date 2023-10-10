---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden
description: Det planerade slutförandedatumet är en beräknad realtidsindikator för när projektet, aktiviteten eller utgåvan ska slutföras. När projektet, aktiviteten eller utgåvan har markerats som Slutförd ändras det planerade slutförandedatumet till datumet för det faktiska slutförandedatumet.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden

Det planerade slutförandedatumet är en beräknad realtidsindikator för när projektet, aktiviteten eller utgåvan ska slutföras. När projektet, aktiviteten eller utgåvan har markerats som Slutförd ändras det planerade slutförandedatumet till datumet för det faktiska slutförandedatumet.

I följande avsnitt beskrivs hur det planerade slutförandedatumet bestäms för projekt, uppgifter och problem, och hur du hittar det.

## Åtkomstkrav

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
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Granska eller senare om du vill visa det planerade slutförandedatumet i en rapport</p> <p>En planlicens för att skapa en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p> <p>Du måste ha behörighet att redigera rapporter, instrumentpaneler och kalendrar för att skapa en rapport</p> <p>Du måste ha behörighet att redigera filter, vyer och grupperingar för att kunna skapa en rapport eller ändra en listvy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i ett projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Hur Adobe Workfront fastställer det planerade slutförandedatumet

Det planerade slutförandedatumet är ett beräkningsfält och kan inte ändras manuellt.

Vilka kriterier som används för att bestämma det planerade slutförandedatumet varierar beroende på vilket objekt du visar:

* **Projekt:** Det planerade slutförandedatumet för projekt motsvarar det planerade slutförandedatumet för den senaste aktiviteten i projektet.

  Ett högre procentvärde för slutförande flyttar till exempel det planerade slutförandedatumet för aktiviteten närmare den aktuella dagen. Om aktivitetens status är Nytt och aktiviteten Planerat slutförandedatum är nära eller har passerat, flyttas det planerade slutförandedatumet in i framtiden.

* **Uppgifter:** Det planerade slutförandedatumet för uppgifter fastställs utifrån följande kriterier:

   * **Förloppsuppdateringar för uppgiften som utförs av den som tilldelats uppgiften:** Förloppsuppdateringar inkluderar ändringar i procent slutfört och ändringar av aktivitetsstatus.
   * **Bekräftelsedatum:** Om den tilldelade aktiviteten anger ett implementeringsdatum ändras det planerade slutförandedatumet så att det matchar implementeringsdatumet.

     Mer information om implementeringsdatum finns i artikeln [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Föregående:** Om det inte blir några förseningar för föregående aktiviteter ska det planerade slutförandedatumet matcha det planerade slutförandedatumet. När fördröjningar inträffar visar de beroende aktiviteterna ett planerat slutförandedatum som är större än det planerade slutförandedatumet.

     Mer information om planerat slutförandedatum för uppgifter finns i [Översikt över aktivitetens planerade slutförandedatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >När en uppgifts föregångare har ett faktiskt slutförandedatum får de beroende aktiviteterna ett planerat slutförandedatum enligt följande scenario:
  >
  >
  >Om projektet har uppgift A, Aktivitet B och Aktivitet C, och Aktivitet B är efterföljare till Aktivitet A, Aktivitet C är efterföljare till Aktivitet B och ett Faktiskt slutförandedatum läggs till i Aktivitet A, beräknas det planerade slutförandedatumet automatiskt om för Aktivitet B (under förutsättning att **Uppdateringstyp** av projektet är inställt på Automatisk och Vid ändring), men det kommer inte att beräknas om för Aktivitet C. För närvarande beräknar Workfront det planerade slutförandedatumet för aktiviteter som ligger en nivå upp eller ned från den uppdaterade aktiviteten, av prestandaskäl. 

* **Problem:** Utgåvan av planerat slutförandedatum är inledningsvis inställd på att matcha det planerade slutförandedatumet för utleverans.

  Om den som har tilldelats utgåvan anger ett datum för implementeringen ändras både det planerade slutförandedatumet och det planerade slutförandedatumet så att de matchar implementeringsdatumet.

  Mer information om implementeringsdatum finns i artikeln [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Visa planerat slutförandedatum

Du kan visa projektens, aktivitetens och problemens beräknade slutförandedatum i rapporter. Du kan visa det planerade slutförandedatumet för projekt och uppgifter i andra områden av Workfront. 

* [Visa planerat slutförandedatum för ett projekt](#view-the-projected-completion-date-of-a-project)
* [Visa planerat slutförandedatum för en uppgift](#view-the-projected-completion-date-of-a-task)
* [Visa planerat slutförandedatum för ett problem](#view-the-projected-completion-date-of-an-issue)

### Visa planerat slutförandedatum för ett projekt {#view-the-projected-completion-date-of-a-project}

1. Gå till det projekt där du vill visa det planerade slutförandedatumet.
1. Klicka **Projektinformation** till vänster.
1. Leta reda på **Planerat slutförandedatum** fältet i **Ökning** -avsnitt.

### Visa planerat slutförandedatum för en uppgift {#view-the-projected-completion-date-of-a-task}

1. Gå till den uppgift där du vill visa det planerade slutförandedatumet.
1. Klicka **Uppgiftsinformation** till vänster.
1. Leta reda på **Planerat slutförandedatum** fältet i **Ökning** -avsnitt.

### Visa planerat slutförandedatum för ett problem {#view-the-projected-completion-date-of-an-issue}

Du kan bara visa det planerade slutförandedatumet för utgåvor i en problemrapport eller listvy. Att skapa en listvy påminner om att skapa vyn i en rapport.

Så här skapar du en problemrapport som innehåller det planerade slutförandedatumet:

1. Skapa en problemrapport enligt beskrivningen i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Välj **Kolumner (vy)** -fliken.
1. Klicka **Lägg till kolumn** och börja skriva **Planerat slutförandedatum** i **Visa i den här kolumnen:** fält.

1. Markera den när den visas i listan, under **Problem** -objekt. 
1. Klicka **Spara + Stäng**.

   The **Planerat slutförandedatum** kolumnen i rapporten fylls i. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
