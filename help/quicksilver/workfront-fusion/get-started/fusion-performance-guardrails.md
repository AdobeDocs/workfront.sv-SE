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
source-git-commit: ec5ed146456c2f75926820f5421bf4feee121399
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] prestandaräkrar

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] kräver en [!DNL Adobe Workfront Fusion]-licens utöver en [!DNL Adobe Workfront license].

Automatisering av arbete kräver snabb bearbetning, så [!DNL Adobe Workfront Fusion] är utformad för höga prestanda. Eftersom långvariga scenarier kan göra arbetet långsammare har vi utformat [!DNL Workfront Fusion] med prestandabevarande säkerhetsdetaljer som begränsar körningstid, datastorlek och andra scenarioparametrar. [!DNL Workfront Fusion]-designers bör vara medvetna om dessa skyddsräcken och införliva dem i sin designpraxis.

## Webbläsare

* Workfront Fusion stöder endast Chrome-baserade webbläsare.

## Scenarier

* Standardtidsgränsen för scenariokörning är **40 minuter**. När körningen når den här tidsgränsen avbryter [!DNL Workfront Fusion] körningen av scenariot efter nästa cykel eller åtgärd, beroende på scenariot. Detta medför att scenariot avbryts kort efter att gränsen på 40 minuter har nåtts
* Den största tillåtna storleken för en scenarioplan är **5 MB**, men vi rekommenderar att du behåller scenariostorleken under **3 MB**.

  Programmoduler som skapar eller uppdaterar data med ett stort antal fält kan orsaka mycket stora utkast.

   * När du använder appen [!DNL Workfront] ska du bara välja fält som behövs för dina användningsfall för att skapa eller uppdatera.
   * När du använder andra program kan du använda anpassade API-moduler för att interagera med valfri posttyp som har ett stort antal fält.

* Även om det inte finns något tak för antalet moduler i ett scenario, påverkar scenarier med fler än 150 moduler prestandan i ditt [!DNL Workfront Fusion]-system negativt. Därför rekommenderar vi inte att du skapar scenarier med fler än 150 moduler.

## Operationer

* Standardåtgärdens timeout är vanligtvis **40 sekunder**.

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
* Webbhooks är begränsade till **100 begäranden per sekund**. När den här gränsen har nåtts skickar Workfront Fusion en 429-status ([!UICONTROL Too Many Requests]).
* [!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den togs emot uppstår felet [!UICONTROL Failed to read file from storage.]
* Webhooks inaktiveras automatiskt om något av följande gäller:

   * Webbkroken har inte varit ansluten till något scenario på mer än fem dagar
   * Webkroken används bara i inaktiva scenarier, som har varit inaktiva i mer än 30 dagar.

* Inaktiverade webhooks tas bort och avregistreras automatiskt om de inte är anslutna till några scenarier och har inaktiverats i över 30 dagar.

## Körningshistorik

* Körningshistorikloggarna är begränsade till storleken **100 MB**. Om körningshistoriken överskrider den här storleken visas endast de första 100 MB.
* Om ett scenario har flera samtidiga körningar. Endast 5 körningar visas i området Körningar på sidan med scenarioinformation. Detta gäller även när fler än fem exekveringar körs.

## Ofullständiga körningar

* Ofullständiga körningar är begränsade till en total storlek på **500 MB**. Om gränsen på 500 MB nås kommer inga fler ofullständiga körningar att lagras.

## Försök igen

* Om ett scenario misslyckas i följd 10 gånger inom en tvåminutersperiod när du använder modulen Bryt och anger direktivet Försök igen inaktiveras scenariot automatiskt.

