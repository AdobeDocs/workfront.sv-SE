---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Köra en rapport
description: Du kan köra alla rapporter som du har åtkomst till Visa.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# Köra en rapport

Du kan köra alla rapporter som du har åtkomst till Visa.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Köra en rapport

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Rapporter**.

1. Välj bland följande alternativ:

   * **Mina rapporter:** Rapporter som du har skapat.
   * **Delas med mig:** Rapporter som andra användare har delat med dig.
   * **Alla rapporter:** Alla rapporter i systemet som du har tillgång till.

1. Klicka på namnet på rapporten som du vill köra.\
   eller\
   Om rapporten skapades med hjälp av uppmaningar väljer du lämplig information i listrutorna och klickar sedan på **Kör rapport**.\
   Mer information om uppmaningar finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   Innehållet i rapporten visas med en tidsstämpel i rapportens övre högra hörn som innehåller datum, tid och tidszon när rapporten kördes från den användare som körde rapporten.

1. (Valfritt) Klicka på **Ikonen Läs in igen** ![](assets/qs-report-refresh-icon.png) om du vill uppdatera resultaten i en rapport om rapporten har visats i webbläsaren ett tag.

1. (Villkorligt) Om rapporten innehåller filter eller uppmaningar klickar du på **Visa filter och frågor** om du vill visa en lista med filter och uppmaningar som används i den rapport du visar. Om rapporten bara innehåller filter eller endast uppmaningar, **Visa filter** eller **Visa frågor** visas i stället.

   ![Visa filter och uppmaningar](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   Informationen visas under rapportnamnet till vänster på sidan. För uppmaningar är detta information om de uppmaningsval som gjordes när rapporten kördes, enligt beskrivningen i steg 4.

1. Om du använder anpassade uppmaningar visas de inte. Endast systemuppmaningarna visas. Egna filter visas alltid.

## Visa en cachelagrad rapport

Din rapport kan cachelagras om den har visats i webbläsaren ett tag. Du kan tvinga en cachelagrad rapport att läsas in igen när du utför någon av följande åtgärder:

* Redigera rapportinställningarna och spara rapporten.
* Ändra vyn, gruppen eller filtret.
* Klicka på **Ikonen Läs in igen**
Det här alternativet är tillgängligt i det övre högra hörnet på sidan i meddelanderutan som anger när rapporten sparades, eller så är det tillgängligt i det övre högra hörnet av instrumentpanelen som rapporten placeras på. Mer information om hur du läser in instrumentpaneler igen finns i avsnittet Visa instrumentpaneler i artikeln [Kom igång med instrumentpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Gå till flikarna Sammanfattning, Matris eller Diagram för att få åtkomst till alla sidor i rapporten efter den första sidan.
