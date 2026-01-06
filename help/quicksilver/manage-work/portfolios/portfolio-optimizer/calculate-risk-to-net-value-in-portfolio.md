---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Beräkna risk till nettovärde i en portfölj
description: I Portfolio Optimizer mäter indikatorn [!UICONTROL Risk to Net Value] den potentiella risken med hänsyn till det nettovärde som anges i alla projekt som visas i Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---

# Beräkna [!UICONTROL Risk to Net Value] i en portfölj

I [!UICONTROL Portfolio Optimizer] mäter indikatorn [!UICONTROL Risk to Net Value] den potentiella risken med hänsyn till [!UICONTROL Net Value] som tillhandahålls av alla projekt som visas i [!UICONTROL Portfolio Optimizer].

För att uppnå maximal effektivitet i portföljen vill du se att indikatorn [!UICONTROL Risk] är låg och att indikatorn [!UICONTROL Net Value] är hög.

Indikatorerna [!UICONTROL Risk] och [!UICONTROL Net Value] representeras utifrån hur de relaterar till varandra.

[!DNL Adobe Workfront] beräknar indikatorerna [!UICONTROL Risk] och [!UICONTROL Net Value] med hjälp av följande formler:

* Indikatorn [!UICONTROL Risk] beräknas med följande formel:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* Indikatorn [!DNL Net Value] beräknas med följande formler:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  eller

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>Indikatorn [!UICONTROL Risk to Net Value] beräknas baserat på de projekt som du visar i [!UICONTROL Portfolio Optimizer] och inte på alla projekt som är associerade med portföljen.
