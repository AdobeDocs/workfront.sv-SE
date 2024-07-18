---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Aggregator-modulen i Adobe Workfront Fusion
description: En aggregeringsmodul är en typ av modul som utformats för att sammanfoga flera datapaket till ett enda paket.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# [!UICONTROL Aggregator]-modulen i [!DNL Adobe Workfront Fusion]

En aggregeringsmodul är en typ av modul som utformats för att sammanfoga flera datapaket till ett enda paket.

Mer information om modultyper finns i [Typer av moduler](../../workfront-fusion/modules/module-types.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## modulen [!UICONTROL Aggregator]

När en [!UICONTROL Aggregator]-modul körs gör den följande:

* Ackumulerar alla paket som tas emot under en enda källmoduls åtgärd.
* Ger ett paket med en array som innehåller ett objekt per ackumulerat paket. Innehållet i arrayens objekt beror på den speciella [!UICONTROL Aggregator]-modulen och dess inställningar.

I följande bild visas en typisk inställning för modulen [!UICONTROL Aggregator]:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Modulen från vilken paketaggregeringen börjar. Källmodulen är vanligtvis en iterator eller en sökmodul som matar ut en serie paket. När du konfigurerar aggregatorns källmodul (och stänger aggregatorns inställning), kapslas vägen mellan källmodulen och aggregatormodulen in i ett grått område så att du tydligt kan se början och slutet av aggregeringen. 
   </p> <p>Mer information om iteratorer finns i modulen <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] i [!DNL Adobe Workfront Fusion]</a></p> <p>Mer information om sökmoduler finns i sökmoduler i <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Olika typer av moduler</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>(Gäller endast för modulen [!UICONTROL Array aggregator].) Den målstruktur i vilken data ska aggregeras. Med standardalternativet, [!UICONTROL Custom], kan du välja objekt som ska aggregeras i utdatapaketets <code>Array </code>objekt för A[!UICONTROL rray aggregator]:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>När du ansluter fler moduler efter modulen [!UICONTROL Array aggregator] och återgår till modulens inställningar, kommer listrutan för strukturtypen [!UICONTROL Target] att innehålla alla följande moduler och deras fält av typen Array med samlingar, vilket visas i fältet [!UICONTROL Attachments] i modulen [!DNL Slack] &gt;[!UICONTROL Create a Message]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>Markera de fält som du vill inkludera i aggregeringsmodulens utdata.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Aggregeringsutdata kan delas upp i flera grupper med hjälp av fältet [!UICONTROL Group by]. Fältet [!UICONTROL Group by] kan innehålla en formel som utvärderas för varje aggregators indatapaket. Aggregeringsvärdet genererar sedan ett paket per värde för varje distinkt formel. Varje paket innehåller två objekt:</p> 
    <ul> 
     <li><code>Key </code>innehåller det tydliga värdet.</li> 
     <li><code>Array </code>innehåller aggregerade data från de paket för vilka formeln utvärderades till värdet <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Stoppa bearbetning efter en tom aggregering</p> </td> 
   <td> <p>Som standard genererar modulen [!UICONTROL Aggregator] resultatet av aggregeringen även om inga paket har nått modulen [!UICONTROL Aggregator] (till exempel eftersom alla har filtrerats bort på vägen). Om alternativet [!UICONTROL Stop processing after an empty aggregation] är aktiverat kommer modulen [!UICONTROL Aggregator] inte att generera något utdatapaket i det här fallet och flödet kommer att stoppas.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Paket som genereras av moduler mellan källmodulen och modulen [!UICONTROL Aggregator] skrivs inte ut av modulen [!UICONTROL Aggregator], så de är inte tillgängliga för modulerna i flödet efter [!UICONTROL Aggregator]. Om du behöver data från ett paket som matats ut av en modul mellan källmodulen och [!UICONTROL Aggregator]-modulen, måste du se till att inkludera det angivna objektet i [!UICONTROL Aggregator]-modulens inställningar (som i fältet [!UICONTROL Aggregated fields] i inställningarna för [!UICONTROL Array aggregator] -modulen).


>[!INFO]
>
>**Exempel:** Användningsfall: Zippar alla e-postbilagor och överför ZIP till [!DNL Dropbox]
>
>Scenariot nedan visar hur man gör:
>
>* Titta på en postlåda för inkommande e-post: [!UICONTROL Email] >[!UICONTROL Watch emails] utlösare kommer att generera ett paket med objektet `Attachments[]`, som är en matris som innehåller alla e-postbilagor.
>
>* Iterera e-postens bilagor: [!UICONTROL Email] >[!UICONTROL Iterate attachments] iterator tar objekten från `Attachments[]`-arrayen en i taget och skickar dem vidare som separata paket.
>
>* Sammanställa de paket som skickas från modulen [!UICONTROL Email] >[!UICONTROL Iterate attachments]: [!UICONTROL Archive] >[!UICONTROL Create an archive aggregator] ackumulerar alla paket som tas emot och returnerar ett enda paket som innehåller ZIP-filen.
>
>* Överför den resulterande ZIP-filen till [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Upload a file] hämtar ZIP-filen från modulen [!UICONTROL Archive] > [!UICONTROL Create an archive] och överför den till [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Nedan visas ett exempel på konfiguration av [!UICONTROL Archive] > [!UICONTROL Create an archive]-aggregatorn:
>
>![](assets/archive-create-an-archive-350x484.png)
