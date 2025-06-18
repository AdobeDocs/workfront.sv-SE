---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Översikt över beräknade datauttryck
description: Du kan använda datauttryck för att definiera beräknade anpassade datafält i Adobe Workfront. Beräknade uttryck kopplar befintliga Workfront-fält i satser som genererar ett nytt fält.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: fe9d3cfbb50bfda672360b918d971cc77b0b8b0a
workflow-type: tm+mt
source-wordcount: '2463'
ht-degree: 0%

---

# Översikt över beräknade datauttryck

<!--Audited: 12/2023-->

Du kan använda datauttryck för att definiera beräknade anpassade fält i Adobe Workfront. Beräknade uttryck kopplar befintliga Workfront-fält i satser som genererar ett nytt fält.

Du kan använda beräknade datauttryck i:

* Ett beräknat anpassat fält i ett anpassat formulär

  Mer information om hur du skapar beräknade anpassade fält i anpassade formulär i Workfront finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* En beräknad anpassad kolumn i en rapport eller lista när du använder textläge

  Mer information om hur du använder textläge i rapporter och vyer finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax för beräknade anpassade fält kontra beräknade anpassade kolumner

Även om funktionerna du använder är desamma kan syntaxen för att skapa ett uttryck i ett beräknat anpassat fält skilja sig från den för att skapa en beräknad anpassad kolumn.

Skillnaderna mellan de två syntaxerna är:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Beräknat eget fält</strong></td> 
   <td><strong>Element för beräknad anpassad rapportering</strong></td> 
  </tr> 
   <td>Omge fältnamn inom klammerparentes</td> 
   <td>Omge inte fältnamn inom parentes eller parentes när du använder dem i en <p><code>valuefield </code></p>linje. <p>Omge fältnamn inom klammerparentes när du använder dem i en <p><code>valueexpression</code></p> linje.</p> </td> 
  </tr> 
  <tr> 
   <td>Avgränsa fälten med punkter</td> 
   <td> <p>Separera fälten med kolon när du använder dem i en <p><code>valuefield </code></p>line</p> <p>Separera fälten efter punkter när du använder dem i en <p><code>valueexpression </code></p>linje. </p> </td> 
  </tr> 
 </tbody> 
</table>

Exempel:

* I ett anpassat fält, i ett anpassat formulär för uppgifter, använder du följande för att generera namnet på det överordnade projektet för den uppgift där det anpassade formuläret är kopplat:


  ` {project}.{name}`


* I en anpassad kolumn i en rapport använder du följande för att lägga till en anpassad kolumn för projektnamn i en aktivitetsrapport:


  `valuefield=project:name`


  eller

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >Samma syntax gäller för alla rapportelement i textläge där beräkningsuttryck används: vyer, filter, grupperingar, uppmaningar.

Mer information om syntaxen som du måste använda i en beräknad anpassad kolumn finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Datauttryck som du kan använda

I listorna nedan definieras de tillgängliga uttryck som du kan använda när du skapar en av de tre olika typerna av beräknade anpassade fält i Workfront:

