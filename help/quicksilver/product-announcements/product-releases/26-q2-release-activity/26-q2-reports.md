---
title: Andra kvartalet 2026 - rapportförbättringar
description: Andra kvartalet 2026 - rapportförbättringar
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
source-git-commit: aceb9f7bd6c62036838b15d74ee2a9b7843e5c11
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Andra kvartalet 2026 - rapportförbättringar

Den här sidan beskriver rapportförbättringar som gjorts i den andra utgåvan av kvartalet 2026 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön enligt vad som anges.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den andra utgåvan av kvartal 2026 finns i [Översikt över den andra utgåvan av kvartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

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
