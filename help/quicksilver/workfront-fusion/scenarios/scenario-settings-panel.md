---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Panelen för scenarioinställningar i Adobe Workfront Fusion
description: I den här artikeln beskrivs de inställningar som är tillgängliga i [!UICONTROL scenario settings] panelen i [!DNL Adobe Workfront Fusion] scenarier.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Öppna scenarioinställningarna

1. Öppna scenarioredigeraren enligt anvisningarna i [Scenarioredigeraren i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Klicka på kugghjulsikonen i sidans nedre vänstra hörn.

   ![](assets/scenario-settings-350x221.png)

   I [!UICONTROL Scenario settings] som visas kan du konfigurera olika avancerade inställningar för scenariot.

## [!UICONTROL Allow storing incomplete executions]

Det här alternativet avgör hur [!DNL Adobe Workfront Fusion] fortsätter om ett fel inträffar när ett scenario körs. När det här alternativet är aktiverat pausas scenariot och flyttas till [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Detta ger dig möjlighet att åtgärda problemet och fortsätta att köra från där scenariot stoppades. Om det här alternativet är inaktiverat stoppas scenariot och en återställningsfas startas.

## [!UICONTROL Sequential processing]

Det här alternativet avgör hur [!DNL Workfront Fusion] fortsätter om ett fel inträffar och körningen av ett scenario flyttas till [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Om [!UICONTROL Sequential processing] om det här alternativet är aktiverat slutar Workfront Fusion att bearbeta aktivitetssekvensen helt tills alla ofullständiga körningar är åtgärdade. Om [!UICONTROL Sequential processing] alternativet är inaktiverat fortsätter scenariot att köras enligt schemat, följt av upprepade försök att köra de ofullständiga körningarna igen.

Mer information om schemaläggning finns i [Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Data är konfidentiella

När ett scenario har körts kan du som standard visa information om vilka data som har bearbetats av moduler i scenariot. Om du inte vill att den här informationen ska lagras aktiverar du [!UICONTROL Data is confidential] alternativ.

Mer information om hur du visar information finns i [Scenariokörningsflöde i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Om du aktiverar det här alternativet kan det vara svårt att lösa fel som kan uppstå när ett scenario körs.

## Aktivera dataförlust

Det här alternativet har att göra med aktivering av dataförlust om [!DNL Workfront Fusion] inte kan spara ett paket i kön till [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (t.ex. på grund av brist på ledigt utrymme). När det här alternativet är aktiverat går data förlorade för att förhindra avbrott i den övergripande scenariokörningen. Detta är användbart för scenarier där högsta prioritet är kontinuerlig körning och inkommande felaktiga data inte är så viktiga.

När ett scenario körs kan en modul ibland stöta på en fil som är större än den tillåtna maxstorleken. I detta fall [!DNL Workfront Fusion] intäkter i enlighet med inställningen av [!UICONTROL Enable data loss] och ett varningsmeddelande visas.

Mer information om maximal filstorlek finns i [Om att mappa filer i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Mer information om varningar finns i [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

The [!UICONTROL Auto commit] inställningarna gäller för transaktioner och definierar hur ett scenario ska bearbetas. Om alternativet för automatisk implementering är aktiverat startar implementeringsfasen för varje modul omedelbart efter att operationsfasen har slutförts. När alternativet Automatisk implementering är inaktiverat utförs ingen implementering förrän åtgärderna körs för alla moduler (det här är standardläget).

Mer information om transaktioner finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximalt antal cykler

Det kan vara praktiskt att ange fler cykler när du vill förhindra avbrott i anslutningen till en tredjepartstjänst och försäkra dig om att alla poster behandlas i en enda scenario.

* Om scenariot börjar med en avsökningsutlösare definierar inställningen det maximala antalet cykler som tillåts under scenariokörningen.

   Mer information om avsökningsutlösare finns i [Avsökningsutlösare](../../workfront-fusion/modules/module-types.md#polling) in [Typer av moduler](../../workfront-fusion/modules/module-types.md).

* Om scenariot börjar med en direktutlösare ignoreras inställningen och alla väntande händelser bearbetas under en enda körning, en händelse per cykel.

   Mer information om direktutlösare finns i [Direktutlösare](../../workfront-fusion/modules/module-types.md#instant) in [Typer av moduler](../../workfront-fusion/modules/module-types.md).

* Om scenariot inte börjar med en utlösare (direkt/avsökning) utförs alltid det angivna maximala antalet cykler.

>[!INFO]
>
>**Exempel:**  [!DNL Workfront] > [!UICONTROL Watch record] söker efter nya utgåvor som kommer in, och [!DNL Workfront] >[!UICONTROL Convert object] konverterar den nya begäran till ett projekt och tilldelar den lämplig mall.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL more cycles] inställningen används bara när du schemalägger din scenariokörning. När du använder [!UICONTROL Run once] -knappen används cykelinställningarna.
>
>### Maximalt antal cykler är 1 (standard)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>The [!UICONTROL Maximum number of returned files] i [!UICONTROL Dropbox] >[!UICONTROL Watch files] modulen är inställd på `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Om 100 begäranden skickas till [!DNL Workfront]och [!UICONTROL Limit] anges till 10, sedan lämnas 90 filer obearbetade efter att ett scenario har körts. De nästa 10 filerna bearbetas i nästa körning av schemalagda scenario.
>
>### Högsta antal cykler är 10
>
>The [!UICONTROL Maximum number of returned files] i [!UICONTROL Dropbox] >[!UICONTROL Watch files] modulen är inställd på `10`.
>
>Om 100 filer läggs till i mappen Dropbox och [!UICONTROL Maximum number of returned files] är inställt på 10, sedan bearbetas 10 filer under den första cykeln, de nästa 10 filerna i den andra cykeln, de nästa 10 filerna i den tredje cykeln och så vidare, tills alla filer har bearbetats.
>
>Alla filer bearbetas inom 1 scenariokörning.
>
>Du kan se de cykler som redan körs i scenarioinformationen:
>
>![](assets/scenario-detail-350x207.png)
>
>Mer information om den här sidan finns på [Scenarioinformation i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Antal efterföljande fel

Definierar det maximala antalet på varandra följande körningsförsök innan körningen av ett scenario inaktiveras (exklusive [!UICONTROL DataError], [!UICONTROL DuplicateDataError] och [!UICONTROL ConnectionError]).

Mer information om fel finns i [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Om ett scenario börjar med en direktutlösare ignoreras inställningen och scenariot inaktiveras omedelbart när det första felet har inträffat.
