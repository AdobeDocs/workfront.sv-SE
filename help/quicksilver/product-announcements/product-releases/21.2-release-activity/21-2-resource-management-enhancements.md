---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatering,release
navigation-topic: 2021-2-release-activity
title: 21.2 Förbättrad resurshantering
description: Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i versionsöversikt 21.2.
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 Förbättrad resurshantering

Den här sidan beskriver alla förbättringar av resurshanteringen som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i [21.2 Versionsöversikt](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vyn på månadsnivå i belastningsutjämnaren

För att du ska kunna hantera resurstilldelningen under större tidsperioder har vi nu implementerat en vy på månadsnivå för belastningsutjämnaren. Du kan visa upp till tre månader i taget och uppdatera månatliga resursallokeringar. Före den här ändringen kan du bara visa arbetsbelastningsutjämnaren per dag eller vecka.

Mer information finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Anslutning mellan scenplanering, arbetsbelastningsutjämnare och uppgiftslista

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

För att hjälpa dig med den strategiska planeringen av dina projekt och se till att de är i linje med scenarioplaneringens helhetsprojekt har vi skapat ett nytt område i projektet som visar krav på jobbroll från initiativen samt planerade timmar som beräknas på projektets arbetsobjekt. Det här området är tillgängligt för belastningsutjämnaren på projektnivå samt för uppgiftslistan i den nya Workfront-upplevelsen. I den klassiska upplevelsen är detta bara tillgängligt för projektets belastningsutjämnare.

Mer information finns i följande artiklar:

* [Översikt över avstämning av resursallokeringar mellan projekt och initiativ](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Den här nya funktionen är synlig för alla användare, både i den nya och klassiska Workfront-upplevelsen. Detta är även synligt för kunder som inte har köpt en Workfront Scenario Planner-licens.

## Använd planerade timmar vid beräkning av nettovärden i resursplaneraren

Med en ny inställning i Resursplaneraren kan du använda Planerade timmar när du beräknar nettovärden.

Före den här förbättringen beräknade Workfront nettovärden endast med Budgeterade timmar. Nettovärden visar skillnaden mellan Tillgängliga och Budgeterade eller Planerade timmar, FTE eller Kostnad. Budgeterade timmar är fortfarande standardinställningen vid beräkning av nettovärden.

Mer information finns i [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 12-veckorsvy i arbetsbelastningsutjämnaren

Du kan nu visa upp till 12 veckors information i Utjämning av arbetsbelastning. Före den här förbättringen kan du visa 2,4 och 6 veckors information.

Mer information om hur du visar arbetsbelastningsutjämnaren finns i [Navigera till arbetsbelastningsutjämnaren](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navigera till Utjämning av arbetsbelastning.

## Ändring av hur filtret Jobbroll fungerar i området Ej tilldelat i Utjämning av arbetsbelastning

För att förbättra hur filtret Jobbroll fungerar i Utjämning av arbetsbelastning och för att motsvara användarnas förväntningar har vi ändrat funktionen för filtret i området Ej tilldelat. Nu kan du bara visa de timmar som tilldelats de jobbroller du har angett i filtret.

Före den här förbättringen visades alla timmar som är associerade med arbetsobjekten som tilldelats till jobbrollerna när jobbrollsfiltret tillämpades på området Ej tilldelat.

Mer information om filtrering av information i Utjämning av arbetsbelastning finns i [Hantera filter i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
