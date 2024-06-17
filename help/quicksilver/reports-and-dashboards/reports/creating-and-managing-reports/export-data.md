---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exportera data
description: Du kan exportera Adobe Workfront-data från olika listor, rapporter, kontrollpaneler och sökningar.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2164'
ht-degree: 0%

---

# Exportera data

<!-- Audited: 12/2023 -->

Du kan exportera Adobe Workfront-data från olika listor, rapporter, kontrollpaneler och sökningar.

Några av orsakerna till att data exporteras är:

* Du vill skicka en kopia av dina data till någon utanför Workfront.
* Du vill skicka resultatet av en rapport som en bifogad fil till en extern användare.
* Du vill skapa en extern säkerhetskopia av dina Workfront-data.
* Det finns en gräns för att endast visa 2 000 resultat på en sida i Workfront webbprogram. Om din rapport producerar mer än 2 000 kan du exportera rapporten till något av de tillgängliga formaten och visa alla resultat i rapporten i en lista.

Du kan antingen exportera en rapport manuellt från Workfront-gränssnittet eller schemalägga en leverans för en rapport så att rapporten skickas till dig vid ett senare tillfälle. Mer information om schemaläggning av levererade rapporter finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Informationen i den här artikeln gäller inte följande exporter:

* Exporterar information från diagramrapporter.

  Mer information om hur du exporterar en diagramrapport finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exporterar information från Gantt-diagrammet.

  Mer information om hur du exporterar Gantt-schemat finns i [Exportera Gantt-schemat till PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exporterar information från resursplaneraren.

  Mer information om hur du exporterar informationen från resursplaneraren finns i &quot;Exportalternativ&quot; i [Översikt över navigering i resursplanering](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
    <p>Nytt: Ljus eller högre</p>
    <p>eller</p>
    <p>Aktuell: Granska eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomst till rapporter, instrumentpaneler och kalendrar för att exportera rapporter</p> <p>Visa eller öka åtkomsten till objekten som du visar i en lista för att exportera listan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörighet till en rapport eller kontrollpanel för att exportera rapporten eller kontrollpanelen</p> <p>Visa eller högre behörigheter för de objekt som du visar i en lista för att exportera listan</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Rapporten måste skapas innan du kan exportera dess data.

Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) eller [Skapa en kopia av en rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Exportformat och -begränsningar

### Exportformat {#export-formats}

Information kan exporteras i följande format:

* PDF (Letter liggande eller stående, Legal, Ledger och A4)
* Excel (.xls)
* Excel (.xlsx)
* Tabbavgränsad

>[!NOTE]
>
>Kontrollpaneler kan antingen skrivas ut eller exporteras endast till en PDF-fil.

### Exportbegränsningar {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Det finns flera begränsningar för hur rapporter visas i Workfront och hur de exporteras via manuell export, en levererad rapport eller via API:t.

* **50 000 celler:** Det maximala antalet celler som tillåts i en rapportexport för Excel-filer.
* **50 000 rader:** Antalet rader med data som tillåts i en rapportexport för PDF- och tabbavgränsade filer.

   * För Excel .xls-filer är den här gränsen **65 000 rader**.
   * För Excel .xlsx-filer är den här gränsen **100 000 rader**.
   * Dessa begränsningar utesluter kolumnrubriker samt rader för grupperingar i rapporten. Om du t.ex. har 6 grupperingar i en rapport och 50 000 rader data, kommer den exporterade filen att ha 50 000 rader.

  >[!IMPORTANT]
  >
  >Om du exporterar en rapport som innehåller en samlingsreferens i en kolumn kan det resultera i ett fel, även om rapporten annars ligger inom de angivna exportgränserna. Om den refererade samlingen är för stor, kommer exportprocessen att få en timeout och resultera i ett fel.
  >
  >För att undvika det här felet bör du antingen exkludera kolumner som refererar till stora samlingar eller minska storleken på de refererade samlingarna innan du exporterar.
  >

  Om rapporten innehåller fler objekt än dessa gränser visas ett felmeddelande om att exporten inte lyckas. Minska antalet objekt som visas på skärmen till ett tal som är mindre än eller lika med dessa gränser för att kunna exportera resultaten.

  Om din rapport innehåller fler än 50 000/65 000/100 000 rader och du vill exportera alla data, rekommenderar vi att du använder filter eller uppmaningar för att få mindre datamängder och utföra flera exporter.

  Mer information om hur du använder filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Mer information om hur du använder uppmaningar finns i [Lägga till en fråga i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Dessa begränsningar gäller för

   * Manuell export av en rapport.
   * En schemalagd rapport.
   * En export via en API-integrering.
   * Data som exporteras med en snabbstart.

     Mer information om hur du exporterar data via direktuppspelning finns i [Exportera data från Adobe Workfront via Quick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Du kan exportera 50 000 rader i en snabbstartfil, men du kan bara exportera data till en Excel-formatfil.

   * Exporterar användningsinformation för ett projekt.

     Mer information om hur du exporterar användningsinformation för ett projekt finns i [Översikt över resursanvändningsrapporten](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10 MB filstorlek:** Filstorleksgräns för exporterade rapporter som är schemalagda för leverans. Om en exporterad fil som bifogas till ett e-postmeddelande är större än 5 MB, skickas en länk dit filen kan hämtas via e-post i stället för den bifogade exporterade rapporten.
* **65 530 hyperlänkar:** Det här är en gräns som gäller för dokument som innehåller fler än 65 530 hyperlänkar. Dessa dokument kan inte öppnas när de exporteras manuellt eller skickas i en levererad rapport. Observera att ett Excel-dokument kanske bara innehåller 200 rader med data, men att dokumentet inte öppnas om det finns fler än 65 530 länkar i dokumentet. Den här gränsen gäller endast för Excel-filer, inte för andra format som stöds. 
* **256 kolumner**: Det här är en gräns som gäller för dokument som innehåller fler än 256 kolumner. Dessa dokument kan inte exporteras manuellt eller skickas i en levererad rapport. Den här gränsen gäller endast för Excel-filer, inte för andra format som stöds.

Om du försöker exportera data utanför gränsen kanske du inte får alla förväntade data i exporten. En ändrad rapport skapas i stället inom gränsen.

Dessutom kommer rapporter som tar längre tid än 60 minuter att köras att stoppas.

Om du har frågor eller funderingar kring din begränsning kan du kontakta Workfront tekniska support.

## Exportera data

### Exportera data från en rapport eller lista {#export-data-from-a-report-or-list}

1. Gå till den rapport eller lista som du vill exportera.
1. Markera de objekt som du vill exportera. (Om du markerar enskilda objekt exporteras endast de objekt du markerar.)

   I ett projekt väljer du t.ex. de uppgifter du vill exportera.

   eller

   Låt alla objekt vara avmarkerade om du vill exportera hela listan.

1. Klicka **Exportera** väljer du sedan ett format.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   eller

   Klicka på **Exportera** icon ![Ikonen Exportera](assets/export-icon-nwe.png)väljer du sedan ett format.

   Vilka alternativ som är tillgängliga för export till PDF beror på språkinställningarna i användarinställningarna för Workfront:

   * Nordamerika - brev (standard), juridisk information, redovisning, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Alla platser utanför Nordamerika - A3, A4 (standard), Letter, Legal, Ledger

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Villkorligt) Beroende på vilket operativsystem du använder kan du ha möjlighet att öppna eller spara filen. Öppna filen med det associerade programmet eller spara den på hårddisken.
1. Fortsätt med [Använda det exporterade dokumentet](#use-the-exported-document).

### Exportera data från en kontrollpanel {#export-data-from-a-dashboard}

Du kan skriva ut informationen från en kontrollpanel eller exportera den som en pdf-fil.

Mer information om hur du exporterar data från en kontrollpanel finns i [Exportera en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Använda det exporterade dokumentet {#use-the-exported-document}

* [Filnamn](#file-names)
* [Titlar](#titles)
* [Tidsstämplar](#timestamps)
* [Formatering](#formatting)
* [Länkar](#links)
* [Varumärke](#branding)

### Filnamn {#file-names}

Oavsett om du exporterar en lista med objekt eller en rapport kommer den exporterade filen att ha ett filnamn och en titel. Du kan hitta den exporterade filen på datorn genom att referera till filnamnet. Rapportens titel ger användarna en indikation på vad den exporterade filen representerar när du delar den med dem.

#### Filnamn för exporterade listor {#file-names-for-exported-lists}

När du exporterar en lista med objekt visas objekttypen i den exporterade filen i filnamnet och i titeln på listan.

När du exporterar en lista med uppgifter eller problem visas **Filnamn** kan vara något av följande:

* När du exporterar uppgiftslistor och utgivningslistor i ett projekt:

   * *The_project_name_Exported_Tasks*(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*
   * *The_project_name_Exported_Issues*(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*

* När du exporterar uppgifter och utgivningslistor i en uppgift (underuppgifter):

   * **The_project_name_the_task_name_Exported_Tasks**(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*
   * **The_project_name_the_task_name_Exported_Issues**(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*

När du exporterar en lista med andra objekt från ett projekt till en PDF-fil, anger det exporterade dokumentets filnamn vilken typ av objekt du har exporterat.\
Filnamnet kan till exempel vara:

* *Exported_Users*, när du exporterar fliken Personer i projektet(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*
* *Exporterad_risk*, när du exporterar en lista med risker i projektet(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*

#### Filnamn för exporterade rapporter {#file-names-for-exported-reports}

När du exporterar en rapport blir den exporterade rapportens filnamn:

*The_report_name*(*i PDF, Excel, Excel (.xlsx) eller tabbavgränsade format)*

### Titlar {#titles}

När du exporterar en lista med objekt kommer bara filen i PDF-format att ha en rubrik. Om du exporterar en lista eller en rapport till Excel, Excel (.xlsx) eller tabbavgränsad format har filen ingen rubrik.

#### Titlar för exporterade listor {#titles-for-exported-lists}

När du exporterar uppgiftslistor och utleveranslistor i ett projekt till en PDF-fil är det exporterade dokumentets titel något av följande:

* *Projektnamn - Exporterade uppgifter*
* *Projektnamn - Exporterade problem*

När du exporterar uppgiftslistor och utleveranslistor i en uppgift till en PDF-fil är rutan i det exporterade dokumentet något av följande:

* *Projektnamn - Aktivitetsnamn - Exporterade uppgifter*
* *Projektnamn - Aktivitetsnamn - Exporterade problem*

När du exporterar en lista med andra objekt från ett projekt till en PDF-fil, anger det exporterade dokumentets namn vilken typ av objekt du har exporterat.\
Titeln kan till exempel vara:

* *Exporterade användare* när du exporterar fliken Personer i projektet.
* *Exporterade risker*, när du exporterar en lista med risker i projektet.

#### Titlar för exporterade rapporter {#titles-for-exported-reports}

En rapport som exporteras till en PDF-fil får en rubrik.

Om rapporten exporteras till Excel, Excel (.xlsx) eller tabbavgränsad format har den exporterade rapporten ingen rubrik. Den exporterade filens namn är rapportens namn så som det visas i Workfront webbprogram.

Om rapporten innehåller en beskrivning inkluderas den i den exporterade filen.

### Tidsstämplar {#timestamps}

En tidsstämpel visas i det exporterade dokumentet från kontexten för den användare som exporterade objektet.

Tidsstämpeln innehåller:

* Datum
* Tid
* Tidszon när objektet exporterades

Beroende på vilken typ av dokument du exporterar visas tidsstämplar på olika platser:

* **PDF:** Tidsstämplar visas i sidfoten på varje sida och i filnamnet.
* **Excel:** Tidsstämplar visas i filnamnet.

### Formatering {#formatting}

När du exporterar ett projekt till .pdf visas alla underaktiviteter som indragna i de överordnade uppgifterna. Exporterade listor komprimerar inte några överordnade åtgärder.

Du får alltid standardfliken för en rapport när en rapport skickas eller schemaläggs för en leverans, såvida inte rapporten har en särskild vy.

Om rapporten har särskild formatering i webbprogrammet bör den levereras med specialformateringen när flikarna Detaljer och Matris visas, endast för PDF- och Excel-filer.

>[!NOTE]
>
>Om de data du exporterar innehåller delade kolumner och du exporterar till ett Excel- eller tabbavgränsat format, separeras dessa kolumner i den exporterade filen.

Mer information om hur du anpassar formatering i en rapport finns i [Använd villkorsstyrd formatering i vyer](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Länkar {#links}

Länkarna kan peka på alla objekt i Workfront som stöder länkning. När du exporterar en lista i Workfront till .pdf kommer alla länkar som stöds i det ursprungliga dokumentet att vara aktiva i det exporterade dokumentet.

>[!TIP]
>
>Om raden `valueformat=HTML` visas i textläge för en anpassad fältkolumn och länkvärdena inte visas i en exporterad PDF-fil, du måste ange ytterligare kodrader i kolumnen i textläge.
>
>Om du t.ex. har ett anpassat fält med namnet Open Q1 Projects som innehåller länkar lägger du till följande kod:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

När du exporterar till ett Excel-format inkluderas bara länkar till objekt i den exporterade filen, och de stöds bara på platser där du kan välja att tillåta länkar i exporterade Excel-dokument, t.ex. rapportleveranser.

## Varumärke {#branding}

>[!IMPORTANT]
>
>Varumärkesprofileringen gäller endast för organisationer som ännu inte anslutit sig till Adobe Experience Cloud.
>
>Om er organisation har anslutit sig till Adobe Experience Cloud är er varumärkning inte tillgänglig.

Om din Workfront-administratör har lagt till anpassad profilering i din Workfront-instans för Global Navigation Bar, innehåller de exporterade PDF-filerna även din anpassade logotyp.

Data som exporteras i något annat format kan inte anpassas med din logotyp.

Mer information om anpassning av din Workfront-instans och Global Navigation Bar finns i [Varumärk din Adobe Workfront-instans](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
