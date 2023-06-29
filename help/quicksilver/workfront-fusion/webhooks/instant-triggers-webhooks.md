---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]
description: Många tjänster tillhandahåller webbhookar för att leverera snabbmeddelanden när en viss förändring inträffar i tjänsten. Om du vill bearbeta dessa meddelanden rekommenderar vi att du använder snabbutlösare. I den här artikeln beskrivs användningen och funktionaliteten hos direktutlösare i Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]

Många tjänster tillhandahåller webbhookar för att leverera snabbmeddelanden när en viss förändring inträffar i tjänsten. Om du vill bearbeta dessa meddelanden rekommenderar vi att du använder snabbutlösare. De här är lätta att känna igen i [!DNL Adobe Workfront Fusion] på grund av deras tagg:

![](assets/instant-350x256.png)

Om tjänsten inte tillhandahåller webhooks måste du använda avsökningsutlösare för att regelbundet avsöka tjänsten.

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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visa en webkroks kö

Alla meddelanden från inkommande webbhooks lagras i webbkrokens kö.

1. Klicka **[!UICONTROL Webhooks]** i menyn till vänster.
1. Hitta den webkrok som du vill visa kön för.
1. Klicka på knappen med en lastbilsikon och antal mottagna webbhooks.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Inkommande webkrockdata lagras alltid i kön oavsett hur du har ställt in alternativet [!UICONTROL Data] är konfidentiell (beskrivs i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Så snart data har bearbetats i ett scenario tas de bort permanent från systemet.

## Schemalägg direktutlösare

Om ditt scenario innehåller en direktutlösare kan du schemalägga att scenariot körs omedelbart:

![](assets/schedule-setting-350x185.png)

I så fall körs ditt scenario omedelbart när [!DNL Workfront Fusion] tar emot nya data från tjänsten. När scenariot har körts räknas det totala antalet väntande webbhooks som väntar i kön och scenariot utför så många cykler som det finns väntande webbhooks, och en webkrok bearbetas per cykel. Mer information finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* En cykel är inte detsamma som en scenariokörning. Det kan finnas flera cykler inom 1 scenario-körning.
>* När du kör ett scenario med en omedelbar utlösare som är schemalagd att vara omedelbar gäller följande undantag:
>
>     * Intervallet mellan två körningar omfattas inte av minimiintervallet enligt prissättningsplanen.
>
>       När till exempel scenariot har slutförts kontrolleras webbkrokens kö igen. Om det finns några väntande webbhooks körs scenariot omedelbart igen och alla väntande webbhooks bearbetas igen.
>   
>     * Inställningen för maximalt antal cykler ignoreras och ställs in på 100, vilket innebär att högst 100 väntande webbhooks bearbetas under en enda scenariokörning (med en hastighet på 1 händelse per cykel).
>


Om du använder någon annan schemainställning än [!UICONTROL Immediately]körs scenariot med de intervall du anger. Eftersom det går att samla in flera webbböcker i kön under intervallet bör du ange [[!UICONTROL Maximum number of cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) till ett högre värde än standard 1 för att bearbeta fler webbhooks i en enda scenario:

1. Klicka på [!UICONTROL Scenario settings] icon ![](assets/gear-icon-settings.png) längst ned i ditt scenario.
1. I **[!UICONTROL Scenario settings]** anger du en siffra i rutan som visas **[!UICONTROL Max number of cycles]** om du vill ange antalet webbböcker från kön som du vill köra varje gång du kör scenariot.

## Kursgränser

Den aktuella hastighetsgränsen är 5 webbhooks per sekund. Om gränsen överskrids returneras en 429-statuskod.

## Inaktiva webhooks förfaller

En webkrok som inte har tilldelats något scenario på mer än 120 timmar tas bort.

## Webkrok-nyttolaster

[!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den skapades uppstår felet &quot;[!UICONTROL Failed to read file from storage.]&quot;

## Felhantering

När ett fel inträffar i ditt scenario med en direktutlösare:

* Stoppar omedelbart - när scenariot är inställt på att köras [!UICONTROL Immediately].
* Stoppar efter 3 misslyckade försök (3 fel) - när scenariot är inställt på att köras enligt schema.

Om ett fel inträffar under scenariokörningen placeras webkroken tillbaka i kön under direktutlösarens återställningsfas. I en sådan situation kan du åtgärda scenariot och köra det igen. Mer information finns i [Återställning](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) i artikeln [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Om det finns en Webkroks svarsmodul i ditt scenario skickas felet till Webkroks svar. Webkroks svarsmodul körs alltid sist (om [!UICONTROL Auto commit] alternativet i scenarieinställningarna är inte aktiverat). Mer information finns i [Svara på webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) i artikeln [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Anpassade webbhotell

Du kan skapa egna webbböcker. Mer information finns i [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webkroks-inaktivering

Webhooks inaktiveras automatiskt om något av följande gäller:

* Webbkroken har inte varit ansluten till något scenario på mer än fem dagar
* Webkroken används bara i inaktiva scenarier, som har varit inaktiva i mer än 30 dagar.

Inaktiverade webhooks tas bort och avregistreras automatiskt om de inte är anslutna till några scenarier och har inaktiverats i över 30 dagar.


