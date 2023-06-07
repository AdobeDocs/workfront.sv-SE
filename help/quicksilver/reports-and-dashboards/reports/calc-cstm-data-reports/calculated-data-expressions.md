---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Beräknade datauttryck
description: Du kan använda datauttryck för att definiera beräknade anpassade datafält i Adobe Workfront. De kopplar befintliga Workfront-fält i satser som genererar ett nytt fält.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 0%

---

# Beräknade datauttryck

Du kan använda datauttryck för att definiera beräknade anpassade datafält i Adobe Workfront. De kopplar befintliga Workfront-fält i satser som genererar ett nytt fält.

Du kan använda beräknade datauttryck i:

* Ett anpassat formulär

   Mer information om hur du skapar beräknade anpassade datafält i anpassade formulär i Workfront finns i [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* En beräknad anpassad kolumn i en rapport eller lista när du använder textläge

   Mer information om hur du använder textläge i rapporter och vyer finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntax för beräknade anpassade fält kontra beräknade anpassade kolumner

Även om funktionerna du använder är desamma kan syntaxen för att skapa ett uttryck i ett beräknat anpassat fält skilja sig från den för att skapa en beräknad anpassad kolumn.

Exempel:

* I ett anpassat fält, i ett anpassat formulär för uppgifter, använder du följande för att generera namnet på det överordnade projektet för den uppgift där det anpassade formuläret är kopplat:

   ```
   {project}.{name}
   ```

* I en anpassad kolumn i en rapport använder du följande för att lägga till en anpassad kolumn för projektnamn i en aktivitetsrapport:

   ```
   valuefield=project:name
   ```

   eller

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >Samma syntax gäller för alla rapportelement i textläge där beräkningsuttryck används: vyer, filter, grupperingar, uppmaningar.

Skillnaderna mellan de två syntaxerna är:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Beräknat anpassat fält</strong></td> 
   <td><strong>Element för beräknad anpassad rapportering</strong></td> 
  </tr> 
   <td>Omge fältnamn inom klammerparentes.</td> 
   <td>Omge inte fältnamn inom parenteser eller parenteser när du använder dem i en <code>valuefield </code>linje. <p>Omge fältnamn inom klammerparentes när du använder dem i en <code>valueexpression</code> linje.</p> </td> 
  </tr> 
  <tr> 
   <td>Avgränsa fälten med punkter.</td> 
   <td> <p>Separera fälten med kolon när du använder dem i en <code>valuefield </code>line</p> <p>Separera fälten efter punkter när du använder dem i en <code>valueexpression </code>linje. </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om syntaxen som du måste använda i en beräknad anpassad kolumn finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Datauttryck som du kan använda

I listorna nedan definieras de tillgängliga uttryck som du kan använda när du skapar en av de tre olika typerna av beräknade anpassade fält i Workfront:

* [Datum och tid för beräknade anpassade fält](#date-time-calculated-custom-fields)
* [Matematiskt beräknade anpassade fält](#mathematical-calculated-custom-fields)
* [Textberäknade anpassade fält](#text-calculated-custom-fields)

### Datum och tid för beräknade anpassade fält {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Om du skapar en datum- och tidsberäkning som inte innehåller någon tidsdel, eller som använder datumjokertecknen $$TODAY eller $$NOW, används datumet enligt UTC-zonen (Coordinated Universal Time), inte enligt din lokala tidszon. Detta kan orsaka ett oväntat datumresultat.

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
   <td> <p>Det här uttrycket lägger till antalet dagar till datumet. Talvärdet kan innehålla delar av dagar (t.ex. 1,5 lägger till en och en halv dag till datumet).</p> <p>Uttrycket formateras på följande sätt:</p><pre>ADDDAYS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Det här uttrycket lägger till antalet veckodagar till datumet. Det här uttrycket lägger bara till heltalsvärden till datumet, avrundat nedåt. </p> <p>Uttrycket formateras på följande sätt:</p><pre>ADDWEEKDAYS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Det här uttrycket lägger till antalet månader till datumet och formateras enligt följande:</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Det här uttrycket lägger till antalet år till datumet och formateras enligt följande:</p><pre>ADDYEARS(datum, nummer)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARME</strong> </td> 
   <td> <p>Det här uttrycket rensar tidsdelen av ett datum och formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATUM</strong> </td> 
   <td> <p>Det här uttrycket konverterar en sträng till ett datum och formateras enligt följande:</p><pre>DATE(sträng)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Det här uttrycket returnerar antalet dagar mellan de två datumen, med beaktande av start- och slutdagarna för den valda perioden samt tidsstämplarna för dessa dagar. Om starttiden för startdatumet till exempel är 3 PM räknas inte startdagen som en heldag.</p> <p>Uttrycket formateras på följande sätt:</p><pre>DATEDIFF(datum1, datum2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Det här uttrycket returnerar datum i månaden som ett tal mellan 1 och 31.</p> <p>Uttrycket formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Det här uttrycket returnerar veckodag för datumet som ett tal mellan 1 (söndag) och 7 (lördag).</p> <p>Uttrycket formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINMÅNAD</strong> </td> 
   <td> <p>Det här uttrycket returnerar totalt antal dagar i månaden med datumet som ett tal och formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINSPLITWEEK</strong> </td> 
   <td> <p>Det här uttrycket returnerar totalt antal veckodagar mellan datumet och slutet av veckan, eller slutet av månaden, beroende på vilket som inträffar först. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p> <p>Uttrycket formateras på följande sätt:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAGSINÅRIT</strong> </td> 
   <td> <p>Det här uttrycket returnerar datumets totala dagar som ett tal och formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Det här uttrycket returnerar det senaste datumet i listan och formateras enligt följande:</p><pre>DMAX(datum1, datum2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Det här uttrycket returnerar det tidigaste datumet i listan och formateras enligt följande:</p><pre>DMIN(datum1, datum2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TIMME</strong> </td> 
   <td> <p>Det här uttrycket returnerar timmen för datumet som ett tal mellan 0 och 23.</p> <p>Uttrycket formateras enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUT</strong> </td> 
   <td> <p>Det här uttrycket returnerar datumets minut som ett tal mellan 0 och 60, formaterat enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MÅNAD</strong> </td> 
   <td> <p>Det här uttrycket returnerar datummånaden som ett tal mellan 1 och 12, formaterat enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ANDRA</strong> </td> 
   <td> <p>Det här uttrycket returnerar den andra delen av datumet som ett tal mellan 0 och 60, formaterat enligt följande. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>VECKDAYDIFF</strong> </td> 
   <td> <p>Det här uttrycket returnerar antalet veckodagar mellan två datum, med beaktande av start- och slutdagarna för den valda perioden samt tidsstämplarna för dessa dagar. Om starttiden för startdatumet till exempel är 3 PM räknas inte startdagen som en heldag.</p> <p>Uttrycket formateras på följande sätt:</p><pre>VECKODAYDIFF(datum2, datum1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Det här uttrycket returnerar antalet schemalagda minuter mellan datumen enligt standardschemat.</p> <p>Uttrycket formateras på följande sätt:</p><pre>WORKMINUTESDIFF(datum1, datum2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ÅR</strong> </td> 
   <td> <p>Det här uttrycket returnerar datumåret som ett fyrsiffrigt tal med följande format. I det här exemplet är datumet postdatumet för ett arbetsobjekt.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Matematiskt beräknade anpassade fält {#mathematical-calculated-custom-fields}

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
   <td>Det här uttrycket returnerar det absoluta värdet för talet och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>GENOMSNITTLIG</strong> </td> 
   <td>Det här uttrycket returnerar medelvärdet av tal och formateras enligt följande:<pre>AVERAGE(tal1, tal2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Detta uttryck avrundar ett tal uppåt till närmaste heltal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Det här uttrycket delar upp alla tal i angiven ordning och formateras enligt följande:<pre>DIV(tal1, tal2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOG</strong> </td> 
   <td>Detta uttryck avrundar ett tal nedåt till närmaste heltal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Detta uttryck returnerar talets naturliga logaritmvärde och formateras enligt följande:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Det här uttrycket returnerar logaritmvärdet för number2 till bastalet1 och formateras enligt följande:<pre>LOG(tal1, tal2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Det här uttrycket returnerar det största objektet i listan och formateras enligt följande:<pre>MAX(objekt1, objekt2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Det här uttrycket returnerar det minsta objektet i listan och formateras enligt följande:<pre>MIN(objekt1, objekt2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMMER</strong> </td> 
   <td>Det här uttrycket konverterar en sträng till ett tal och formateras enligt följande:<pre>NUMBER(sträng)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>KRAFT</strong> </td> 
   <td>Detta uttryck returnerar ett tal upphöjt till en potens och formateras enligt följande:<pre>POWER(tal, effekt)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Det här uttrycket multiplicerar alla tal och formateras enligt följande:<pre>PROD(number1, number2, ....)</pre>
   <b>ANMÄRKNING</b>

När du multiplicerar fält som innehåller timmar ska du kontrollera om timmarna i de markerade fälten sparas i minuter, timmar eller sekunder i databasen. Om timmarna sparas i minuter eller sekunder men visas i timmar i Workfront-gränssnittet kan du behöva räkna med konverteringen från minuter eller sekunder till timmar när du skriver ett uttryck med den här beräkningen.
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Det här uttrycket avrundar talet till angivna decimaler och formateras enligt följande:<p>ROUND(tal, precision)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Det här uttrycket ordnar talen i stigande ordning och formateras enligt följande:</p><pre>SORTASCNUM(tal1,tal2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Det här uttrycket ordnar talen i fallande ordning och formateras enligt följande:<pre>SORTDESCNUM(tal1, tal2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Det här uttrycket returnerar en kvadratrot av ett tal och formateras enligt följande. I det här exemplet används antalet objekt under objektet som det anpassade formuläret är kopplat till.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Det här uttrycket subtraherar alla tal i angiven ordning och formateras enligt följande:<pre>SUB(tal1, tal2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Det här uttrycket lägger till alla tal och formateras enligt följande:<pre>SUM(tal1, tal2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Textberäknade anpassade fält {#text-calculated-custom-fields}

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
   <td><strong>ÄRENDE</strong> </td> 
   <td> <p>Det här uttrycket används med andra uttryck för att välja ett värde från en lista baserat på ett indexvärde. Ett indexvärde är ett fält eller en funktion som returnerar ett numeriskt värde (vanligtvis i ett känt intervall).</p> <p>Uttrycket formateras på följande sätt:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>Följande uttryck returnerar till exempel namnet på veckodagen, där 1=söndag, 2=måndag och så vidare, i en beräknad kolumn:</p><pre>FALL(DAYOFWEEK({entryDate}),"söndag","måndag","tisdag","onsdag","torsdag","fredag","lördag")</pre> <p>Det här uttrycket fungerar bäst med andra uttryck som returnerar ett tal, till exempel DAYOFWEEK, DAYOFMONTH och MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>KONKAT</strong> </td> 
   <td> <p>Detta uttryck sammanfogar strängen och formateras enligt följande:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Här följer några exempel på avgränsare som du kan inkludera:</p> 
    <ul> 
     <li>ett blanksteg: " "</li> 
     <li>ett streck: "-"</li> 
     <li>ett snedstreck: "/"</li> 
     <li>komma: ","</li> 
     <li>ett ord: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>INNEHÅLLER</strong> </td> 
   <td>Det här uttrycket returnerar true om strängen findText finns i strängen withinText och har följande format:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Det här uttrycket utelämnar alla specialtecken i strängen så att de kan inkluderas i ett URL-argument.<p>Uttrycket formateras på följande sätt:</p><pre>ENCODEURL(sträng)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Det här uttrycket utvärderar ett villkor som du anger och returnerar värdet för trueExpression om det är true, eller värdet för falseExpression om det är false.</p> <p>Uttrycket formateras på följande sätt:</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>Du kan till exempel jämföra två olika datumfält följt av ett sant/falskt resultat som en datasträng:</p><pre>IF({projiceradSlutförandedatum}&gt;{planeradSlutförandedatum},"Av-spår","På-spår")</pre> <p>I dagligt tal betyder det här uttrycket: "OM mitt objekts beräknade slutförandedatum är "större än" det planerade slutförandedatumet för samma objekt, visar du orden "Från spår" i det här fältet. I annat fall visas ordet"På spår".</p> <p>Om du inte vill märka uttrycken true eller false måste du infoga en tom etikett i programsatsen, till exempel:</p><pre>IF({projiceradSlutförandedatum}&gt;{planeradSlutförandedatum},"","Vid spår")</pre> <p>eller</p><pre>IF({projiceradSlutförandedatum}&gt;{planeradSlutförandedatum},"Av-spår",")</pre> <p>Mer information om att skapa IF-satser finns i <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Översikt över IF-satser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Med det här uttrycket kan du söka efter ett specifikt värde i en sträng med möjliga värden. Om värdet som du söker efter är lika med ett av de angivna värdena returnerar uttrycket trueExpression; I annat fall returneras falseExpression.</p> <p>Uttrycket formateras på följande sätt:</p><pre>IFIN(value, value1, value2,.., trueExpression, falseExpression)</pre> <p>Du kan till exempel hitta en specifik projektägare och markera projekten med en angiven tagg i en projektvy: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> I dagligt tal betyder det här uttrycket: "Om projektägaren är Jennifer Campbell eller Rick Kuvec markerar du det här projektet med"Marketing Team". I annat fall markerar du det med"Andra team".</p> <p> Om du inte vill märka uttrycken true eller false måste du infoga en tom etikett i programsatsen, till exempel: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>eller </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Detta uttryck returnerar true om värdet är lika med ett av de angivna värdena. Annars returneras false.</p> <p>Uttrycket formateras på följande sätt:</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Detta uttryck returnerar true om värdet är null eller tomt; Annars returneras false.</p> <p>Uttrycket formateras på följande sätt:</p><pre>ISBLANK(värde)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>VÄNSTER</strong> </td> 
   <td> <p>Det här uttrycket returnerar ett angivet antal tecken från den vänstra sidan av en sträng och formateras enligt följande:</p><pre>LEFT(sträng, längd)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Det här uttrycket returnerar längden på en sträng och formateras enligt följande:</p><pre>LEN(sträng)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LÄGRE</strong> </td> 
   <td>Det här uttrycket returnerar strängen med gemener och formateras enligt följande:<pre>LOWER(sträng)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ERSÄTT</strong> </td> 
   <td> <p>Det här uttrycket ersätter alla förekomster av sträng2 med sträng3 i sträng1.</p> <p>Uttrycket formateras på följande sätt:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HÖGER</strong> </td> 
   <td> <p>Det här uttrycket returnerar ett angivet antal tecken från strängens högra sida och formateras enligt följande:</p><pre>RIGHT(sträng, längd)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SÖK</strong> </td> 
   <td> <p>Det här uttrycket returnerar indexvärdet för den första förekomsten av findText i strängen withinText, med början vid den angivna startpositionen, eller -1 om texten inte hittas.</p> <p>Uttrycket formateras på följande sätt:</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRÄNG</strong> </td> 
   <td> <p>Det här uttrycket konverterar ett tal till en sträng och formateras enligt följande:</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Det här uttrycket sorterar en lista med strängar i stigande ordning och formateras enligt följande:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Det här uttrycket sorterar en lista med strängar i fallande ordning och formateras enligt följande:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ÄMNE</strong> </td> 
   <td> <p>Det här uttrycket returnerar tecken i en sträng baserat på det start- och slutindex som anges och formateras enligt följande:</p><pre>SUBSTR({string}, antal startpositioner, antal slutpositioner)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Det här uttrycket tar bort mellanrum från början och slutet av en sträng och formateras enligt följande:</p><pre>TRIM(sträng)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ÖVRE</strong> </td> 
   <td> <p>Det här uttrycket returnerar en sträng i versaler och formateras enligt följande:</p><pre>UPPER(sträng)</pre> </td> 
  </tr> 
 </tbody> 
</table>
