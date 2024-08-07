---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Projektförbättringar
description: Den här sidan beskriver alla förbättringar som gjorts i Project med version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 2020.1 Projektförbättringar

Den här sidan beskriver alla förbättringar som gjorts i Project med version 2020.1. Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön i slutet av mars eller början av april 2020.

En lista över alla ändringar som är tillgängliga i version 2020.1 finns i [2020.1 versionsöversikt](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Se enklare vilka som är taggade i en uppdatering

Det är nu enklare att se vilka användare som är taggade i en uppdatering. Det taggade användarnamnet visas i blått och länkar till användarprofilen.

Taggade användare visas också i kommentarsrutan.

Före den här förbättringen visades inte de användare som tidigare taggats i rutan Meddela.

Mer information finns i [Tagga andra om uppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inkludera och identifiera citerad text i en uppdateringskommentar eller svar

När du skriver en kommentar kan du markera en del av kommentaren som citerad text för att skilja den från din egen kommentar. Använd knappen Blockcitat i HTML-redigeraren.

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citera en tidigare kommentar i en uppdateringskommentar eller svar

När du kommenterar i en uppdateringstråd kan du snabbt ta med text från en tidigare kommentar i kopplingen. Leta efter alternativet Offertsvar på menyn Mer bredvid kommentaren som du vill citera.

Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Ytterligare riskinformation

För att du bättre ska kunna förstå riskerna med dina projekt kan du nu se vilka och när en risk angavs och när den uppdaterades i ett projekt. Du kan få tillgång till den här informationen i en riskvy och via det offentliga Workfront-API:t. Dessa fält är tillgängliga med API-version 11, som släpps med 2020.1 Production.

Mer information om risker i Workfront finns i [Skapa och redigera risker i projekt](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Ytterligare fält har lagts till för baslinjer och baslinjeaktiviteter

För att du bättre ska kunna förstå de ekonomiska framstegen i dina projekt kan du nu inkludera ytterligare kostnads- och intäktsinformation i en baslinje- eller en baslinjeaktivitetsrapport. Den ytterligare ekonomiska informationen läggs inte till i de baslinjer som du har sparat, men den läggs till för nya baslinjer.

Mer information om ekonomiska fält för projekt och aktiviteter som är tillgängliga från objekten Baslinje och Originalaktivitet finns i [Projektfinanser ingår i projektbaslinjer](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Problem med statusen&quot;Avslutade-väntande godkännande&quot; anses vara ofullständiga

Hur Workfront hanterar problem i statusen&quot;Slutför väntande godkännande&quot; har ändrats. Nu uppfattas dessa problem som öppna och projektet kan inte markeras som fullständigt förrän godkännandet är löst.

Före den här ändringen beaktades stängda problem i statusen&quot;Avslutade godkännande&quot;.

Alla problem som har placerats i en stängd - Väntande godkännandestatus före den här ändringen fungerar på samma sätt som tidigare, anses vara slutförda och gör att projektet även kan slutföras. Alla problem som har placerats i den här statusen efter den här ändringen kommer att betraktas som ofullständiga.

Mer information om projektstatus finns i [Åtkomst till listan över systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

