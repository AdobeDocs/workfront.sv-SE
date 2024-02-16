---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 1 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2017.3. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 9 augusti 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 2017.3 Beta 1 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2017.3. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 9 augusti 2017. Den kommer att göras tillgänglig i produktionsmiljön i början av november 2017.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.3 finns på  [Aktivitetsöversikt för 2017.3-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Beta 1-versionen från 2017.3 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer:**

* [Förhindra att uppgifter och problem tas bort när timmar loggas](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Borttagning av inställningen &quot;tidig åtkomst&quot; från inställningsområdet](#removal-of-the-early-access-setting-from-the-setup-area)
* [Ändra standardadress för e-postadress](#workfront-default-email-address-change)

**För alla användare:**

* [Förbättringar av resursplanering](#resource-scheduling-improvements)
* [Widescreen](#widescreen-display)
* [Ändra storlek på och ordna om kolumner i rapporter och listor](#resize-and-reorder-columns-in-reports-and-lists)
* [Alternativet Rensa anpassade data vid kopiering av uppgifter och problem](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Skapa ett projekt direkt från en mall](#create-a-project-directly-from-a-template)
* [Meddelande i appen för prenumererade objekt](#in-app-notification-for-subscribed-objects)
* [@Taggning är för närvarande inte tillgänglig i förhandsvisningsmiljön](#tagging-currently-not-available-in-the-preview-environment)
* [Inkludera information om användarallokering i användningsrapporten för ett projekt](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Förbättringar av resursplanering {#resource-scheduling-improvements}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Följande förbättringar av resursplanering är tillgängliga vid schemaläggning av resurser för ett team, för ett projekt eller för flera projekt som resurshanterare:

* [Visa schemaläggningsområde i helskärmsläge](#view-scheduling-area-in-full-screen-mode)
* [Fler datumintervallalternativ för visning av resursplaneringsområdet](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Visa beräknade datum på tidslinjen för schemaläggning](#view-projected-dates-on-the-scheduling-timeline)

### Visa schemaläggningsområde i helskärmsläge {#view-scheduling-area-in-full-screen-mode}

Du kan visa tidslinjen för schemaläggning i helskärmsläge, så att du kan se mer information i en enda vy. 

Mer information finns i Kom igång med resursschemaläggning.

### Fler datumintervallalternativ för visning av resursplaneringsområdet {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Du kan visa följande alternativ för ytterligare datumintervall när du visar tidslinjen för schemaläggning:

* Endagsvy
* 4-veckorsvy
* 6-veckorsvy

Före den här ändringen kunde du bara visa tidslinjen för schemaläggning i en 1-veckorsvy, 2-veckorsvy eller 3-veckorsvy. Dessa datumintervall är fortfarande tillgängliga utöver de nya datumintervallen.

När du visar tidslinjen för schemaläggning i en endagsvy, kan inte användarallokeringar (inklusive totalt antal timmar per dag) visas.

Mer information finns i Kom igång med resursschemaläggning.

### Visa beräknade datum på tidslinjen för schemaläggning {#view-projected-dates-on-the-scheduling-timeline}

Nu kan du konfigurera tidslinjen för schemaläggning så att den visar planerade datum i stället för planerade datum för aktiviteter och ärenden. 

Före den här ändringen visade aktiviteter och problem på tidslinjen endast Planerade datum.

När du visar Planerade datum på tidslinjen för tidsplanering kan inte användarallokeringar (inklusive totalt antal timmar per dag) visas.

Mer information finns i Kom igång med resursschemaläggning.

## Widescreen {#widescreen-display}

När du visar något av följande objekt i Workfront fylls hela webbläsarfönstret automatiskt i:

* Projekt
* Uppgifter
* Problem
* Rapporter
* Kontrollpaneler
* Kalendrar

Före den här ändringen fanns det två vita sidofält på båda sidor om det visade området. Nu justeras widescreen-vyn dynamiskt till bredden på skärmen och i webbläsarfönstret.

## Ändra storlek på och ordna om kolumner i rapporter och listor {#resize-and-reorder-columns-in-reports-and-lists}

Nu kan du ändra ordning på och ändra storlek på kolumner i en rapport eller lista utan att behöva redigera rapporten. (Den här funktionen togs bort i och med att miljön för tidig åtkomst togs bort tidigare i år. Den återinförs nu.)

Den här funktionen är inte tillgänglig för kontrollpanelslistor eller rapporter eftersom dessa listor har omdesignats i en ny datarutnätstruktur. Alla andra listor kommer att ha den här funktionen aktiverad i den här versionen.

Mer information om hur du ändrar storlek på och ändrar ordning på kolumner finns i [Ändra kolumnbredd och -ordning](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Alternativet Rensa anpassade data vid kopiering av uppgifter och problem {#clear-custom-data-option-when-copying-tasks-and-issues}

När du kopierar en uppgift eller ett problem kan du nu välja ett alternativ för att rensa anpassade data. När du väljer att rensa anpassade data för en uppgift eller ett problem kopieras formuläret till det nya objektet, men det är inte anpassade data i formuläret. När du rensar anpassade data påverkas även de anpassade formulär som är kopplade till dokumenten som är kopplade till objekten, eller de anpassade formulär som är kopplade till utgifterna för uppgiften.

Före den här ändringen kopierades även anpassade data som ingår i ett anpassat formulär till det nya objektet när du kopierade uppgiften eller utgåvan. 

Mer information om att kopiera uppgifter finns i [Kopiera och duplicera uppgifter](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Mer information om kopieringsproblem finns i [Kopiera problem](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Skapa ett projekt direkt från en mall {#create-a-project-directly-from-a-template}

Nu kan du skapa ett projekt från en mall på mallnivå.

Före den här ändringen kan du bara skapa ett projekt från en mall på fliken Projekt i området Projekt i Workfront med hjälp av **Nytt projekt från mall** alternativ.

Mer information om hur du skapar ett projekt från en mall finns i [Skapa ett projekt med en mall](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Förhindra att uppgifter och problem tas bort när timmar loggas {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Nu kan du konfigurera Workfront så att du antingen tillåter eller förhindrar att uppgifter och problem som har loggats i timmar tas bort.

När du tog bort en uppgift eller ett problem där timmar loggades, togs timmarna bort med uppgiften eller utgåvan eller så flyttades de till projektet, beroende på dina tidrapporter och timinställningar.

Mer information om hur du tar bort uppgifter finns i [Ta bort uppgifter](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Mer information om hur du tar bort problem finns i [Ta bort problem](../../../../manage-work/issues/manage-issues/delete-issues.md).

Mer information om hur du aktiverar systeminställningen för borttagning av uppgifter och problem finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Borttagning av inställningen &quot;tidig åtkomst&quot; från inställningsområdet {#removal-of-the-early-access-setting-from-the-setup-area}

Vi håller på att ta bort inställningen som tillåter Workfront-administratörer att registrera användare för att delta i tidig åtkomst-miljön. Funktionen har tagits bort sedan slutet av 2016. Vi har inte släppt några nya funktioner för tidig åtkomst 2017 och alla funktioner som fanns kvar i den miljön har flyttats till Produktion.

Före den här ändringen kunde Workfront-administratörer fortfarande lägga till användare i tidig åtkomst-miljön, men det fanns inga nya funktioner att komma åt.

## Ändra standardadress för e-postadress {#workfront-default-email-address-change}

Standardadressen för utgående e-post från Workfront har ändrats från [noreply@attask.com](mailto:noreply@attask.com) till [noreply@my.workfront.com](mailto:noreply@workfront.com).

Om du för närvarande filtrerar e-postmeddelanden som skickas från Workfront måste du ändra filtret så att det motsvarar den nya standardadressen. 

Ändringen av standardadressen påverkar inte konfigurerade Workfront-e-postadresser. 

Mer information finns i .

## Meddelande i appen för prenumererade objekt {#in-app-notification-for-subscribed-objects}

När en användare kommenterar projekt, uppgifter och utgåvor som du prenumererar på får du nu ett meddelande i appen. Mer information om prenumerationer i appmeddelanden finns i [Visa och hantera meddelanden i appen](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Beroende på vilka funktioner din Workfront-administratör har aktiverat kan du även få e-postmeddelanden om prenumerationsobjekt. Du kan enkelt avbeställa en prenumeration via en länk i ett e-postmeddelande som beskrivs i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md).

Du har alltid fått ett e-postmeddelande om prenumerationsobjekt och det fanns inget alternativ för att få ett meddelande i appen.

Du kan inaktivera e-post för prenumeration, men du kan inte inaktivera meddelanden i appen för prenumerationsobjekt. Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Mer information om att prenumerera på objekt finns i [Prenumerera på objekt i Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Taggning är för närvarande inte tillgänglig i förhandsvisningsmiljön {#tagging-currently-not-available-in-the-preview-environment}

När vi arbetar med att lägga till funktioner för RTF-format i uppdateringsflödet kan du för tillfället inte använda symbolen @ för att tagga andra användare i uppdateringsflödet för följande objekt i förhandsvisningsmiljön:

* Projekt
* Uppgift
* Problem
* Tidrapport

Du kan fortfarande tagga andra genom att klicka på **Inkludera andra i den här uppdateringen** -ikon.

Mer information finns i [Tagga andra för uppdateringar](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inkludera information om användarallokering i användningsrapporten för ett projekt {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Verktygen för resursschemaläggning har tagits bort från Workfront i version 23.1. Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Användningsrapporten för ett projekt tar nu hänsyn till om de planerade timmarna har omfördelats under en uppgifts varaktighet. När användarallokeringen för timmar har ändrats (enligt beskrivningen i Hantera användarallokeringar i schemaläggningsområdena) kan informationen i användningsrapporten påverkas om de datum som valts i användningsrapporten bara innehåller en del av en aktivitet.

Mer information finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
