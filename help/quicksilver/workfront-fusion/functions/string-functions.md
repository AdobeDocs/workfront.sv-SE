---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Strängfunktioner i Adobe Workfront Fusion
description: Följande strängfunktioner är tillgängliga på panelen för mappning av Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Strängfunktioner i [!DNL Adobe Workfront Fusion]

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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
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

## [!UICONTROL ascii (text; [remove diacritics])]

Tar bort alla tecken som inte är ASCII-tecken från en textsträng.

>[!INFO]
>
>**Exempel:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   Returnerar: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   Returnerar: [!UICONTROL escrz]

## [!UICONTROL base64 (text)]

Omformar text till base64.

>[!INFO]
>
>**Exempel:**
>
>`base64( workfront )`
>
>Returnerar: d29ya2Zyb250==

## [!UICONTROL capitalize (text)]

Konverterar det första tecknet i en textsträng till versaler.

>[!INFO]
>
>**Exempel:**
>
>`capitalize( workfront )`
>
>Returnerar: [!DNL Workfront]

## contains (text; söksträng)

Verifierar om texten innehåller söksträngen.

>[!INFO]
>
>**Exempel:**
>
>* `contains( Hello World ; Hello )`
>
>   Returnerar: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Returnerar: [!UICONTROL false]

## [!UICONTROL decodeURL (text)]

Avkodar specialtecken i en URL till text.

>[!INFO]
>
>**Exempel:**
>`decodeURL( Automate%20your%20workflow )`
>
>Returnerar: [!UICONTROL Automate your workflow]

## [!UICONTROL encodeURL (text)]

Kodar specialtecken i text till en giltig URL-adress.

## [!UICONTROL escapeHTML (text)]

Ignorerar alla HTML-taggar i text.

>[!INFO]
>
>**Exempel:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Returnerar: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Ignorerar alla markeringstaggar i text.

>[!INFO]
>
>**Exempel:**
>
>`escapeMarkdown( # Header )`
>
>Returnerar: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

Returnerar positionen för den första förekomsten av ett angivet värde i en sträng. Den här metoden returnerar &#39;-1&#39; om det värde som söks efter inte finns där. Startvärdet anger var i strängen sökningen ska börja.

>[!INFO]
>
>**Exempel:**
>
>* `indexOf( Workfront ; o )`
>
>   Returnerar: 1
>
>* `indexOf( Workfront ; x )`
>
>   Returnerar: -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   Returnerar: 6

## [!UICONTROL length (text or buffer)]

Returnerar längden på textsträngen (antal tecken) eller binär buffert (buffertstorlek i byte).

>[!INFO]
>
>**Exempel:**
>
>`length( hello )`
>
>Returnerar: 5

## [!UICONTROL lower (text)]

Konverterar alla alfabetiska tecken i en textsträng till gemener.

>[!INFO]
>
>**Exempel:**
>
>`lower( Hello )`
>
>Returnerar: hej

## [!UICONTROL md5 (text)]

Beräknar md5-hash för en sträng.

>[!INFO]
>
>**Exempel:**
>
>`md5( Workfront )`
>
>Returnerar: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL replace (text;search string; replacement string)]

Ersätter söksträngen med den nya strängen.

>[!INFO]
>
>**Exempel:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Returnerar: [!UICONTROL Hi World]

Reguljära uttryck (omges av `/.../`) kan användas som söksträng med en kombination av flaggor (till exempel `g`, `i`, `m`) tillagd:

>[!INFO]
>
>**Exempel:**
>
>![](assets/replace---1-350x31.png)
>
>Alla dessa siffror X X X X X ersätts med X

Ersättningssträngen kan innehålla följande speciella ersättningsmönster:

* `$&` Infogar den matchande delsträngen.
* `$n` Om n är ett positivt heltal som är mindre än 100 infogar delmatchningssträngen med den n:te parentesen. Detta är 1-indexerat.

>[!INFO]
>
>**Exempel:**
>
>![](assets/variable-value-350x63.png)
>
>Returnerar: Telefonnummer `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Returnerar: Telefonnummer: `+420777111222`

>[!CAUTION]
>
>Använd inte namngivna hämtningsgrupper som `/ is (?<number>\d+)/` i ersättningssträngsargumentet. Om du gör det uppstår ett fel.

Mer information om reguljära uttryck finns i [Textparser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (text; [encoding]; [key])]

Beräknar sha1-hash för en sträng. Om nyckelargumentet anges returneras sha1 HMAC-hash i stället. Kodningar som stöds: &quot;hex&quot; (standard), &quot;base64&quot; eller &quot;latin1.&quot;

>[!INFO]
>
>**Exempel:**
>
>`sha1( workfront )`
>
>Returnerar: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [encoding]; [key])]

Beräknar sha256-hash för en sträng. Om nyckelargumentet anges returneras sha256 HMAC-hash i stället. Kodningar som stöds: &quot;hex&quot; (standard), &quot;base64&quot; eller &quot;latin1&quot;.>

>[!INFO]
>
>**Exempel:**
>
>`sha256( workfront )`
>
>Returnerar: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (text; [output encoding]; [key]; [key encoding])]

Beräknar sha512-hash för en sträng. Om nyckelargumentet anges returneras sha512 HMAC-hash i stället.

Kodningar som stöds:

* &quot;[!UICONTROL hex]&quot; (standard)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Nyckelkodningar som stöds:

* &quot;[!UICONTROL text]&quot; (standard)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; eller &quot;[!UICONTROL binary]&quot;

Vid användning av[!UICONTROL binary]&quot;nyckelkodning, en nyckel måste vara en buffert, inte en sträng.

>[!INFO]
>
>**Exempel:**
>
>`sha512(workfront)`
>
>Returnerar: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd19b 85e1e19db58bb44b234493af35fd431639c0345adf2cf7ec26e9f4a7fb19

## [!UICONTROL split (text; separator)]

Delar en sträng i en array med strängar genom att dela strängen i delsträngar.

>[!INFO]
>
>**Exempel:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL startcase (text)]

Ändrar den första bokstaven i varje ord till versaler och gemener i alla andra bokstäver.

>[!INFO]
>
>**Exempel:**
>`startcase( hello WORLD )`
>
>Returnerar: [!UICONTROL Hello World]

## [!UICONTROL stripHTML (text)]

Tar bort alla HTML-taggar från text.

>[!INFO]
>
>**Exempel:**
>
>`stripHTML( <b>Hello</b> )`
>
>Returnerar: Hej

## [!UICONTROL substring (text; start;end)]

Returnerar en del av en textsträng mellan start- och slutpositionen.

>[!INFO]
>
>**Exempel:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Returnerar: Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Returnerar: el

## [!UICONTROL toBinary (value)]

Konverterar alla värden till binära data.

Du kan också ange kodning som ett andra argument för att tillämpa binära konverteringar från hex eller base64 på binära data.

>[!INFO]
>
>**Exempel:**
>
>* `toBinary( Workfront )`
>
>   Returnerar: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Returnerar: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (value)]

Konverterar alla värden till en sträng.

## [!UICONTROL trim (text)]

Tar bort blankstegstecken i början eller slutet av texten.

## [!UICONTROL upper (text)]

Konverterar alla alfabetiska tecken i en textsträng till versaler.

>[!INFO]
>
>**Exempel:**
>
>`upper( Hello )`
>
>Returnerar: [!UICONTROL HELLO]
