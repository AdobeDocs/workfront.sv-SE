---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Direktutlösare (webhooks) i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 0%

---

# Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artiklarna:
>
>* [Direktutlösare (webhooks)](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/webhooks-reference.html)
>* [Visa en webkroks kö](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-webhook-queue.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Många tjänster tillhandahåller webbhookar för att leverera snabbmeddelanden när en viss förändring inträffar i tjänsten. Om du vill bearbeta dessa meddelanden rekommenderar vi att du använder snabbutlösare. Du kan enkelt identifiera dessa i [!DNL Adobe Workfront Fusion] på grund av deras tagg:

![](assets/instant-350x256.png)

Om tjänsten inte tillhandahåller webhooks måste du använda avsökningsutlösare för att regelbundet avsöka tjänsten.

En videointroduktion till webbhooks i Workfront Fusion finns på:

* [Introduktion till Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Mellanliggande webbhooks](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## Visa en webkroks kö

Alla meddelanden från inkommande webbhooks lagras i webbkrokens kö.

1. Klicka på **[!UICONTROL Webhooks]** på menyn till vänster.
1. Hitta den webkrok som du vill visa kön för.
1. Klicka på knappen med en lastbilsikon och antal mottagna webbböcker.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Inkommande webkrockdata lagras alltid i kön oavsett hur du har angett alternativet [!UICONTROL Data] är konfidentiellt (beskrivs i [Panelen för scenarioinställningar i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Så snart data har bearbetats i ett scenario tas de bort permanent från systemet.

## Schemalägg direktutlösare

Om ditt scenario innehåller en direktutlösare kan du schemalägga att scenariot körs omedelbart:

![](assets/schedule-setting-350x185.png)

I det här fallet körs ditt scenario omedelbart när [!DNL Workfront Fusion] tar emot nya data från tjänsten. När scenariot har körts räknas det totala antalet väntande webbhooks som väntar i kön och scenariot utför så många cykler som det finns väntande webbhooks, och en webkrok bearbetas per cykel. Mer information finns i [Körning av scenario, cykler och faser i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

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


Om du använder någon annan schemainställning än [!UICONTROL Immediately] körs scenariot med de intervall du anger. Eftersom flera webhooks kan samlas in i kön under intervallet, bör du ange ett högre värde för [[!UICONTROL Maximum number of cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) än standardvärdet 1 för att bearbeta fler webhooks i ett scenario:

1. Klicka på ikonen [!UICONTROL Scenario settings] ![](assets/gear-icon-settings.png) längst ned i ditt scenario.
1. I rutan **[!UICONTROL Scenario settings]** som visas anger du en siffra i rutan **[!UICONTROL Max number of cycles]** för att ange hur många webbböcker från kön du vill köra varje gång du kör scenariot.

## Kursgränser

Den aktuella hastighetsgränsen är 5 webbhooks per sekund. Om gränsen överskrids returneras en 429-statuskod.

## Inaktiva webhooks förfaller

En webkrok som inte har tilldelats något scenario på mer än 120 timmar tas bort.

## Webkrok-nyttolaster

[!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den skapades uppstår felet [!UICONTROL Failed to read file from storage.]

## Felhantering

När det finns ett fel i ditt scenario med en direktutlösare:

* Stoppar omedelbart - när scenariot är inställt på att köra [!UICONTROL Immediately].
* Stoppar efter 3 misslyckade försök (3 fel) - när scenariot är inställt på att köras enligt schema.

Om ett fel inträffar under scenariokörningen placeras webkroken tillbaka i kön under direktutlösarens återställningsfas. I en sådan situation kan du åtgärda scenariot och köra det igen. Mer information finns i [Återställning](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) i artikeln [Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Om det finns en Webkroks svarsmodul i ditt scenario skickas felet till Webkroks svar. Webkroks svarsmodul körs alltid sist (om alternativet [!UICONTROL Auto commit] i scenarieinställningarna inte är aktiverat). Mer information finns i [Svara på webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) i artikeln [Webbhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Anpassade webbhotell

Du kan skapa egna webbböcker. Mer information finns i [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webkroks-inaktivering

Webhooks inaktiveras automatiskt om något av följande gäller:

* Webbkroken har inte varit ansluten till något scenario på mer än fem dagar
* Webkroken används bara i inaktiva scenarier, som har varit inaktiva i mer än 30 dagar.

Inaktiverade webhooks tas bort och avregistreras automatiskt om de inte är anslutna till några scenarier och har inaktiverats i över 30 dagar.


