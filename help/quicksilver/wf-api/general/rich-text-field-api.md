---
content-type: api
navigation-topic: general-api
title: RTF-fält i Adobe Workfront API
description: RTF-fält i Adobe Workfront API
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# RTF-fält i Adobe Workfront API

Vissa objekt i Adobe Workfront tillåter lagring av text med formatering av formaterad text. I Workfront API lagras RTF-text som JSON med hjälp av den öppna källkodsmiljön Draft.js.

## Exempel på översikt

Ett anpassat fält med formatering av formaterad text anropas **Fält med formaterad text** och kan ha följande värden kopplade till sig:

![](assets/rich-text-example-350x158.png)

**Exempel:** En grundläggande begäran om GET för att hämta värdet för det anpassade formulärfältet **Fält med formaterad text**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Exempel:** Denna begäran returnerar värdet för **Fält med formaterad text** i JSON som lagras i **parameterValue** **DE:Fält med formaterad text**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Exempel:** Detta är en formaterad version av svaret som visas i figuren direkt ovan

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Block

JSON-objekten som lagrar RTF-innehållet består av två huvuddelar: **block** och **entityMaps**.

Ett block är ett JSON-objekt som representerar en rad med formaterad text. Eftersom ett enskilt anpassat fält kan innehålla mer än en textrad, har varje textrad ett eget block och varje block representeras som ett element i en överordnad array som kallas **block**.

**Exempel:** Här mappas varje textrad från ett anpassat fält till ett blockelement i arrayblocken

![](assets/copy-of-rich-text-mapping-350x159.png)

Eftersom varje blockelement också är ett JSON-objekt består varje block av elementen: **key**, **text**, **type**, **djup**, **inlineStyleRanges**, **entityRanges** och **data**. Var och en av dessa element fungerar enligt följande:

* **Nyckel** är den unika identifieraren för det blocket. Nyckeln används för att mappa en textrad via entityMaps. Information om entityMaps finns i avsnittet entityMaps i det här dokumentet.
* **Text** är raden med textinnehåll som lagras från det anpassade fältet.
* **Typ** beskriver den typ av text som representeras. En textrad som lagras i ett block kan till exempel vara en del av en lista. Om den textraden var en del av en osorterad lista skulle dess typ definieras som: unordered-list-item.
* Listor stöds för närvarande inte, men bör vara tillgängliga inom kort.
* **Djup** Den här parametern definierar radens djup när raden är en kapslad del av en ordnad eller osorterad lista.
* **inlineStyleRanges** Är en array som beskriver den eller de formattyper som tillämpades på textraden som representeras av det aktuella blocket.

**Exempel:** Här är en inlineStyleRanges-array som beskriver alla format på teckennivå. I detta fall: 9 tecken (längd: 9) med början från index 0 (förskjutning: 0) hade formatet **Fet** använd:

![](assets/copy-of-rich-text-mapping-2-350x136.png)

Om flera typer av formatering har använts på en rad kopplas formaten till ytterligare element i arrayen** inlineStyleRanges**.

**Exempel:** Så här ser ett block ut när du lagrar en textrad som innehåller den blandade formateringen: **Fet text och kursiv**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Alla versioner efter version 20.3 har stöd för formatering med fet stil, kursiv och understrykning.

## EntityMaps och entityRanges

Ett datablock kan innehålla entiteter som hyperlänkar eller andra typer av formatering som är kopplade till datakällor utanför det anpassade textfältet.

## Exempel

### Hämtar oformaterad text från JSON

När ett anpassat fält med formatering av formaterad text skickas, lagras all text i arrayen **block**. Varje rad i den fullständiga texten lagras dock i **textparameter** inom vart och ett av de separata blockelementen som utgör den överordnade arrayen **block**. För att kunna hämta hela texten måste varje separat textrad extraheras och delas upp igen. Detta kan du göra genom att göra en slinga över alla element i blocken och sammanfoga alla textparametrar med en radavgränsare (\n).

**Exempel:** Så här kan din JS se ut:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Spara ett RTF-fältvärde med Workfront API

Så här sparar du följande värden i ett RTF-fält med Workfront API:
<pre>
		Hej <strong>World</strong>!!!
		Det här är min första <strong>RTF</strong></pre>

1. Skapa JSON som representerar värdet för det RTF-fält som du försöker hämta genom att ordna varje textrad i ett blockelement, i arrayen **block**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Fånga formateringen med **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Om du vill fånga den andra raden måste texten &quot;RTF&quot; vara formaterad med både fet och kursiv stil.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >Funktionen EntityMap stöds inte i den första versionen, men det är ändå ett obligatoriskt fält att skicka denna JSON i en begäran

1. Använd **stringify** på den JSON som beskrivs ovan för att skapa en **PUT** begära och skicka uppdateringar

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
