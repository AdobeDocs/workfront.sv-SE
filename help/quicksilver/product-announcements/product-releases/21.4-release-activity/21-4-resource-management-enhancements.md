---
title: 21.4 Förbättrad resurshantering
description: 21.4 Förbättrad resurshantering
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c978e88b-ee07-4af9-b5df-cb62dab4b3ac
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# 21.4 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 21.4 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 4 oktober 2021.

En lista över alla ändringar som är tillgängliga i version 21.4 finns i [21.4 Versionsöversikt](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Gör snabba tilldelningar i Utjämning av arbetsbelastning

Nu kan du effektivt balansera resurser i Utjämning av arbetsbelastning med minsta möjliga klick genom att dra ett objekt från området Ej tilldelat och släppa det på en användares rad i området Tilldelad. Med dra och släpp kan du också ta bort tilldelning av objekt från användare och flytta dem tillbaka till området Ej tilldelade samt flytta dem till andra användare.

Före den här förbättringen kunde du bara tilldela objekt genom att klicka på Mer-menyn för en uppgift eller ett problem och sedan använda alternativet Tilldela. Nu uppdateras de planerade timmarna som tilldelats användaren i realtid medan uppgifterna dras.

Mer information om hur du tilldelar arbetsobjekt i Arbetsbelastningsutjämnaren finns i [Översikt över tilldelning av arbete i belastningsutjämnaren](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Nytt standardalternativ för Utjämning av arbetsbelastning

Som en del av vår strävan att ta bort schemaläggningen och göra Workfront viktigaste resurstilldelningsverktyg för arbetsbelastningsutjämning, har vi gjort Workfront Balancer till standardalternativet för alla nya användare. Schemaläggning är för närvarande standardalternativet. Den här ändringen gäller för alla områden där du kan komma åt Schemaläggning från vilka du kan använda området Resurser (i den nya Adobe Workfront-upplevelsen) eller i området Personer (i Adobe Workfront Classic), samt projekt- och teamnivå.

## Ny filterupplevelse i Utjämning av arbetsbelastning

>[!NOTE]
>
>Den här funktionen släpptes till förhandsvisningsmiljön den 16 september 2021.

Vi har gjort om filterupplevelsen i arbetsbelastningsutjämnaren så att den innehåller följande extra funktioner:

* Enklare och effektivare användargränssnitt som matchar den nya Workfront-upplevelsen
* Ytterligare fält som du kan filtrera efter
* Kan duplicera ett filter
* Dela filter med andra användare

Mer information finns i [Hantera filter i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

>[!NOTE]
>
>Med filteruppdateringarna har vi eliminerat **Alla arbetsobjekt** och **Det här projektets arbetsobjekt** inbyggda filter i ett projekts belastningsutjämnare.

