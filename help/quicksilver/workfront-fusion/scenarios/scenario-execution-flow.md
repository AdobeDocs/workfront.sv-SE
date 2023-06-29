---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Körningsflöde för scenarier i Adobe Workfront Fusion
description: I den här artikeln beskrivs hur ett scenario körs och hur data flödar genom det. Där förklaras också var du kan hitta information om bearbetade data och hur du läser dem.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Scenariokörningsflöde i [!DNL Adobe Workfront Fusion]

I den här artikeln beskrivs hur ett scenario körs och hur data flödar genom det. Där förklaras också var du kan hitta information om bearbetade data och hur du läser dem.

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

## Körningsflöde för scenarier

När ett scenario har konfigurerats korrekt och aktiverats körs det enligt det definierade schemat.

När scenariot börjar svarar den första modulen på en händelse som den har ställts in att bevaka. Om det returnerar paket (data) skickas de vidare till nästa modul och scenariot fortsätter och skickar paketen genom varje efterföljande modul, en i taget.

Om paketprocessen fungerar som den ska i alla moduler markeras scenariot som lyckat i scenariedetaljområdet, vilket förklaras i [Scenarioinformation i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Mer information om hur du konfigurerar ett scenario finns i [Grundscenarieinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Mer information om hur du aktiverar ett scenario finns i [Aktivera eller inaktivera ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Mer information om att schemalägga ett scenario finns i [Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Mer information om moduler finns i [Typer av moduler](../../workfront-fusion/modules/module-types.md).

### Exempel: [!UICONTROL [!DNL Workfront Fusion] for Work Automation]

>[!INFO]
>
>**Exempel:** I ett scenario som söker efter inkommande begäranden i [!DNL Workfront] och sedan konvertera dem till [!DNL Workfront] data flödar enligt följande.
>
>Scenariots första steg, som utförs av den första modulen, är att bevaka begäranden. Varje begäran som kommer in betraktas som ett paket. Om modulen körs utan att några paket hittas avslutas scenariot efter den första modulen.
>
>Om den första modulen returnerar ett paket, skickas paketet igenom resten av scenariot. I det här exemplet består resten av scenariot av den andra och sista modulen, som konverterar begäran till ett projekt.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Exempel: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]

>[!INFO]
>
>**Exempel:** I ett scenario som hämtar dokument från [!DNL Adobe Workfront] och skickar dem till en mapp i [!DNL Dropbox]skulle data flöda enligt följande.
>
>Scenariots första steg, som utförs av den första modulen, är att bevaka paket (dokument). I det här exemplet bevakar modulen paket i [!DNL Workfront]. Om det inte returnerar ett paket avslutas scenariot efter den första modulen.
>
>Om ett paket returneras skickas paketet igenom resten av scenariot. I det här exemplet består resten av scenariot av den andra och sista modulen, som överför paketet till [!DNL Dropbox] mapp.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Om den första modulen returnerar flera paket överförs det första paketet till [!DNL Dropbox] innan det andra paketet överförs. Sedan överförs det andra paketet, det tredje och så vidare.

## Information om bearbetade paket

För varje modul går paketet igenom en process i fyra steg innan du går vidare till nästa modul eller når det slutliga målet. Processen i fyra steg är Initalization, Operation, Commit/Rollback och Finalization. Detta kallas transaktionsbearbetning och förklarar hur data har bearbetats i en modul.

När ett scenario har körts visas en ikon som visar antalet åtgärder som har utförts i varje modul. Du kan klicka på den här ikonen om du vill visa detaljerad information om de bearbetade paketen i det format som beskrivs ovan. Du kan se vilka modulinställningar som användes och vilka paket som returnerades av vilken modul.

![](assets/info-processed-bundles-350x396.png)

En modul tog emot indatainformation som:

* Konverterad bild
* Vald mapp där bilden ska överföras till
* Ursprungligt namn på [!DNL Facebook] image

Efter bearbetning returnerade modulen följande utdatainformation:

* Bild-ID tilldelat av [!DNL Dropbox]
* Fullständig sökväg där [!DNL Dropbox] [!DNL Workfront Fusion] överförde filen

Ovanstående information hämtas separat för varje paket, vilket markeras av listrutorna [!UICONTROL Operation 1] och [!UICONTROL Operation 2] i bilden.

Mer information om transaktionsbearbetning finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Ett fel uppstod när ett scenario kördes

Ett fel kan uppstå under scenariot. Om du till exempel tar bort [!DNL Dropbox] som du har angett som målmapp i modulinställningen avslutas scenariot med ett felmeddelande. Mer information om hur du hanterar fel finns i [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
