---
title: Andra förbättringar under den andra kvartersversionen 2025
description: Andra förbättringar under den andra kvartersutgåvan 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Andra förbättringar under den andra kvartersversionen 2025

Den här sidan beskriver förbättringar som gjorts i den andra utgåvan av kvartal 2025 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den andra utgåvan av kvartal 2025 finns i [Översikt över den andra utgåvan av kvartal 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Uppgradera till den nya prenumerationsversionen med versionsuppgraderingsslutpunkter

>[!NOTE]
>
>Produktion för alla kunder: 6 mars 2025

Workfront har nu versioner av eventprenumerationer. Den nya versionen är inte en ändring av Workfront API, utan snarare en ändring av prenumerationsfunktionen för evenemang.

Möjligheten att uppgradera eller nedgradera abonnemang säkerställer att befintliga prenumerationer inte bryts när händelsestrukturen ändras, vilket gör att du kan testa och uppgradera till den nya versionen utan avbrott i prenumerationen.

Mer information om skillnaderna mellan de två versionerna finns i artikeln [Versionsinformation för händelseprenumeration](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Mer information om slutpunkterna som används för att uppgradera eller nedgradera en händelseprenumeration mellan olika versioner finns i avsnittet [Version av händelseprenumeration](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) i artikeln Prenumerations-API.

## Representera Adobe Admin Console användarändringar som&quot;System&quot; i Workfront uppdateringsfeed

>[!NOTE]
>
>Förhandsversion: 23 januari 2025; Produktion för snabb release: Med version 25.2 (13 februari 2025); Produktion för kvartalsvis publicering: Med version 25.4 (april 2025)

När administratören för Adobe Admin Console nu gör en ändring i användarinformationen för en Workfront-användare, registrerar Workfront denna ändring på fliken Systemaktivitet i användarens uppdateringsområde som tillhör &quot;System&quot;. Detta avser Adobe Admin Console-administratören.

Innan den här uppdateringen har användarändringar som gjorts av Admin Console-administratören registrerats som gjorda av Workfront huvudsystemadministratör.

Mer information om hur du hanterar användare i Adobe Admin Console finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
