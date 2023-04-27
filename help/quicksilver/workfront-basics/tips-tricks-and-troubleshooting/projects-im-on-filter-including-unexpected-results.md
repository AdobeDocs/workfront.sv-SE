---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekt jag arbetar med filtrerar inklusive oväntade resultat
description: Läs den här artikeln om du vill felsöka de projekt jag är på, inklusive oväntade resultat.
feature: Get Started with Workfront
author: Nolan
source-git-commit: ba261e5121b4a28f71c58f883c784f4e8d2ada81
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Projekt som jag är på-filter innehåller oväntade resultat

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
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licens</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

The [!UICONTROL **Projekt jag är på**] Filtret innehåller resultat som jag inte förväntar mig, eftersom jag inte är tilldelad eller associerad med dessa projekt.

## Lösning

The [!UICONTROL **Projekt jag är på**] filtret innehåller projekt som innehåller användaren i någon av dess [!UICONTROL **Projektinformation**] fält, inklusive fält som är enkla att missa eller som fyllts i automatiskt, t.ex. [!UICONTROL **Anges av**] eller [!UICONTROL **Sponsorns-ID**]. Det finns två möjliga lösningar för att ta bort oönskade resultat:

1. Kontrollera [!UICONTROL **Projektinformation**] för varje oväntat projekt som ingår i filtret, och ta bort ditt namn från alla fält.

   ELLER

1. Försök med ett liknande filter, som [!UICONTROL **Projekt jag äger**], som endast innehåller projekt som är specifikt tilldelade dig.

Mer information om hur du använder filter i [!DNL Workfront], se [Filteröversikt i [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)