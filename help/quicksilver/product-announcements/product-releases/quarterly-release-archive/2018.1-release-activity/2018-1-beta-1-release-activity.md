---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 1. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 1 december 2017. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# 2018.1 Beta 1 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i 2018.1 Beta 1. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 1 december 2017. Den kommer att göras tillgänglig i produktionsmiljön i mars 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.1 finns på  [Aktivitetsöversikt för version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 1 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Uppdaterad layoutmall som stöder hemområdet](#updated-layout-template-to-support-the-home-area)
* [Inaktivera korrektur av e-postmeddelanden som skickats från Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Nya resurser har lagts till i händelseprenumerationer](#new-resources-added-to-event-subscriptions)

**För alla användare**

* [Hemma (min arbetsyta har uppdaterats)](#home-area-updated-my-work-area)
* [Visa resursplaneringsdata under Affärsärende och uppdaterad affärsfallssammanfattning](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Visa procentandelen för allokering av planerad timma i resursplaneraren](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Uppdateringstyperna Automatisk och Vid ändring och Endast ändring utlöser uppdateringar till överordnade objekt samtidigt som aktiviteter uppdateras](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Ögonblicksbild för tidslinje tillgänglig i Gantt-schema](#timeline-snapshot-available-in-the-gantt-chart)

## Hem (uppdaterade min arbetsyta) {#home-area-updated-my-work-area}

Den nya Hem-området ger en alternativ, förbättrad vy till samma data som för närvarande är tillgängliga i Min arbetsyta. Hem-området ger följande fördelar jämfört med Min arbetsyta:

* Ett smidigare och mer intuitivt gränssnitt
* Förbättrade prestanda
* Uppdatera uppgifter och problem med formaterad text

## Uppdaterad layoutmall som har stöd för hemområdet {#updated-layout-template-to-support-the-home-area}

Som Workfront-administratör kan du avgöra om användare i din organisation har tillgång till Hem-området genom att konfigurera den layoutmall de är tilldelade. Användare som inte har tilldelats någon layoutmall har alltid tillgång till Hem-området.

Mer information finns i&quot;Skapa och hantera layoutmallar&quot;.

## Inaktivera korrektur av e-postmeddelanden som skickats från Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Du kan nu konfigurera om användare i din Workfront-instans ska få e-postmeddelanden från Workfront när en kommentar görs i ett korrektur.

Tidigare skickades alltid korrekturmeddelanden från Workfront när en kommentar gjordes på ett korrektur. Om meddelanden även har aktiverats i Workfront Proof får användarna dubblettmeddelanden. 

För befintliga Workfront-kunder är Workfront som standard konfigurerat att skicka e-postmeddelanden när en kommentar görs på ett korrektur.

Mer information om hur du inaktiverar e-postmeddelanden för korrektur i Workfront så att korrekturmeddelanden endast skickas från Workfront Proof finns i .  

## Visa data om resursplanering under Affärsärende och uppdaterad ärendesammanfattning {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

Resursbudgeteringsområdet är nu tillgängligt i ett projekts affärsfall. I det här området kan du granska beräknade budgettimmar för dina resurser i resursplaneraren och den budgeterade arbetskostnad som är kopplad till dem.

Området Resursberäkning i affärsärendet har bytt namn till Äldre resursuppskattningar.

Som en del av den här ändringen innehåller nu Översikt över affärsärenden ekonomisk information baserad på både Resursberäkning och Resursbudgetering.

Före den här ändringen kunde du inte se information om resursplanering för projektets affärsmodell. Du kan bara se information om resursuppskattningar som har angetts i Kapacitetsplaneraren för de äldre resurspoolerna.

Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Visa procentandelen för allokering av planerad timma i resursplaneraren {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

Användarvyn för resursplaneraren innehåller nu en ny kolumn som gör att du kan visa den planerade timtilldelningen som en procentandel av det totala antalet tillgängliga timmar för användaren och jobbrollen.

Före den här ändringen kunde du bara visa det totala antalet planerade och tillgängliga timmar för användare och jobbroller i separata kolumner.

Mer information om kolumnen Procentandel för allokering av timmar finns i avsnittet Visa skillnaden mellan tillgängliga och planerade timmar eller FTE i resursplaneraren i [Översikt över resursplaneraren](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Uppdateringstyperna &quot;Automatisk och Vid ändring&quot; och &quot;Ändra endast&quot; utlöser uppdateringar till överordnade objekt samtidigt som uppgifter uppdateras {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Vi har ändrat det sätt på vilket överordnade uppgifter och projektet uppdateras när ett objekt på låg nivå uppdateras i ett projekt. Den tid då ett överordnat objekt uppdateras bestäms av fältet Uppdateringstyp i ett projekt. Du kan välja mellan följande uppdateringstyper:

* Automatiskt och vid ändring
* Ändra endast
* Endast automatiskt
* Endast manuellt

När du nu väljer uppdateringstyperna &quot;Automatiskt och vid ändring&quot; eller &quot;Endast ändring&quot; tillämpas de ändringar du gör på de enskilda uppgifterna även på den överordnade aktiviteten och projektet direkt.

Före den här ändringen var du tvungen att uppdatera sidan för att se till att även de överordnade objekten och tidslinjen i projektet uppdaterades.

Mer information om uppdateringstypen för ett projekt finns i [Välj projekttyp](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Ögonblicksbild för tidslinje tillgänglig i Gantt-schema {#timeline-snapshot-available-in-the-gantt-chart}

Nu kan du snabbt rulla till en viss punkt i ett projekts livstid genom att använda den nya ögonblicksbilden av tidslinjen i Gantt-diagrammet.

När du väljer en mer detaljerad tidsram för Gantt-schemat när du visar en uppgift eller en projektlista visas en vågrät rullningslist längst ned i Gantt-schemat. Om du klickar på rullningslisten kan du se hela tidslinjen för projektet i en ögonblicksbild. Du kan klicka var som helst inuti ögonblicksbilden av Gantt-schemat för att navigera till en viss punkt under projektets livstid.

Före den här ändringen var du tvungen att rulla vågrätt i hela Gantt-diagrammet för att hitta en viss tidpunkt, eller så var du tvungen att zooma ut ur den detaljerade vyn.

Mer information om hur information visas i Gantt-schemat finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nya resurser har lagts till i händelseprenumerationer {#new-resources-added-to-event-subscriptions}

Nu kan du skapa evenemangsprenumerationer för följande resurser:

* **Utgift:** Meddelar dig när en utgift läggs till eller ändras.
* **Tilldelning:** Meddelar dig när en tilldelning läggs till eller ändras för en aktivitet eller ett problem för en användare, en jobbroll eller ett team.
* **Tidrapport:** Meddelar dig när en tidrapport har skickats, avvisats eller godkänts.

Mer information om händelseprenumerationer finns i [API för händelseprenumeration](../../../../wf-api/general/event-subs-api.md).
