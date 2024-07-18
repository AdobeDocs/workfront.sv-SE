---
title: Konfigurera en KPI-visualisering i rapportarbetsytan
description: Konfigurera en KPI-visualisering i rapportarbetsytan
hidefromtoc: true
hide: true
exl-id: 38beccf6-d7bc-478f-8bba-56607d315e6f
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Konfigurera en KPI-visualisering i rapportarbetsytan

En KPI-visualisering (Key Performance Indicator) kan hjälpa dig att snabbt förmedla organisationens aktuella prestanda.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurera en KPI-visualisering

>[!TIP]
>
>Alla ändringar sparas automatiskt när du skapar och redigerar blocken i rapporten.

1. Börja med att lägga till ett visualiseringsblock med visualiseringstypen **KPI** i en rapport, vilket förklaras i [Lägg till eller redigera ett visualiseringsblock i Rapporteringsarbetsyta](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Klicka på ikonen Redigera visualisering ![](assets/edit-icon.png) i det övre högra hörnet av visualiseringen och gör sedan något av följande.

   1. På fliken **Inställningar**:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualiseringstyp</td>
         <td><p>Växla till en annan typ av visualisering. Om du gör det kan de efterföljande alternativen på menyn ändras.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Source</td>
         <td>Markera de data som du vill ska visas i visualiseringen.</td>
        </tr>
        <tr>
         <td role="rowheader">Sammansättningstyp</td>
         <td><p> Ange hur du vill att värdena ska summeras:</p>
          <ul>
           <li><p><b>Antal</b>: Antalet värden</p></li>
           <li><p><b>Summa</b>: Summan av alla värden </p></li>
           <li><p><b>Medel</b>: Medelvärdet av alla värden</p></li>
           <li><p><b>Minimum</b>: Endast det lägsta värdet</p></li>
           <li><p>Maximum: endast det högsta värdet</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. På fliken **Data**:

      | Datakälla (listruta) | Ändra datakällan för visualiseringen till en annan tabell på rapportarbetsytan. |
      |---|---|
      | Visa data i Source | Aktivera det här alternativet om du vill visa källtabellen för visualiseringen på rapportarbetsytan eller inaktivera alternativet att dölja den. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Klicka var som helst utanför menyn för visualiseringsinställningar för att stänga den.
