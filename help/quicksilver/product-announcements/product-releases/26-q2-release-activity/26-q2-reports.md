---
title: Andra kvartalet 2026 - rapportförbättringar
description: Andra kvartalet 2026 - rapportförbättringar
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 1ef6ead705231a41cbf62b8a8b35f480da004970
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Andra kvartalet 2026 - rapportförbättringar

Den här sidan beskriver rapportförbättringar som gjorts i den andra utgåvan av kvartalet 2026 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den andra utgåvan av kvartal 2026 finns i [Översikt över den andra utgåvan av kvartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Aktuellt versionsfält för dokumentversioner

>[!NOTE]
>
>Förhandsgranska: 2 april 2026
>Production fast release: 15 april 2026
>Produktion för alla: 16 april 2026

Vi har lagt till ett `currentVersion` booleskt fält i dokumentversionsobjektet för att göra det enklare att identifiera och rapportera om den senaste versionen av ett dokument.
Med den här uppdateringen:

* Du kan använda `currentVersion` i filter, vyer, grupperingar och diagram.
* Fältet är tillgängligt i arbetsytans fältväljare för dokumentversionsrapporter.

* När en ny version har överförts:

   * Den nya versionen är markerad som `TRUE`
   * Tidigare versioner har markerats som `FALSE`

* Rapporterna kan konsekvent identifiera aktuella versioner på arbetsytans kontrollpaneler och äldre rapporter

Befintliga filter för klassiska rapporter som använder `isCurrentVersion` eller `isDocumentCurrentVersion` fortsätter att fungera som dokumenterat.

## Schemalagd rapportleverans stöder nu länkbaserade e-postmeddelanden

>[!NOTE]
>
>Förhandsgranska: 3 april 2026
>Production fast release: 15 april 2026
>Produktion för alla: 16 april 2026

Workfront innehåller nu en ny typ av länkleverans för schemalagda rapporter. I stället för att generera och bifoga en fil skickar det här alternativet ett e-postmeddelande som innehåller en direktlänk till rapporten i Workfront, vilket gör att mottagarna kan visa {{$include }} de senaste data som finns i programmet.

Alternativet Länka är nu standardleveranstyp för nya leveransregler för schemalagda rapporter, medan befintliga filbaserade format (HTML, PDF, Excel och TSV) fortfarande är tillgängliga.

Med den här förändringen har vi även uppdaterat utseendet och känslan i e-postmeddelandet för rapportleverans.

Mer information finns i [Schemalägg en automatisk rapportleverans](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Köra rapporter som en specifik användare på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 2 april 2026
>Production fast release: 15 april 2026
>Produktion för alla: 16 april 2026
>
>Kontrollpaneler för arbetsytan är för närvarande i betaversion.

Nu kan du konfigurera rapporter på arbetsytans kontrollpaneler så att de körs som en specifik användare. När det här alternativet är aktiverat visas data baserat på den valda användarens åtkomst i stället för användarens behörigheter.

Detta ger enhetligare och tillförlitligare data i olika kontrollpanelsvisningsprogram, även när åtkomst till planeringsarbetsytor, posttyper eller auktoriseringsinställningar skiljer sig åt.

Mer information finns i [Skapa en KPI-rapport på en Canvas-kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Skapa en diagramrapport på en Canvas-kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) eller [Skapa en tabellrapport på en Canvas-kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## Nya autentiseringsalternativ för dataanslutning

>[!NOTE]
>
>Förhandsgranska: 12 mars 2026
>Production fast release: 12 mars 2026
>Produktion för alla: 16 april 2026

Nu kan du autentisera till Data Connect med RSA-nycklar eller PAT-anslutningar (Programmatic Access Tokens), vilket ger säkrare och flexiblare alternativ till traditionella inloggningsuppgifter för användarnamn/lösenord.

Med dessa nya alternativ kan organisationer upprätthålla stabila anslutningar från Power BI, Tableau och andra BI-verktyg från tredje part utan att förlita sig på användarbaserade inloggningsmetoder.

>[!IMPORTANT]
>
>I juni 2026 krävs användarnamn/lösenord för att använda multifaktorautentisering (MFA). Vi rekommenderar att du övergår till antingen RSA- eller PAT-baserad autentisering för tjänstanvändarkonton som används för att läsa in data från Data Connect till tredjepartsverktyg för visualisering, dataprocessorer och skript som inte fungerar med MFA i autentiseringsprocessen.

## Anpassade fältetiketter visas när rapporter skapas

>[!NOTE]
>
>Förhandsgranska: 26 februari 2026
>Production fast release: 12 mars 2026
>Produktion för alla: 16 april 2026

Etiketten för det anpassade fältet visas nu före fältnamnet och objektet i rapportbyggverktygen, vilket gör det enklare att hitta fälten. Fältetiketter visas också när du definierar filter, vyer och grupperingar i listor.

Etiketten för det anpassade fältet är avsedd för systemgränssnittet, medan fältnamnet ofta används för API- och backend-lagring och kanske inte är lika användbart när ett fält hittas.

Mer information finns i [Skapa en anpassad rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Delningsbara rapportmappar

>[!NOTE]
>
>Förhandsgranska: 26 februari 2026
>Production fast release: 12 mars 2026
>Produktion för alla: 16 april 2026

Nu kan du ordna och dela rapporter med delningsbara rapportmappar. Den här nya funktionen hjälper team som hanterar stora mängder rapporter att upprätthålla en skalbar och konsekvent åtkomstkontroll:

* **Skapa ordnade mappstrukturer**: Systemadministratörer kan skapa mappar på den översta nivån, och användare med hanterad åtkomst kan skapa undermappar på upp till 4 nivåer.
* **Detaljerade behörighetskontroller**: Dela mappar med två behörighetsnivåer:
   * Visa: Användare kan öppna rapporter och dela mappar
   * Hantera: Användare kan redigera mappinformation, lägga till/ta bort objekt och automatiskt få åtkomst till alla rapporter i mappen
* **Ärvda behörigheter**: Behörigheter överlappar från överordnade mappar till alla undermappar och rapporter i mappträdet
* **Förbättrad listupplevelse**: När du aktiverar delningsbara mappar får du tillgång till den förbättrade listupplevelsen. Mer information finns i [Använd förbättrade listor](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Mer information finns i [Använd delningsbara rapportmappar](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Förbättrade datumetiketter för diagramgrupperingar på arbetsytans kontrollpaneler

>[!NOTE]
>
>Förhandsgranska: 26 februari 2026
>Production fast release: 12 mars 2026
>Produktion för alla: 16 april 2026

>[!NOTE]
>
>Kontrollpaneler för arbetsytan är för närvarande i betaversion.

Diagram som grupperar data efter datum visar nu tydligare och mer läsbara datumetiketter. Med den här uppdateringen justeras datumetiketter dynamiskt baserat på den valda gruppen efter alternativ - som dag, vecka, månad eller år - vilket gör det enklare att läsa och tolka diagram:

<table> <tbody> <tr> <td>Dag</td> <td>Visar det fullständiga datumet. Exempel: 3/12/2026</td> </tr> <tr> <td>Vecka</td> <td>Visar ett formaterat veckonas startdatum. Exempel: 8 mars 2026</td> </tr> <tr> <td>Månad</td> <td>Visar månad och år. Exempel mars 2026</td> </tr> <tr> <td>År</td> <td>Visar endast året. Exempel: 2026</td> </tr> </tbody> </table>

Tidigare visade diagramgrupperingar alltid startdatumet för den markerade perioden i numeriskt format.
