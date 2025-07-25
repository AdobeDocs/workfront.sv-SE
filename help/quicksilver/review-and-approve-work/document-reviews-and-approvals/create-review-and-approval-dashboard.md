---
product-area: documents
navigation-topic: approvals
title: Skapa en kontrollpanel för granskning och godkännande
description: Du kan granska godkännandevärden på arbetsytans kontrollpaneler.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 0b4884d6c9a88c096b15af65a2aff0a54ca66811
workflow-type: tm+mt
source-wordcount: '2520'
ht-degree: 0%

---

# Skapa en rapportkontrollpanel för granskning och godkännande

Du kan skapa en rapportkontrollpanel i kontrollpanelerna på arbetsytan för att visa både högnivåinformation och detaljerad information om granskningar och godkännanden med funktionen för enhetliga godkännanden.

>[!IMPORTANT]
>
>Den här funktionen är endast tillgänglig för kunder som använder tjänsten för enhetliga godkännanden och som är inskrivna i Canvas Dashboards beta. Mer information finns i [Betaversionsinformation för arbetsytans kontrollpaneler](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).


![exempelinstrumentpanel](assets/whole-dashboard.png)

## Skapa en instrumentpanel

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.
1. Klicka på **Ny instrumentpanel**.
1. Ge instrumentpanelen ett namn.
1. (Valfritt) Lägg till en beskrivning.
1. Klicka på **Skapa**.
   ![lägg till instrumentpanelens namn och beskrivning](assets/create-a-dashboard.png)

När du har skapat en kontrollpanel kan du börja lägga till KPI:er, diagram och tabeller. Mer information finns i följande avsnitt:

