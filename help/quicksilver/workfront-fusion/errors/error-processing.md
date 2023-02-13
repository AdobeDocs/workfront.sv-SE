---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fel vid bearbetning av [!DNL Adobe Workfront Fusion]
description: Ibland kan ett fel inträffa när ett scenario körs. Detta händer vanligtvis om en tjänst inte är tillgänglig på grund av ett fel med anslutningen till en tjänst eller om en validering misslyckas. I den här artikeln beskrivs de vanligaste felen som kan uppstå.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Fel vid bearbetning av [!DNL Adobe Workfront Fusion]

Ibland kan ett fel inträffa när ett scenario körs. Detta händer vanligtvis om en tjänst inte är tillgänglig på grund av ett fel med anslutningen till en tjänst eller om en validering misslyckas. I den här artikeln beskrivs de vanligaste felen som kan uppstå.

[!DNL Adobe Workfront Fusion] skiljer mellan flera grundläggande feltyper. Den kommer att reagera annorlunda beroende på vilken typ av fel som inträffade.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Anslutningsfel

`ConnectionError`

Anslutningsfel är ett av de vanligaste felen som vanligtvis orsakas av att tredjepartstjänsten inte är tillgänglig av olika anledningar (överbelastning, underhåll, driftstopp osv.). Standardhanteringen av det här felet beror på vilken modul det påträffades i:

* Om felet inträffar i den första modulen avslutas körningen av scenariot med ett varningsmeddelande. [!DNL Workfront Fusion] försöker sedan upprepade gånger att köra scenariot igen med ökande tidsintervall (dessa beskrivs nedan). Om alla försök misslyckas, [!DNL Workfront Fusion] inaktiverar scenariot.
* Om anslutningsfelet inträffar i en annan modul än i den första, beror efterföljande steg på [Tillåt lagring av ofullständiga körningar](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) i scenariot avancerade inställningar:

   * Om det här alternativet är aktiverat flyttas körningen av scenariot till [!UICONTROL Incomplete executions] mapp där [!DNL Workfront Fusion] försöker upprepade gånger att köra scenariot igen med ökande tidsintervall. Om alla försök misslyckas finns körningen kvar i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) mapp som väntar på manuell upplösning av användaren.
   * Om alternativet är inaktiverat avslutas körningen av scenariot med ett fel följt av en återställningsfas. [!DNL Workfront Fusion] försöker sedan upprepade gånger att köra scenariot igen med ökande tidsintervall. Om alla försök misslyckas, [!DNL Workfront Fusion] inaktiverar scenariot.

### Öka tidsintervall

Algoritmen för att öka tidsintervallen multiplikativt mellan försöken när ett fel inträffar kallas exponentiell säkerhetskopiering. De ökande tidsintervallen anges enligt följande:

1. 10 minuter
1. 1 timme
1. 3 timmar
1. 12 timmar
1. 24 timmar

Huvudorsaken till att de ökade tidsintervallen används i [!DNL Workfront Fusion] är att förhindra att ofta utförda scenarier använder åtgärder vid upprepade misslyckade försök.

>[!INFO]
>
>**Exempel:**
>
>Ett scenario innehåller [!DNL Google Sheets] trigger [!UICONTROL Watch Rows]. [!DNL Google Sheets] är inte tillgängligt på 30 minuter på grund av underhåll när [!DNL Workfront Fusion] startar scenariot, så det går inte att hämta nya rader. Scenariot stoppas och försöker igen om 10 minuter. Eftersom tjänsten fortfarande inte är tillgänglig inom den här tidsramen [!DNL Workfront Fusion] kan fortfarande inte få information om nya rader. Nästa omgång av scenariot är schemalagd om en timme. [!DNL Google Sheets] är tillgängligt igen inom den här tiden och scenariot kan köras.

## Datafel

`DataError`