* [Anpassade fält för datum och tid ](#date-time-calculated-custom-fields)
* [Matematiskt beräknade anpassade fält](#mathematical-calculated-custom-fields)
* [Textberäknade anpassade fält](#text-calculated-custom-fields)

Du kan använda uttrycken nedan för att skapa beräknade anpassade kolumner. Du måste dock använda rätt syntax för en beräknad anpassad kolumn, enligt beskrivningen i avsnittet [Syntax för beräknade anpassade fält kontra beräknade anpassade kolumner](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) i den här artikeln.

### Anpassade fält för datum och tid {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Om du skapar en datum- och tidsberäkning som inte innehåller någon tidsdel, eller som använder datumjokertecknen $$TODAY eller $$NOW, används datumet enligt UTC-zonen (Coordinated Universal Time), inte enligt din lokala tidszon. Detta kan orsaka ett oväntat datumresultat.

Du kan skapa ett anpassat datum- eller tidsfält med följande uttryck:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uttryck</th> 
   <th>Förklaring och exempel</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Lägger till antalet dagar till datumet. Talvärdet kan innehålla delar av dagar. 1.5 lägger till exempel till en och en halv dag till datumet.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Lägger till antalet veckodagar till datumet. Det här uttrycket lägger bara till heltalsvärden till datumet, avrundat nedåt. </p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Lägger till antalet månader till datumet och formateras enligt följande:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Lägger till antalet år i datumet och formateras enligt följande:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>Lägger till antalet timmar till datumet och formateras enligt följande:</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Obs! Det här uttrycket stöds inte i Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>RENSA</strong> </td> 
   <td> <p>Rensar tidsdelen av ett datum och formateras enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Konverterar en sträng till ett datum och formateras enligt följande:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Returnerar antalet dagar mellan de två datumen, med beaktande av start- och slutdagarna för den valda perioden samt tidsstämplarna för dessa dagar. Om starttiden för startdatumet till exempel är 3 PM räknas inte startdagen som en hel dag.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Returnerar dag i månaden för datumet som ett tal mellan 1 och 31.</p> <p>Uttrycket formateras på följande sätt. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Returnerar veckodag för datumet som ett tal mellan 1 (söndag) och 7 (lördag).</p> <p>Uttrycket formateras på följande sätt. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINMÅNAD</strong> </td> 
   <td> <p>Returnerar det totala antalet dagar i månaden med datumet som ett tal och formateras enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINSPLITWEEK</strong> </td> 
   <td> <p>Returnerar det totala antalet veckodagar mellan datumet och slutet av veckan, eller slutet av månaden, beroende på vilket som inträffar först. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINYEAR</strong> </td> 
   <td> <p>Returnerar det totala antalet dagar under datumåret som ett tal och formateras enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Returnerar det senaste datumet i listan och har följande format:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Returnerar det tidigaste datumet i listan och formateras enligt följande:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TIMME</strong> </td> 
   <td> <p>Returnerar timmen för datumet som ett tal mellan 0 och 23.</p> <p>Uttrycket formateras på följande sätt. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUT</strong> </td> 
   <td> <p>Returnerar minuten för datumet som ett tal mellan 0 och 60, formaterat enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MÅNAD</strong> </td> 
   <td> <p>Returnerar månaden för datumet som ett tal mellan 1 och 12, formaterat enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ANDRA</strong> </td> 
   <td> <p>Returnerar den andra delen av datumet som ett tal mellan 0 och 60, formaterat enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>VECKODAYDIFF</strong> </td> 
   <td> <p>Returnerar antalet veckodagar mellan två datum, med beaktande av start- och slutdagarna för den valda perioden samt tidsstämplarna för dessa dagar. Om starttiden för startdatumet till exempel är 3 PM räknas inte startdagen som en heldag.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Returnerar antalet schemalagda minuter mellan datumen enligt standardschemat.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ÅR</strong> </td> 
   <td> <p>Returnerar datumåret som ett fyrsiffrigt tal, formaterat enligt följande. I det här exemplet är datumet startdatum för ett arbetsobjekt.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Matematiskt beräknade anpassade fält {#mathematical-calculated-custom-fields}

Du kan skapa ett beräknat anpassat fält som använder några av följande matematiska uttryck:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uttryck</th> 
   <th>Förklaring</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Returnerar talets absoluta värde och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>GENOMSNITT</strong> </td> 
   <td>Returnerar medelvärdet av tal och formateras enligt följande:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Avrundar ett tal uppåt till närmaste heltal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Dividerar alla tal i angiven ordning och med följande format:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Avrundar ett tal nedåt till närmaste heltal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Returnerar det naturliga logaritmvärdet för talet och formateras enligt följande:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOGG</strong> </td> 
   <td>Returnerar logaritmvärdet för number2 till bastalet1 och formateras enligt följande:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Returnerar det största objektet i listan och formateras enligt följande:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Returnerar det minsta objektet i listan och formateras enligt följande:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Konverterar en sträng till ett tal och formateras enligt följande:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>KRAFT</strong> </td> 
   <td>Returnerar ett tal upphöjt till en potens och formateras enligt följande:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multiplicerar alla tal och formateras enligt följande:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>ANMÄRKNING</b></p>

<p>När du multiplicerar fält som innehåller timmar ska du kontrollera om databasen sparar timmarna i markerade fält på några minuter, timmar eller sekunder. Om timmarna sparas i minuter eller sekunder men visas i timmar i Workfront-gränssnittet kan du behöva räkna med konverteringen från minuter eller sekunder till timmar när du skriver ett uttryck med den här beräkningen. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>RUNDA</strong> </td> 
   <td>Avrundar talet upp till angivna decimaler och formateras enligt följande:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordnar talen i stigande ordning och formateras enligt följande:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordnar talen i fallande ordning och formateras enligt följande:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Returnerar en kvadratrot av ett tal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Subtraherar alla tal i angiven ordning och formateras enligt följande:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Lägger till alla tal och formateras enligt följande:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Textberäknade anpassade fält {#text-calculated-custom-fields}

Du kan skapa ett beräknat anpassat fält som visar ett textformaterat värde med följande uttryck:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Uttryck</th> 
   <th>Förklaring</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ARRAY</strong> </td> 
   <td> <p>Konverterar en sträng till en array. Avgränsaren kan vara vilken sträng som helst.</p> 
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>

<tr> 
   <td><strong>ARRAYCONTAINS</strong> </td> 
   <td> <p>Söker efter ett specifikt värde i en lista eller array. Om värdet hittas returnerar funktionen True, annars returneras False. </p> 
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>ARRAYCONTAINS(array, value)</code></p> 
   </td> 
  </tr>


<tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>Returnerar antalet element i arrayen och formateras enligt följande:</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>Returnerar elementet vid det angivna talet i arrayen. Om indexvärdet ligger utanför intervallet returneras tomt.</p> 
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>Ordnar arrayelementen i stigande ordning och konverterar dem till det första elementets typ.</p>
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Till exempel blir ["-12.6", -13.0] ["-12.6", "-13"].</p>
   <p>Obs! Det här uttrycket stöds inte i Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>Ordnar arrayelementen i fallande ordning och konverterar dem till det första elementets typ.</p>
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Till exempel blir ["-12.6", -13.0] ["-13", "-12.6"].</p>
   <p>Obs! Det här uttrycket stöds inte i Workfront Planning.</p></td> 
  </tr>
  <tr>   
   <td><strong>ÄRENDE</strong> </td> 
   <td> <p>Används med andra uttryck för att välja ett värde från en lista baserat på ett indexvärde. </p>
   <p>Ett indexvärde är ett fält eller en funktion som returnerar ett numeriskt värde (vanligtvis i ett känt intervall).</p> 
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Följande uttryck returnerar till exempel namnet på veckodagen, där 1=söndag, 2=måndag och så vidare, i en beräknad kolumn:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Fungerar bäst med andra uttryck som returnerar ett tal, till exempel DAYOFWEEK, DAYOFMONTH och MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>KONKAT</strong> </td> 
   <td> <p>Sammanfogar strängen och formateras enligt följande:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Här följer några exempel på avgränsare som du kan inkludera:</p> 
    <ul> 
     <li>ett blanksteg: " "</li> 
     <li>ett streck: "-"</li> 
     <li>ett snedstreck: "/"</li> 
     <li>ett komma: ","</li> 
     <li>a word: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>INNEHÅLLER</strong> </td> 
   <td>Returnerar true om strängen findText finns i strängen withinText och har följande format:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Undertrycker alla specialtecken i strängen så att de kan inkluderas i ett URL-argument.<p>Uttrycket formateras på följande sätt:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMAT</strong> </td> 
   <td><p>Returnerar formaterad text. Endast de parameteralternativ som anges här tillåts med FORMAT.</p>
   <p>Färgalternativen är $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE och de andra formateringsalternativen är $$BOLD, $$ITALIC, $$UNDERLINE. Endast ett färgalternativ tillåts, tillsammans med upp till tre andra formateringsalternativ. Om inget färgalternativ anges används systemets standardfärg.</p>
   <p>Uttrycket formateras på följande sätt:</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Obs! Det här uttrycket stöds inte i Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Utvärderar ett villkor som du anger och returnerar värdet för trueExpression om det är true, eller värdet för falseExpression om det är false.</p>

<p>Uttrycket formateras på följande sätt:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Du kan till exempel jämföra två olika datumfält följt av ett sant/falskt resultat som en datasträng:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>I det dagliga talet betyder den här satsen:"OM mitt objekts beräknade slutförandedatum är"Större än" det planerade slutförandedatumet för mitt objekt, visar du sedan ordet"Av-spår" i det här fältet. Annars visar du ordet"Vid spår"."</p>

<p>Om du inte vill märka uttrycken true eller false måste du infoga en tom etikett i programsatsen, till exempel:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>eller</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Mer information om hur du skapar IF-satser finns i Översikt över <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref"> IF-satser </a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Gör att du kan söka efter ett specifikt värde i en sträng med möjliga värden. Om värdet som du söker efter är lika med ett av de angivna värdena returnerar uttrycket trueExpression, annars returneras falseExpression.</p> 
   <p>Uttrycket formateras på följande sätt:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Du kan till exempel hitta en specifik projektägare och markera projekten med en angiven tagg i en projektvy: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> I det dagliga talet betyder det här meddelandet:"Om projektägaren är Jennifer Campbell eller Rick Kuvec markerar du projektet med"Marketing Team", annars markerar du det med"Other Teams"."</p> 
    <p> Om du inte vill märka uttrycken true eller false måste du infoga en tom etikett i programsatsen, till exempel: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>eller </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Returnerar true om värdet är lika med ett av de angivna värdena, annars returneras false.</p> <p>Uttrycket formateras på följande sätt:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ÄRBLANK</strong> </td> 
   <td> <p>Returnerar true om värdet är null eller tomt, annars returneras false.</p> <p>Uttrycket formateras på följande sätt:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>VÄNSTER</strong> </td> 
   <td> <p>Returnerar ett angivet antal tecken från den vänstra sidan av en sträng och formateras enligt följande:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Returnerar längden på en sträng och formateras enligt följande:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LÄGRE</strong> </td> 
   <td>Returnerar strängen med gemener och formateras enligt följande:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ERSÄTT</strong> </td> 
   <td> <p>Ersätter alla förekomster av sträng2 med sträng3 i sträng1.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HÖGER</strong> </td> 
   <td> <p>Returnerar ett angivet antal tecken från strängens högra sida och formateras enligt följande:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SÖK</strong> </td> 
   <td> <p>Returnerar indexvärdet för den första förekomsten av findText i strängen withinText, med början vid den angivna startpositionen, eller -1 om texten inte hittas.</p> <p>Uttrycket formateras på följande sätt:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Konverterar ett tal till en sträng och formateras enligt följande:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Sorterar en lista med strängar i stigande ordning och formateras enligt följande:</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Sorterar en lista med strängar i fallande ordning och formateras enligt följande:</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Returnerar tecken i en sträng baserat på det start- och slutindex som anges och formateras enligt följande:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>VÄXLA</strong> </td> 
   <td> <p>Utvärderar uttrycket mot en lista med värden och returnerar resultatet som motsvarar det första matchande värdet.</p>
   <p>Uttrycket formateras enligt följande:</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Det här uttrycket stöds inte i Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Tar bort mellanrum från början och slutet av en sträng och formateras enligt följande:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Returnerar en sträng med versaler och formateras enligt följande:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
