---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna budgeterad kostnad för utfört arbete (BCWP)
description: BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar det belopp som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas.
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Beräkna budgeterad kostnad för utfört arbete (BCWP)

## Översikt över budgeterad kostnad för utfört arbete (BCWP)

BCWP (Budgeted Cost of Work Performed) kallas även för Earned Value och är ett projektresultatmått som representerar det belopp som faktiskt har slutförts vid den tidpunkt då mätvärdet beräknas.

Adobe Workfront beräknar BCWP (Budgeted Cost of Work Performed) för både projekt och uppgifter.

Tänk på följande när du granskar värdena för BCWP för en uppgift eller ett projekt:

* Workfront beräknar BCWP för en uppgift baserat på din konfiguration för projektets PMI (Performance Index Method).

   Du kan konfigurera projektet för att beräkna PMI med timmar eller kostnad och BCWP beräknas även med samma värden.

   Information om hur du konfigurerar hur BCWP beräknas finns i avsnittet [Konfigurera hur BCWP beräknas](#configure-how-bcwp-is-calculated) i den här artikeln.

* Workfront beräknar BCWP för ett projekt genom att lägga till alla BCWP-värden från alla överordnade och enskilda uppgifter i projektet.

   Värdena från underordnade uppgifter läggs inte till i projektets BCWP.

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
   <td> <p>Redigera åtkomst till projekt</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera hur BCWP beräknas {#configure-how-bcwp-is-calculated}

Du kan konfigurera om BCWP ska beräknas i timmar eller kostnader genom att konfigurera hur PIM (Performance Index Method) för projektet ska beräknas.

1. Gå till ett projekt och expandera **Projektinformation** i den vänstra panelen.
1. I **Ekonomi** område, leta reda på **Resultatindexmetod** och dubbelklicka för att redigera det.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Välj bland följande alternativ:

   | Alternativ | Hur beräkningen utförs |
   |---|---|
   | Timbaserad | Workfront beräknar BCWP med hjälp av aktiviteternas planerade timmar. |
   | Kostnadsbaserad | Workfront beräknar BCWP med hjälp av uppgiftens planerade kostnad. |

1. Klicka **Spara ändringar**.

BCWP för projektets uppgifter beräknas utifrån timmar eller kostnader.

## Beräkna BCWP

Workfront beräknar BCWP (Budgeted Cost of Work Performed) för en uppgift eller ett projekt med hjälp av följande formler:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

Följande värden används i beräkningen:

| Värde som används | Beskrivning av det använda värdet |
|---|---|
| Faktisk procent slutfört | Detta är den faktiska procentandelen färdigt arbete som det visas i Workfront. |
| Uppgiftsbudget | Detta är värdet för aktivitetens planerade timmar eller planerade kostnad. |

Om till exempel den faktiska procentandelen slutfört för aktiviteten är 25 % och aktivitetsbudgeten eller den planerade kostnaden är 10 000 USD, är BCWP för aktiviteten:

```
BCWP = 25% x $10,000 = $2,500
```

## Hitta BCWP för ett projekt eller en uppgift

Du kan visa värdet för Budgeterad kostnad för arbete som utförts i en rapport eller lista genom att lägga till BCWP-kolumnen i vyn.

1. Gå till en lista med uppgifter eller projekt.
1. Expandera **Visa** meny och välj **Ny vy** eller **Anpassa vy**.

1. Klicka **Lägg till kolumn**.
1. I **Visa i den här kolumnen:** fältstart skriva **BCWP** och klicka för att markera den när den visas i listan.

   ![](assets/bcwp-project-view.png)

1. Klicka **Spara vy**.
1. BCWP-fältet visas i vyn.
