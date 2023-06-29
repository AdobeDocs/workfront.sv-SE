---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Flödeskontroll i Adobe Workfront Fusion
description: När du skapar eller redigerar ett scenario kan du konfigurera inställningar för att styra hur data flödar genom det.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Flödeskontroll i Adobe Workfront Fusion

När du skapar eller redigerar ett scenario kan du konfigurera inställningar för att styra hur data flödar genom det.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Upprepare

Du kan använda en [!UICONTROL Repeater] för att upprepa en uppgift ett visst antal gånger. A [!UICONTROL Repeater] modulen genererar paket, det ena efter det andra.

Du kan till exempel använda en [!UICONTROL Repeater] för att skicka fem e-postmeddelanden med avsnitten &quot;Hello 1&quot;, &quot;Hello 2&quot; och så vidare, genom att ansluta **[!UICONTROL Email]>[!UICONTROL Send me an email]** till [!UICONTROL Repeater] -modul.

Så här använder du en [!UICONTROL Repeater] modul:

1. Klicka på [!UICONTROL Flow Control] icon ![](assets/flow-control-icon.gif) längst ned på skärmen klickar du på **[!UICONTROL Repeater]** på menyn som visas.
1. Klicka på [!UICONTROL Repeater] paketet och klicka sedan på **[!UICONTROL Connect automatically]** i rutan som visas.
1. I [!UICONTROL Flow Control] som visas anger du antalet upprepningar (utgående paket) som du vill ha i dialogrutan **[!UICONTROL Repeats]** box.

   I vårt e-postexempel skriver du 5.

   ![](assets/repeater-2-350x207.png)

   Värdet för objektet ökar i varje repetition med det här värdet som anges i **[!UICONTROL Step]** -fält som du kan visa genom att markera **[!UICONTROL Show advanced settings]**. Numret är som standard 1.

1. Klicka **[!UICONTROL OK]** för att stänga **[!UICONTROL Flow Control]** box.

1. Klicka på appen eller tjänstmodulen som är ansluten till [!UICONTROL Repeater] -modul.
1. Skriv den information som du vill upprepa i rutan som visas.

   I vårt e-postexempel skriver du Hello i [!UICONTROL Subject] box, then map `i` från upprepningsmodulen.

   ![](assets/repeater-3-350x207.png)

| Objekt | Beskrivning |
|---|---|
| [!UICONTROL Initial value] | Ange eller mappa numret som du vill att modulen ska ange som `i` i den första iterationen. Standardvärdet är 1. |
| [!UICONTROL Repeats] | Ange eller mappa det antal gånger som du vill att modulen ska upprepas. Talet måste vara större än eller lika med 0 och mindre än eller lika med 10 000. |
| [!UICONTROL Step] | Detta är talet som modulen ökar värdet för `i`. Standardvärdet är 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Antalet upprepningar bestäms inte av värdet för `i`, som det skulle vara i en slinga i programmeringen. Modulen upprepas det antal gånger som anges i [!UICONTROL Repeats] fält. Värdet `i` ändras för varje iteration i [!DNL repeater] och kan mappas till senare moduler. Exemplet ovan mappar värdet för `i` i Hello-meddelandet, vilket resulterar i meddelanden som innehåller&quot;Hello 1&quot;,&quot;Hello 2&quot; osv.

## [!UICONTROL Iterator]

An [!UICONTROL Iterator] är en särskild typ av modul som konverterar en array till en serie paket. Varje matrisobjekt blir ett separat paket i [!UICONTROL Iterator] modulutdata. Mer information finns i [[!UICONTROL Iterator] modulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Matrisaggregering

En arrayaggregator är en speciell typ av modul som gör det möjligt att sammanfoga flera paket till ett enda paket. Mer information finns i [[!UICONTROL Aggregator] i Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

The [!UICONTROL Router] kan du dela in ditt flöde i flera olika flöden och bearbeta data i varje flöde på olika sätt. En gång en [!UICONTROL Router] modulen tar emot ett paket som vidarebefordrar det till varje ansluten rutt i den ordning som rutterna kopplades till [!UICONTROL Router] -modul. Mer information finns i [Routermodul i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
