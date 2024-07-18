---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 3 - versionsaktivitet
description: 2017.3-utgåvan kommer att göras tillgänglig i produktionsmiljön i början av november 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 2017.3 Beta 3 - versionsaktivitet

2017.3-utgåvan kommer att göras tillgänglig i produktionsmiljön i början av november 2017.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.3 finns på  [Aktivitetsöversikt för version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

2017.3 Beta 3 innehåller förbättringar för alla användare:

* [Anpassa diagramfärger](#customize-chart-colors)
* [Ytterligare alternativ vid kopiering av projekt](#additional-options-when-copying-projects)
* [Förbättrad resursplanering: Filter](#resource-planner-improvement-filters)
* [Förbättring av resursplanering: Visa utfärdandetimmar i området Inställningar](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [SSO-information för sandlådorna för anpassad uppdatering och förhandsvisning Uppdatera inte](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Uppdaterade supportkrav för webbläsare för Workfront Proof](#updated-browser-support-requirements-for-workfront-proof)

## Anpassa diagramfärger {#customize-chart-colors}

Nu kan du anpassa färgerna för elementen i diagram. Detta gäller för alla diagramtyper i rapporter. Detta gäller inte Gantt-schemat.

Före den här ändringen markerades färgerna för elementen i alla diagram som standard av Workfront. Mer information om hur du anpassar diagramfärger finns i avsnittet Anpassa diagramfärger i [Lägga till ett diagram i en rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Ytterligare alternativ vid kopiering av projekt {#additional-options-when-copying-projects}

När du kopierar ett projekt matchar nu alternativen de som är tillgängliga när du kopierar uppgifter eller utgåvor. Du kan också ändra status på det kopierade projektet medan du kopierar det.

Före den här uppdateringen kunde du inte ändra status för det kopierade projektet när det kopierades, och bara två alternativ var tillgängliga när ett projekt kopierades:

* Behålla tilldelningar för aktiviteter och projektet
* Bevara förloppet för uppgifter och projekt

Med den nya funktionen har de tidigare alternativen tagits bort och följande alternativ har lagts till när du kopierar ett projekt:

* Rensa uppdrag
* Rensa finansiell information
* Rensa förlopp
* Rensa godkännandeprocess
* Rensa anpassade data
* Rensa påminnelsemeddelanden
* Rensa dokument
* Rensa utgifter
* Rensa alla föregående
* Rensa behörigheter
* Markera alla

Mer information om de nya funktionerna för att kopiera projekt finns i avsnittet Kopiera ett projekt i förhandsvisningsmiljön i   [Kopiera ett projekt](../../../../manage-work/projects/manage-projects/copy-project.md).

## Förbättrad resursplanering: Filter {#resource-planner-improvement-filters}

Nu kan du filtrera informationen som visas i resursplaneraren efter följande objekt:

* Portfolio
* Projektstatus
* Team
* Jobbroll
* Resurspool

Du kan också lägga till ett eget filter baserat på dessa objekt.

Mer information om hur du använder resursplaneraren finns i [Resursplaneringsöversikt](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Förbättring av resursplanering: Visa utgivningstimmar i området Inställningar {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Det finns ett nytt inställningsområde i resursplaneraren som visar flera alternativ för att anpassa resursplaneraren. I den här versionen har vi lagt till det första alternativet som inkluderar planerade timmar från utgåvor i kolumnerna Planerade timmar i Resursplaneraren.

Mer information om hur du använder resursplaneraren finns i [Resursplaneringsöversikt](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## SSO-information för sandlådorna för anpassad uppdatering och förhandsvisning Uppdatera inte {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

Från och med den här versionen kopieras inte SSO-informationen från din produktionsmiljö och inaktiveras inte heller när du uppdaterar dina anpassade uppdaterings- och förhandsgranskningssandlådor. Före den här ändringen inaktiverades SSO-informationen i sandlådorna för anpassad uppdatering och förhandsgranskning och var inställd på &quot;Ingen&quot;.

Mer information om anpassad sandlådemiljö för uppdatering finns i [Anpassad sandlådemiljö för Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Mer information om sandlådemiljön för förhandsgranskning finns i [Sandlådemiljön för Adobe Workfront Preview](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Uppdaterade supportkrav för webbläsare för Workfront Proof {#updated-browser-support-requirements-for-workfront-proof}

Krav för webbläsarstöd för Workfront Proof har uppdaterats. Mer information finns i [Adobe Workfront webbläsarkrav](../../../../workfront-basics/workfront-browser-requirements.md).
