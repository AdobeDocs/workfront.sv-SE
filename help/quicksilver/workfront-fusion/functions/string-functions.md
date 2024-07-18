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
source-git-commit: 0b286e43ed77669329fbee25618394ee5641e428
workflow-type: tm+mt
source-wordcount: '603'
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
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Alla</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licens</td>  
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td>  
   <td> 
   <p>Aktuell: Inga [!DNL Workfront Fusion]-licenskrav.</p> 
   <p>eller</p> 
   <p>Äldre: Alla </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Planen [!DNL Workfront Fusion] ingår.</li></ul> 
   <p>eller</p> 
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL length (text or buffer)]

Returnerar längden på textsträngen (antal tecken) eller binär buffert (buffertstorlek i byte).

>[!INFO]
>
>**Exempel:**
>
>`length( hello )`
>
>Returer: 5

## [!UICONTROL lower (text)]

Konverterar alla alfabetiska tecken i en textsträng till gemener.

>[!INFO]
>
>**Exempel:**
>
>`lower( Hello )`
>
>Returnerar: hej

## [!UICONTROL capitalize (text)]

Konverterar det första tecknet i en textsträng till versaler.

>[!INFO]
>
>**Exempel:**
>
>`capitalize( workfront )`
>
>Returnerar: [!DNL Workfront]

## [!UICONTROL startcase (text)]

Ändrar den första bokstaven i varje ord till versaler och gemener i alla andra bokstäver.

>[!INFO]
>
>**Exempel:**
>`startcase( hello WORLD )`
>
>Returnerar: [!UICONTROL Hello World]

## [!UICONTROL ascii (text; [remove diacritics])]

Tar bort alla icke-ASCII-tecken från en textsträng.

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



## [!UICONTROL replace (text;search string; replacement string)]

Ersätter söksträngen med den nya strängen.

>[!INFO]
>
>**Exempel:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Returnerar: [!UICONTROL Hi World]

Reguljära uttryck (omslutna av `/.../`) kan användas som söksträng med en kombination av flaggor (till exempel `g`, `i`, `m`) tillagda:

>[!INFO]
>
>**Exempel:**
>
>![](assets/replace---1-350x31.png)
>
>Alla dessa siffror X X X X X ersätts med X

Ersättningssträngen kan innehålla följande speciella ersättningsmönster:

* `$&` Infogar den matchande delsträngen.
* `$n` Där n är ett positivt heltal mindre än 100 infogar den n:te parentesala delmatchningssträngen. Detta är 1-indexerat.

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
>Använd inte namngivna hämtningsgrupper som `/ is (?<number>\d+)/` i ersättningssträngargumentet. Om du gör det uppstår ett fel.

Mer information om reguljära uttryck finns i [Textparser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL trim (text)]

Tar bort blankstegstecken i början eller slutet av texten.

## [!UICONTROL upper (text)]

Konverterar alla bokstäver i en textsträng till versaler.

>[!INFO]
>
>**Exempel:**
>
>`upper( Hello )`
>
>Returnerar: [!UICONTROL HELLO]

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
>   Returer: 6

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

## [!UICONTROL encodeURL (text)]

Kodar specialtecken i text till en giltig URL-adress.

## [!UICONTROL decodeURL (text)]

Avkodar specialtecken i en URL till text.

>[!INFO]
>
>**Exempel:**
>`decodeURL( Automate%20your%20workflow )`
>
>Returnerar: [!UICONTROL Automate your workflow]

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

## [!UICONTROL stripHTML (text)]

Tar bort alla HTML-taggar från text.

>[!INFO]
>
>**Exempel:**
>
>`stripHTML( <b>Hello</b> )`
>
>Returnerar: Hej

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

## [!UICONTROL split (text; separator)]

Delar en sträng i en array med strängar genom att dela strängen i delsträngar.

>[!INFO]
>
>**Exempel:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (text)]

Beräknar md5-hash för en sträng.

>[!INFO]
>
>**Exempel:**
>
>`md5( Workfront )`
>
>Returnerar: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (text; [encoding]; [key])]

Beräknar sha1-hash för en sträng. Om nyckelargumentet anges returneras sha1 HMAC-hash i stället. Kodningar som stöds: &quot;hex&quot; (standard), &quot;base64&quot; eller &quot;latin1&quot;.

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
* [!UICONTROL base64]
* [!UICONTROL latin1]

Nyckelkodningar som stöds:

* &quot;[!UICONTROL text]&quot; (standard)
* [!UICONTROL hex]
* [!UICONTROL base64] eller [!UICONTROL binary]

När [!UICONTROL binary]-tangentkodning används måste en nyckel vara en buffert, inte en sträng.

>[!INFO]
>
>**Exempel:**
>
>`sha512(workfront)`
>
>Returnerar: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119 b85e1e19db58bb44b234493af35fd431639c0345adf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (text)]

Omformar text till base64.

>[!INFO]
>
>**Exempel:**
>
>`base64( workfront )`
>
>Returnerar: d29ya2Zyb250===
