---
title: 22.4 Förbättringar av administratören
description: 22.4 Förbättringar av administratören
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4 Förbättringar av administratören

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 22.4 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga den 3 oktober 2022.

En lista över alla ändringar som är tillgängliga i version 22.4 finns i [22.4 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Använda olåsta statusvärden i en godkännandeprocess

>[!NOTE]
>
>Den här funktionen introducerades först i förhandsvisningsmiljön under 22.3-versionen. Den lanseras i Production 15 september 2022.

För att du ska få större kontroll över godkännandeprocesserna och statusvärdena i ditt system har vi gjort det möjligt att skapa en godkännandeprocess som baseras på en olåst systemstatus. Dessutom kan du nu låsa upp status som redan används i en godkännandeprocess. Tidigare var det nödvändigt att låsa en systemstatus som användes i en godkännandeprocess. Detta gjorde den tillgänglig för alla grupper - utan möjlighet att ta bort eller byta namn på den - så att gruppadministratörerna inte kunde effektivisera sin grupps lista över statusar efter deras specifika behov.

## Ikonen för utkast på huvudmenyn styrs nu av layoutmallar

Systemadministratörer kan nu lägga till eller ta bort ikonen för utkast på huvudmenyn via layoutmallskonfigurationen. Detta ger bättre kontroll över vem som kan bläddra i katalogen med utkast.

Ikonen för utkast visas på huvudmenyn när:

* Användaren har ingen tilldelad layoutmall

* Användarens layoutmall har alternativet Utkast i listan Aktiva objekt

* I användarens layoutmall finns alternativet Utkast i listan Tillgängliga objekt. Ikonen visas inte på huvudmenyn.

Befintliga layoutmallar innehåller automatiskt ikonen för utkast, och administratörer kan ta bort ikonen från layoutmallar för att begränsa synligheten för katalogen med utkast. Nya layoutmallar som skapas efter version 22.4 kommer att innehålla ikonen för utkast i listan Aktiva objekt.

Mer information finns i [Konfigurera åtkomst till utkast](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Anpassning av problemhuvud

Som Workfront- eller gruppadministratör kan du nu anpassa fälten som visas i huvudet i ett problem när du använder en layoutmall.

Uppdateringen innehåller följande förbättringar:

* Ta bort eller ordna om befintliga fält från utgåvans huvud.

* Lägg till nya fält för problemöversikt som inte kan redigeras. Du kan inte lägga till anpassade fält eller fält som kan redigeras. Du kan även visa redigerbara fält som för närvarande finns i utgåvans huvud (till exempel Status eller Procent färdigt).

* Utgivningsrubriken kan innehålla upp till fem fält.

* Nu kan du lägga till fältet&quot;Löst av&quot; i utgåvans huvud. När ett matchande objekt är kopplat till problemet ändras fältet &quot;Löst av&quot; till &quot;Lösning av problem&quot;, &quot;Åtgärda aktivitet&quot; eller &quot;Lösning av projekt&quot; beroende på vilken typ av objekt som är associerat med problemet.

Före den här versionen gick det bara att anpassa projekt- och uppgiftshuvuden.



Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Visa en videodemonstration av den här funktionen](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Anpassning av aktivitetshuvud

Som Workfront- eller gruppadministratör kan du nu anpassa fälten som visas i en uppgifts sidhuvud när du använder en layoutmall.

Uppdateringen innehåller följande förbättringar:

* Ta bort eller ordna om befintliga fält från uppgiftshuvudet.

* Lägg till nya, icke-redigerbara fält för aktivitetsöversikt. Du kan inte lägga till anpassade fält eller fält som kan redigeras. Du kan även visa redigerbara fält som finns i uppgiftshuvudet (till exempel Status eller Procent färdigt).

* Uppgiftshuvudet kan innehålla upp till fem fält.

Före den här versionen gick det bara att anpassa projektrubriker.

Mer information finns i [Anpassa objektrubriker med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Tidig anmälan av nya funktioner för de senaste funktionerna på anslagstavlan

Vi är glada över att kunna öppna nya anslagstavlor för tidig anmälan av funktioner. Det här valfria verktyget är tillgängligt för alla organisationer.

Endast en Workfront-administratör kan välja att använda de tidiga funktionerna. När administratören väljer att använda funktioner i ett tidigt skede är alla användare i organisationen anslutna och de extra funktionerna är aktiverade i din Workfront produktionsmiljö.

Mer information finns i [Anmäl dig till Adobe Workfront Boards för tidig funktion](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## Redigerare för beräkning av anpassat formulärfält visar felinformation

>[!NOTE]
>
>Den här funktionen introducerades först i förhandsvisningsmiljön under 22.3-versionen. Den lanseras i Production med version 22.4.

Det är nu enklare att redigera beräkningar för anpassade fält eftersom felinformation som anges direkt i beräkningen är användbar. När du skapar ett beräknat fält i ett anpassat formulär markeras fel i rosa. När du hovrar över den markerade delen visas ett verktygstips som beskriver vad problemet är.

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migrering till Adobe Unified Experience

OBS! Migreringen har skjutits upp till Q1-Q2 2023. Alla berörda kunder meddelas vid den tidpunkten.

Om din organisation har anslutit sig till Adobe Admin Console migreras din Workfront-instans till Adobe Unified Experience med version 22.4.

Adobe enhetliga upplevelse omfattar:

* En enda inloggning för alla Adobe-program via Adobe Experience Cloud

* En&quot;företagsväljare&quot; för att växla mellan Workfront organisationer och miljöer

* Navigering med alternativ för Workfront-sidor, Adobe Experience Cloud-inställningar och din Workfront-profil

Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412388/){target=_blank}
