---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatera
navigation-topic: product-releases
title: 21.1 Andra förbättringar
description: Den här sidan beskriver alla andra förbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.

En lista över alla ändringar som är tillgängliga i version 21.1 finns i [21.1-versionsöversikt](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Uppdateringar av kraven för misslyckade händelseprenumerationer

Vi uppdaterar kraven för mjuk inaktivering vid fel med händelseprenumeration. Förutom de befintliga kraven inaktiveras nu även Event-prenumerationer om de inte lyckas leverera inom 2 000 försök. Detta är för att stärka den befintliga 70-procentiga felregeln, som under vissa omständigheter kan leda till alltför många fel.

Dessutom kommer vi att lägga till krav på inaktivering från och med februari 2021.

Mer information om de nya kraven för mjuk inaktivering och inaktivering finns i [Vanliga frågor och svar - Händelseprenumerationer](../../../wf-api/general/event-subs-faq.md).

## Nya Team-fält tillgängliga för Daily Digest

Vi har lagt till fälten för teamgodkännande och tilldelningar i e-postmeddelandet Åtgärd krävs varje dag.

Mer information finns i [Meddelanden: Åtgärd krävs](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Ersätta POP-e-postalternativ i begärandeköer

Vi ersätter POP-e-postalternativet för begärandeköer med ett nytt system som hanteras av Workfront. Du kan fortfarande skicka begäranden via e-post, men du måste konfigurera en ny e-postadress som hanteras av Adobe Workfront i området Begärandekö i stället.

Dessa ändringar är tillgängliga för test i förhandsvisning.

E-post inaktiveras automatiskt i alla förhandsvisningsmiljöer. Information om hur du aktiverar e-post för testning finns i [Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådemiljön](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Mer information finns i [Gör det möjligt för användare att skicka ett problem via e-post till ett begärandeköprojekt](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Mer information om varför vi gör den här ändringen finns i [Nytt Adobe Workfront-hanterat system som ersätter POP-e-post för begärandeköer med 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Den här funktionen ingår nu i [köhanteringen i den nya inlärningsvägen för Workfront Experience](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) på Workfront One.

## Begränsa timredigering för tidrapporter

För att få bättre kontroll över tidrapporter och timredigering har vi lagt till en inställning som tillåter dig att begränsa timredigering till tidrapportsägare och systemadministratörer.

Tidigare kunde användare med alternativet Tidrapporter och timmar aktiverat på åtkomstnivån redigera timmar på alla tidrapporter.

Mer information finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Förbättrade filter och vyer i området Tidrapporter

Vi har lagt till följande förbättringar när du lägger till ett projekt, en uppgift eller ett problem i en tidrapport:

* Filter: Vi har lagt till filter för projekt och problem. Klicka på Fler alternativ för att visa dessa filter. Tidigare var det bara Aktiviteter som hade filtrering tillgängliga.
* Vyer: Vi har lagt till alternativen Visa och Gruppera på söksidan.

Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Dölja övertidsrutan i tidrapporter

Du kan nu dölja övertidsrutan för att förenkla för användaren om du inte spårar övertid i Workfront. Du kan dölja övertidsrutan för en enskild tidrapport eller i tidrapportprofilen:

* Enkel tidrapport: När du väljer att dölja övertidsrutan i en enskild tidrapport döljs den bara för den tidrapporten. Mer information finns i [Skapa en tidrapport för engångsbruk](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Tidrapportprofil: När du väljer att dölja rutan för övertid i tidrapportprofilen kommer alla framtida tidrapporter som skapas för de användare som tilldelats den profilen inte att se rutan för övertid. Mer information finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Tidigare kunde du inte dölja övertidsrutan på tidrapporter.

## Expandera eller komprimera objekt i navigeringen i vägbeskrivningar

För att det ska bli enklare att visa hela sökvägen har vi lagt till funktionerna för att expandera och komprimera.

Nu grupperas alla trunkerade objekt före projektet med texten &quot;mer&quot;. &quot;3 till&quot; betyder t.ex. att det finns 3 objekt som inte visas.

Tidigare var du tvungen att klicka på ellipsen för att visa trunkerade objekt i en nedrullningsbar meny.

Om du vill visa alla objekt i den synliga sökvägen klickar du på &quot;mer&quot; i början av den synliga sökvägen för att expandera objekten. När du har expanderat kan du klicka på Mindre om du vill komprimera objekten igen.

## Nytt utseende och ny känsla för banbrytande navigering

För att hjälpa användare att bättre identifiera var de befinner sig i Workfront och enklare navigera mellan objekt har följande förbättringar gjorts för att underlätta navigering i vägbeskrivningar:

* Varje objekt i vägbeskrivningsfilen innehåller nu en objektetikett.
* Den aktuella sidan finns nu med i sidutrymmet och är kursiv.
* Tangentbordsnavigering och skärmläsarnavigering är nu tillgängliga för vägbeskrivningar.
* Ytterligare mindre formatändringar

