---
title: 22.2 Förbättrad resurshantering
description: 22.2 Förbättrad resurshantering
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 2.2 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

den 4 april 2022.

En lista över alla ändringar som är tillgängliga i version 2.2 finns i [22.2 Versionsöversikt](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Förbättringar av navigeringen för belastningsutjämnare för arbetsbelastning

För att förbättra din upplevelse när du använder belastningsutjämnaren har vi infört följande förbättringar:

* Knapparna Avbryt och Spara när du justerar tilldelningar är nu fortfarande kvar, även när uppgiften är längre än den tidsram som finns på skärmen eller när panelen Sammanfattning visas.
* Den vänstra panelen som visar namnen på användare och arbetsobjekt är nu fast så att du kan rulla vågrätt under längre tidsramar och fortfarande kunna läsa namnen på objekten som visas på panelen.
* Du kan komprimera och expandera alla objekt i den vänstra panelen med ett klick i stället för på användar- eller projektnivå.
* Nu går det även att ändra storlek på den vänstra panelen.
* Det finns nu ett helskärmsläge för Utjämning av arbetsbelastning.

Mer information om hur du navigerar i arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Åtkomst till avancerade tilldelningar i arbetsbelastningsutjämnaren

Om du vill göra det enklare och exaktare att tilldela arbetsobjekt kan du nu göra avancerade uppdrag när du tilldelar arbetsobjekt manuellt i Arbetsbelastningsutjämnaren. Före den här förbättringen har du åtkomst till avancerade uppdrag när du redigerar objekt, objektens rubriker eller i listor.

Mer information finns i [Tilldela arbete manuellt med hjälp av Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Ny formel för beräkning av användartillgänglighet när inställningen Standardschema har valts

För att kunna ge mer korrekt information i resurshanteringsverktygen har vi ändrat formeln som Workfront använder för att beräkna användartillgänglighet när Workfront-administratören väljer Standardschema i Resurshanteringsinställningar. I den nya uppdateringen använder Workfront följande formel för att beräkna användartillgänglighet:

Tillgängliga timmar för användare = (standardtimmar för schema - undantag) &#42; FTE - ledig tid

Före den här uppdateringen använde Workfront följande formel för att beräkna användartillgänglighet när Standardschema valdes:

Tillgängliga timmar för användare = (standardtimmar för schema - (schemaundantag + lediga timmar) &#42; Användarens FTE-värde

Mer information finns i [Konfigurera inställningar för resurshantering](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

