---
title: Konfigurera en kolumnvisualisering i rapportarbetsytan
description: Konfigurera en kolumnvisualisering i rapportarbetsytan
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Konfigurera en kolumnvisualisering i rapportarbetsytan

En kolumnvisualisering kan hjälpa dig att snabbt berätta en historia om dina data genom att markera viktig information med hjälp av lodräta kolumner.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurera en kolumnvisualisering

>[!TIP]
>
>Alla ändringar sparas automatiskt när du skapar och redigerar blocken i rapporten.

1. Börja med att lägga till ett visualiseringsblock med **Kolumn** visualiseringstyp till en rapport, vilket förklaras i [Lägga till eller redigera ett visualiseringsblock i rapportarbetsytan](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Klicka på ikonen Redigera visualisering ![](assets/edit-icon.png) i det övre högra hörnet av visualiseringen gör något av följande.

   1. På **Inställningar** tab:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualiseringstyp</td>
         <td><p>Växla till en annan typ av visualisering. Om du gör det kan de efterföljande alternativen på menyn ändras.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Vågrät axel</td>
         <td><p>Markera de data som du vill avbilda längs den vågräta axeln eller X-axeln i kolumnvisualiseringen. I visualiseringen jämförs objekten på den här axeln utifrån varje objekt på den lodräta axeln.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Lodrät axel</td>
         <td><p>I den vänstra listrutan markerar du de data som du vill avbilda längs den vågräta axeln eller Y-axeln. Visualiseringen visar objekt på den här axeln som jämförande kolumner, baserat på deras värden.</p><p>I den högra listrutan väljer du hur du vill att dessa värden ska beräknas i visningen:</p>
          <ul>
           <li><p><b>Antal</b>: Antal värden</p></li>
           <li><p><b>Summa</b>: Summan av alla värden </p></li>
           <li><p><b>Genomsnittlig</b>: Medelvärdet för alla värden</p></li>
           <li><p><b>Minimum</b>: Endast det lägsta värdet</p></li>
           <li><p><b>Maximal</b>: Endast det högsta värdet</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. På **Data** tab:

      | Datakälla (listruta) | Ändra datakällan för visualiseringen till en annan tabell på rapportarbetsytan. |
      |---|---|
      | Visa datakälla | Aktivera det här alternativet om du vill visa källtabellen för visualiseringen på rapportarbetsytan eller inaktivera alternativet att dölja den. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Klicka var som helst utanför menyn för visualiseringsinställningar för att stänga den.
