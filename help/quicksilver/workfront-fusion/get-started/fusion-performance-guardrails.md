---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scenario,prestanda
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion - prestandaräknare
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: a866fec950343c73712f22a08e2e045e8b80dbd9
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] skyddsräcken

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver [!DNL Adobe Workfront Fusion] utöver en [!DNL Adobe Workfront license].

Automatisering kräver snabb bearbetning, så [!DNL Adobe Workfront Fusion] har utformats för höga prestanda. Eftersom långvariga scenarier kan göra arbetet långsammare har vi utformat [!DNL Workfront Fusion] med prestandabevarande säkerhetsfunktioner som begränsar körningstid, datastorlek och andra scenarioparametrar. [!DNL Workfront Fusion] Designers bör vara medvetna om dessa skyddsräcken och införliva dem i sin designpraxis.

## Webbläsare

Wokfront Fusion stöder endast Chrome-baserade webbläsare.

## Scenarier

* Standardtidsgränsen för scenariokörning är **40 minuter**. När körningen når denna tidsgräns, [!DNL Workfront Fusion] avbryter scenariokörning efter nästa cykel eller åtgärd, beroende på scenariot. Detta medför att scenariot avbryts kort efter att gränsen på 40 minuter har nåtts
* Den största tillåtna storleken för en scenarioplan är **5 MB** men vi rekommenderar att du håller scenariostorleken under **3 MB**.

  Programmoduler som skapar eller uppdaterar data med ett stort antal fält kan orsaka mycket stora utkast.

   * När du använder [!DNL Workfront] ska du bara välja fält som behövs för att skapa eller uppdatera användningsfall.
   * När du använder andra program kan du använda anpassade API-moduler för att interagera med valfri posttyp som har ett stort antal fält.

* Även om det inte finns något tak för antalet moduler i ett scenario, påverkar scenarier med mer än 150 moduler prestandan negativt för dina [!DNL Workfront Fusion] system. Därför rekommenderar vi inte att du skapar scenarier med fler än 150 moduler.

## Operationer

* Standardtidsgränsen för åtgärden är vanligtvis **40 sekunder**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Filer

* Fusions totala bearbetningskapacitet för filer är **1 GB**. Gränsen baseras på en total minneskostnad. Alla operationer bidrar till den kostnaden. Om en fil på 400 MB laddas ned och överförs blir den totala kostnaden för filkapaciteten 800 MB.

## Serverminnesanvändning

* Serverminnesanvändningen för en enskild körning är begränsad till **1 GB**.

  Många faktorer, till exempel stora filer eller komplexa moduler, kan påverka minnesanvändningen på ett sätt som är svårt att förutse eller kontrollera. På grund av detta kan din scenariokörning överskrida minnesgränsen på 1 GB, även om scenariot följer alla andra prestandaskydd. Om du överskrider minnesgränsen misslyckas körningen.

## Webhooks

* Den maximala standardstorleken för en nyttolast är **5 MB**.
* Webhooks är begränsade till **100 begäranden per sekund**. När denna gräns har nåtts skickar Workfront Fusion en 429-siffra ([!UICONTROL Too Many Requests]).
* [!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den togs emot genereras felet &quot;[!UICONTROL Failed to read file from storage.]&quot;
* Webhooks inaktiveras automatiskt om något av följande gäller:

   * Webbkroken har inte varit ansluten till något scenario på mer än fem dagar
   * Webkroken används bara i inaktiva scenarier, som har varit inaktiva i mer än 30 dagar.

* Inaktiverade webhooks tas bort och avregistreras automatiskt om de inte är anslutna till några scenarier och har inaktiverats i över 30 dagar.

## Körningshistorik

* Körningshistorikloggarna är begränsade till en storlek på **100 MB**. Om körningshistoriken överskrider den här storleken visas endast de första 100 MB.

