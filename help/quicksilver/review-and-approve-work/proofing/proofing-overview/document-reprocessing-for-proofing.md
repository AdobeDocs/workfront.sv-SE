---
product-area: documents
navigation-topic: proofing-overview
title: Dokumentombearbetning för korrekturläsning - översikt
description: När du skickar ett dokument (DOCX, PDF, XLSX, AI) för korrektur, bearbetar Adobe Workfront om det så att det kan visas i korrekturläsaren utan det program du använde för att skapa det.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Dokumentombearbetning för korrekturläsning - översikt

När du skickar ett dokument (DOCX, PDF, XLSX, AI) för korrektur, bearbetar Adobe Workfront om det så att det kan visas i korrekturläsaren utan det program du använde för att skapa det. 

Varje sida i dokumentet visas i korrekturläsaren som en miniatyrbild. När du klickar på en miniatyrbild kan du zooma in i en bitmappsversion av den sidan med 100 %, 200 % och 400 %. För korrektur som är större än 800 mm i höjd eller bredd är den maximala zoomnivån 200 %.

Färgerna i dokumentet visas i sRGB med färgkonvertering från det senaste Adobe-biblioteket. Språkgranskaren har stöd för ICC-profiler (International Color Consortium) som är inbäddade i dokumentet.

All teckensnittstext extraheras i sitt lager så länge du inkluderar rätt filtillägg när du överför dokumentet till systemet. Text som inkluderas som bilder eller kurvor visas inte.

>[!NOTE]
>
>Workfront stöder för närvarande dokument som innehåller upp till 2 000 sidor. Detta inkluderar kombinerade korrektur. Mer information finns i [Skapa ett korrektur för flera sidor](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Allmänna tips

* Eftersom PDF-filer är de mest standardiserade och tillförlitliga rekommenderar vi att du konverterar dokument till detta format innan du överför dem.
* Använd den senaste versionen av programmet för att skapa originaldokument.
* Om du är osäker på vilka inställningar som ska användas när du sparar eller exporterar dina dokument i det program där du skapade dem använder du standardinställningarna. 
* Glöm inte att bädda in alla teckensnitt du använder i ett dokument. Om du använder anpassade teckensnitt visas dessa teckensnitt endast på de datorer där de är installerade.
* Placera om möjligt alla textelement i de översta lagren i din design. Detta bör säkerställa att texten extraheras och kan markeras i textanteckningsverktyget.
* Placera alla bilder och element i dokumentet. Om du länkar dem från externa källor, t.ex. en annan fil på datorn, visas de inte i det korrektur som du skapar.
* Skapa dokumentet enligt de standarder som rekommenderas för dess typ och optimera det innan du överför det. Detta säkerställer att dokumentet öppnas korrekt i korrekturläsaren, liksom i alla andra program och plattformar.
* Prova att köra preflight-alternativ i designprogrammet för att se om dokumentet genererar några varningar. De här alternativen är tillgängliga i de flesta program som förhandsgranskning av utdata, tryckproduktion och så vidare. Mer information finns i programdokumentationen.
* Kontrollera att färginställningarna är desamma i hela dokumentet.
* Om dokumentet är skyddat mot åtgärder som t.ex. filkopiering kanske inte verktyget för korrekturextrahering kan komma åt innehållet.

## Processtider

Vanligtvis tar bearbetningen några sekunder per sida. Men det kan räcka av olika faktorer, till exempel nätverkstrafik/bandbredd, lokal anslutningshastighet och internationell anslutningshastighet (för användare utanför USA). Följande kan också påverka bearbetningstiden:

* För statiska dokument och bilder: sidantal, siddimensioner, textvolym, bild- och objektkomplexitet (element som flera vektorelement, lager, genomskinlighet).
* För videoklipp: långa varaktigheter, stora dimensioner och kodekar som används.
* För webbklipp: inläsningstider för webbsidor och siddimensioner.

## Processsteg

De skickade filerna går igenom några eller alla följande steg:

1. **Inlämning**. När du överför ett dokument till systemet gör du det på sidan Nytt korrektur eller med ett API. 
1. **Kö**. Under långa trafikperioder kan Workfront behöva placera inskickade data i kö för att förhindra att systemet överbelastas. De flesta korrektur tillbringar bara några sekunder i en kö. 
1. **Bearbetar.** Filerna når bearbetningsmaskinerna enligt innehållstyp. Vi använder olika verktyg för att bearbeta videokorrektur, webbklipp, statiska bilder och dokument. ZIP (Rich Media containers) och Interactive web capture-överföringar kräver inte bearbetning.
