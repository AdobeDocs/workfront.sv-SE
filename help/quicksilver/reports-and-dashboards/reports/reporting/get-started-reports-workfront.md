---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Kom igång med rapporter i Adobe Workfront
description: Rapporterna ger insyn i vad som händer med användare och arbete. Med hjälp av rapporter kan du visa information om objekt i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '3449'
ht-degree: 0%

---

# Kom igång med rapporter i Adobe Workfront

Rapporterna ger insyn i vad som händer med användare och arbete. Med hjälp av rapporter kan du visa information om objekt i Adobe Workfront.

Mer information om hur du förstår objekt och hur de kan rapporteras i Workfront-programmet finns i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Rapportelement

Rapporterna är en kombination av följande tre element i Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Visa</td> 
   <td> <li>Definierar kolumnerna i rapporten och vilken information du kan inkludera i varje kolumn.</li> <li>Mer information om vyer finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Översikt över vyer i Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gruppering</td> 
   <td> <li>Kategoriserar information baserat på en vanlig informationsdel och visar resultatet av rapporten under blå rubriker.</li> <li>Mer information om grupperingar finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Översikt över grupperingar i Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <li>Styr mängden information som visas i en rapport.</li> <li>Mer information om filter finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Översikt över filter i Adobe Workfront</a>.</li> <li>Mer information om filtermodifierare finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- och villkorsmodifierare</a>.</li> <li>Du kan filtrera med jokertecken för att göra filtren mer allmänna och ge dem mer flexibilitet.</li> <li>Mer information om hur du använder jokertecken i filter finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variabler för jokertecken</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>När du väljer ett nytt filter, en ny vy eller en gruppering i en lista behålls markeringen även om du loggar ut från Workfront eller stänger webbläsaren.

