---
title: Förbättringar av projektet för tredje kvartalet 2025
description: Förbättringar av projektet för tredje kvartalet 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: a5a61045bad5a97fb1413fac4a5a2666b753fa83
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Förbättringar av projektet för tredje kvartalet 2025

Den här sidan beskriver projektförbättringar som gjorts i tredje kvartalet 2025-versionen till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2025 finns i [Översikt över utgåvan tredje kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Ändringar i hur faktiska timmar lagras i databasen för API-anrop

>[!NOTE]
>
>* Förhandsgranska: 27 maj 2025
>* Production fast release: 27 maj 2025
>* Produktion för alla kunder: 27 maj 2025

Uppdateringen förändrar det sätt på vilket faktiska timmar för projekt, uppgifter och ärenden lagras i databasen. Från och med den här uppdateringen används ett värdefält på `actualWorkRequiredDouble` (med ett värde i timmar).

Före den här uppdateringen lagrades de faktiska timmarna med värdefältet `actualWorkRequired` (med ett värde i minuter). Uppdateringen ger en mer korrekt räkning av de faktiska timmarna när de beräknas med ett API-anrop.

På grund av den här ändringen kan du behöva uppdatera alla API-anrop som refererar till det ursprungliga värdefältet. Du bör inte göra några ändringar om du använder värdefältet `actualWorkRequiredExpression` i API-anropen.

Den här uppdateringen ändrar inte beräkningarna för Faktiska timmar för projekt, uppgifter och utgåvor i beräknade anpassade fältkolumner.

## Uppdatera i med reglaget Procent färdigt i en uppgift eller ett ärende

>[!NOTE]
>
>* Förhandsgranska: 27 maj 2025
>* Production fast release: 27 maj 2025
>* Produktion för alla kunder: 27 maj 2025

Vi har uppdaterat hur procentreglaget fungerar för uppgifter och problem.

Följande funktionalitet är nu tillgänglig:

* När du drar den blå bubblan Procent färdigt i en uppgift eller i en utgåva uppdateras aktiviteten Procent färdigt i steg om fem punkter. Före den här uppdateringen uppdaterades aktiviteterna eller problemen i steg om en punkt genom att den blå bubblan Procent färdigt flyttades.

* Du kan dubbelklicka på den blå bubblan och manuellt uppdatera den med önskat nummer utan att använda skjutreglaget. Den här funktionen har inte ändrats.

Det finns inga andra ändringar som har gjorts för att uppdatera Procent färdigt för uppgifter och problem inom andra områden av Workfront.

Mer information finns i [Visa och uppdatera Procent färdigt för uppgifter](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Mer genomskinlighet när du använder AI Assistant för projekt, uppgifter och ärenden

>[!NOTE]
>
>* Förhandsgranska: 19 maj 2025
>* Production fast release: 19 maj 2025
>* Produktion för alla kunder: 19 maj 2025

För att klargöra hur AI Assistant hittar svar på frågor om Workfront projekt, uppgifter och problem har vi lagt till den här informationen i svaret på frågan. Nu inkluderar AI Assistant sökinformationen i utdata. Du kan använda den här informationen som ett sätt att kontrollera att AI Assistant har identifierat den fråga du ställde och att förstå svarets sammanhang.

Tidigare var denna information inte tillgänglig i AI Assistants svar.

Mer information om hur du använder AI Assistant för att få information om Workfront-objekt finns i [Använd AI Assistant för att arbeta med projekt, uppgifter och problem](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
