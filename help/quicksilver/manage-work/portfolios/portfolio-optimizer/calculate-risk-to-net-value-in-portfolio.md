---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Beräkna risk till nettovärde i en portfölj
description: I Portfolio Optimizer finns [!UICONTROL Risk to Net Value] Indikatorn mäter den potentiella risken med beaktande av det nettovärde som tillhandahålls av alla projekt som visas i optimeringsfunktionen för Portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---

# Beräkna [!UICONTROL Risk to Net Value] i en portfölj

I [!UICONTROL Portfolio Optimizer], [!UICONTROL Risk to Net Value] Indikatorn mäter den potentiella risken med beaktande av [!UICONTROL Net Value] från alla projekt som visas i [!UICONTROL Portfolio Optimizer]. 

För att uppnå maximal effektivitet i portföljen vill du se att [!UICONTROL Risk] indikatorn är låg och [!UICONTROL Net Value] indikatorn är hög. 

The [!UICONTROL Risk] och [!UICONTROL Net Value] indikatorerna representeras utifrån hur de hänger ihop.

[!DNL Adobe Workfront] beräknar [!UICONTROL Risk] och [!UICONTROL Net Value] indikatorer med hjälp av följande formler:

* The [!UICONTROL Risk] Indikatorn beräknas med följande formel:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* The [!DNL Net Value] Indikatorn beräknas med följande formler:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   eller

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>The [!UICONTROL Risk to Net Value] indikatorberäkningarna baseras på de projekt som du visar i [!UICONTROL Portfolio Optimizer]och inte i alla projekt som är kopplade till portföljen. 