Mer information om rapportelement finns i artikeln [Rapportelement: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Du kan förbättra dina rapporter genom att lägga till följande element:

* Ett diagram: en visuell representation av resultaten i rapporten.\
   Mer information om diagramrapporter finns i artikeln [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* En matrisgruppering: sammanfattar informationen i rapporten i ett aggregerat tabellformat.\
   Mer information om matrisrapporter finns i artikeln [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* A prompt: ett öppet filter som du kan anpassa och använda på olika sätt varje gång du kör rapporten.\
   Mer information om uppmaningar finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

När du skapar en rapport kan du ändra dessa element individuellt i rapportverktyget.

Ett annat sätt att göra informationen i dina rapporter mer relevant är genom att använda villkorsstyrd formatering i dina vyer.\
Mer information om att använda villkorsstyrd formatering finns i [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Systemrapporter

Workfront tillhandahåller flera systemrapporter som hämtas till ditt system som standard.\
När du har angett information i systemet kan du använda dessa rapporter för att visa informationen visuellt.

Mer information om hur du får åtkomst till systemrapporter finns i avsnittet [Använd inbyggda rapporter från Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md) i artikeln [Använd inbyggda rapporter från Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Mer information om vilka systemrapporter som är tillgängliga finns i artikeln [Använd inbyggda rapporter från Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Skapa rapporter

Utöver systemrapporterna som Workfront tillhandahåller kan du skapa egna anpassade rapporter som passar organisationens behov.

Om du vill skapa en rapport kan du göra något av följande:

* Bygg en helt ny rapport.
* Kopiera en befintlig rapport.\
   Du måste ha minst behörigheten Visa för att kunna kopiera en rapport som har skapats av någon annan. Mer information om hur du kopierar en rapport finns i artikeln [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Mer information om hur du skapar rapporter finns i artikeln [Översikt över kalenderrapporter](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* [Krav för att skapa rapporter](#prerequisites-for-creating-reports)
* [Anmäl ägarskap](#report-ownership)
* [Skapa rapporter i Builder-gränssnittet](#create-reports-in-the-builder-interface)
* [Skapa rapporter i textläge](#create-reports-in-text-mode)

### Krav för att skapa rapporter {#prerequisites-for-creating-reports}

* Du måste ha en planlicens för att kunna skapa egna rapporter.\
   Mer information om Workfront License Types finns i artikeln [Översikt över Adobe Workfront-licenser](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

* Din Workfront-administratör måste ge dig åtkomst till Redigera rapporter på din åtkomstnivå.\
   Mer information om hur du beviljar åtkomst till redigeringsrapporter finns i artikeln [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Din Workfront-administratör måste ge dig åtkomst till Redigera filter, Vyer och grupperingar på din åtkomstnivå.

   Mer information om hur du ger åtkomst till redigeringsfilter, vyer och grupperingar finns i [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Du måste definiera ett objekt som du vill rapportera om. Rapporterna är objektspecifika i Workfront och du måste börja med att välja en objekttyp innan du kan börja skapa rapporten. Du kan bara rapportera om objekt som är tillgängliga i Workfront gränssnitt.

### Anmäl ägarskap {#report-ownership}

När du skapar en rapport i Workfront blir du standardägare av rapporten och den visas i avsnittet Mina rapporter. Du kan inte ändra rapportens ägare.

När du kopierar en rapport blir du automatiskt ägare till den kopierade rapporten.

Information om hur du kopierar rapporter finns i artikeln [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Du kan se vem som äger en rapport genom att kontrollera **Anges av** fält.

![](assets/nwe-entered-by-350x218.png)

### Skapa rapporter i Builder-gränssnittet {#create-reports-in-the-builder-interface}

Vi rekommenderar att du använder gränssnittet för att skapa rapporter först för att skapa en ny rapport. Gränssnittet innehåller en smidig uppsättning verktyg som hjälper dig att sätta ihop olika element för att skapa den rapport du vill ha. Du har objekt och fält som du kan välja från listor och lägga till i alla rapportelement.\
Mer information om hur du skapar rapporter i rapportbygggränssnittet finns i artikeln [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

En lista med objekt som du kan rapportera om finns i [Rapport om objekt](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Mer information om fälten som du kan visa i rapporter finns i artikeln [Ordlista för Adobe Workfront-terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Skapa rapporter i textläge {#create-reports-in-text-mode}

Ibland kanske du inte kan hitta vissa fält i Builder-gränssnittet, men de kan finnas i API:t.\
Mer information om vilka fält som är tillgängliga i API:t finns i artikeln [API Explorer](../../../wf-api/general/api-explorer.md).

Mer information om hur du använder API-utforskaren finns i artikeln [Använda API Explorer](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>Du kan inte rapportera objekt som inte är tillgängliga i Report Builder i Workfront-gränssnittet. Du kan dock rapportera fält som är kopplade till objekten i rapportbyggaren om dessa fält är tillgängliga via API:t. Du måste använda gränssnittet Textläge för att göra detta.

I textläget kan du skapa mer komplexa vyer, filter, grupperingar och uppmaningar genom att låta dig använda fält som inte är tillgängliga i standardlägesgränssnittet.

* [Terminologi för textläge](#text-mode-terminology)
* [Beräknade kolumner, Villkorlig formatering och andra användningsområden för textläge](#calculated-columns-conditional-formatting-and-other-uses-of-text-mode)
* [Textlägesexempel](#text-mode-samples)

#### Terminologi för textläge {#text-mode-terminology}

Du måste använda en specifik syntax för att använda Workfront textläge.

Mer information om Workfront syntax för textläge finns i [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Beräknade kolumner, Villkorlig formatering och andra användningsområden för textläge {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

Förutom att rapportera om fält som inte är tillgängliga i Builder-gränssnittet kan du använda textläge för att visa beräkningar eller jämförelser mellan vissa fält.

En lista över de vanligaste användningsområdena för textläge i en rapport finns i artikeln [Översikt över vanliga användningsområden för textläge](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Mer information om hur du inkluderar beräknade anpassade data i rapporter finns i avsnittet [Beräknade anpassade data i rapporter](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Mer information om hur du jämför fält i villkorsstyrd formatering finns i artikeln [Jämför fält i villkorsstyrd formatering](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

Du kan även referera till samlingsfält med hjälp av textläge i rapporter.\
Mer information om hur du använder textläge för att visa samlingsinformation i en rapport finns i artikeln [Referenssamlingar i en rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Textlägesexempel {#text-mode-samples}

Vi har ett bibliotek med exempel på de mest använda vyerna, filtren och grupperingarna som du kan skapa i textläge.

Om du vill bläddra i det här biblioteket och använda några av de exempel vi erbjuder kan du läsa artikeln [Exempel på anpassad vy, filter och gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Flikarna i en rapport

En rapport kan innehålla flera flikar när du kör rapporten i gränssnittet.

Mer information om hur du kör en rapport finns i artikeln [Köra en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

På varje flik visas den information du inkluderar i rapporten i något olika format. Välj det format som bäst passar er organisation.

Du kan göra vilken flik som helst till rapportens standardflik. Standardfliken är den första fliken som visas när du klickar på namnet på en rapport för att öppna den, och det är den flik som visas när du placerar rapporten på en kontrollpanel.

Beroende på vilka element du väljer i rapporten kan rapporten innehålla följande flikar:

* [Fliken Detaljer](#details-tab)
* [Fliken Sammanfattning](#summary-tab)
* [Fliken Matris](#matrix-tab)
* [Fliken Diagram](#chart-tab)
* [Fliken Fråga](#prompts-tab)

### Fliken Detaljer {#details-tab}

Fliken Detaljer i en rapport visar rapporternas objekt och de attribut du väljer för objektet i ett listformulär. Varje rapport har en flik Detaljer.

>[!IMPORTANT]
>
>Information på fliken Detaljer kan visas på ett annat sätt än på fliken Diagram beroende på din tidszon.\
>Till exempel slutförde en användare i Kalifornien en uppgift kl. 21.30 PST den 12 februari. När en användare i New York visar en rapport som innehåller den här uppgiften som slutförd, visas det faktiska slutförandedatumet som den 13 februari på båda fliken Information eftersom den slutfördes kl. 12.30 den 13 februari. I diagrammet inkluderas det dock i grupperingen 12 februari tills du expanderar diagramelementet.

### Fliken Sammanfattning {#summary-tab}

Rapporter som innehåller en gruppering har fliken Sammanfattning.

Samma information som visas i listformat på fliken Detaljer sammanfattas och sammanställs enligt grupperingarna i rapporten på fliken Sammanfattning.

Mer information om grupperingar finns i artikeln [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Fliken Matris {#matrix-tab}

Rapporter som innehåller en matrisgruppering har en matrisflik.

Samma information som visas i listformat på fliken Detaljer visas i ett tabellformat, grupperat efter grupperingarna i rapporten på fliken Matris.

När du lägger till en matrisgruppering i en rapport ersätts fliken Sammanfattning av fliken Matris.

Mer information om hur du skapar en matrisgruppering finns i artikeln [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Fliken Diagram {#chart-tab}

Rapporter som innehåller ett diagram har en diagramflik.

Överväg att inkludera ett diagram i rapporterna för att se hur effektiva statuspanelerna är för era chefer. Diagram är ett koncist sätt att visa informationen i en rapport. Du kan expandera ett diagramelement genom att klicka på det, så visas de objekt som ingår i det elementet.

>[!IMPORTANT]
>
>När du klickar på ett diagramelement kan den utökade informationen visas på ett annat sätt än det diagram som är baserat på din tidszon.\
>Till exempel slutförde en användare i Kalifornien en uppgift kl. 21.30 PST den 12 februari. När en användare i New York visar en rapport som innehåller den här uppgiften som slutförd, visas det faktiska slutförandedatumet som den 13 februari på både fliken Information och diagraminformationen eftersom den slutfördes kl. 12.30 EST den 13 februari. I diagrammet inkluderas det dock i grupperingen 12 februari tills du expanderar diagramelementet.

Mer information om hur du skapar en rapport med ett diagram finns i artikeln [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Fliken Fråga {#prompts-tab}

Rapporter som innehåller en fråga har fliken Fråga.

Med en uppmaning kan du lägga till ett filter i en rapport varje gång du kör rapporten. När du lägger till en fråga i rapporten blir fliken Fråga automatiskt rapportens standardflik. Detta kan inte ändras till en annan flik.

Mer information om hur du skapar ett meddelande för en rapport finns i artikeln [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Dela rapporter

När du har skapat en rapport kan du dela den med andra användare.

Du kan dela en rapport med andra användare på följande sätt:

* [Ge delningsbehörigheter till en rapport](#give-sharing-permissions-to-a-report)
* [Boka en rapportleverans](#schedule-a-report-delivery)
* [Exportera resultatet av en rapport](#export-the-results-of-a-report)
* [Lägga till en rapport på en instrumentpanel](#add-a-report-to-a-dashboard)

### Ge delningsbehörigheter till en rapport {#give-sharing-permissions-to-a-report}

Du kan ge delningsbehörigheter till en annan användare för att visa eller hantera en rapport som du skapar. Du kan ge en annan användare en behörighetsnivå som är lika med eller mindre än din. Du kan även göra en rapport offentlig med delningsbehörigheter. Mer information om hur du delar en rapport finns i [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Boka en rapportleverans {#schedule-a-report-delivery}

Du kan schemalägga en rapport för leverans. De användare som du delar rapporten med får ett e-postmeddelande med en bifogad rapport. Den bifogade filen kan ha följande format:

* HTML
* PDF
* Excel
* .TSV

Mer information om schemaläggning av rapportleverans finns i artikeln [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Exportera resultatet av en rapport {#export-the-results-of-a-report}

Du kan exportera resultatet av en rapport till följande filformat

* PDF
* Excel (.xls- och .xlsx-format)
* Tabbavgränsad

Mer information om hur du exporterar resultaten från en rapport finns i artikeln [Exportera data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

När rapporten har exporterats till något av dessa format kan du dela den med andra användare genom att skicka den med e-post som en bifogad fil eller skriva ut den.

### Lägga till en rapport på en instrumentpanel {#add-a-report-to-a-dashboard}

Du kan lägga till en rapport på en kontrollpanel och dela kontrollpanelen med andra användare. Mer information om hur du lägger till rapporter på en kontrollpanel finns i artikeln [Lägga till en rapport på en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Skapa kalendrar

Om du vill visa data i ett kalenderformat kan du skapa kalendrar i stället för rapporter.

Mer information om hur du skapar kalendrar finns i artikeln.

Mer information om hur du använder kalendrar finns i artikeln [Översikt över kalenderrapporter](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Rapportanvändning

När du har skapat rapporter och delat dem med andra användare kan du spåra hur ofta de använder dessa rapporter.\
Mer information om rapportanvändning, inklusive hur ofta de visas, vilken användare och vilka instrumentpaneler de visas på finns i artikeln [Översikt över rapportanvändning](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Vanliga termer som används som referens för rapporter

Följande termer används som referens för Workfront-rapporter:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Term eller fras</strong> </th> 
   <th><strong>Definition</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Avancerade alternativ</td> 
   <td> <p>Hänvisar till länken på fliken Kolumner (Visa) i rapportverktyget som ger möjlighet att göra följande:</p> 
    <ul> 
     <li>Ange villkorsstyrd formatering för text och bilder baserat på villkor som du väljer.</li> 
     <li>Ge kolumnen ett nytt namn.</li> 
     <li>Formatera värdena i kolumnen.</li> 
    </ul> <p>Du kan till exempel visa alla överordnade uppgifter i fet stil eller visa det planerade slutförandedatumet i rött om aktiviteten är sen.</p> </td> 
  </tr> 
  <tr> 
   <td>Attribut</td> 
   <td> Fältet för ett objekt enligt definitionen i databasen. Den används i ett textlägesuttryck. <br>Statusfältet visas som <em>status</em> när det används i ett textlägesuttryck. </td> 
  </tr> 
  <tr> 
   <td>Bean eller JavaBean</td> 
   <td>En Bean representerar ett återanvändbart programmeringselement. Termen Bean identifierar relationer mellan olika objekt i Workfront-programmet. Det är viktigt att du känner till dessa relationer när du försöker visa ytterligare attribut för ett objekt som inte är tillgängliga i de grundläggande rapportverktygen.</td> 
  </tr> 
  <tr> 
   <td>Builder Interface eller Report Builder</td> 
   <td>Gränssnittet Builder är den serie med nedrullningsbara menyer som innehåller fält som visas på flikarna Kolumner(Visa), Filter och Gruppering. Den ger en intuitiv mappning av Bean-relationerna som gör det lättare att identifiera kolumnerna i en vy, kriterierna för ett filter och de gemensamma attributen för en gruppering.</td> 
  </tr> 
  <tr> 
   <td>Camera Case</td> 
   <td> <p>Camel Case refererar till ett specifikt sätt att skriva programmeringselement till strängar för flerordsattribut tillsammans. När du stavar ett attribut i Camera Case är den första bokstaven i det första ordet gemen, det finns inget mellanrum mellan orden, och den första bokstaven i efterföljande ord är versaler.</p> <p>Hemgrupp skrivs till exempel som <em>homeGroup</em>, resurspoolen blir <em>resourcePool</em>och faktiskt startdatum blir <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Diagram</td> 
   <td> <p>En flik i Report Builder, en rapportflik, när du har sparat rapporten, samt ett valfritt element i en rapport som du kan använda för att lägga till ett diagram i en rapport. Du måste definiera en gruppering i rapporten innan du kan skapa ett diagram.</p> <p>Följande typer av diagram kan läggas till i alla rapporter:<br></p> 
    <ul> 
     <li>Kolumn</li> 
     <li>Liggande</li> 
     <li>Cirkel</li> 
     <li>Linje</li> 
     <li>Mätare</li> 
     <li>Bubbla</li> 
    </ul> <p>Mer information om hur du lägger till diagram i rapporter finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Lägga till ett diagram i en rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Detaljer</td> 
   <td>Det här är en av flikarna i en rapport när du har sparat rapporten. Här visas resultatet av rapporten, som visas i den vy och gruppering som du väljer.</td> 
  </tr> 
  <tr> 
   <td>Uttryck</td> 
   <td>Ett uttryck är en skriven formel i textläge som förmedlar information som du kan söka efter eller visa i gränssnittet för textläge. Det är oftast en rad i en större textlägesprogramsats.</td> 
  </tr> 
  <tr> 
   <td>Fält</td> 
   <td> <p>Avser objektens attribut. "Status" är till exempel ett fält för Projekt, Aktivitet eller Problem. "Portfolio Manager" är ett fält för objektet Portfolio.</p> <p>Du kan också ha anpassade fält som du skapar själv och lägger till i anpassad Forms.<br>Mer information om hur du skapar anpassade Forms finns i artikeln <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Fältnamn </td> 
   <td>Värdet för ett attribut som visas i en vy, används i villkoret för ett filter eller som ett gemensamt element i en gruppering. Alternativen för Fältnamn är beroende av valet av fältkälla.</td> 
  </tr> 
  <tr> 
   <td>Fältkälla </td> 
   <td>Värdet för ett objekt som visas i en vy, eller används i ett filtervillkor eller som ett gemensamt element i en gruppering. Alternativen i Fältkälla beror på objekttypen för det gränssnittselement som skapas. Med fältkällan kan du referera till attribut från andra objekt än objekttypen för UI-elementet.</td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td>Ett huvudrapportelement som bestämmer vilka resultat som visas i rapporten.</td> 
  </tr> 
  <tr> 
   <td>Formulär </td> 
   <td>Används omväxlande med "Anpassat formulär". Fält och avsnitt läggs till i formulär, som sedan bifogas till ett objekt för att utöka antalet fält som du kan associera med ett objekt.</td> 
  </tr> 
  <tr> 
   <td>Gruppering </td> 
   <td>Ett huvudrapportelement som identifierar hur en resultatlista är ordnad. Grupperingen skapar vågräta staplar i hela rapporten för att gruppera resultaten efter gemensamma attribut som definieras när den skapas. Grupperingar används i matrisrapporter för att samla in data, liksom i diagram, för att bestämma axlarna för diagram.</td> 
  </tr> 
  <tr> 
   <td>Objekt- eller objekttyp</td> 
   <td> Ett objekt är ett Workfront-programelement (t.ex. Project, Task, Group, Company, Filter). Objekttypen används när du skapar en ny rapport, vy, filter eller gruppering för att identifiera vilket objekt som är i fokus för rapporten. Rapporter kan bara ha en objekttyp, vilket är rapportens huvudobjekt.<br>Överordnade objekt kan refereras i samma rapport.<br>Mer information om objekthierarkin finns i avsnittet om ömsesidigt beroende och hierarki i artikeln <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Fråga</td> 
   <td> <p>Ett valfritt rapportelement som kan läggas till i en rapport när du behöver köra ett annat filter före varje gång du kör rapporten.</p> <p>Mer information om frågor finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- och villkorsmodifierare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Kvalificerare eller villkorsmodifierare</td> 
   <td> <p>Det här fältet visas i följande områden i en rapport:</p> 
    <ul> 
     <li>På fliken Filter</li> 
     <li>Skärmen Avancerade alternativ för kolumnen på fliken Kolumner (Visa). Genom att definiera en kvalificerare kan du jämföra fältnamnet med ett annat fält eller värde.</li> 
     <li> I en anpassad fråga<br>Mer information om anpassade frågor finns i avsnittet"Skapa en fråga" i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- och villkorsmodifierare</a>.</li> 
    </ul> <p>Om du till exempel skapar ett filter för uppgifter med dagens planerade slutförandedatum väljer du <strong>Jämn</strong> i fältet Kvalificerare och dagens datum i fältet Datum:</p> <p><em>Aktivitet &gt; Planerat slutförandedatum &gt; lika med&gt;(dagens datum)</em> </p> <p>I det här scenariot är kvalificeraren <strong>Jämn</strong>.<br>Mer information om kvalificerare finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- och villkorsmodifierare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Rapport </td> 
   <td>Kombinationen av en vy, ett filter och (ibland) en gruppering. Syftet med en rapport är att visa data på ett enhetligt sätt i hela gränssnittet, att distribuera information och att eliminera behovet av att köra samma sökning eller fråga regelbundet.</td> 
  </tr> 
  <tr> 
   <td>Utdrag</td> 
   <td>Består av flera uttryck som sätts samman för att definiera vilken information som visas i en rapport när du använder textläge. En sats kan skapas för en vy, ett filter, en gruppering eller för en anpassad fråga i en rapport.</td> 
  </tr> 
  <tr> 
   <td>Sammanfattning</td> 
   <td>Det här är en av flikarna i en rapport när du har sparat rapporten. Fliken skapas bara när du definierar en gruppering för rapporten. Den sammanfattar information baserat på den gruppering som har definierats när rapporten skapades och ger en snabb översikt av rapportens aggregerade objekt. Det visar inte alla objekt i rapporten, bara de som är aggregerade.</td> 
  </tr> 
  <tr> 
   <td>Textlägesgränssnitt</td> 
   <td>Ger möjlighet att skapa eller ändra koden för anpassade vyer, filter, grupperingar och uppmaningar som ursprungligen skapades via Builder-gränssnittet. Vi föreslår att rapportelement skapas via Builder-gränssnittet och sedan konverteras till textläge när de har sparats för att förenkla kodningen av avancerade vyer, filter, grupperingar eller uppmaningar.</td> 
  </tr> 
  <tr> 
   <td>Användargränssnitt</td> 
   <td>Avser komponenterna eller byggstenarna i vad som visas på en användares skärm vid en viss tidpunkt.</td> 
  </tr> 
  <tr> 
   <td>Visa (eller kolumner)</td> 
   <td>Ett av huvudinslagen i en rapport. Den identifierar de kolumnrubriker som ska visas i en rapportlista.</td> 
  </tr> 
 </tbody> 
</table>
