---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Visningsbegränsningar för resursplanering
description: För att förbättra prestandan begränsar Adobe Workfront mängden information som du kan visa och mängden information som du kan exportera från resursplaneraren.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Resursplanering - visningsbegränsningar

För att förbättra prestandan begränsar Adobe Workfront mängden information som du kan visa och mängden information som du kan exportera från resursplaneraren.

När du närmar dig den här gränsen visas ett varningsmeddelande i Workfront som talar om att du har nått den gränsen.

Om den information som du förväntar dig visas i resursplaneraren inte visas är det möjligt att du försöker visa för mycket information och vissa data har inte visats på grund av den här begränsningen.

Vi rekommenderar följande för optimala prestanda när du visar och exporterar resursplaneraren:

* Använd filter för att minska mängden information som visas i resursplaneraren och endast visa information som är relevant för dig.
* Använd alla exportalternativ för att minska den mängd information du exporterar samtidigt och för att vara säker på att du bara exporterar relevant information.\
  Mer information om hur du använder filter och exportalternativ i resursplaneraren finns i [Filtrera information i resursplaneraren](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Mer information om att exportera information från resursplaneraren finns i [Exportera information från resursplaneraren](../../resource-mgmt/resource-planning/export-resource-planner.md).

Hur mycket information du kan visa eller exportera beror på vilken vy du använder och vilken miljö du använder för att komma åt resursplaneraren.

## Begränsningar i projektvyn

Tänk på följande när du använder projektvyn på resursplaneraren:

* Du kan bara se projekt som du har åtkomst till för att hantera.
* Du kan expandera varje projekt för att visa roller som är kopplade till det och varje roll för att visa de användare som är kopplade till det.

  Du kan visa upp till 300 projekt när du bläddrar längst ned i listan, såvida det inte finns mer än 30 000 rader med projekt, roller och användare. Du får sedan ett varningsmeddelande om att du har nått gränsen på 30 000 rader.

* Du kan visa tre eller fyra tidsperioder i taget, beroende på skärmstorleken.

Tänk på följande när du exporterar information från projektvyn i resursplaneraren när du har använt alla filter och exportalternativ:

* När du väljer att exportera allt (projekt, roller och användare) i resursplaneraren visas alla objekt som matchar dina villkor i den exporterade filen, oavsett om du har rullat längst ned i listan för att visa dem eller inte.
* Rader utan allokeringsinformation inkluderas i den exporterade filen.

* Du kan exportera upp till 30 000 rader.

## Begränsningar i rollvyn

Tänk på följande när du använder rollvyn i resursplaneraren när du har använt alla lämpliga filter:

* Du kan bara se roller som är kopplade till projekt som du kan hantera.

* Du kan se upp till 300 roller när du bläddrar till slutet av listan, såvida det inte finns mer än 30 000 rader med roller, projekt och användare. Du får sedan ett varningsmeddelande om att du har nått gränsen på 30 000 rader för vad du kan visa på skärmen.
* Du kan expandera varje roll för att visa en lista över projekt och varje projekt för att visa en lista över användare som kan uppfylla de rollerna i projekten.

  20 projekt visas som standard och du kan använda alternativet Läs in mer för att visa ytterligare projekt, eller rulla under varje projekt för att läsa in fler användare.

* Du kan visa tre eller fyra tidsperioder beroende på skärmens storlek.

Tänk på följande när du exporterar information från rollvyn i resursplaneraren när du har använt alla filter och exportalternativ:

* När du väljer att exportera allt (roller, projekt och användare) i resursplaneraren visas alla objekt som matchar dina villkor i den exporterade filen, oavsett om du har rullat längst ned i listan för att visa dem eller inte.
* Rader utan allokeringsinformation inkluderas i den exporterade filen.
* Du kan exportera upp till 30 000 rader.

## Begränsningar i användarvyn

Tänk på följande när du använder användarvyn i resursplaneraren:

* Du kan visa alla användare som uppfyller följande villkor:

   * Du har åtkomst till vyn
   * Är aktiva
   * Har loggat in minst en gång.

* Du kan expandera varje användare för att visa projekt som är kopplade till den och varje projekt för att visa roller som är kopplade till den.\
  De första 50 projekten och rollerna visas som standard, och du kan använda alternativet Läs in mer för att visa ytterligare projekt eller roller.

  >[!NOTE]
  >
  >Om du har filtrerat listan över användare efter projekt kan bara de användare som är kopplade till de filtrerade projekten expanderas och även visa timinformation

* Du kan se upp till 2 000 användare i webbgränssnittet. Workfront visar ett varningsmeddelande när du når den här gränsen.
* Du kan visa tre eller fyra tidsperioder beroende på skärmens storlek.

Tänk på följande när du exporterar information från användarvyn i resursplaneraren, efter att du har använt alla filter och exportalternativ:

* När du väljer att exportera allt (användare, roller och projekt) i resursplaneraren inkluderas alla roller, projekt och användare i den exporterade filen, oavsett om de är utökade eller inte i webbgränssnittet.

* Du kan exportera upp till 30 000 rader som innehåller användare, liksom projekt och roller som listas under, oavsett om du har rullat längst ned i listan för att visa dem eller inte. Alla användare, projekt och roller inkluderas i den exporterade filen, oavsett om de är utökade eller inte i webbgränssnittet.
* Rader utan allokeringsinformation inkluderas i den exporterade filen.
