---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Panelen för scenarioinställningar i Adobe Workfront Fusion
description: I den här artikeln beskrivs de inställningar som är tillgängliga på panelen [!UICONTROL scenario settings] i dina [!DNL Adobe Workfront Fusion] scenarier.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 1b729960a23e43252bda16d9bfb7ca9656a115a1
workflow-type: tm+mt
source-wordcount: '1024'
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
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Öppna scenarioinställningarna

1. Öppna scenarioredigeraren enligt beskrivningen i [Scenarieredigeraren i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Klicka på kugghjulsikonen i det nedre vänstra hörnet på sidan.

   ![](assets/scenario-settings-350x221.png)

   På panelen [!UICONTROL Scenario settings] som visas kan du konfigurera olika avancerade inställningar för scenariot.

## [!UICONTROL Allow storing incomplete executions]

Det här alternativet avgör hur [!DNL Adobe Workfront Fusion] fortsätter om ett fel inträffar under körningen av ett scenario. När det här alternativet är aktiverat pausas scenariot och flyttas till [Visa och löser ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Detta ger dig möjlighet att åtgärda problemet och fortsätta att köra från där scenariot stoppades. Om det här alternativet är inaktiverat stoppas scenariot och en återställningsfas startas.

## [!UICONTROL Sequential processing]

Det här alternativet avgör hur [!DNL Workfront Fusion] fortsätter om ett fel inträffar och körningen av ett scenario flyttas till [vyn och löser ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Om alternativet [!UICONTROL Sequential processing] är aktiverat slutar Workfront Fusion att bearbeta aktivitetssekvensen helt tills alla ofullständiga körningar har lösts. Om alternativet [!UICONTROL Sequential processing] är inaktiverat fortsätter scenariot att köras enligt schemat, tillsammans med upprepade försök att köra de ofullständiga körningarna igen.

>[!NOTE]
>
>Sekventiell bearbetning kan orsaka en fördröjning i körningen av ett scenario. Om det fortfarande finns ofullständiga körningar i kön när en utlösare för ett instansscenario eller ett schemalagt scenario är inställt på att köras, kommer det scenariot att köras när alla körningar är slutförda innan det är klart.
>
>Om användningsfallet för dina scenarier inte kräver sekventiell bearbetning rekommenderar vi att du inaktiverar alternativet för sekventiell bearbetning.

Mer information om schemaläggning finns i [Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Data är konfidentiella

När ett scenario har körts kan du som standard visa information om vilka data som har bearbetats av moduler i scenariot. Om du inte vill att den här informationen ska lagras aktiverar du alternativet [!UICONTROL Data is confidential].

Mer information om hur du visar information finns i [Körningsflöde för scenarier i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Om du aktiverar det här alternativet kan det vara svårt att lösa fel som kan uppstå när ett scenario körs.

## Aktivera dataförlust

Det här alternativet har att göra med aktivering av dataförlust om [!DNL Workfront Fusion] inte kan spara ett paket i kön för [Visa och lösa ofullständiga körningar i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (till exempel på grund av brist på ledigt utrymme). När det här alternativet är aktiverat går data förlorade för att förhindra avbrott i den övergripande scenariokörningen. Detta är användbart för scenarier där högsta prioritet är kontinuerlig körning och inkommande felaktiga data inte är så viktiga.

När ett scenario körs kan en modul ibland stöta på en fil som är större än den tillåtna maxstorleken. I det här fallet fortsätter [!DNL Workfront Fusion] i enlighet med inställningen för alternativet [!UICONTROL Enable data loss] och ett varningsmeddelande visas.

Mer information om maximal filstorlek finns i [Om att mappa filer i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Mer information om varningar finns i [Felbearbetning i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

Inställningarna [!UICONTROL Auto commit] gäller för transaktioner och definierar hur ett scenario ska bearbetas. Om alternativet för automatisk implementering är aktiverat startar implementeringsfasen för varje modul omedelbart efter att operationsfasen har slutförts. När alternativet Automatisk implementering är inaktiverat utförs ingen implementering förrän åtgärderna körs för alla moduler (det här är standardläget).

Mer information om transaktioner finns i [Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximalt antal cykler

Det kan vara praktiskt att ange fler cykler när du vill förhindra avbrott i anslutningen till en tredjepartstjänst och försäkra dig om att alla poster behandlas i en enda scenario.

* Om scenariot börjar med en avsökningsutlösare definierar inställningen det maximala antalet cykler som tillåts under scenariokörningen.

  Mer information om avsökningsutlösare finns i [Avsökningsutlösare](../../workfront-fusion/modules/module-types.md#polling) i [Olika typer av moduler](../../workfront-fusion/modules/module-types.md).

* Om scenariot börjar med en direktutlösare ignoreras inställningen och alla väntande händelser bearbetas under en enda körning, en händelse per cykel.

  Mer information om snabbutlösare finns i [Direktutlösare](../../workfront-fusion/modules/module-types.md#instant) i [Olika typer av moduler](../../workfront-fusion/modules/module-types.md).

* Om scenariot inte börjar med en utlösare (direkt/avsökning) utförs alltid det angivna maximala antalet cykler.

>[!INFO]
>
>**Exempel:** [!DNL Workfront] > [!UICONTROL Watch record] söker efter nya problem som kommer in, och [!DNL Workfront] >[!UICONTROL Convert object] konverterar den nya begäran till ett projekt och tilldelar den lämplig mall.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>En [!UICONTROL more cycles]-inställning används bara när du schemalägger din scenariokörning. När du använder knappen [!UICONTROL Run once] beaktas cykelinställningarna.
>
>### Maximalt antal cykler är 1 (standard)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL Maximum number of returned files] i modulen [!UICONTROL Workfront] >[!UICONTROL Watch records] är inställd på `10`.
>Om 100 begäranden skickas till [!DNL Workfront], och fältet [!UICONTROL Limit] är inställt på 10, lämnas 90 filer obearbetade efter att ett scenario har körts. De nästa 10 filerna bearbetas i nästa körning av schemalagda scenario.
>
>### Högsta antal cykler är 10
>
>[!UICONTROL Maximum number of returned files] i modulen [!UICONTROL Dropbox] >[!UICONTROL Watch files] är inställd på `10`.
>
>Om 100 filer läggs till i mappen Dropbox och alternativet [!UICONTROL Maximum number of returned files] är inställt på 10, bearbetas 10 filer under den första cykeln, de nästa 10 filerna i den andra cykeln, de kommande 10 filerna i den tredje cykeln o.s.v. tills alla filer har bearbetats.
>
>Alla filer bearbetas inom 1 scenariokörning.
>
>Du kan se de cykler som redan körs i scenarioinformationen:
>
>![](assets/scenario-detail-350x207.png)
>
>Mer information om den här sidan finns i [Scenarioinformation i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Antal efterföljande fel

Definierar det maximala antalet på varandra följande körningsförsök innan körningen av ett scenario inaktiveras (exklusive [!UICONTROL DataError], [!UICONTROL DuplicateDataError] och [!UICONTROL ConnectionError]).

Mer information om fel finns i [Felbearbetning i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Om ett scenario börjar med en direktutlösare ignoreras inställningen och scenariot inaktiveras omedelbart när det första felet har inträffat.
