---
product-area: documents
navigation-topic: proofing-overview
title: Översikt över korrektur av interaktivt material
description: Interaktivt material ger flera sätt att engagera tittarna. Myndigheter kan mäta framgången med sina kampanjer med hjälp av analyser som samlats in från svar på detta innehåll.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Översikt över korrektur av interaktivt material

<!-- Audited: 01/2024 -->

Interaktivt material ger flera sätt att engagera tittarna. Myndigheter kan mäta framgången med sina kampanjer med hjälp av analyser som samlats in från svar på detta innehåll.

Exempel på interaktivt innehåll är:

* Webbplatser
* Inbäddade eller direktuppspelade videor
* Interaktiva banners
* HTML5-animeringar
* Mikroplatser
* Interaktiva e-postmeddelanden

## Skapa korrektur för interaktivt innehåll

Du kan skapa ett korrektur för interaktivt innehåll på något av följande sätt:

* Skapa ett korrektur av en ZIP-fil som innehåller det interaktiva innehållet.

  Adobe Workfront packar upp innehållet från ZIP-filen och lagrar det på en Workfront-server. Eftersom det lagras på det här sättet kan du lita på att innehållet är detsamma under hela korrekturgranskningen.

* Ange innehållets URL.

  Det här är det enklaste sättet att skapa korrektur för interaktivt innehåll. Detta är också det enda sättet att granska ditt innehåll interaktivt när användarna upplever det på Internet.

  Med den här metoden lagrar och värdar en extern server som Workfront inte känner till innehållet.

  Vi rekommenderar den här metoden för stora webbplatser eftersom det är svårt att samla alla filer som utgör en stor webbplats. Eftersom korrekturens innehåll lagras externt kan Workfront inte skydda det mot ändringar som görs av utvecklarna som arbetar med det, så du kanske inte kan lita på att innehållet är detsamma under hela korrekturgranskningsprocessen.

## Förbereda interaktivt innehåll i en ZIP-fil för korrektur

När du paketerar interaktivt innehåll i en ZIP-fil för korrektur måste det innehålla följande specifikationer:

* Alla resurser, som CSS, JavaScript, videor, ljud och bilder, ska inkluderas i paketfilen.
* Interaktivt innehåll ska innehålla huvudfilen (index.html, index.htm). Om den här filen inte placeras på rotplatsen söker verktyget automatiskt efter mappen. Huvudfilen behöver inte ha namnet index.html/index.htm, men det kan bara finnas en .html/.htm-fil på huvudplatsen.
* Filen måste innehålla minst en statisk filwebbsida.
* Den maximala paketstorleken är 500 MB.
* När det gäller ZIP-filer som skapats i iOS identifierar verktyget automatiskt den mapp där innehållet finns.
* Interaktiva projekt stöds bara som ZIP-arkiv. Inlämning av zip-standardfiler misslyckas.
* Webbplatsen måste vara säker (HTTPS).

  Detta är inget krav när du använder Desktop Proofing Viewer.

  Mer information finns i [Förstå Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Webbplatsen måste kunna visas i en iframe.

  Detta är inget krav när du använder Desktop Proofing Viewer.

  Mer information finns i [Förstå Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Skapa ett interaktivt korrektur

Skapa ett interaktivt korrektur när du har förberett ZIP-paketfilen.

Mer information finns i [Skapa ett korrektur för interaktivt innehåll i en ZIP-fil](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Eller, om du använder Workfront Proof, se avsnittet [Generera ett korrektur för interaktivt innehåll](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) i artikeln [Skapa korrektur i Workfront-korrektur](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Granska interaktiva korrektur

Vi rekommenderar att du använder det fristående Desktop Proofing Viewer som standardvisningsprogram för interaktiva korrektur. Om din organisations regler inte tillåter att appen Desktop Proofing Viewer används, kan din Workfront-administratör konfigurera ditt system så att du kan granska interaktivt innehåll som paketerats i en ZIP-arkivfil i Web Proofing Viewer. Jämförande information om Desktop Proofing Viewer och Web Proofing Viewer finns i [Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer - översikt](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
