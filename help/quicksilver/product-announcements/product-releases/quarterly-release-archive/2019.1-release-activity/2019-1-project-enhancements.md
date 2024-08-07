---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Projektförbättringar
description: Den här sidan beskriver alla projektförbättringar som ingår i version 2019.1. Funktionen är för närvarande tillgänglig i förhandsvisningsmiljön. Den kommer att göras tillgänglig i produktionsmiljön i .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# 2019.1 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som ingår i version 2019.1. Funktionen är för närvarande tillgänglig i förhandsvisningsmiljön. Den kommer att göras tillgänglig i produktionsmiljön i .

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2019.1 finns i&quot;Översikt över versionsaktivitet 2019.1&quot;.

**För administratörer**

* [Återställ mallar från papperskorgen](#restore-templates-from-the-recycle-bin)
* [Visa tidsstämplar för datumfält i Hem](#show-timestamps-for-date-fields-in-home)
* [Alla varaktighetstyper som är tillgängliga under Projektinställningar](#all-duration-types-available-under-project-preferences)

**För alla användare**

* [Agile Improvements](#agile-improvements)
* [Lägg till aktiviteter och ärenden från en lista till en iteration](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Nya pappersstorlekar för Gantt-diagramexport](#new-paper-sizes-for-gantt-chart-export)
* [Åtkomst till dialogrutor i Gantt-schemat i redigeringsläge har tagits bort](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Visa aktivitetsinformation i Gantt-schemat för projektlistan i ett program eller Portfolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Öppna Gantt-schemat för uppgiftslistan i mallar](#access-the-task-list-gantt-chart-on-templates)
* [Bytt namn på projektvyn i Gantt-schemat](#renamed-the-project-view-on-the-gantt-chart)
* [What-If-scenarier i Gantt-schemat för aktivitetslista](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Förbättringar av uppgiftslistan](#task-list-improvements)
* [Visa listor i helskärmsläge](#display-lists-in-full-screen)
* [Nya listor i ytterligare områden](#new-lists-in-additional-areas)
* [Skicka en rapport i XLSX-format](#send-a-delivered-report-in-xlsx-format)
* [Exportera granskningsloggar](#export-audit-logs)

## Återställ mallar från papperskorgen {#restore-templates-from-the-recycle-bin}

Workfront-administratörer kan nu återställa mallar från papperskorgen. Precis som för andra borttagna objekt kan du återställa en mall upp till 30 dagar från den tidpunkt då den togs bort.

Mer information finns i&quot;Återställer borttagna objekt&quot;.

## Visa tidsstämplar för datumfält i hemmet {#show-timestamps-for-date-fields-in-home}

Som Workfront-administratör kan du nu välja att visa eller dölja tidsstämplar för förfallodatum i arbetslistan och kalendern med hjälp av layoutmallar. Som standard är tidsstämplar synliga för både mallanvändare och icke-mallanvändare.

Mer information finns i&quot;Anpassa hemområdet&quot; i artikeln&quot;Skapa och hantera layoutmallar&quot;.

## Alla varaktighetstyper som är tillgängliga under Projektinställningar {#all-duration-types-available-under-project-preferences}

När du ställer in standarduppgiften och varaktighetstypen för utleverans i Inställningar > Projektinställningar kan du använda något av följande alternativ:

Enkel

Ansträngningsstyrd

Beräknad tilldelning

Beräknat arbete

Tidigare gick det inte att välja Beräknat uppdrag och Beräknat arbete om du angav Simple eller Effort Driven som standardvaraktighetstyp.

Mer information om hur du anger standardinställningar för aktivitets- och problemvaraktighet finns i Inställningar för aktiviteter och ärenden

## Flexibla förbättringar {#agile-improvements}

Följande förbättringar är nu tillgängliga i Agile-verktyget:

Kanban

Lägg till uppgifter och utgåvor till en Kanban-tavla från en uppgiftslista eller rapport.

Tidigare kunde du bara lägga till aktiviteter till Kanban-tavlan från efterloggen. Du kunde inte lägga till problem.

Filtrera Kanban-tavlan efter enskilda användare i teamet.

Mer information finns i&quot;Använda Kanban-styrelsen&quot;.

Visa och hantera problem i Kanban-eftersläpningen.

Mer information finns i Använda Kanban-styrelsen.

Tidigare kunde du inte lägga till eller hantera utgåvor på en Kanban-styrelse.

Scrum

Filtrera artikelpanelen efter enskilda användare i teamet.

Mer information finns i&quot;Using the Scrum Agile Story Board&quot;.

Tidigare gick det inte att filtrera efter användare på Kanban- eller trumtavlor.

## Lägg till uppgifter och ärenden från en lista till en iteration {#add-tasks-and-issues-from-a-list-to-an-iteration}

Du kan nu använda en uppgift eller en problemlista, en rapport eller en kontrollpanel för att lägga till artiklar i en iteration. Du kan också ha flera team tilldelade artiklar på en gång.

Tidigare kunde du bara lägga till en artikel i en iteration från sidan med uppgifter eller ärenden, och du kunde bara lägga till artiklar i iterationer som skapats av ditt team.

Mer information finns i&quot;Skapa och hantera Agile-iterationer&quot;.

## Skicka en levererad rapport i XLSX-format {#send-a-delivered-report-in-xlsx-format}

Nu kan du schemalägga en rapport som ska levereras i MS Excel-format (.xlsx), utöver alla andra aktuella format.

Tidigare kunde du bara leverera en rapport i följande format:

HTML

PDF

MS Excel (.xls)

TSV

Mer information om schemaläggning av leveransrapporter finns i&quot;Setting Up Report Deliflows&quot;.

## Förbättringar av uppgiftslistan {#task-list-improvements}

[uppdatera 18.3 Beta 4 där detta togs bort från ]

De nya uppgiftslistorna har återaktiverats efter en kort borttagning i betaversionen av 18.3. Vi har även infört följande ytterligare funktioner i uppgiftslistorna som inte ingick i den ursprungliga versionen:

Om du ersätter högerklicksmenyn med ikonen Mer när du redigerar en åtgärd.

De alternativ som var tillgängliga på högerklicksmenyn när du redigerade flera uppgifter samtidigt har nu flyttats till ikonerna som visas högst upp i uppgiftslistan.

Som standard visas 2 000 uppgifter i uppgiftslistor.

När Workfront beräknar om tidslinjer har frågetecknen intill de uppgifter vars datum uppdateras ersatts med grå områden.

Mer information om hur du redigerar uppgifter finns i&quot;Kopiera och duplicera uppgifter&quot; och&quot;Skapa föregående relationer genom att kedja uppgifter&quot;.

Mer information om hur du beräknar om projekttidslinjer finns i&quot;Beräkna om tidslinjer för projekt&quot;.

## Visa listor i helskärmsläge {#display-lists-in-full-screen}

När en lista med projekt eller uppgifter är större än skärmstorleken visas nu listan automatiskt i hela webbläsarfönstret när du rullar. Detta ökar mängden information som visas samtidigt och gör det lättare att hantera listor.

Du kan visa följande listor i helskärmsläge:

En lista med projekt på följande flikar och underflikar:

Projekt som jag är på

Projekt jag äger

Alla projekt

Fliken Projekt i en Portfolio

Fliken Projekt i ett program

En lista med uppgifter på följande flikar:

Fliken Uppgifter i ett projekt

Fliken Underuppgifter i en uppgift

Mer information om hur du visar objekt i listor finns i&quot;Visa objekt i en lista&quot;.

## Nya listor i ytterligare områden {#new-lists-in-additional-areas}

Vi har förbättrat prestandan och utseendet på projekt- och uppgiftslistor inom följande områden:

Flikarna Portfolio och Program i området Projekt

Fliken Underuppgifter på aktivitetsnivå

Före den här förbättringen fanns de nya listorna bara tillgängliga i följande områden:

Fliken Projekt i området Projekt

Fliken Åtgärder på projektnivå

Mer information om hur du visar objekt i listor finns i&quot;Visa objekt i en lista&quot;.

## Visa aktivitetsinformation i Gantt-schemat för projektlistan i ett program eller Portfolio {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Nu kan du visa information om ett projekts uppgifter i Gantt-schemat för projektlistor i ett program eller Portfolio.

Tidigare kunde du bara visa information om uppgifter i Gantt-schemat för projektlistor på fliken Projekt.

Mer information finns i&quot;Visa information i Gantt-schemat&quot;.

## What-If-scenarier i Gantt-schema för uppgiftslista {#what-if-scenarios-in-the-task-list-gantt-chart}

Du kan nu utföra följande åtgärder för uppgifter i ett projekt när de visas i redigeringsläget i Gantt-schemat:

Lägga till uppgifter

Ta bort uppgifter

Inline-redigeringsuppgifter

Duplicera uppgifter

Ordna om aktiviteter

Ändra underaktiviteter

Även om du kan se hur ändringarna påverkar tidslinjen i projektet sparas de inte direkt. Du kan spara dem för att permanent uppdatera projekttidslinjen eller avbryta dem.

Tidigare gick det inte att förhandsgranska ändringar i uppgiftslistan i Gantt-diagrammet.

Mer information om hur du redigerar uppgifter i Gantt-schemat finns i&quot;Uppdatera information i Gantt-schemat för uppgiftslistor&quot;.

## Öppna Gantt-schemat för uppgiftslistor i mallar {#access-the-task-list-gantt-chart-on-templates}

Du kan nu komma åt Gantt-schemat för uppgiftslistor i en projektmall.

Tidigare gick det inte att visa Gantt-diagrammet i uppgiftslistan i en mall.

Mer information finns i&quot;Komma igång med Gantt-schemat&quot;.

## Nya pappersstorlekar för Gantt-diagramexport {#new-paper-sizes-for-gantt-chart-export}

Nu kan du skriva ut Gantt-schemat på pappersformaten A1 och A2.

Tidigare kunde du bara exportera till Letter, Legal, Ledger, A3 (endast tillgängligt för vissa språk) och A4.

Mer information finns i&quot;Exportera Gantt-schemat till PDF&quot;.

## Byt namn på projektvyn i Gantt-schemat {#renamed-the-project-view-on-the-gantt-chart}

Vi döpte om visningsalternativet &quot;Projekt&quot; i Gantt-diagrammet till &quot;Anpassa alla&quot;. Visningsalternativet fungerar fortfarande som det gjorde tidigare. Det nya namnet ska vara mer beskrivande vad du ser när alternativet är markerat.

Mer information finns i&quot;Visa information i Gantt-schemat&quot;.

## Åtkomst till dialogrutor i Gantt-schemat i redigeringsläget har tagits bort {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Du kan inte längre komma åt dialogrutan Avancerade uppdrag när Gantt-diagrammet är i redigeringsläge. Du kan bara göra infogade redigeringar medan Gantt-schemat för uppgiftslistan är i redigeringsläge.

Tidigare kunde du öppna dialogrutan Avancerade uppdrag när Gantt-diagrammet var i redigeringsläge, men då sparades ändringarna i Gantt-schemat och redigeringsläget stängdes.

Mer information om hur du redigerar Gantt-schemat för uppgiftslistor finns i&quot;Uppdatera information i Gantt-schemat för uppgiftslistor&quot;.

## Exportera granskningsloggar {#export-audit-logs}

Nu kan du exportera granskningsloggposter till en CSV-fil. Du kan exportera upp till 50 000 granskningsloggposter till en CSV-fil samtidigt.

Mer information finns i Hantera granskningsloggar.
