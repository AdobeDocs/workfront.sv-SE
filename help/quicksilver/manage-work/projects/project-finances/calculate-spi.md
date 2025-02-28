---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna SPI (Schedule Performance Index)
description: Schemalägg prestandaindex (SPI) beskriver förhållandet mellan det planerade schemat och det faktiska schemat.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Beräkna SPI (Schedule Performance Index)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Schemalägg prestandaindex (SPI) beskriver förhållandet mellan det planerade schemat och det faktiska schemat. Adobe Workfront beräknar SPI på projekt- och uppgiftsnivå. Projektledare granskar den här mätningen för att identifiera om aktiviteter eller projekt håller på att följa upp i förväg eller efter schemat.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Ljus eller högre</p>
   <p>eller</p>
   <p>Aktuell: Granska eller senare</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Visa åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter för projektet med behörighet att visa ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över SPI (Schedule Performance Index)

* [Vad SPI-värdet visar](#what-the-spi-value-shows)
* [Hur Workfront beräknar SPI](#how-workfront-calculates-spi)

### Vad SPI-värdet visar {#what-the-spi-value-shows}

Projektledare är införstådda med att SPI-värdet 1 innebär att projektet är planerat eller tidsplanerat.  Värden större än 1 visar att ett projekt ligger före schemat och värden mindre än 1 innebär att ett projekt ligger efter schemat.  Ju längre bort från 1, desto större avvikelse från planen.

| **SPI-värde** | **Indikation på schemat** |
|---|---|
| 1 | Vid plan eller tidplan |
| > 1 (större än 1) | Före schemat |
| &lt; 1 (mindre än 1) | Efter schema |

{style="table-layout:auto"}

### Hur Workfront beräknar SPI  {#how-workfront-calculates-spi}

Workfront beräknar SPI enligt följande formel:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Om planerade timmar är schemalagda till datum = 0, SPI = 1*.

Planerade timmar Schemalägg till datum beräknas vid den tidpunkt då du utför beräkningarna. Här visas antalet planerade timmar till dagens datum. Den kan beräknas om automatiskt när du ändrar dina finansiella data så att de blir korrekta. Det finns inget fält i Workfront som anger det här värdet.

Om du till exempel har ett projekt med en aktivitet och aktiviteten har 10 planerade timmar och en 10-dagars varaktighet, är schemat för planerade timmar till datum 5 dag. 

## Hitta SPI i ett projekt eller en uppgift

1. Gå till det projekt eller den uppgift där du vill visa SPI.
1. Beroende på om du vill visa SPI för ett projekt eller en uppgift gör du något av följande:

   1. Klicka på **Projektinformation** i den vänstra panelen och visa sedan området **Ekonomi**.

   1. Klicka på **Uppgiftsinformation** i den vänstra panelen och visa sedan området **Ekonomi**.

      ![SPI i projekt](assets/spi-on-project-nwe.png)

1. Hitta fältet **CPI/SPI/CSI**.
