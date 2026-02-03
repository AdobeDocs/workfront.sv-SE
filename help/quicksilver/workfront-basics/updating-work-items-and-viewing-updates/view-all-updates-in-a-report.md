---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visa alla uppdateringar i en anteckningsrapport
description: Om du vill se alla uppdateringar som någon av användarna har angett för ett objekt kan du skapa en anteckningsrapport som visar alla uppdateringar.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Visa alla uppdateringar i en anteckningsrapport

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Under Uppdateringar för ett objekt visas maximalt 200 uppdateringar som standard. Om du vill se alla uppdateringar som någon av användarna har angett för ett objekt kan du skapa en anteckningsrapport som visar alla uppdateringar.

>[!NOTE]
>
>Du kan skapa en rapport för att visa uppdateringar av objekt i Förhandsgranska med journalpostrapporten. Mer information finns i [Rapport om uppdateringsområdet med en journalpostrapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomsten och skapa följande:</p> 
    <ul> 
     <li> <p>Rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Filter, vyer och grupperingar</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för objekten i rapporten</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa en anteckningsrapport

Att skapa en rapport för anteckningar för ett objekt är identiskt, oavsett objektet.

Om du till exempel vill skapa en anteckningsrapport för alla anteckningar i ett projekt:

{{step1-to-reports}}

1. Klicka på **Ny rapport** i det övre vänstra hörnet på sidan och välj sedan **Obs!**.

1. (Valfritt) Klicka på **(Kolumner) Visa** och sedan på **Lägg till kolumn** för att lägga till **namnet** för **projektet** i rapportvyn.

1. (Valfritt) Om du rapporterar flera projekt samtidigt klickar du på **Grupperingar** och sedan på **Lägg till gruppering** för att gruppera efter **namnet** för **projektet**. Detta gör att anteckningarna grupperas efter deras respektive projekt, vilket gör rapporten lättare att läsa.

1. (Valfritt) Klicka på **Filter** och sedan på **Lägg till en filterregel**.
1. Lägg till ett filter för **Obs!** > **Anteckningstext** > **Är inte tom**.

   ![Anteckningstextfältet är inte ett tomt filter](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Om ett projektfält uppdaterades men ingen anteckning lades till vid tidpunkten för uppdateringen, visas **anteckningstexten** för uppdateringen som **(Ingen text har lagts till för uppdatering)**.


1. (Valfritt) Lägg till ett annat filter för **Projekt** > **Namn** > **Lika med** och lägg till ett eller flera projektnamn som du vill visa anteckningar för.
1. Klicka på **Spara + Stäng**. Alla uppdateringar som har angetts i projektet av alla användare med behörighet att visa projektet visas i rapporten.
