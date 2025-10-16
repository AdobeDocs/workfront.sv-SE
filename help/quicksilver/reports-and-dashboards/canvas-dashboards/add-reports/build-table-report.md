---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Skapa en tabellrapport på en Canvas Dashboard
description: Du kan lägga till en tabellrapport på en Canvas-kontrollpanel för att visa data i ett tabellformat.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 0%

---

# Skapa en tabellrapport på en Canvas Dashboard

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

Du kan lägga till en tabellrapport på en Canvas-kontrollpanel för att visa data i ett tabellformat.

![Exempel på tabellrapport](assets/table-example-main.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr>  
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan skapa en tabellrapport.


## Skapa en tabellrapport på en Canvas Dashboard

Det finns många konfigurationsalternativ för att skapa en tabellrapport. I det här avsnittet går vi igenom den allmänna processen att skapa en.

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel** anger du instrumentpanelens **namn** och **beskrivning**.

1. Klicka på **Skapa**.

1. Välj **Skapa rapport** i rutan **Lägg till rapport**.

1. Välj **Tabell** till vänster.

1. Klicka på **Skapa rapport** i det övre högra hörnet.

1. (Valfritt) Följ stegen nedan för att konfigurera avsnittet **Detaljer**:

   1. Ange en rapport **Namn**.

   1. Ange en rapport **Beskrivning**.

1. Följ stegen nedan för att konfigurera avsnittet **Bygg tabell**:

   1. Klicka på ikonen **Tabellkolumner** ![Skapa tabell](assets/drilldown-column.png) i den vänstra panelen.

   1. Klicka på **Lägg till kolumn** och markera sedan det fält som du vill visa som en kolumn i tabellen. Kolumnen visas i förhandsvisningsavsnittet till höger.



   1. Upprepa ovanstående steg för varje kolumn som du vill lägga till.

1. Följ stegen nedan för att konfigurera avsnittet **Filter**:

   1. Klicka på ikonen **Filter** ![Filter](assets/filter-icon.png) i den vänstra panelen.

   1. Välj **Redigera filter**.

   1. Klicka på **Lägg till villkor** och ange sedan fältet som du vill filtrera efter och modifieraren som definierar vilken typ av villkor som fältet måste uppfylla. Kolumnen visas i förhandsvisningsavsnittet till höger.

1. (Valfritt) Klicka på **Lägg till filtergrupp** om du vill lägga till ytterligare en uppsättning filtervillkor. Standardoperatorn mellan uppsättningarna är AND. Klicka på operatorn för att ändra den till ELLER.

1. Följ stegen nedan för att konfigurera avsnittet **Inställningar för grupper med nedladdning**:

   1. Klicka på ikonen **Gruppinställningar** ![Gruppinställningar](assets/drilldown-group-icon.png) i den vänstra panelen.

   1. Klicka på knappen **Lägg till gruppering** och markera sedan det fält som du vill skapa som en gruppering. Grupperingskolumnen visas i förhandsvisningsavsnittet till höger.

1. Klicka på **Spara** för att skapa rapporten och lägga till den på kontrollpanelen.

## Skapa ett exempel på en tabellrapport

I det här avsnittet går vi igenom stegen för att skapa en tabellrapport som visar väntande dokumentgodkännanden.

Mer information om exempel på tabellrapporter finns i [Skapa en rapportkontrollpanel för granskning och godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel** anger du instrumentpanelens **namn** och **beskrivning**.

1. Klicka på **Skapa**.

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

## Att tänka på när du skapar en tabellrapport

### Använda fältväljaren

Listrutan **Avsnitt** i avsnittet **Skapa tabell** är utformad för att begränsa valen i en fältväljare så att ett objekt blir lättare att hitta när en tabellrapport skapas. Börja med att välja ett basenhetsobjekt.

* **Alla avsnitt**: Alla objekttyper i Workfront Workflow och Workfront Planning.
* **Workfront-objekt**: Inbyggda Workfront Workflow-objekt.
* **Planering av posttyper**: Anpassade posttyper har definierats i Workfront Planning.

![Listrutan Avsnitt](assets/sections-dropdown.png)

När basentitetsobjektet har valts uppdateras listrutan **Avsnitt** med tillämpliga fälttypsalternativ att välja bland.

* **Alla avsnitt**: Inbyggda fält, anpassade fält och relaterade objekt.
* **Alla fält**: Både interna och anpassade fält (exkluderar relationer).
* **Anpassade fält**: Kunddefinierade fält antingen i ett anpassat formulär eller i en planeringspost.
* **Workfront-fält**: Endast inbyggda fält.
* **Relationer**: Anslutna poster.

![Val av Rapporteringsbara objekt](assets/reportable-objects-selection.png)

### Referera underordnade objekt

Tillgängliga relationer för ytterligare kolumner, filteralternativ och grupperingsattribut är i allmänhet begränsade till objekt som är högre upp i Workfront objekthierarki eller har på annat sätt en markering på rapportens basenhetsobjekt. Det finns några undantag i detta, bland annat följande:

* Projekt > Åtgärder
* Dokumentgodkännande > Dokumentgodkännandesteg
* Dokumentgodkännandesteg > Deltagare i dokumentgodkännandefasen

När du använder någon av de överordnade-till-underordnade-relationer som anges ovan visas en rad i tabellen för varje underordnad post som är kopplad till det överordnade objektet.
