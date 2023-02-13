---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Översikt över IF-programsatser
description: Du kan använda IF-programsatser i allmänna programmeringsspråk. I Adobe Workfront kan du använda IF-satser för att jämföra, formatera och strängsätta datafält, både för rapportering och för anpassade datamängder. Att tänka matematiskt på"IF"-satser leder också till en bättre konceptuell förståelse eftersom variabler för uttryck ofta används.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Översikt över IF-satser

Du kan använda IF-programsatser i allmänna programmeringsspråk. I Adobe Workfront kan du använda IF-satser för att jämföra, formatera och strängsätta datafält, både för rapportering och för anpassade datamängder. Att tänka matematiskt på&quot;IF&quot;-satser leder också till en bättre konceptuell förståelse eftersom variabler för uttryck ofta används.

## Recommendations for &quot;IF&quot;-programsatser

Tänk på följande innan du skapar en IF-programsats:

* Vi rekommenderar en grundläggande förståelse för alla allmänna programmeringsspråk, men vi behöver det inte, för den här guiden.
* Vi behöver en mer avancerad förståelse för Workfront textläge. Detta gör det lättare att förstå terminologin i Workfront API och att förstå syntaxen för anpassade data i dessa specifika format.

   Mer information om Workfront API finns i [Grunderna i API](../../../wf-api/general/api-basics.md).

   Mer information om hur du använder textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Du kan skapa IF-satser för följande Workfront-element:

   * Vyer
   * Grupperingar
   * Beräknade anpassade fält

* Du kan inte skapa IF-satser för filter. Detta resulterar i ett &quot;Hopp&quot;-fel i Workfront.
* Supportteamet hjälper inte till med att skapa anpassade data. Du kan kontakta supportteamet när du har skapat anpassade fält eller kolumner och du inte ser önskat resultat. Om du vill ha hjälp med att skapa ett uttryck kan du kontakta din kontoansvarige och fråga om våra konsultalternativ.
* Vi rekommenderar att du först skriver dessa uttryck i en textredigerare, till exempel Sublime eller Visual Studio Code, eftersom det gör att du kan se data tydligare än vad som skulle visas i Workfront.

## Komponenter i en IF-programsats

Du kan skapa IF-satser i Workfront med följande format:
<pre>IF(villkor,sant uttryck,falskt uttryck)</pre>Komponenterna i en IF-programsats är:

* **IF**= Detta är det beräknade Workfront-datauttrycket för &quot;function&quot;. På samma sätt som SUM- och PROD-uttrycken anger detta först att funktionen ska tolkas som en IF-sats. Använd alltid versaler för &quot;IF&quot; i den här kontoutdraget.\
   En lista över alla beräknade datameddelanden finns i [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Villkor**= Detta är villkoret som Workfront-variabeln måste uppfylla och det är grunden för den här ekvationen. Allt som senare kan anges i ekvationen beror på villkoret. Du kan använda ett antal referenser, jämförelser eller matematiska uttryck för att starta en ekvation. Några exempel på villkor är:

   * Ett datum är större än ett annat datum för ett angivet objekt.
   * En status är lika med en av de tillgängliga statusvärdena för ett angivet objekt.
   * Procent färdigt av en uppgift är mindre än eller större än en viss procentandel.

* **Villkorsoperator** = det här är den operator som hjälper dig att skapa villkoret för programsatsen&quot;IF&quot;. &quot;är lika med&quot; eller &quot;är större än&quot; är villkorsoperatorer. En lista över villkorsoperatorer som du kan använda i programsatser finns i [Villkorsoperatorer i beräknade anpassade uttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**= Det här är variabeln &quot;True&quot;, som anger vilken indikator som ska visas när villkoren för villkoret är uppfyllda (sanna indikatorer).

* **Falskt uttryck**= Det här är variabeln &quot;False&quot;, som anger vilken indikator som ska visas för ekvationen när villkoren för villkoret inte uppfylls (falska indikatorer).

I följande exempel används det ursprungliga programsatsformatet för att skriva ett enkelt datauttryck för en IF-programsats. Uttrycket jämför två olika datumfält i Workfront följt av ett True/False-resultat som en datasträng:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

I det dagliga talet skulle det här uttrycket betyda: Om mitt objekts beräknade slutförandedatum är &quot;större än&quot;, det planerade slutförandedatumet för samma objekt, visar du ordet &quot;Av-spår&quot; i det här fältet. Om inte, visa ordet&quot;Vid spår&quot;.

## Skapa beräknade fält i anpassade formulär eller anpassade kolumner med hjälp av IF-satser

Du kan skapa IF-satser i ett beräkningsfält i ett anpassat formulär eller i en anpassad kolumn.

Det finns en skillnad i syntaxen som du använder i ett beräknat anpassat formulär jämfört med en beräknad anpassad kolumn. Se följande exempel:

* [En&quot;IF&quot;-programsats](#single-if-statements)
* [Flera IF-satser](#multiple-if-statements)

### En&quot;IF&quot;-programsats {#single-if-statements}

Nedan följer exempel på ett beräknat anpassat fält och dess motsvarande kolumn som använder en IF-programsats:

* Beräknat anpassat fält:

Använd följande syntax för en IF-sats när du skapar ett anpassat fält:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Beräknad anpassad kolumn:

När du skapar en anpassad kolumn bör du använda följande syntax för programsatsen &quot;IF&quot; på värdeuttrycksraden:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Flera IF-satser {#multiple-if-statements}

Du kan sätta ihop flera IF-satser med följande programsats för att skapa ett mer komplext och dynamiskt uttryck:

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>Observera att det nu inte finns någon falsk programsats för den första"IF". Istället ersatte vi den med början av en andra "IF".

Följande är exempel på ett beräknat anpassat fält och dess motsvarande anpassade kolumn som använder flera IF-satser:

* Beräknat anpassat fält:

   ```
   IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
   ```

* Beräknad anpassad kolumn:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

I det här exemplet har samma sak gjorts genom att sätta ihop två olika kriterievariabler.\
Du kan utforska dessa alternativ ytterligare genom att återskapa exemplen i din egen miljö.

Det bästa sättet att lära sig detta är att experimentera med olika fält och scenarier. Bekanta dig också med API Explorer, som visar fältnamnen som kan användas. Mer information om API Explorer finns i [API Explorer](../../../wf-api/general/api-explorer.md).

Mer information om Workfront-syntax för beräknade datauttryck finns i [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
