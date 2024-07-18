---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Resurshanteringsförbättringar
description: Den här sidan beskriver alla förbättringar av resurshanteringen som ingår i version 2019.1. Funktionerna är nu tillgängliga i produktionsmiljön.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 2019.1 Resurshanteringsförbättringar

Den här sidan beskriver alla förbättringar av resurshanteringen som ingår i version 2019.1. Funktionerna är nu tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2019.1 finns i [Översikt över versionsaktivitet för 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Uppdaterat standardfilter i resursplaneraren

Standardfiltret i resursplaneraren filtreras inte längre av projektgruppen.

När du visar resursplaneraren visas nu bara de projekt som är aktuella och datumkänsliga som standard. Information från följande projekt inkluderas som standard:

* Med ett planerat slutförandedatum som infaller efter dagens första datum i månaden.
* Med ett planerat startdatum som infaller före det sista datumet i den fjärde månaden från idag.
* Med statusen Aktuell eller Planering.

Tidigare hämtade standardfiltret information från följande ytterligare projekt:

* Med ett planerat slutförandedatum som infaller efter dagens första datum i månaden.
* Med ett planerat startdatum som infaller före det sista datumet i den fjärde månaden från idag.
* Med statusen Aktuell eller Planering.
* Med en grupp som matchar hemgruppen för den användare som är inloggad.

Mer information om hur du använder filter i resursplaneraren finns i [Filtrera information i resursplaneraren](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Använda jokertecken för resursplaneringsfilter

Du kan nu använda jokertecken när du skapar filter i resursplaneraren. Du kan till exempel använda $$USER.ID för att filtrera efter information om användaren som är inloggad, eller $$USER.companyID för att filtrera information om alla användare som tillhör samma företag som användaren som är inloggad. En fullständig lista över användarbaserade variabler finns i avsnittet [Användarbaserade jokerteckensfiltervariabler](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) i [Jokerteckensfiltervariabler](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Tidigare var jokertecken inte tillgängliga för resursplaneringsfiltren.

Mer information om filtrering i resursplaneraren finns i [Filtrera information i resursplaneraren](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Stöd för datumbaserade jokerteckensfiltervariabler i resursplaneraren

Du kan nu använda vilken version som helst av jokerteckensfiltervariabeln $$TODAY när du skapar ett filter i resursplaneraren.

Före den här förbättringen kunde du bara använda användarbaserade jokerteckensfiltervariabler.

Mer information om filtrering i resursplaneraren finns i [Filtrera information i resursplaneraren](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Mer information om filtervariabler för jokertecken finns i [Variabler för jokertecken](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Exportalternativ för rollvyn i resursplaneraren

Du kan nu välja vilka informationsnivåer som ska exporteras från resursplaneraren i rollvyn. Du kan exportera följande:

* Endast roller
* Roller och projekt
* Roller, projekt och användare

Före den här förbättringen exporterades alla informationsnivåer i rollvyn. Dessa alternativ har lagts till i projekt- och användarvyerna i en tidigare version.

Mer information om att exportera information från resursplaneraren finns i [Exportera information från resursplaneraren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Dataformateringsalternativ för export av resursplaneraren

Nu kan du välja hur du vill visa information i Excel-filen när den exporteras från resursplaneraren.

Du kan visa tillgänglighet och allokering av information som exporterats från resursplaneraren på följande sätt:

* Delas upp efter namnet på de objekt som den tillhör. I det här fallet visas namnen på de objekt som det hör till på varje datarad. (det här är standardalternativet)
* Grupperad efter namnet på de objekt som den tillhör. I så fall visas informationen i den exporterade filen som den visas i Workfront.

Före den här förbättringen visades informationen i den exporterade filen så som den visas i Workfront.

Mer information om att exportera information från resursplaneraren finns i [Exportera information från resursplaneraren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Tidslinje för beständig schemaläggning

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

När du schemalägger tidslinjer behålls nu den tidsram du har valt när du uppdaterar tidslinjen eller navigerar bort från sidan.

Före den här förbättringen återgick tidslinjerna för schemaläggning till standardtidsramen när du uppdaterade eller navigerade bort från sidan.

Den här förbättringen finns i följande områden:

* Fliken Schemaläggning i området Personer
* Fliken Arbeta i team
* Underfliken Schemaläggning på fliken Anställning i ett projekt

Information om hur du arbetar med tidslinjen i resursplaneringsområdena finns i&quot;Kom igång med resursplanering&quot;.

## Nya exportalternativ i resursplaneraren

Du kan nu välja vilka informationsnivåer som ska exporteras från resursplaneraren. I projektvyn kan du exportera något av följande:

* Endast projekt
* Projekt och roller
* Projekt, roller och användare

I användarvyn kan du exportera något av följande:

* Endast användare
* Användare och projekt
* Användare, projekt, roller, uppgifter och problem

Före den här förbättringen exporterades alla informationsnivåer som standard i alla vyer av resursplaneraren.

Mer information om att exportera information från resursplaneraren finns i [Exportera information från resursplaneraren](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Uppdatera till användarvyn i resursplaneraren

Alla användare i systemet visas nu i användarvyn för resursplaneraren, men endast de användare som är associerade med de filtrerade projekten visar också timinformation.

Före den här uppdateringen är det bara de användare som har tilldelats till arbetsobjekt i de projekt som du filtrerar för som visas i användarvyn i resursplaneraren.

Du kan använda användarbaserade filter för att minska antalet användare som visas i användarvyn till endast de som är tilldelade till de projekt som du vill visa.

Mer information om filter i resursplaneraren finns i [Filtrera information i resursplaneraren](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
