---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Tillgängliga Adobe Workfront Fusion-mallar
description: Följande offentliga mallar är för närvarande tillgängliga i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: 3897606db8a80d04a3b8d8f0cba69365ceb86c17
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Tillgängliga Adobe Workfront Fusion-mallar

Följande offentliga mallar är för närvarande tillgängliga i Adobe Workfront Fusion.

Teamet eller organisationen kan ha andra mallar som skapats av team tillgängliga.

Om du vill visa tillgängliga mallar klickar du på **Mallar** icon ![](assets/fusion-template-icon.png) i navigeringsmenyn i Fusion.

## Workfront-mallar

Mallarna automatiserar Workfront processer och arbetsflöden.

### Workfront - Kopiera programanpassade Forms- och fältdata till associerade nya projekt

Den här automatiseringen söker efter nya projekt i program med anpassade formulär. Sedan läggs dessa anpassade formulär och fält till i de nya projekten.

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

### Sök efter projektmallar som inte används i principtid och meddela

Granska dina projektmallar en gång i månaden med hjälp av din egen policy med den här enkla mallen som meddelar lämpliga användare om mallar i strid med din policy.

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

## Workfront-Marketo-mallar

Mallarna stöder integrering mellan Workfront och Marketo.

>[!NOTE]
>
> Du måste ha en licens för Workfront Fusion for Work Automation och Integration för att kunna använda mallarna i det här avsnittet.

### Godkänn e-postutkastet från Marketo Engage med Workfront arbetsflöden för godkännande

Detta ingår i integreringen mellan Workfront och Marketo Engage för granskning och godkännande. Den här mallen identifierar om ett e-postkorrektur i Workfront har godkänts och uppdaterar sedan motsvarande e-postmeddelande i Marketo Engage som godkänt.

### Ta emot förfrågningar från marknadsföringskampanjer i Workfront och automatisera framtagningen av kampanjer i Marketo Engage

Detta scenario är ett programmatiskt sätt att skapa e-post- och webbinarikampanjer i Marketo Engage utifrån en begäran som gjorts i Workfront. Genom att använda automatisering för att skapa, organisera och konfigurera kampanjer kan teamen förbättra effektiviteten.

### Granska ett e-postkorrektur av ditt e-postutkast från Marketo Engage i Workfront

Den här mallen identifierar om en Workfront-uppgift har ställts in på en granskningsstatus och exporterar sedan e-postutkastet från Marketo Engage för att spara det som ett korrektur i Workfront.

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
