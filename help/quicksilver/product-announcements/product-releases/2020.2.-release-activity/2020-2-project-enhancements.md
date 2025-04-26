---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Projektförbättringar
description: Den här sidan beskriver alla projektförbättringar som gjorts med 2020.2-utgåvan till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts med 2020.2-utgåvan till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.

En lista över alla ändringar som är tillgängliga i version 2020.2 finns i [2020.2 versionsöversikt](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## För Workfront-administratörer: Ny felsäker när projektstatusen för nya projekt är dold eller olåst

Under Konfigurera konfigurerar du en inställning som ser till att alla nya projekt har en viss status när projektet skapas. Detta är viktigt eftersom ett projekt alltid behöver en status för att fungera korrekt i Workfront, även när projektet är helt nytt.

För att säkerställa att nya projekt alltid har en status, även om en administratör döljer eller låser upp statusen som konfigurerats för nya projekt, tilldelar systemet nu den första statusen i statuslistan till alla nya projekt tills du konfigurerar den nya statusen för nya projekt igen.

Mer information om hur du anger inställningar för status för alla nya projekt finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (eller om du använder Adobe Workfront Classic, se [Ange projektinställningar](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## För Workfront-administratörer: Förbättrad design i projektinställningarna

Upplevelsen av att ange projektinställningar är nu mer intuitiv och lättanvänd:

* Titlar är större än alternativetiketter så du hittar det du söker snabbare.
* Genom att dela upp linjer och extra tomt utrymme separeras varje avsnitt så att du enklare kan fokusera på det du gör.
* Om du anger ett ogiltigt nummer för ett alternativ som&quot;Normalt antal timmar per arbetsdag&quot; visas ett varningsmeddelande omedelbart i stället för att visas när du klickar på Spara.
* Alternativetiketter matchar motsvarande gränssnittstext någon annanstans i Workfront, t.ex. området Detaljer och rapporterna.

Mer information om området Projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (eller om du använder Adobe Workfront Classic, se [Ange projektinställningar](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Markerat filter, vy och gruppering som finns i rapportlistor

Nu väljs det senaste filtret, vyn eller grupperingen som tillämpats på en viss rapport, även om användaren loggar ut och in på Workfront igen.

Tidigare, när en användare tillämpade ett filter, en vy eller en gruppering på en rapportlista och sedan navigerade bort från den sidan, visades standardfiltret, vyn eller grupperingen nästa gång användaren navigerade till samma rapport.

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront
* Adobe Workfront Classic

## När du flyttar och kopierar uppgifter till ett annat projekt behålls uppgiftsbegränsningen när uppgifterna får plats inom projektets tidslinje

Vi har förbättrat sättet som Workfront hanterar den datumspecifika uppgiftsbegränsningen för en uppgift när du kopierar uppgiften eller flyttar den till ett annat projekt. Exempel på datumspecifika aktivitetsbegränsningar är Måste starta, Måste sluta på, Fasta datum, Starta inte senare än och så vidare.

Om du till exempel flyttar eller kopierar en uppgift med en must Start On-begränsning till ett annat projekt vars planerade startdatum är före startdatumet för aktiviteten, behåller aktiviteten villkoret när den har kopierats eller flyttats. När du flyttar eller kopierar en uppgift med en must Start On-begränsning till ett projekt vars planerade startdatum är efter startdatumet för aktiviteten, ändras aktivitetsbegränsningen till Så snart som möjligt.

Före den här ändringen ändras alltid aktivitetsbegränsningen till Så snart som möjligt.

Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md) (eller om du använder Adobe Workfront Classic, se [Flytta uppgifter](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

Information om hur du kopierar uppgifter finns i [Kopiera och duplicera uppgifter](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (eller om du använder Adobe Workfront Classic, se [Kopiera och duplicera uppgifter](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

En översikt över alla aktivitetsbegränsningar finns i [Översikt över aktivitetsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (eller om du använder Adobe Workfront Classic, se [Översikt över aktivitetsbegränsning](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Förhindra dataförlust vid ändringar på fliken Detaljer eller i en uppgiftslista

För att förhindra dataförlust när du uppdaterar information på detaljsidan för ett objekt eller uppgifter i en uppgiftslista på projektnivå när du sparar ändringar manuellt, visas ett varningsmeddelande som meddelar dig om att du har osparade ändringar innan du försöker redigera information i rubriken. De enda åtgärder som är tillåtna innan du sparar ändringarna är att prenumerera eller lägga till objektet i dina favoriter.

Mer information om hur du redigerar uppgifter i en lista finns i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront

