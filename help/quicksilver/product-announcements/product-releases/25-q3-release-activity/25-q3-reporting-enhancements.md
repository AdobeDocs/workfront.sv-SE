---
title: Tredje kvartalet 2025 Rapporteringsförbättringar
description: Förbättringar av projektet för tredje kvartalet 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Tredje kvartalet 2025 Rapporteringsförbättringar

På den här sidan beskrivs alla rapportförbättringar som gjorts i den tredje utgåvan av kvartalet 2025 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2025 finns i [Översikt över utgåvan tredje kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

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

