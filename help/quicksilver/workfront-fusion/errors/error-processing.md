---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fel vid bearbetning i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Fel vid bearbetning i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Feltyper](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/error-processing.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Anslutningsfel

`ConnectionError`

Anslutningsfel är ett av de vanligaste felen som orsakas av att tredjepartstjänsten inte är tillgänglig av olika anledningar (överbelastning, underhåll, driftstopp osv.). Standardhanteringen av det här felet beror på vilken modul det påträffades i:

* Om felet inträffar i den första modulen avslutas körningen av scenariot med ett varningsmeddelande. [!DNL Workfront Fusion] försöker sedan upprepade gånger att köra scenariot igen med ökande tidsintervall (dessa beskrivs nedan). Om alla försök misslyckas inaktiverar [!DNL Workfront Fusion] scenariot.
* Om anslutningsfelet inträffar i en annan modul än i den första, beror efterföljande steg på alternativet [Tillåt lagring av ofullständiga körningar](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) i scenariets avancerade inställningar:

   * Om det här alternativet är aktiverat flyttas körningen av scenariot till mappen [!UICONTROL Incomplete executions] där [!DNL Workfront Fusion] upprepade gånger försöker köra scenariot igen med ökande tidsintervall. Om alla försök misslyckas finns körningen kvar i mappen Ofullständiga körningar i väntan på manuell lösning av användaren.

     Mer information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Om det här alternativet är inaktiverat avslutas körningen av scenariot med ett fel följt av en återställningsfas. [!DNL Workfront Fusion] försöker sedan upprepade gånger att köra scenariot igen med ökande tidsintervall. Om alla försök misslyckas inaktiverar [!DNL Workfront Fusion] scenariot.

### Öka tidsintervall

Algoritmen för att öka tidsintervallen multiplikativt mellan försöken när ett fel inträffar kallas exponentiell säkerhetskopiering. De ökande tidsintervallen anges enligt följande:

1. 10 minuter
1. 1 timme
1. 3 timmar
1. 12 timmar
1. 24 timmar

Huvudorsaken till att de ökande tidsintervallen i [!DNL Workfront Fusion] används är att förhindra att ofta utförda scenarier använder åtgärder vid upprepade misslyckade försök.

>[!INFO]
>
>**Exempel:**
>
>Ett scenario innehåller [!DNL Google Sheets]-utlösaren [!UICONTROL Watch Rows]. [!DNL Google Sheets] är inte tillgängligt på 30 minuter på grund av underhåll när [!DNL Workfront Fusion] startar scenariot, så det går inte att hämta nya rader. Scenariot stoppas och försöker igen om 10 minuter. Eftersom [!DNL Google Sheets] fortfarande inte är tillgänglig kan [!DNL Workfront Fusion] fortfarande inte få information om nya rader. Nästa omgång av scenariot är schemalagd om en timme. [!DNL Google Sheets] är tillgängligt igen för tillfället och scenariot kan köras.

## Datafel

`DataError`

Ett datafel genereras när ett objekt är felaktigt mappat och inte godkänns vid den validering som har utförts på sidan [!DNL Workfront Fusion] eller på sidan av den tredjepartstjänst som används.

Om det här felet inträffar flyttas scenariot, fram till där modulen misslyckades, till mappen för ofullständiga körningar där du kan felsöka problemet. Scenariot avbryts dock inte och fortsätter att köras enligt schemat. Om du vill stoppa körningen av scenariot när ett datafel visas aktiverar du alternativet Sekventiell bearbetning på panelen Scenarioinställningar.

Om du inte har aktiverat alternativet [!UICONTROL Allow storing incomplete executions] i scenarioinställningarna avslutas körningen av scenariot med felet och en återställning utförs.

Mer information om mappning finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Mer information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Mer information om scenarioinställningspanelen finns i [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Mer information om scheman finns i [Schemalägg ett scenario i Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Fel vid duplicering av data

`DuplicateDataError`

Om [!DNL Workfront Fusion] försöker infoga samma paket två gånger i en tjänst som inte tillåter dubblettdata, genereras ett dubblettdatafel. Om det här felet inträffar fortsätter [!DNL Workfront Fusion] på samma sätt som för datafel.

## Ogiltigt åtkomsttokenfel

`InvalidAccessTokenError`

Ett ogiltigt åtkomsttokenfel inträffar när [!DNL Workfront Fusion] inte kan komma åt ditt konto som är registrerat hos en tredjepartstjänst. Detta inträffar vanligtvis när du återkallar åtkomstbehörighet för [!DNL Workfront Fusion] i administrationen av en viss tjänst, men relaterade scenarier fortsätter att köras enligt schemat.

Om det här felet inträffar stoppas körningen av ett scenario omedelbart. Resten av scenariot med början från modulen där felet inträffade flyttas till mappen för ofullständiga körningar.

Mer information om ofullständiga körningar finns i [Visa och lös ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Hastighetsbegränsningsfel

`RateLimitError`

Om en gräns som angetts av en viss tjänst överskrids genereras ett hastighetsbegränsningsfel. Om det här felet inträffar fortsätter [!DNL Workfront Fusion] på samma sätt som för anslutningsfelet.

Mer information finns i [Anslutningsfel](#connection-error).

## Ofullständigt datafel

`IncompleteDataError`

Ett ofullständigt datafel inträffar bara med utlösare. Det här felet genereras om en utlösare inte kan hämta nödvändiga data från en viss tjänst.

Om ett scenario avslutas med `IncompleteDataError` beror det ytterligare beteendet på inställningen [!UICONTROL Max number of consecutive errors].

Mer information finns i [Antal efterföljande fel](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) i artikeln [Panelen Sceninställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exempel:**
>
>Ett scenario har [!DNL Workfront]-utlösaren [!UICONTROL Watch Record] inställd på att bevaka dokument. Scenariot körs medan du överför ett stort dokument, till exempel en lång video. Eftersom [!UICONTROL Workfront Fusion] försöker hämta videon medan den fortfarande överförs till Workfront avslutas scenariot med `IncompleteDataError`.

## Körningsfel

`RuntimeError`

Om något annat fel (som inte nämns ovan) inträffar under scenariokörningen rapporteras det som en `RunTimeError`.

Om ett scenario avslutas med `RuntimeError` beror det ytterligare beteendet på inställningen [!UICONTROL Max number of consecutive errors]. Mer information finns i [Antal efterföljande fel](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) i artikeln [Panelen Sceninställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Om ett scenario börjar med en direktutlösare ignoreras inställningen [!UICONTROL Max number of consecutive errors] och scenariot inaktiveras omedelbart när det första felet har inträffat. Mer information finns i [Direktutlösare](../../workfront-fusion/modules/module-types.md#instant) i artikeln [Typer av moduler](../../workfront-fusion/modules/module-types.md).

## Inkonsekvens-fel

`InconsistencyError`

Om något av de fel som beskrivs ovan inträffar under implementerings- eller återställningsfasen avslutas ett scenario med ett inkonsekvens-fel. Mer information finns i [Körning av scenario, cykler och faser i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Om det här felet uppstår i ett scenario stoppas körningen av scenariot omedelbart.

## Varning

När du kör ett scenario kan du få en varning som informerar dig om ett problem. Det förhindrar dock inte att scenariot slutförs korrekt.

En varning kan till exempel visas när den största tillåtna filstorleken överskrids och alternativet [!UICONTROL Enable data loss] inaktiveras. Mer information finns i [Aktivera dataförlust](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) i artikeln [Panelen för scenarioinställningar i Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
