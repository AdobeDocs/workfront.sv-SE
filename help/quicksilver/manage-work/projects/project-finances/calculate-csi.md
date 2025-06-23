---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna prestanda för kostnadsschema (CSI)
description: CSI (Cost Schedule Performance Index) är en automatisk beräkning som kombinerar kostnadsprestandaindexet (CPI) och SPI (Schedule Performance Index) till ett allmänt mått som balanserar kostnad och schema.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Beräkna prestanda för kostnadsschema (CSI)

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Översikt över CSI (Cost Schedule Performance Index)

CSI (Cost Schedule Performance Index) är en automatisk beräkning som kombinerar kostnadsprestandaindexet (CPI) och SPI (Schedule Performance Index) till ett allmänt mått som balanserar kostnad och schema. Genom att multiplicera dessa värden tillsammans kan ett enda mätvärde ta hänsyn till ett långsamt schema till en lägre budget eller vice versa. Projektledare kan använda detta för att fastställa den allmänna statusen för projekt eller uppgifter när kostnaden har offrats för att driva schemat efter projektet.

>[!TIP]
>
>Adobe Workfront beräknar CSI för både uppgifter och projekt, men inte för problem.

Du kan bara dra nytta av informationen i det här måttet om följande scenarier finns i din organisation:

* Dina användare loggar in på det arbete de utför. Detta beräknar CSI baserat på timmar.
* Dina användare eller jobbroller har associerade kostnader per timme. Detta beräknar CSI baserat på kostnader.

## Hur Workfront beräknar prestandaindex för kostnadsschema (CSI)

Workfront beräknar kostnadsprestandaindex (CSI) för ett projekt eller en uppgift med följande formel:

`CSI = CPI x SPI`

Mer information om CPI finns i artikeln [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Mer information om SPI finns i artikeln [Beräkna SPI (Schedule Performance Index)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI har följande tre möjliga värden:

* 1 = Följer den övergripande planen
* \>1 = Kombination av budgetplan
* &lt;1 = Kombination av överbudgeterat schema

![CSI](assets/csi-highlighted.png)

## Leta reda på CSI (Cost Schedule Performance Index)

>[!CAUTION]
>
>Du måste ha tillgång till Visa ekonomiska data på din åtkomstnivå och behörigheter för att visa projektet eller uppgiften för att kunna se CSI-värdet för ett projekt eller en uppgift.

Du hittar CSI i följande områden i Workfront:

* Finansieringsområdet i avsnittet Projektinformation.
* Ekonomi i avsnittet Uppgiftsinformation.
* Ett projekt eller en uppgiftsvy.
* Ett projekt eller en uppgiftsrapport.
