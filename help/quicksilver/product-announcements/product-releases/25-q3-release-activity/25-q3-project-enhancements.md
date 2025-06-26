---
title: Förbättringar av projektet för tredje kvartalet 2025
description: Förbättringar av projektet för tredje kvartalet 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: e3fa5f6fd86f0fe9ba221fb7c20f46f966437a42
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Förbättringar av projektet för tredje kvartalet 2025

Den här sidan beskriver projektförbättringar som gjorts i tredje kvartalet 2025-versionen till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2025 finns i [Översikt över utgåvan tredje kvartalet 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Fältet Befintliga faktiska timmar har ersatts med fältet Äldre faktiska timmar och det nya fältet Faktiska timmar har skapats

>[!NOTE]
>
> Förhandsgranskning och produktion: 24 juni 2025 

Det befintliga fältet Faktiska timmar har bytt namn till Tidigare faktiska timmar. I det här fältet lagras den tid som har loggats för projekt, uppgifter och ärenden på några minuter. Fältet lagras i Workfront-databasen som actualWorkRequired.

Vi har lagt till ett nytt fält för faktiska timmar som lagrar den tid som loggats för projekt, uppgifter och utgåvor i timmar, med decimalprecision. Fältet lagras i Workfront-databasen som actualWorkRequiredDouble.

Fälten Faktiska timmar och Äldre faktiska timmar visas i projekt-, uppgifts- och problemvyer och rapporter.

Fältet Faktiska timmar som visas i avsnittet Projekt, uppgifter och ärenden representerar de nya Faktiska timmarna.



>[!IMPORTANT]
>
>Beroende på när timmarna loggades kan det finnas en diskrepans mellan faktiska timmar och faktiska timmar för äldre för ett projekt, en uppgift eller en utgåva.<br>
>&#x200B;>Följande scenarier finns:
>
>* De faktiska timmarna som representerar timmar som har loggats för projekt, uppgifter och utgåvor sedan maj 2021 har flyttats från fältet Gammal faktisk timme till det nya fältet Faktisk timme.
>* De faktiska timmarna som representerar timmar som loggats för projekt, uppgifter och utgåvor före maj 2021 räknas bara i fältet Gammal faktisk tid.
>  &#x200B;><br>Du kan behöva uppdatera rapporterna så att de återspeglar det nya fältet och dess värden.


Mer information finns i [Visa faktiska timmar](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).


## Ändringar i hur faktiska timmar lagras i databasen för API-anrop

>[!NOTE]
>
>* Förhandsgranska: Med nästa API-version, som planeras släppas senare under 2025
>* Snabb produktion: Med nästa API-version, som planeras släppas senare under 2025
>* Produktion för alla kunder: Med nästa API-version, som planeras släppas senare under 2025

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
