---
title: Konfigurera en fältvisualisering i rapportarbetsytan
description: Konfigurera en fältvisualisering i rapportarbetsytan
author: Nolan
feature: Reports and Dashboards
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Konfigurera en fältvisualisering i rapportarbetsytan

En fältvisualisering kan hjälpa dig att snabbt berätta en historia om dina data genom att markera viktig information med vågräta fält.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurera en fältvisualisering

>[!NOTE]
>
>Alla ändringar sparas automatiskt när du skapar och redigerar blocken i rapporten.

1. Börja med att lägga till ett visualiseringsblock med **Liggande** visualiseringstyp till en rapport, vilket förklaras i [Lägga till eller redigera ett visualiseringsblock i rapportarbetsytan](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">Lodrät axel</td>
         <td><p>Markera de data som du vill avbilda längs den lodräta vänstra kanten eller längs Y-axeln i fältvisualiseringen. I visualiseringen jämförs objekten på den här axeln utifrån varje objekt på den vågräta axeln.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Vågrät axel</td>
         <td><p>I den vänstra listrutan markerar du de data som du vill avbilda längs den vågräta axeln eller X-axeln. Objekten på den här axeln visas som jämförande fält, baserat på deras värden.</p><p>I den högra listrutan väljer du hur du vill att visualiseringen ska beräkna och visa värdena längs den vågräta axeln:</p>
          <ul>
           <li><p><b>Antal</b>: Antal värden</p></li>
           <li><p><b>Summa</b>: Summan av alla värden </p></li>
           <li><p><b>Genomsnittlig</b>: Medelvärdet för alla värden</p></li>
           <li><p><b>Minimum</b>: Endast det lägsta värdet</p></li>
           <li><p><b>Maximal</b>: Endast det högsta värdet</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Lägg till värde</td>
         <td>Lägg till ett annat fält som du vill spåra längs den vågräta axeln.</td>
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