* [Lägg in gransknings- och godkännandeinformation på hög nivå med nyckeltal och diagram](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Lägg in detaljerad gransknings- och godkännandeinformation i tabeller](#add-detailed-review-and-approval-information-with-tables)

## Lägg in gransknings- och godkännandeinformation på hög nivå med nyckeltal och diagram

Du kan visa högnivåinformation om dokumentgodkännanden med nyckeltal och diagram.

Mer information finns i [Skapa en KPI-rapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) och [Skapa en diagramrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

### KPI:er

![KPI-exempel](assets/kpi-dashboard.png)

#### Väntande godkännanden

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **KPI** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv *Väntande* i fältet **Namn**.
   1. Skriv *Väntande godkännanden* i fältet **Beskrivning**. Detta visas som en bildtext under KPI-värdet.

1. Följ stegen nedan för att konfigurera avsnittet **Build KPI**:

   1. Klicka på ikonen **Skapa KPI** ![Skapa KPI](assets/build-kpi-icon.png) i den vänstra panelen.

   1. Klicka på **Markera fält**.

   1. Leta reda på och välj mappen **Dokumentgodkännande**.

   1. Välj **Status**.

   1. Välj **Antal** i listrutan **Aggregationstyp**.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor**.

   1. Klicka på det tomma villkorsfiltret, klicka på **Välj ett fält** och välj sedan **Status**.
   1. Låt operatorn vara **lika med** och skriv sedan _väntande granskning_ i textrutan.
      ![väntande kpi-filterexempel](assets/pending-kpi-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.


#### Försenade godkännanden

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **KPI** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Försenad_ i fältet **Namn**.
   1. Skriv _Deadline för godkännandefas i fältet_ Beskrivning **i fältet**. Den här beskrivningen visas som en beskrivning under KPI-värdet.

1. Följ stegen nedan för att konfigurera avsnittet **Build KPI**:

   1. Klicka på ikonen **Skapa KPI** ![Skapa KPI](assets/build-kpi-icon.png) i den vänstra panelen.

   1. Klicka på **Markera fält**.

   1. Leta reda på och välj mappen **Dokumentgodkännande**.

   1. Välj **Status**.

   1. Välj **Antal** i listrutan **Aggregationstyp**.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor**.

   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.

   1. Välj **Godkännandefas** > **Deadline**.
   1. Ändra operatorn till **mindre än**.
   1. Växla **Ange det relativa datumet** till **ON** och skriv sedan _$$TODAY_ i textrutan.
      ![Exempel på försenat kpi-filter](assets/overdue-kpi-filter.png)
   1. Klicka på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Status**.
   1. Ändra operatorn till **Innehåller inte** och skriv sedan _godkänt_ i textrutan.
      ![Exempel på försenat kpi-filter 2](assets/overdue-kpi-filter-2.png)
1. Klicka på **Spara** i skärmens övre högra hörn.


#### Slutförda godkännanden


1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **KPI** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Slutförd_ i fältet **Namn**.
   1. Skriv _Antal godkännandestatusvärden_ i fältet **Beskrivning**. Den här beskrivningen visas som en beskrivning under KPI-värdet.

1. Följ stegen nedan för att konfigurera avsnittet **Build KPI**:

   1. Klicka på ikonen **Skapa KPI** ![Skapa KPI](assets/build-kpi-icon.png) i den vänstra panelen.

   1. Klicka på **Markera fält**.

   1. Leta reda på och välj mappen **Dokumentgodkännande**.

   1. Välj **Status**.

   1. Välj **Antal** i listrutan **Aggregationstyp**.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor**.

   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.

   1. Välj **Status**.

   1. Ändra operatorn till **Innehåller** och skriv _godkänt_ i textrutan.
      ![slutfört kpi-filterexempel](assets/completed-kpi-filter.png)
   1. Klicka på **Lägg till villkor**.
   1. Klicka på **And** om du vill ändra den till **Or**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Status**.
   1. Ändra operatorn till **Lika med** och skriv sedan _Granskad_ i textrutan.
      ![slutfört kpi-filterexempel](assets/completed-kpi-filter-2.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

#### Övergivna godkännanden

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **KPI** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Borttagen_ i fältet **Namn**.
   1. Skriv _Deadline för godkännande över 2 veckor efter_ i fältet **Beskrivning**. Den här beskrivningen visas som en beskrivning under KPI-värdet.

1. Följ stegen nedan för att konfigurera avsnittet **Build KPI**:

   1. Klicka på ikonen **Skapa KPI** ![Skapa KPI](assets/build-kpi-icon.png) i den vänstra panelen.

   1. Klicka på **Markera fält**.

   1. Leta reda på och välj mappen **Dokumentgodkännandestadium**.

   1. Välj **Deadline**.

   1. Välj **Antal** i listrutan **Aggregationstyp**.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor**.

   1. Klicka på det tomma villkorsfiltret och klicka på **Välj ett fält**.

   1. Välj **Status**.

   1. Ändra operatorn till **Innehåller inte** och skriv _godkänt_ i textrutan.
      ![övergivet kpi-filterexempel](assets/abandoned-kpi-filter.png)
   1. Klicka på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Deadline**.
   1. Ändra operatorn till **mindre än** och växla sedan **Ange relativt datum** till **ON**.
   1. Skriv _$$TODAY-2w_ i textrutan.
      ![övergivet kpi-filterexempel](assets/abandoned-kpi-filter-2.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

### Diagram

![Diagramexempel](assets/chart-dashboard.png)

#### Godkännanden per beslutsstapeldiagram

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Diagram** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Godkännanden genom beslut_ i fältet **Namn**.
   1. (Valfritt) Skriv en beskrivning i fältet **Beskrivning**. Den här texten visas som ett verktygstips bredvid diagramnamnet.
1. Följ stegen nedan för att konfigurera avsnittet **Bygg diagram**:

   1. Klicka på ikonen **Skapa diagram** ![Skapa diagram](assets/build-chart-icon.png) i den vänstra panelen.

   1. Låt **Bar** vara markerat på den nedrullningsbara menyn **Diagramtyp**.
   1. Låt **Enkel** vara markerat i den nedrullningsbara menyn **Stapeltyp**.
   1. Klicka på **Uppdatera fält** för **undre axeln (X)** och välj sedan **Dokumentgodkännande** > **Status**.
   1. Ange **aggregeringstypen** som **Antal**.
   1. Klicka på **Uppdatera fält** för axeln **Vänster (Y)** och välj sedan **Status**.
1. Följ stegen nedan för att konfigurera avsnittet **Filter**:
   1. Klicka på ikonen **Filter** ![filterflik](assets/filter-tab.png) i den vänstra panelen.
   1. Klicka på **Redigera filter** och sedan på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Dokumentversion** > **Version**.
   1. Ändra operatorn till **Är inte null**.
      ![filterexempel](assets/approvals-by-decision-chart-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.


#### Diagram över ändringar

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Diagram** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Revisioner_ i fältet **Namn**.
   1. Skriv _Antal revisioner för dokument med ofullständiga beslut som har planerats före månadens slut_ i fältet **Beskrivning**. Den här texten visas som ett verktygstips bredvid diagramnamnet.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg diagram**:

   1. Klicka på ikonen **Skapa diagram** ![Skapa diagram](assets/build-chart-icon.png) i den vänstra panelen.

   1. Låt **Bar** vara markerat på den nedrullningsbara menyn **Diagramtyp**.
   1. Låt **Enkel** vara markerat i den nedrullningsbara menyn **Stapeltyp**.
   1. Klicka på **Uppdatera fält** för **Understa (X) axeln** och välj sedan **Dokumentgodkännande** > **Dokumentversion** > **Version**.
   1. Ange **aggregeringstypen** som **Antal**.
   1. Klicka på **Uppdatera fält** för axeln **Vänster (Y)** och välj sedan **Dokumentgodkännande** > **Dokumentversion** > **Dokument** > **Namn**.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:
   1. Klicka på ikonen **Filter** ![filterflik](assets/filter-tab.png) i den vänstra panelen.
   1. Klicka på **Redigera filter** och sedan på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.

   1. Välj **Godkännandefas** > **Godkännandefasdeltagare** > **Beslutsdatum**.

   1. Ändra operatorn till **Är null**.
      ![Exempel på ändringsdiagramfilter](assets/revision-chart-filter.png)
   1. Klicka på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Godkännandefas** > **Deadline**.
   1. Ändra operatorn till **mindre än eller lika med** och växla sedan **Ange relativt datum** till **ON**.
   1. Skriv _$$TODAYem_ i textrutan.
      ![Exempel på ändringsdiagramfilter](assets/revision-chart-filter-2.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

## Lägg in detaljerad gransknings- och godkännandeinformation i tabeller

Mer information om hur du skapar en tabellrapport finns i [Skapa en tabellrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

![tabellexempel](assets/table-dashboard.png)

### Väntande godkännandelista

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.
1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Tabell** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Väntande godkännanden_ i fältet **Namn**.
   1. Skriv en beskrivning i fältet **Beskrivning**. Den här texten visas som ett verktygstips bredvid diagramnamnet.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg tabell**:

   1. Klicka på ikonen **Tabellkolumner** ![Tabellkolumner](assets/drilldown-column.png) i den vänstra panelen.
   1. Klicka på **Lägg till kolumn**.
   1. Bläddra nedåt och välj **Dokumentgodkännanden** > **Status**.
   1. Lägg till följande kolumner:

   <table>
    <tr>
    <td><strong>Projektnamn</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Namn</td>
    </tr>
    <tr>
    <td><strong>Dokumentnamn</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Skriv <em>Namn</em> i sökrutan.</td>
    </tr>
    <tr>
    <td><strong>Dokumentversion</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Deadline</strong></td>
    <td>Dokumentgodkännande &gt; Godkännandefas &gt; Deadline</td>
    </tr>
    <tr>
    <td><strong>Begärd av</strong></td>
    <td>Dokumentgodkännande &gt; Godkännandefas &gt; Deltagare i godkännandefasen* &gt; Beställare &gt; typ <em>Namn</em> i sökrutan.</td>
    </tr>
    <tr>
    <td><strong>Begärt datum</strong></td>
    <td>Dokumentgodkännande &gt; Godkännandefasen &gt; Deltagare i godkännandefasen* &gt; Skapat vid</td>
    </tr>
    <tr>
    <td><strong>Godkännare</strong></td>
    <td>Dokumentgodkännande &gt; Godkännandesteg &gt; Deltagare i godkännandefasen* &gt; Deltagaranvändare &gt; skriv <em>Namn</em> i sökrutan.</td>
    </tr>
    </table>


   *Deltagare i godkännandefasen har trunkerats till _Godkännandefas-Pa.._


1. Följ stegen nedan för att konfigurera avsnittet **Filter**:
   1. Klicka på ikonen **Filter** ![filterflik](assets/filter-tab.png) i den vänstra panelen.
   1. Klicka på **Redigera filter** och sedan på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Status**.
   1. Ändra operatorn till **Lika med** och skriv sedan _väntande godkännande_ i textrutan.
      ![Exempel på väntande godkännandetabellfilter](assets/pending-approval-table-filter.png)
   1. (Valfritt) Lägg till ytterligare filter enligt beskrivningen i avsnittet **Valfria filter** nedan.
1. Klicka på **Spara** i skärmens övre högra hörn.


**Valfria filter**

Om du vill visa mer specifik information beroende på hur du använder exemplet kan du lägga till ytterligare filtervillkor. Du kanske vill återskapa tabellen och lägga till nya filtervillkor per användningsfall.

+++ Expandera om du vill visa ytterligare filteralternativ

**Mina projekt**

1. Klicka på **Redigera filter** > **Lägg till villkor**:
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Dokumentversion** > **Dokument** > **Projekt** > **Ägare** > skriv _Namn_ i sökrutan.
   1. Ändra operatorn till **Lika med** och välj sedan **Jag (inloggad användare)** för att visa projekt i Workfront där du är markerad som projektägare.
      ![Exempel på väntande godkännandetabellfilter](assets/pending-approvals-my-project-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

**Godkännanden jag har skickat**

1. Klicka på **Redigera filter** > **Lägg till villkor**:
   1. Klicka på det tomma villkorsfiltret och klicka på **Välj ett fält**.
   1. Välj **Godkännandefas** > **Deltagare i godkännandefas** > **Beställare** > skriv _Namn_ i sökrutan.
   1. Ändra operatorn till **Lika med** och välj sedan **Jag (inloggad användare)** för att visa projekt i Workfront där du är markerad som projektägare.
      ![Exempel på väntande godkännandetabellfilter](assets/pending-approvals-my-project-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

+++

### Lista över försenade godkännanden

1. [Skapa en instrumentpanel](#create-a-dashboard) enligt beskrivningen i avsnittet ovan.

1. Klicka på **Lägg till rapport** i det övre högra hörnet på sidan med instrumentpanelsinformation.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Tabell** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. Följ stegen nedan för att konfigurera avsnittet **Information**:

   1. Skriv _Försenade godkännanden_ i fältet **Namn**.
   1. (Valfritt) Skriv en beskrivning i fältet **Beskrivning**. Den här texten visas som ett verktygstips bredvid diagramnamnet.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg tabell**:

   1. Klicka på ikonen **Tabellkolumner** ![Tabellkolumner](assets/drilldown-column.png) i den vänstra panelen.
   1. Klicka på **Lägg till kolumn**.
   1. Bläddra nedåt och välj **Dokumentgodkännanden** > **Status**.
   1. Lägg till följande kolumner:

      <table>
        <tr>
        <td><strong>Projektnamn</strong></td>
        <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Namn</td>
        </tr>
        <tr>
        <td><strong>Dokumentnamn</strong></td>
        <td>Dokumentversion &gt; Dokument &gt; Skriv <em>Namn</em> i sökrutan.</td>
        </tr>
        <tr>
        <td><strong>Dokumentversion</strong></td>
        <td>Dokumentversion &gt; Dokument &gt; Version</td>
        </tr>
        <tr>
        <td><strong>Deadline</strong></td>
        <td>Dokument &gt; Godkännandefas &gt; Deadline</td>
        </tr>
        <tr>
        <td><strong>Begärd av</strong></td>
        <td>Dokument &gt; Godkännandefas &gt; Deltagare i godkännandefasen* &gt; Beställare &gt; typ <em>Namn</em> i sökrutan.</td>
        </tr>
        <tr>
        <td><strong>Begärt datum</strong></td>
        <td>Dokument &gt; Godkännandefas &gt; Deltagare i godkännandefas* &gt; Skapat på</td>
        </tr>
        <tr>
        <td><strong>Godkännare</strong></td>
        <td>Dokument &gt; Godkännandefas &gt; Deltagare i godkännandefasen* &gt; Deltagaranvändare &gt; skriv <em>Namn</em> i sökrutan.</td>
        </tr>
        </table>

      *Deltagare i godkännandefasen har trunkerats till _Godkännandefas-Pa.._

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:
   1. Klicka på ikonen **Filter** ![filterflik](assets/filter-tab.png) i den vänstra panelen.
   1. Klicka på **Redigera filter** och sedan på **Lägg till villkor**.
   1. Klicka på det tomma villkorsfiltret och klicka sedan på **Välj ett fält**.
   1. Välj **Godkännandefas** > **Deadline**.
   1. Ändra operatorn till **Mindre än** och växla sedan **Ange relativt datum** till **ON**.
   1. Skriv _$$TODAY_ i textfältet.
      ![Exempel på förfallet godkännandetabellfilter](assets/overdue-approval.png)
   1. (Valfritt) Lägg till ytterligare filter enligt beskrivningen i avsnittet **Valfria filter** nedan.
1. Klicka på **Spara** i skärmens övre högra hörn.



**Valfria filter**

Om du vill visa mer specifik information beroende på hur du använder exemplet kan du lägga till ytterligare filtervillkor. Du kanske vill återskapa tabellen och lägga till nya, valfria filtervillkor per användningsfall.

+++ Expandera om du vill visa ytterligare filteralternativ

**Mina projekt**

1. Klicka på **Redigera filter** > **Lägg till villkor**:
   1. Klicka på det tomma villkorsfiltret och klicka på **Välj ett fält**.
   1. Välj **Dokumentversion** > **Dokument** > **Projekt** > **Ägare** > skriv _Namn_ i sökrutan.
   1. Ändra operatorn till **Lika med** och välj sedan **Jag (inloggad användare)** för att visa projekt i Workfront där du är markerad som projektägare.
      ![Exempel på väntande godkännandetabellfilter](assets/pending-approvals-my-project-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

**Godkännanden jag har skickat**

1. Klicka på **Redigera filter** > **Lägg till villkor**:
   1. Klicka på det tomma villkorsfiltret och klicka på **Välj ett fält**.
   1. Välj **Godkännandefas** > **Deltagare i godkännandefas** > **Beställare** > skriv _Namn_ i sökrutan.
   1. Ändra operatorn till **Lika med** och välj sedan **Jag (inloggad användare)** för att visa projekt i Workfront där du är markerad som projektägare.
      ![Exempel på väntande godkännandetabellfilter](assets/pending-approvals-my-project-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.

**Mitt team**

1. Klicka på **Redigera filter** > **Lägg till villkor**:
   1. Klicka på det tomma villkorsfiltret och klicka på **Välj ett fält**.
   1. Välj **Godkännandefas** > **Deltagare i godkännandefas** > **Deltagargrupp** > skriv _Namn_ i sökrutan.
   1. Ändra operatorn till **Lika med** och välj sedan **Mina standardteam (inloggad användare)** eller **Mina andra team (inloggad användare)** för att visa projekt som tilldelats ditt standardteam eller andra team som du är på.
      ![Exempel på väntande godkännandetabellfilter](assets/approvals-ive-submitted-filter.png)
1. Klicka på **Spara** i skärmens övre högra hörn.
+++
