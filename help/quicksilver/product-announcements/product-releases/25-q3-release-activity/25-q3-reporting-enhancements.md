---
title: Tredje kvartalet 2025 Rapporteringsförbättringar
description: Förbättringar av projektet för tredje kvartalet 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Tredje kvartalet 2025 Rapporteringsförbättringar

På den här sidan beskrivs alla rapportförbättringar som gjorts i den tredje utgåvan av kvartalet 2025 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2025 finns i [Översikt över utgåvan tredje kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Förbättrad leveranssäkerhet för rapporter

* Förhandsgranska: 26 juni 2025
* Produktion: Avveckling från 26 juni 2025 till 9 juli 2025

Vi har förbättrat leverans av schemalagda rapporter för att säkerställa att Workfront-meddelanden bara skickas till e-postdomäner som godkänts i tillåtelselista.

Tidigare, om din organisation hade definierat en begränsning för vilka e-postdomäner som Workfront aviserar, skulle vi göra en kontroll mot tillåtelselista när e-postmeddelanden lades till.

Nu kontrollerar vi också att e-postadressen som anges överensstämmer med e-postadressen som tillåtslista när vi skickar e-postmeddelandet. Den här förbättrade kontrollen gäller både e-postadresser som är kopplade till användare och ad hoc-e-postmeddelanden som läggs till i rapportmottagarlistan.

Mer information finns i [Schemalägg en automatisk rapportleverans](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## Jokertecken för användare returnerar inte längre resultat med ett null-värde vid filtrering

>[!NOTE]
>
>* Förhandsgranska: 30 april 2025
>* Production fast release: 15 maj 2025
>* Produktion för alla kunder: 17 juli 2025

Vi har uppdaterat användarens jokerteckenbeteende så att null-värde utesluts när en rapport filtreras. Den här ändringen gör att filtret ger mer korrekta resultat i stället för att returnera resultat som inte har en användare korrekt konfigurerad (ett null-resultat).

Tidigare, när ett jokertecken för användare genererade ett null-värde, skulle en rapport visa alla poster som också har ett null-värde.

Den här ändringen gäller följande jokerteckenfilter:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
