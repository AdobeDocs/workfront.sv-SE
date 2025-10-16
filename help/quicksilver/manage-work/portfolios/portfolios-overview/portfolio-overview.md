---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: Förstå Portfolio-metoder
description: En Portfolio är en samling projekt som har enhetliga egenskaper. Dessa projekt konkurrerar vanligtvis om samma resurser, budget eller tidskortplats. Du kan dela upp portföljer i Program och associera projekten med Program innan de läggs till i en Portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Förstå portföljmetodik

<!-- Audited: 1/2024 -->

Portfolio eller Project Portfolio Management (PPM) är processen att prioritera och hantera en lista med projekt för att uppnå specifika affärsmål.

Allmän information om PPM finns i [Portfolio Management overview](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md).

I Adobe Workfront är en portfölj en samling projekt som har enhetliga egenskaper. Dessa projekt konkurrerar vanligtvis om samma resurser, budget eller tidskortplats. Du kan dela upp portföljer i Program och associera projekten med Program innan de läggs till i en Portfolio.

Du kan använda Portföljer och Program för att ordna projekt. Genom att organisera projekt kan du jämföra liknande projekt och avgöra var resurser ska användas bäst.

Mer information om hur du använder program finns i [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

Den här artikeln innehåller allmän information om portföljer i Workfront.

## Åtkomst krävs för att skapa portföljer

<!--leave the table uncollapsed as this article is about access-->

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paket</td> 
   <td> <p>Workfront Prime eller senare</p>
   <p>Arbetsflöde Prime eller senare</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till portföljer</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du har skapat en portfölj har du som standard behörighet att hantera den</p> 
   <p>Hantera behörigheter för att redigera en portfölj eller lägga till projekt i den</p>
   <p>Visa behörigheter för en portfölj för att visa den i Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Förstå portföljmetoden [!DNL Adobe Workfront]

I [!DNL Workfront] kan du lägga till projekt i portföljer för att skapa och organisera dina portföljer.

Vi rekommenderar att du följer dessa steg för att få en effektiv organisation av dina portföljer:

1. Skapa ett affärsärende för ett projekt och koppla projektet till en Portfolio.

   Om du vill skapa effektiva portfolior som ger företaget mervärde måste du börja med en projektförfrågan där du definierar affärsärendet för varje projekt som senare läggs till i portföljen.

   [!UICONTROL Business Case] innehåller följande information:

   * Allmän information om projektet (beskrivning, Portfolio- och programtilldelningar, projektägare och sponsor)
   * Projektets mål
   * Uppskattade utgiftskostnader
   * Resursbudgetar för arbetskostnader
   * Ett justeringsmoment
   * En riskbedömning

   Mer information om [!UICONTROL Business Case] finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   Du kan associera projektet med en portfölj när du skapar ett affärsärende. Du måste skapa en portfölj innan du kan associera den med ett projekt. Mer information finns i [Skapa en portfölj](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)

   Den information du samlar in när du skapar ett affärsärende används i [!UICONTROL portfolio optimizer] och [!UICONTROL resource planner] för att underlätta hanteringen av projektval.
1. Associera resurspooler med projekt när du skapar deras affärsärende.

   Portföljer är vanligtvis konfigurerade för att motsvara resurspooler. Programmen i en Portfolio är också anpassade till en resurspool. Korrelationen säkerställer att all resursplanering passar in i Portfolio eftersom projekten inom samma Portfolio vanligtvis konkurrerar om samma resurser.

   Mer information finns i [Skapa resurspooler](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

1. Få [!UICONTROL Business Case] godkänd av din Portfolio Manager.

   Mer information finns i [Godkänn ett affärsärende](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md).
1. Hantera prestanda för dina projekt i portföljen i [!UICONTROL Portfolio Optimizer].

   Portfolio-chefer kan spåra ekonomiska resultat i portföljen med hjälp av Portfolio dashboard. Kontrollpanelen visas i Portfolio sidhuvud.

   Mer information om ett Portfolio finansfält finns i avsnittet [Förstå finansfält i Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection) i [Portfolio Optimizer-översikt](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).
