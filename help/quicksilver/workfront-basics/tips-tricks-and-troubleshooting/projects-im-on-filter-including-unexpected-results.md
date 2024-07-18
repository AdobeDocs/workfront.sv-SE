---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekt jag arbetar med filtrerar inklusive oväntade resultat
description: Läs den här artikeln om du vill felsöka de projekt jag är på, inklusive oväntade resultat.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Projekt jag arbetar med har oväntade resultat

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront]-licens</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Filtret [!UICONTROL **Projekt som jag är i**] innehåller resultat som jag inte förväntar mig, eftersom jag inte har tilldelats eller associerats med dessa projekt.

## Lösning

Filtret [!UICONTROL **Projekt som jag är i**] innehåller projekt som innehåller användaren i något av dess [!UICONTROL **projektinformationsfält**], inklusive enkelt missade eller automatiskt ifyllda fält som [!UICONTROL **Anges av**] eller [!UICONTROL **Sponsorns-ID**]. Det finns två möjliga lösningar för att ta bort oönskade resultat:

1. Kontrollera [!UICONTROL **projektinformationen**] för varje oväntat projekt som ingår i filtret och ta bort ditt namn från alla fält.

   ELLER

1. Försök med ett liknande filter, till exempel [!UICONTROL **Projekt som jag äger**], som bara innehåller projekt som har tilldelats dig.

Mer information om hur du använder filter i [!DNL Workfront] finns i [Filteröversikt](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
