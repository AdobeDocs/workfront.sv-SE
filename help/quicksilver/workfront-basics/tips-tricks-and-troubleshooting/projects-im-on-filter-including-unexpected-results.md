---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekt jag arbetar med filtrerar inklusive oväntade resultat
description: Läs den här artikeln om du vill felsöka de projekt jag är på, inklusive oväntade resultat.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# Projekt jag arbetar med har oväntade resultat

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table>
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Prime eller Ultimate</p>
    <p>Arbetsflöde Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-licenser
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Problem

Filtret [!UICONTROL **Projekt som jag är i**] innehåller resultat som jag inte förväntar mig, eftersom jag inte har tilldelats eller associerats med dessa projekt.

## Lösning

Filtret [!UICONTROL **Projekt som jag är i**] innehåller projekt som innehåller användaren i något av dess [!UICONTROL **projektinformationsfält**], inklusive enkelt missade eller automatiskt ifyllda fält som [!UICONTROL **Anges av**] eller [!UICONTROL **Sponsorns-ID**]. Det finns två möjliga lösningar för att ta bort oönskade resultat:

1. Kontrollera [!UICONTROL **projektinformationen**] för varje oväntat projekt som ingår i filtret och ta bort ditt namn från alla fält.

   ELLER

1. Försök med ett liknande filter, till exempel [!UICONTROL **Projekt som jag äger**], som bara innehåller projekt som har tilldelats dig.

Mer information om hur du använder filter i [!DNL Workfront] finns i [Filteröversikt](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
