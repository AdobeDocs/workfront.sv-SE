---
product-area: documents
navigation-topic: approvals
title: Översikt över objektbehörigheter och åtkomstnivå för Adobe Enterprise-lagringsmodell
description: Adobe Enterprise-lagringsbehörigheter och åtkomstöversikt
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
source-git-commit: 8b8f638f089ff967fe7d4fb641b23f5836ac86b5
workflow-type: tm+mt
source-wordcount: '851'
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

## Objektbehörigheter

Objektbehörigheterna avgör vad du kan se och göra med projekt, uppgifter, problem och dokument i Workfront. Behörigheter tilldelas när någon delar ett objekt med dig.

>[!IMPORTANT]
>
>I Adobe Enterprise-lagring fungerar dokumentbehörigheter annorlunda än i äldre Workfront-lagring. Dokument ärver behörigheter från det projekt, den uppgift eller det ärende som de är länkade till.


### Hur dokumentbehörigheter fungerar

Dokumentbehörigheter styrs av objektet som dokumentet är länkat till. Du kan inte ange behörigheter för enskilda dokument.

När du överför ett dokument till en uppgift eller ett problem skapas en systemgenererad mapp med hjälp av uppgifts- eller utgivningsnamnet. Den här mappen är länkad till uppgiften eller problemet och ärver dess behörigheter.

Du kan skapa undermappar i den systemgenererade mappen för att ordna dokumenten ytterligare. Alla undermappar ärver behörigheter från den överordnade mappen. På projektnivå kan du överföra dokument utanför en mapp, men bara användare med åtkomst på projektnivå kan se dem.

På projektnivå visar systemgenererade mappar ett länkat objekt. Det här är vanligtvis uppgifts- eller problemnamnet och det är så systemet vet vilken åtgärd eller vilket problem mappen ska ses på.

### Projektbehörigheter

När du har behörighet på projektnivå kan du visa och hantera dokument för det projektet i Workfront och andra Adobe-produkter som Frame.io och Adobe Creative Cloud. Projektnamnet visas också i de verktygen. Andra projektdata visas inte utanför Workfront.

### Aktivitets- och utfärdandebehörigheter

Aktiviteter och ärenden ärver behörigheter från projektet. När du har behörighet på uppgifts- eller utfärdandenivå kan du visa och hantera dokument som är länkade till den uppgiften eller utgåvan i Workfront och andra Adobe-produkter som Frame.io och Adobe Creative Cloud.

**Systemgenererade mappar**

* Mappåtkomst tas inte bort automatiskt om du tar bort användare från en uppgift eller ett problem. De kan fortfarande ha åtkomst via behörigheter på projektnivå.
* Underaktiviteter ärver inte systemgenererade mappbehörigheter från överordnade aktiviteter. Du måste läggas till direkt i en underuppgift för att komma åt den systemgenererade mappen.
* Om du lägger till användare i en uppgift eller utfärdar delningar av objektets systemgenererade mapp med dem.

**Flytta och byta namn på systemgenererade mappar:**

* Systemgenererade mappar kan byta namn och flyttas.
* Om en systemgenererad mapp flyttas till en annan plats, uppdateras dess länkade objekt till det nya objektet. Behörigheterna ärvs sedan från det nya överordnade objektet.

Förfrågningar följer samma beteende som uppgifter och ärenden.

### Godkännanden

När du läggs till i ett arbetsflöde för dokumentgodkännande kan du se följande, oavsett projektbehörigheter:

* Projektnamn
* Dokumentnamn
* Dokumentminiatyr










