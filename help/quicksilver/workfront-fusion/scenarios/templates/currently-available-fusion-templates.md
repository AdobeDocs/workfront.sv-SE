---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Tillgängliga Adobe Workfront Fusion-mallar
description: Följande offentliga mallar är för närvarande tillgängliga i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: b397e93842db742456f374a0baf130495b711a2c
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Tillgängliga Adobe Workfront Fusion-mallar

Följande offentliga mallar är för närvarande tillgängliga i Adobe Workfront Fusion.

Teamet eller organisationen kan ha andra mallar som skapats av team tillgängliga.

Om du vill visa tillgängliga mallar klickar du på **Mallar** icon ![](assets/fusion-template-icon.png) i sidnavigeringsmenyn.

## Workfront-mallar

Mallarna automatiserar Workfront processer och arbetsflöden.

### Workfront - konvertera godkänt problem till projekt

Den här mallen konverterar ärenden till projekt. Du kan ändra den så att den uppfyller organisationens standarder.

### Skräddarsytt meddelande baserat på fältändring

Den här mallen skapar anpassade uppdateringar (och relaterade meddelanden) till personer som arbetar med ett Workfront-projekt baserat på en unik händelse, till exempel en ändring av ett fältvärde. Scenariot söker efter Workfront när ett angivet fält ändras i en aktivitet eller ett problem. När ett scenario påträffas utvärderas information i det relaterade projektet och en skräddarsydd uppdatering skapas för en person som tilldelats en specifik roll i projektet.

### Workfront - Bifoga gruppvis till projektnamn med vedertagen standard

Den här mallen för massuppdatering byter namn på alla projekt som uppfyller villkoren i en sökning (ingår i en portfölj) och byter namn på dem till ett standardformat.

### Workfront - Byt namn på projekt enligt konvention

I den här mallen hittas alla projekt som uppfyller villkoren för ett filter (ingår i en portfölj) och namnet på dem ändras till ett standardformat.

### Workfront - Skapa baslinje vid statusändring

Den här mallen hämtar en projektbaslinje vid alla projektstatusändringar som noterats i switchmodulerna och skapar en uppdatering i uppdateringsströmmen för loggning.

### Workfront - Skapa baslinjer varje vecka

Den här mallen hämtar en projektbaslinje varje måndag kl. 6.00 (ET) för projekt som filtreras efter portfölj och skapar en uppdatering i uppdateringsflödet för loggning.

## Workfront - Workfront korrekturmallar

Mallarna automatiserar arbetsflöden som kombinerar Workfront med Workfront Proof.

### Workfront Proof > Workfront - Project Update on Proof Decision

När ett beslut fattas om ett korrektur som läggs till direkt i ett projekt, samlar denna automatisering in information om bevisbeslutet, t.ex. vem som har fattat beslutet, och speglar sedan denna utveckling i motsvarande Workfront-projekt som en uppdatering.

### Workfront-korrektur > Workfront - Uppgiftsuppdatering och slutförande (om godkänt) på korrekturbeslut

Om enskilda korrektur är knutna till enskilda uppgifter stängs den tillhörande uppgiften när ett beslut om godkännande av korrekturet fattas. Om det godkänns slutförs uppgiften och projektet uppdateras.

## HTTP - Workfront-mallar

Mallarna hämtar information från en webbtjänst och hämtar informationen till Workfront.

>[!NOTE]
>
> Du måste ha en licens för Workfront Fusion for Work Automation och Integration för att kunna använda mallarna i det här avsnittet.

### APILayer > Workfront - Daily Exchange Rate Update (EUR)

Den här mallen skapar ett scenario som automatiserar uppdateringen av en valutakurs vid en viss tidpunkt. I det här scenariot hämtas priset euro (EUR) till USD från APIlayers.com och frekvensen uppdateras i Workfront.

## Workfront-Anaplan-mallar

Dessa mallar stöder integreringen mellan Workfront och Anaplan och förväntar sig en specifik konfiguration i båda Anaplan i Workfront. Mer information om de här mallarna och deras konfigurationer finns i artiklarna för de enskilda mallarna.

Mer information om integrationen mellan Workfront och Anaplan finns i [Adobe Workfront med Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> Du måste ha en licens för Workfront Fusion for Work Automation och Integration för att kunna använda mallarna i det här avsnittet.

### Arbetsflöden för utgiftsoptimering

* [Skicka [!DNL Adobe Workfront] projektuppdateringar till [!DNL Anaplan] listobjekt](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [Skicka [!DNL Adobe Workfront] utgifter för [!DNL Anaplan] listobjekt](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [Skicka [!DNL Adobe Workfront] faktiskt antal timmars uppdateringar av en [!DNL Anaplan] listobjekt](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### Arbetsflöden för länkning av budgetbegäranden

* [Skapa en [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] budgetförfrågan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Använd en [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] projekt](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### Arbetsflöden för att länka kampanjförfrågningar

* [Skapa en [!DNL Anaplan] listobjekt från en [!DNL Adobe Workfront] kampanjförfrågan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Använd en [!DNL Anaplan] budgetallokering till en [!DNL Adobe Workfront] kampanjförfrågan eller kampanjprojekt](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
