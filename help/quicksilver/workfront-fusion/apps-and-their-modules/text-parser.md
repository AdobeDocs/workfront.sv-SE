---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Textparser
description: Du kan använda textanalysverktyget för att tolka text som ska användas i andra [!DNL Adobe Workfront Fusion] scenariomoduler. Textparsern kräver ingen anslutning.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# [!UICONTROL Text parser]

Du kan använda [!UICONTROL Text parser tool] tolka text som ska användas i andra [!DNL Adobe Workfront Fusion] scenariomoduler. The [!UICONTROL Text parser] kräver ingen anslutning.

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

## [!UICONTROL Text parser] moduler och deras fält

När du konfigurerar [!UICONTROL Text parser] moduler, [!DNL Adobe Workfront Fusion] visar fälten som listas nedan. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformers

* [[!UICONTROL Get Elements from HTML]](#get-elements-from-html)
* [[!UICONTROL Get Elements from text]](#get-elements-from-text)
* [[!UICONTROL HTML to Text]](#html-to-text)
* [[!UICONTROL Match Pattern]](#match-pattern)
* [[!UICONTROL Replace]](#replace)

#### [!UICONTROL Get Elements from HTML]

Hämtar önskade element från HTML-kod.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>Aktivera det här alternativet för att se till att modulen inte stoppar scenariot om den inte returnerar några resultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> Markera den typ av element som du vill hämta från HTML-koden. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Ange eller mappa den HTML-kod som du vill hämta de angivna elementtyperna från.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Elements from text]

Tolkar element från text baserat på det angivna mönstret.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>Ange eller mappa texten som du vill tolka.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Markera mönstret som återspeglar elementen som du vill tolka från texten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>Markera den här rutan om du vill ignorera dubblettförekomster av ett textelement.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML to Text]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Ange den HTML-kod som du vill konvertera till oformaterad text.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>Välj typ av radbrytning.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>Aktivera det här alternativet om du vill konvertera text i rubriktaggar (t.ex. &lt;h2&gt; &lt;/h2&gt;) till text med versaler.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Match Pattern]

The [!UICONTROL Match pattern] Med -modulen kan du söka efter och extrahera strängelement som matchar ett sökmönster från en viss text. I den här modulen används reguljära uttryck (kallas även regex eller regexp).

Ett reguljärt uttryck är en teckensekvens där varje tecken antingen är ett metatecken med en speciell innebörd eller ett reguljärt tecken med en litteral betydelse. Dessa tecken och metatecken identifierar ett mönster som kan användas för att söka efter text. Om du t.ex. vill söka efter namn kan du skapa ett reguljärt uttryck som söker efter ett mönster som består av två ord i följd som börjar med versaler. Reguljära uttryck är ett kraftfullt verktyg för att söka efter och ändra text.

En diskussion om reguljära uttryck ligger utanför den här artikelns räckvidd. Vi rekommenderar följande resurser:

* En fullständig lista med metatecken finns på [Reguljära uttryck](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) i MDN-webbdokument.
* Vi rekommenderar en självstudiekurs om hur du skapar reguljära uttryck [RegexOne](https://regexone.com/).
* För att experimentera med reguljära uttryck rekommenderar vi [Reguljära uttryck 101](https://regex101.com/) webbplats. Markera ECMAScript-FLAVOR (JavaScript) på den vänstra panelen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Ange mönstret för det reguljära uttrycket. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extraherar alla siffror i den angivna texten.</p> <p>Obs!  <p>Mönstret ska innehålla minst en hämtningsgrupp inom parentes <code>()</code>. Om mönstret inte innehåller några hämtningsgrupper är utdatapaketet tomt.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Aktivera det här alternativet om du vill hämta alla matchningar i texten. Alla matchningar görs i ett separat paket. Om det här alternativet är inaktiverat hämtar modulen endast den första posten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Aktivera det här alternativet för den här modulen för att behandla text som skiftlägeskänslig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Aktivera det här alternativet för att säkerställa att metatecken för början och slut (<code>^</code> och <code>$</code>) matchar början eller slutet av varje rad, inte bara början eller slutet av hela indatasträngen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivera det här alternativet för att säkerställa att perioden (.) matchar radmatningstecken (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>Aktivera det här alternativet för att se till att modulen inte stoppar scenariot om den inte returnerar några resultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Ange eller mappa den text som du vill matcha mönstret.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace]

Söker efter ett angivet värde eller reguljärt uttryck i den angivna texten och ersätter resultatet med det nya värdet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Ange söktermen. Du kan också använda ett reguljärt uttryck. Mer information om det reguljära uttrycket finns i <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a> -modul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> Ange ett värde som ersätter söktermen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Aktivera det här alternativet om du vill hämta alla matchningar i texten. Alla matchningar görs i ett separat paket. Om det här alternativet är inaktiverat hämtar modulen endast den första posten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Aktivera det här alternativet för den här modulen för att behandla text som skiftlägeskänslig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Aktivera det här alternativet för att säkerställa att metatecken för början och slut (<code>^</code> och <code>$</code>) matchar början eller slutet av varje rad, inte bara början eller slutet av hela indatasträngen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Aktivera det här alternativet för att säkerställa att perioden (.) matchar radmatningstecken (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Ange den text som du vill söka i.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Dataskrapning

Dataskrapning, som ibland kallas webbskrapning, dataextrahering eller webbskörning, är processen att samla in data från webbplatser och lagra dem i din lokala databas eller kalkylblad. Om du vill skrapa data från en webbplats och inte känner till reguljära uttryck, kan du använda ett dataskrapningsverktyg.

Om verktyget för dataskrapning tillhandahåller ett REST API kan du ansluta till det via vårt universella [[!UICONTROL HTTP] moduler](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) och [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) moduler.
