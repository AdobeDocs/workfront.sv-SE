---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatering,release
navigation-topic: 2021-2-release-activity
title: 21. 2 Förbättrade rapporter
description: Den här sidan beskriver alla rapportförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i versionsöversikt 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 21. 2 Förbättrade rapporter

Den här sidan beskriver alla rapportförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i [21.2 versionsöversikt](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Begränsa timredigering i projekt och rapporter

För att få bättre kontroll över timredigeringen på fliken Timmar i ett projekt och timrapporter har vi lagt till en inställning som tillåter Workfront-administratörer att begränsa timredigering till timägare och systemadministratörer.

Tidigare kunde användare med tidrapporter och timmar aktiverade på åtkomstnivån redigera timmar.

Mer information finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nytt utseende och ny känsla för uppdragsfältet i uppdaterade listor och rapporter

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För att matcha det moderna utseendet i andra områden i den nya Workfront-upplevelsen har formatet ändrats för fältet Uppdrag i uppdaterade listor och rapporter. Denna nya design innehåller följande:

* En rundad avatar för användarprofilbilder, jobbroller och team
* Inledande visning för användare utan profilbilder
* Ikon för en ny jobbroll
* En ny personikon för avancerade uppdrag
* En ny ikon för begränsad åtkomst
* Andra mindre designändringar

Mer information om tilldelningar i listor finns i [Tilldela uppgifter](../../../manage-work/tasks/assign-tasks/assign-tasks.md) eller [Tilldela ärenden](../../../manage-work/issues/manage-issues/assign-issues.md).

![Uppdragsuppdateringar](assets/assignments-updates-350x193.png)

## Nytt utseende och känsla för typsnittsfält i uppdaterade listor och rapporter

>[!NOTE]
>
>Tillfälligt borttagen från produktionsmiljön den 20 maj 2021.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För att matcha det moderna utseendet i andra områden i den nya Workfront-upplevelsen har formateringen ändrats för typsnittsfält i uppdaterade listor och rapporter. Bland dessa ändringar finns:

* Typehead-ikonen har tagits bort från fältet.
* När du klickar på ett texthuvudsfält visas nu förslagsmenyn innan du anger text.
* Menyn med förslag är mer responsiv med värdenas längd och dessa värden trunkeras nu i slutet när teckengränsen nås i stället för i mitten av värdet.

Mer information om uppdaterade listor finns i avsnittet [Skillnaden mellan de uppdaterade och äldre listorna](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) i artikeln [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![Typhead-fält](assets/typeahead-updates-350x336.png)

## Rapport om systemuppdateringar

Den nya rapporten Journal Entry ger dig större möjligheter att granska systemuppdateringar, bland annat:

* Statusändringar för ett projekt, en uppgift eller ett ärende
* Borttagna uppgifter eller problem
* Värden i anpassade fält
* Planerade slutförandedatum
* Ändringar av projektägare

Du kan till exempel konfigurera den här rapporten så att den visar aktivitet runt ett specifikt anpassat fält, inklusive projektet för det anpassade fältet, när ett värde först angavs, vilket värdet var, när fältet uppdaterades, vilket det tidigare värdet var, vilket det nyligen angivna värdet var, vilka användare som slutförde dessa åtgärder osv.

Tidigare kunde du bara rapportera om systemuppdateringar via Workfront API.

Mer information om den här rapporten och vad du kan använda den för finns i [Rapport om uppdateringsområdet med en journalrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

