---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Felmeddelande i kalendern: "Den här kalendern har visningsrättigheter för en inaktiverad användare."'
description: Läs mer om felmeddelandet "Den här kalendern har visningsrättigheter för en inaktiverad användare".
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Felmeddelande i kalendern: &quot;Den här kalendern har visningsrättigheter för en inaktiverad användare.&quot;

## Åtkomstkrav

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
     <p>Standard</p>
     <p>Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en kalender</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problem

Du får följande fel när du använder en kalender som delas med dig: 

*Den här kalendern har visningsrättigheterna för en inaktiverad användare. Be en administratör att korrigera kalenderbehörigheterna.*

## Orsak

Användaren som har skapat den här kalendern (den ursprungliga ägaren) är en användare som har inaktiverats. 

## Lösning

Du kan lösa detta på följande sätt:

1. Kopiera den ursprungliga kalendern. När du kopierar en kalender blir du ägare till kalendern. Den kopierade kalendern ska visa all information från den ursprungliga kalendern.\
   Mer information om hur du kopierar en kalender finns i [Kopiera en kalenderrapport](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Dela den kopierade kalendern med samma användare som den ursprungliga kalendern. Alla användare bör se samma information i den nya kalendern.
1. (Valfritt och villkorligt) Om du har behörighet att hantera den ursprungliga kalendern tar du bort alla andra användare som kalendern delas med från kalenderdelningsområdet. Detta eliminerar förvirringen hos de användare som försöker visa fel kalender.
