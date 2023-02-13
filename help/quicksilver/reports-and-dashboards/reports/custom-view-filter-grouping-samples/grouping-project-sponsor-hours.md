---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: Projektsponsor för timmar'
description: Den här timgrupperingen organiserar timmar av sponsorn för projektet där timmarna är loggade. Standardgränssnittet för Report Builder för timgrupperingar innehåller ingen mappning till fältet Project Sponsor. Du måste använda gränssnittet Textläge för att komma åt det här fältet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Gruppering: Projektsponsorer i timmar

Den här timgrupperingen organiserar timmar av sponsorn för projektet där timmarna är loggade. Standardgränssnittet för Report Builder för timgrupperingar innehåller ingen mappning till fältet Project Sponsor. Du måste använda gränssnittet Textläge för att komma åt det här fältet.

![hour_report_grouped_by_sponor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

## Åtkomstkrav

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Gruppera efter projektsponsorer i timmar

Så här använder du den här grupperingen:

1. Gå till en lista med timmar.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Klicka **Växla till textläge**.
1. Ta bort texten i **Gruppera din rapport** område.

1. Ersätt texten med följande kod:

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueFormat=HTML<br>textmode=true<br></pre>

1. Klicka **Spara gruppering**.
