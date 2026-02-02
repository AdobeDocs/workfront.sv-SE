---
product-area: documents
navigation-topic: approvals
title: Översikt över objektbehörigheter och åtkomstnivå för Adobe Enterprise-lagringsmodell
description: Adobe Enterprise-lagringsbehörigheter och åtkomstöversikt
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Översikt över objektbehörigheter och åtkomstnivå för Adobe Enterprise-lagringsmodell

<!--linked in UI -->

Adobe Enterprise-lagring är en molnbaserad lagringslösning som fungerar som central lagringsplats för resurser i Adobe företagsprodukter. Workfront-miljöer som använder Adobe Enterprise-lagring har något annorlunda objektbehörigheter och åtkomstnivåbeteenden än de som använder äldre Workfront-dokumentlagring.

## Åtkomstnivåer

Workfront åtkomstnivåer gäller endast inom Workfront. Projekt- och dokumentbegränsningar i Workfront gäller inte alltid i andra Adobe-program.

### Miljöer som använder både Adobe Enterprise-lagring och Workfront-lagring

Åtkomsten till dokumenten fungerar på olika sätt beroende på om projektet gäller Adobe Enterprise-lagring eller äldre Workfront-lagring:

* **Äldre Workfront-lagring**: Projekt, program, portföljer och mallar som använder äldre Workfront-lagring följer Workfront standardlogik för åtkomstnivå för dokumentåtkomst. När en åtkomstnivå har **Ingen åtkomst** har valts för dokument kan de inte se dokument i Workfront eller andra Adobe-produkter som Frame.io eller Creative Cloud.
* **Adobe Enterprise-lagring**: Projekt, program, portföljer och mallar som använder Adobe Enterprise-lagring följer Adobe Enterprise-lagringsåtkomstnivålogik för andra Adobe-produkter.


   * **Behörigheter för projekt, program, portföljer och mallobjekt**: När **Ingen åtkomst** har valts för projekt, program, portföljer och mallar, men objektet delas med dem, kan användarna inte se objektet i Workfront, men de kan fortfarande visa objektnamnet och tillhörande dokument i andra Adobe-verktyg, som Frame.io och Adobe Creative Cloud.
   * **Dokumentbehörigheter**: När **Ingen åtkomst** har valts för dokument på en åtkomstnivå, kan användare inte se dokument i projekt i Workfront, men de kan fortfarande visa och hantera dokument för projekt som delas med dem i andra Adobe-verktyg, som Frame.io och Adobe Creative Cloud. Detta beror på att dokumentåtkomsten avgörs av behörigheter på projektnivå i Adobe Enterprise-lagring, i stället för enbart Workfront åtkomstnivåer.

Om du har aktiverat Adobe Enterprise-lagring i din Workfront-miljö kan du skapa både Adobe Enterprise-lagringsprojekt och äldre Workfront-lagringsprojekt. I äldre Workfront-lagringsprojekt visas en ikon bredvid projektnamnet, oavsett var det visas i Workfront. Adobe Enterprise-lagringsprojekt har ingen ikon.

![ikon för äldre arbetsfärgrymd bredvid projektnamnet](assets/legacy-project-icon.png)


### Miljöer som endast använder Adobe Enterprise-lagring

Du kan inte ändra dokumentbehörigheter på åtkomstnivå för projekt, program och portföljer som använder Adobe Enterprise-lagring.

Alla åtkomstnivåer har redigeringsåtkomst till dokument. Behörigheter på projektnivå styr dokumentåtkomsten i andra Adobe-verktyg.

Du kan inte begränsa åtkomst till dokumentarv.


### Miljöer som endast använder äldre Workfront-lagring

Inga ändringar av dokumentåtkomstnivåer eller -beteende.


## Projekt

Användare med projektnivåbehörighet kan visa och hantera dokument för projekt i andra Adobe-produkter som Frame.io och Adobe Creative Cloud.

Projektnamn visas även utanför Workfront för ESM-projekt.

Finansiella data är inte synliga utanför Workfront för ESM-projekt.

## Uppgifter och problem

Dokument lagras på projektnivå men kan delas med enskilda uppgifter och ärenden efter behov. Användare med uppgifter och ärenden ärver automatiskt dokumentåtkomst från projektet. Du kan inte ändra deras åtkomstnivå. De har antingen behörighet eller ingen åtkomst.