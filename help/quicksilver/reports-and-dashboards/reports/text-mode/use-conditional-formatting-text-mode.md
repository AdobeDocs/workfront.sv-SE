---
product-area: reporting
navigation-topic: text-mode-reporting
title: Använda villkorsstyrd formatering i textläge
description: Använda villkorsstyrd formatering i textläge
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 0%

---

# Använda villkorsstyrd formatering i textläge

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

Standardgränssnittsverktyget ger stor flexibilitet när det gäller att skapa rapportelement som uppfyller organisationens behov.

Du kan använda villkorsstyrd formatering i en vy med standardgränssnittet.\
Mer information om hur du använder villkorsstyrd formatering i en vy finns i [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera vyer i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera vyer i en rapport</p> <p>Hantera behörigheter till en vy för att redigera den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Villkorsstyrd formatering i textläge

I textläget kan du skapa mer komplexa vyer, filter, grupperingar och uppmaningar genom att låta dig använda fält som inte finns i standardgränssnittet.

En fullständig lista över alla våra rapportbara fält finns i  [API Explorer](../../../wf-api/general/api-explorer.md).

Mer information om hur du använder textlägessyntax finns i [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Du kan också använda textläge för att formatera vyer i rapporter och listor. Med villkorsstyrd formatering kan du ändra rapportens vyer genom att ändra teckensnittstyp och bakgrund för resultaten i rapporten samt ikoner och flaggor. Vi rekommenderar att du alltid bygger upp dina vyer med standardgränssnittet först och växlar till textlägesgränssnittet endast när det är absolut nödvändigt.

>[!NOTE]
>
> Det går inte att använda CSS-format för att anpassa villkorsstyrd formatering. Du måste i stället använda de fördesignade formateringsalternativen som finns i Adobe Workfront.

## Lägga till villkorsstyrd formatering i vyer

Mer information om hur du använder villkorsstyrd formatering i en vy i standardbygggränssnittet finns i [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Så här lägger du till villkorsstyrd formatering i en vy i textlägesgränssnittet:

1. Gå till en lista med objekt.
1. Expandera den nedrullningsbara menyn för en vy där du vill lägga till villkorsstyrd formatering.
1. Klicka **Anpassa vy**.
1. Klicka på den kolumn i vyn som du vill använda villkorsstyrd formatering på.
1. Klicka **Växla till textläge**.
1. I **Visa i den här kolumnen:** område, klicka **Klicka för att redigera text**.
1. Lägg till kodexemplen i [Formatera vyer med textläge](#format-views-using-text-mode) längst ned i texten i den markerade kolumnen.
1. Klicka **Spara** och sedan klicka **Spara vy**.

## Formatera vyer med textläge {#format-views-using-text-mode}

Du kan lägga till följande komponenter i en kolumn i en vy om du vill formatera den villkorligt i textläge:

* [Kolumninställningar](#column-settings)
* [Kolumnregler](#column-rules)
* [Villkorligt formatera ett värdeuttryck](#conditionally-format-a-valueexpression)

### Kolumninställningar {#column-settings}

Du måste känna till textlägesgränssnittet innan du kan lägga till villkorsstyrd formatering i vyerna.

Du kan anpassa följande element i en kolumn när du använder villkorsstyrd formatering i en vy:

* [Kolumnrubriker](#column-headers)
* [Formatera datum](#format-dates)
* [Formatera tal](#format-numbers)

#### Kolumnrubriker {#column-headers}

Om du vill ändra den kolumnrubrik som visas lägger du till följande kod i kolumnen: `displayname= [Name of column]`. Om du till exempel vill namnge en kolumn som Projektägare ser textkoden ut så här:

```
displayname=Project Owner
```

#### Formatera datum {#format-dates}

Datum kan konfigureras för visning i en mängd olika format.

Mer information finns i [Formatera datum i textlägesrapporter](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### Formatera tal {#format-numbers}

Du kan formatera numeriska värden för att visa information som bäst passar dina rapporteringsbehov.

Mer information finns i [Formatera tal, valuta och procentvärden i textlägesrapporter](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### Kolumnregler {#column-rules}

Med kolumnregler kan du lägga till bilder, färg, formatering och textåsidosättningar i en vy. Kolumnregler kan upprättas oberoende av varandra eller innehålla flera villkor för en kolumn.

* [Villkorsstyrd formatering](#conditional-formatting)
* [Flera villkorsstyrda format](#multiple-conditional-formats)
* [Använd text](#apply-text)
* [Använda radformat](#apply-row-formats)
* [Använd bilder](#apply-images)

#### Villkorsstyrd formatering {#conditional-formatting}

En specifik textlägesprogramsats måste användas när färg eller formatering infogas.

>[!NOTE]
>
>Villkorsstyrd formatering kanske inte stöds i sammanslagna kolumner.\
>Mer information om hur du sammanfogar kolumner med textläge finns i [Visa: sammanfoga information från flera kolumner i en delad kolumn](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Infoga följande kod i en kolumn där du vill lägga till villkorsstyrd formatering:

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>The *styledef.case.0.comparison.icon* -raden är alltid false om du inte arbetar med ikoner.
>
>The *styledef.case.0.comparison.truetext* raden lämnas alltid tom tills du arbetar med att skriva över text.
>
>The *styledef.case.0.comparison.rightText* raden är tom när kvalificeraren inte är tom.

Om vi till exempel vill visa företagsnamnet i grön text i en projektrapport kan du använda följande kod:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* Även om den här programsatsen kan användas för en företagsnamnkolumn, kan den även användas för andra kolumner i rapporten. Grön text visas bara om projektet har ett associerat företag. Kom ihåg `[field name]`, `[value]`och `[qualifier]` kör om konditioneringen slutligen visas i kolumnen eller inte.
>* När vi arbetar med kvalificerare rekommenderar vi att du använder `cicontains` i stället för `equal`. Som standard `equal` söker efter ID-nummer. Använda `cicontains` kan du komma åt objekt efter deras namn.

![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

Oavsett om Textfärg, Justering, Teckensnittsformat eller Bakgrundsfärg används i ett textläge används samma programsats (se ovan).

Följande rader måste ändras för att återspegla motsvarande formatering som behövs för kolumnen:

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Använd följande tabeller för att identifiera vilka rader som behöver ändras och vilka värden du bör ange för att definiera kolumnformatet:

| **Textfärg** | **Rad: textcolor=** |
|---|---|
| Svart | `000000` |
| Mörk blå | `0c6aca` |
| Blågrön | `1b878c` |
| Grön | `03a219` |
| Lila | `6408c4` |
| Grå | `767676` |
| Röd | `d30519` |
| Gul | `e19503` |

{style="table-layout:auto"}

| **Justering** | **Rad: align=** |
|---|---|
| Vänsterjustering | `left` |
| Högerjustering | `right` |
| Centrera | `center` |

{style="table-layout:auto"}

| Teckensnitt | Rad: ***fontstyle=*** |
|---|---|
| Fet | `bold` |
| Kursiv | `italic` |

{style="table-layout:auto"}

| **Bakgrundsfärg** | **Rad: bgcolor=** |
|---|---|
| Blågrön | `dcf6f7` |
| Grön | `def6e2` |
| Grå | `e8e8e8` |
| Blå | `e8f1ff` |
| Lila | `e9def4` |
| Röd | `eac6c9` |
| Gul | `feecc8` |
| Vit | `ffffff` |

{style="table-layout:auto"}

#### Flera villkorsstyrda format {#multiple-conditional-formats}

Du kan använda mer än ett formateringsformat på en sats. Programsatsen core förblir oförändrad och eventuella ytterligare formateringsuttryck läggs till i programsatsen.

Om du till exempel använder den tidigare programsatsen för att inkludera företagsnamn i grön, fetstilt text. Programsatsen skulle skrivas med följande kod:

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>Om du inkluderar mer än ett villkorsstyrt formateringsuttryck måste varje uttryck i programsatsen identifieras numeriskt. Observera att uttryck 0 och uttryck 1 har identifierats.

#### Använd text {#apply-text}

Om du vill ersätta de standardvärden som finns i en kolumn med ett valfritt värde, är det möjligt att använda text i kolumnen.

I en projektrapport anger du till exempel att kolumnvärdet för Planerat startdatum inte ska visa det planerade startdatumet för projektet, utan istället texten&quot;Inte idag&quot;. Använd följande kod för kolumnen Planerat startdatum:

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>Raderna som börjar med `case.0.` jämföra skiftläge med att identifiera textanvändning. Raderna som börjar med **styledef.case.0.** är tidiga villkorsstyrda formateringssatser där vi identifierar textanvändning via `truetext` -uttryck. Se till att ange `truetext` till ett värde i stället för att lämna det tomt.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### Använda radformat {#apply-row-formats}

Om du vill använda ett villkor för hela raden använder du följande kod tillsammans med kolumnkoden:

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### Använd bilder {#apply-images}

På samma sätt som för formatering med text kan bilder användas för att visa information i rapporter. Workfront har ett antal inbyggda bilder för att förmedla visuell information i en rapportinställning. Om du vill använda bilder i den villkorliga formateringsinställningen krävs följande programsats:

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

Om du till exempel har en projektrapport vill du skapa en kolumn där du vill visa ett urholkat ansikte för varje planerat slutförandedatum som inte är lika med dagens datum. Använd följande textlägeskod för att lägga till ikonen i kolumnen:

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>Observera att programsatsen använder `icon=true` -uttryck. Programsatsen skiljer sig också från andra villkorliga formateringssatser eftersom den inte använder `style.def` -format, men i stället ett unikt bildformat.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

Om du vill använda de bilder som är tillgängliga använder du följande kod och värden:

| **Ikon** | **Rad: image.case.0.comparison.truetext=** |
|---|---|
| Frostat ansikte ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Glad ansikte ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Blå flagga  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Grön flagga  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Röd flagga  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Gul flagga  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Svart cirkel  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Blå cirkel ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Grå cirkel ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Grön cirkel ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Orange cirkel ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Rosa cirkel ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Lila cirkel ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Röd cirkel ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Vit cirkel ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Gul cirkel ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style="table-layout:auto"}

### Formatera en `valueexpression` {#conditionally-format-a-valueexpression}

Om du vill visa ett beräknat värde i en kolumn kan du ersätta `valuefield` kodrad i kolumnen med en `valueexpression`. Med ett beräknat värde kan du visa ett nytt värde för ett objekt baserat på beräkningen mellan två befintliga fält på samma objekt.

Mer information om hur du formaterar `valueexpression line`, se [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Du kan inte villkorligt formatera en kolumn som innehåller en `valueexpression` kodrad. I stället kan du lägga till ett beräknat anpassat fält i ett anpassat formulär och koppla det till de objekt som visas i rapporten. Sedan kan du villkorligt formatera kolumnerna som visar det här fältet.

Mer information om beräknade anpassade fält finns i [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Lägga till ett aggregeringsvärde i en textlägeskolumn

Vi rekommenderar att du skapar kolumnen i Builder-gränssnittet först, lägger till aggregeringsvärdet där och sedan redigerar kolumnen i textläge.

Tänk på följande när du lägger till aggregerare i en kolumn i textläge:

* Värdena i kolumnen måste ha ett format som kan sammanfattas. De måste till exempel ha något av följande format:

   * Nummer
   * Datum
   * Valuta

* Du kan lägga till en aggregator i en kolumn som visar en beräkning. Det aggregerade värdet visas i grupperingen av vyn eller rapporten. Mer information finns i [Gruppering: visa resultatet av att aggregera flera beräknade värden i en gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* Kodraderna för definitionen av kolumnen måste vara identiska med kodraderna som inför aggregatorn och föregås av &quot;aggregator&quot;. Om du till exempel har en kolumn där du visar Planerade timmar i ett projekt, är textläget för kolumnhuvudraderna:

  ```
  valuefield=workRequired
  valueformat=compound
  ```

  När du vill aggregera värdet för alla rader i vygrupperingen kan vi lägga till följande kod för att lägga till aggregeringsvärdena: `aggregator.valuefield=workRequired` ( `aggregator.valuefield` raden måste vara samma som `valuefield` som beskriver kolumnen) `aggregator.valueformat=compound` ( `aggregator.valueformat` raden måste ha samma värde som `valueformat` som beskriver kolumnen) `aggregator.function=SUM` (det här är en obligatorisk rad som anger hur du vill samla kolumnen, och i det här fallet vill du lägga till alla enskilda planerade timmar i ett nummer på grupperingsraden) `aggregator.displayformat=minutesAsHoursString` (eftersom timmar lagras i Workfront på några minuter vill vi ange `displayformat` i timmar när de lagras i minuter)
