---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Felhantering av fel i Adobe Workfront Fusion
description: I vissa fall kanske du vill stoppa scenariokörningen följt av återställnings- eller implementeringsfasen eller stoppa bearbetningen av en väg och eventuellt lagra den i kön för Visa och lösa ofullständiga körningar i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Felhantering av utlösta fel i [!DNL Adobe Workfront Fusion]

I vissa fall kanske du vill stoppa scenariokörningen följt av fasen [Återställning](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) eller [Verkställ](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) eller stoppa bearbetningen av en väg och eventuellt lagra den i kön med ofullständiga körningar.

För närvarande kan inte felhanteringsdirektiven användas utanför omfånget för en [Felhanterarväg](../../workfront-fusion/errors/error-handling.md#error) och [!DNL Adobe Workfront Fusion] erbjuder inte en modul som gör att du enkelt kan generera (utlösa) fel villkorligt.

Mer information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Mer information om felhanteringsdirektiv finns i [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Tillfällig lösning för Throw

Om du vill att ett fel ska utlösas villkorligt kan du konfigurera en modul så att den eventuellt kan misslyckas under åtgärden. Ett sätt är att använda modulen [!UICONTROL JSON] > [!UICONTROL Parse JSON] (se [ JSON-moduler](../../workfront-fusion/apps-and-their-modules/json-modules.md)), som konfigurerats för att utlösa ett fel (BundleValidationError i det här fallet):

Du kan sedan bifoga ett av felhanteringsdirektiven till felhanteringsvägen till:

* Tvinga scenariokörningen att stoppa och utföra återställningsfasen: [!UICONTROL Rollback]
* Tvinga scenariokörningen att stoppa och utföra implementeringsfasen: [!UICONTROL Commit]
* Stoppa bearbetning av en väg: [!UICONTROL Ignore]
* Stoppa bearbetningen av en väg och lagra den i kön med ofullständiga körningsmappar: [!UICONTROL Break]

I följande exempel visas hur direktivet [!DNL Rollback] används:

![](assets/rollback-directive-350x175.png)
