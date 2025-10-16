---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna budgeterad kostnad för schemalagt arbete (BCWS)
description: BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den mängd aktivitet som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Beräkna budgeterad kostnad för schemalagt arbete (BCWS)

## Översikt över BCWS (Budgeted Cost of Work Scheduled)

BCWS (Budgeted Cost of Work Scheduled) kallas även för Planerat värde och är ett projektresultatmått som representerar den mängd aktivitet som skulle ha slutförts vid den tidpunkt då mätvärdet beräknas.

Adobe Workfront beräknar BCWS (Budgeted Cost of Work Scheduled) för både projekt och aktiviteter.

Tänk på följande när du granskar värdena för BCWS för en uppgift eller ett projekt:

* Workfront beräknar BCWS för en uppgift baserat på din konfiguration för projektets PIM (Performance Index Method).

  Du kan konfigurera projektet för att beräkna PIM med timmar eller kostnad och BCWS beräknas också med samma värden.

  Information om hur du konfigurerar hur BCWS beräknas finns i avsnittet [Konfigurera hur BCWS beräknas](#configure-how-bcws-is-calculated) i den här artikeln.

* Workfront beräknar BCWS för ett projekt genom att lägga till alla BCWS-värden från alla överordnade och enskilda uppgifter i projektet.

  Värden från underordnade uppgifter läggs inte till i projektens BCWS.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till projekt</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för projektet</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera hur BCWS beräknas {#configure-how-bcws-is-calculated}

Du kan konfigurera om BCWS ska beräknas i timmar eller kostnader genom att konfigurera hur PIM (Performance Index Method) för projektet ska beräknas.

1. Gå till ett projekt och klicka på **Projektinformation** i den vänstra panelen.
1. I området **Ekonomi** letar du reda på fältet **Resultatindexmetod** och dubbelklickar på det för att redigera det.

   ![PIM-alternativ](assets/pim-options-hour-cost-based-nwe.png)

1. Välj bland följande alternativ:

   | Alternativ | Hur beräkningen utförs |
   |---|---|
   | Timbaserad | Workfront beräknar BCWS med hjälp av aktiviteternas planerade timmar. |
   | Kostnadsbaserad | Workfront beräknar BCWS med hjälp av aktiviteternas planerade kostnad. |


1. Klicka på **Spara ändringar**.

   BCWS för aktiviteterna i projektet beräknas med hjälp av timmar eller kostnader.

## Beräkna BCWS

Workfront beräknar BCWS (Budgeted Cost of Work Scheduled) för aktiviteter eller projekt med hjälp av följande formler:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

Följande värden används i den här beräkningen:

| Värde som används | Beskrivning av använt värde |
|---|---|
| Planerad procent slutfört | Detta är vad procentandelen slutfört för uppgiften ska vara genom att titta på hur lång tid som förflutit mellan början av uppgiften och idag. |
| Uppgiftsbudget | Detta är värdet för aktivitetens planerade timmar eller planerade kostnad. |

Om det till exempel är den 12 februari i dag och en aktivitet är schemalagd att pågå från den 10 februari till den 20 februari, bör aktiviteten vara 20 % färdig i dag. Om aktivitetsbudgeten (planerad kostnad) är $10 000 är BCWS för aktiviteten:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Hitta BCWS för ett projekt eller en uppgift

Du kan visa värdet för Budgeterad kostnad för arbete som schemalagts i en rapport eller lista genom att lägga till BCWS-kolumnen i vyn.

1. Gå till en lista med uppgifter eller projekt.
1. Expandera menyn **Visa** och välj **Ny vy** eller **Anpassa vy**.

1. Klicka på **Lägg till kolumn**.
1. I **Visa i den här kolumnen:** börjar du skriva **BCWS** och klickar för att markera det när det visas i listan.

   ![BCWS i projektvyn](assets/bcws-in-project-view.png)

1. Klicka på **Spara vy**.
1. Fältet **BCWS** visas i vyn.
