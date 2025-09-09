---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Redigera en rapport på en arbetsytans kontrollpanel
description: Du kan redigera en kontrollpanelsrapport för arbetsytan när den har skapats.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: fd659f56-d67f-4a0f-8735-b214934903ac
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Redigera en rapport på en arbetsytans kontrollpanel

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

När du har lagt till rapporter på en Canvas-kontrollpanel kan du redigera rapportens information och ändra de data som visas på kontrollpanelen.

Alla ändringar som görs i en rapport påverkar alla användare som har åtkomst till den instrumentpanel som innehåller den.


+++ Expandera om du vill visa åtkomstkraven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Aktuell: Planera </p> 
<p>Nytt: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td><p>Hantera behörigheter för kontrollpanelen</p>
  </td> 
  </tr>
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Förutsättningar

Du måste lägga till en rapport på en kontrollpanel innan den kan redigeras.

Mer information finns i [Skapa en arbetsytans kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Redigera en rapport

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på ikonen **Mer** **Mer** i det övre högra hörnet av rapporten som du vill redigera på sidan ![Arbetsytans kontrollpaneler](assets/more-icon.png) och välj sedan **Redigera** .

   ![Redigera en rapport](assets/edit-report-box.png)

1. Redigera informationen i avsnitten till vänster i dialogrutan **Konfigurera**. De här avsnitten varierar beroende på vilken rapporttyp du redigerar.

1. (Valfritt) Om du redigerar en KPI-rapport kan du redigera information efter behov i följande avsnitt:

   * **Information**
   * **Skapa KPI**
   * **Filter**
   * **Kolumninställningar för detaljnivå**
   * **Inställningar för detaljnivågrupp**

   Mer information om de här avsnitten finns i [Skapa en KPI-rapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md).

1. (Valfritt) Om du redigerar en diagramrapport kan du redigera information efter behov i följande avsnitt:

   * **Information**
   * **Skapa diagram**
   * **Filter**
   * **Kolumninställningar för detaljnivå**
   * **Inställningar för detaljnivågrupp**

   Mer information om de här avsnitten finns i [Skapa en diagramrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

1. (Valfritt) Om du redigerar en tabellrapport kan du redigera information i följande avsnitt:

   * **Information**
   * **Skapa tabell**
   * **Filter**
   * **Gruppinställningar**

   Mer information om de här avsnitten finns i [Skapa en tabellrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

1. Klicka på **Spara** för att uppdatera rapporten.

## Redigera en befintlig rapport

När du redigerar en befintlig rapport åsidosätter de rapportdata du väljer de data som för närvarande visas i widgeten. Om du vill lägga till ytterligare en befintlig rapport i stället för att ersätta en bör du skapa en separat rapportwidget.

Mer information finns i [Lägga till en befintlig rapport på en arbetsytans kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md)

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på ikonen **Mer** **Mer** i det övre högra hörnet av rapporten som du vill redigera på sidan ![Arbetsytans kontrollpaneler](assets/more-icon.png) och välj sedan **Redigera** .

1. I rutan **Rapportval** klickar du på **Lägg till** i linje med den rapport som du vill ersätta den befintliga rapportwidgetens data med.