Ett datafel genereras när ett objekt är felaktigt mappat och inte godkänns i den validering som utförts på [!DNL Workfront Fusion] sida vid eller bredvid den tredjepartstjänst som används. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Om det här felet inträffar flyttas scenariot, fram till där modulen misslyckades, till mappen för ofullständiga körningar där du kan felsöka problemet. Scenariot avbryts dock inte och fortsätter att köras enligt schemat. Om du vill stoppa körningen av scenariot när ett datafel visas aktiverar du alternativet Sekventiell bearbetning på panelen Scenarioinställningar.

Om du inte har aktiverat [!UICONTROL Allow storing incomplete executions] i scenarioinställningarna avslutas körningen av scenariot med felet och en återställning utförs.

Information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Information om scenarioinställningspanelen finns i [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Mer information om scheman finns i [Schemalägg ett scenario i Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Fel vid duplicering av data

`DuplicateDataError`

If [!DNL Workfront Fusion] försöker infoga samma paket två gånger i en tjänst som inte tillåter dubblettdata, ett dubblettdatafel genereras. Om detta fel inträffar [!DNL Workfront Fusion] fortsätter på samma sätt som för datafel.

## Ogiltigt åtkomsttokenfel

`InvalidAccessTokenError`

Ett ogiltigt åtkomsttokenfel inträffar när [!DNL Workfront Fusion] kan inte komma åt ditt konto som är registrerat hos en tredjepartstjänst. Detta händer oftast när du återkallar åtkomsträttigheter för [!DNL Workfront Fusion] vid administration av en viss tjänst, men relaterade scenarier fortsätter att köras enligt schema.

Om det här felet inträffar stoppas körningen av ett scenario omedelbart. Resten av scenariot med början från modulen där felet inträffade flyttas till mappen för ofullständiga körningar.

Information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Hastighetsbegränsningsfel

`RateLimitError`

Om en gräns som angetts av en viss tjänst överskrids genereras ett hastighetsbegränsningsfel. Om det här felet inträffar [!DNL Workfront Fusion] fortsätter på samma sätt som för anslutningsfelet. Mer information finns i [Anslutningsfel](#connection-error).

## Ofullständigt datafel

`IncompleteDataError`

Ett ofullständigt datafel inträffar bara med utlösare. Det här felet genereras om en utlösare inte kan hämta nödvändiga data från en viss tjänst.

Om ett scenario avslutas med `IncompleteDataError`, beror dess ytterligare beteende på inställningen av [!UICONTROL Max number of consecutive errors]. Mer information finns i [Antal efterföljande fel](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) i artikeln [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exempel:** Ett scenario har [!DNL Workfront] trigger [!UICONTROL Watch Record] för att bevaka dokument. Scenariot körs medan du överför ett stort dokument, till exempel en lång video. För [!UICONTROL Workfront Fusion] försöker hämta videon medan den fortfarande överförs till Workfront, avslutas scenariot med `IncompleteDataError`.

## Körningsfel

`RuntimeError`

Om något annat fel (som inte nämns ovan) inträffar under scenariokörningen rapporteras det som ett `RunTimeError`.

Om ett scenario avslutas med `RuntimeError`, beror dess ytterligare beteende på inställningen av [!UICONTROL Max number of consecutive errors]. Mer information finns i [Antal efterföljande fel](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) i artikeln [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Om ett scenario börjar med en direktutlösare anges inställningen för [!UICONTROL Max number of consecutive errors] ignoreras och scenariot inaktiveras omedelbart när det första felet har inträffat. Mer information finns i [Direktutlösare](../../workfront-fusion/modules/module-types.md#instant) i artikeln [Typer av moduler](../../workfront-fusion/modules/module-types.md).

## Inkonsekvens-fel

`InconsistencyError`

Om något av de fel som beskrivs ovan inträffar under implementerings- eller återställningsfasen avslutas ett scenario med ett inkonsekvens-fel. Mer information finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Om det här felet uppstår i ett scenario stoppas körningen av scenariot omedelbart.

## Varning

När du kör ett scenario kan du få en varning som informerar dig om ett problem. Det förhindrar dock inte att scenariot slutförs korrekt.

En varning kan till exempel visas när den största tillåtna filstorleken överskrids och [!UICONTROL Enable data loss] är inaktiverat. Mer information finns i [Aktivera dataförlust](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) i artikeln [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
