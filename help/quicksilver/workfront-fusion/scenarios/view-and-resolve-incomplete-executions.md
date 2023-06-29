---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]
description: The [!UICONTROL Incomplete executions] mappen lagrar scenariokörningar som inte slutfördes korrekt på grund av ett fel. Varje lagrad ofullständig körning kan lösas antingen manuellt eller automatiskt.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]

The [!UICONTROL Incomplete executions] mappen lagrar scenariokörningar som inte slutfördes korrekt på grund av ett fel. Varje lagrad ofullständig körning kan lösas antingen manuellt eller automatiskt.

>[!NOTE]
>
>Som standard är lagring av ofullständiga körningar inaktiverat. Aktivera [!UICONTROL Allow storing incomplete executions] i scenariot avancerade inställningar.
>
>Mer information om scenarioinställningar finns i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Visa ofullständiga körningar

Om en modul påträffar ett fel under åtgärden läggs en ny ofullständig körning till i mappen Ofullständiga körningar. Varje ofullständig körning innehåller scenariots plan och alla paket som kan mappas till den misslyckade modulen. Du kan öppna listan över ofullständiga körningar genom att klicka på [!UICONTROL Incomplete Executions] på sidan med scenarioinformation:

![](assets/incomplete-executions-tab-350x102.png)

Mer information finns i [Fel som leder till ofullständiga körningar](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>Den aktuella storleksgränsen för mappen för olösta ofullständiga körningar per organisation är 500 MB. Om din organisation överskrider denna gräns kan följande fel uppstå:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Mer information finns i [Aktivera dataförlust](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Lös ofullständiga körningar

När en ny ofullständig körning sparas kan du lösa den på följande sätt:

1. Klicka på **[!UICONTROL Incomplete Executions]** -fliken.
1. Leta reda på den ofullständiga körning som du vill lösa och klicka på **[!UICONTROL Detail]**.


   Om du vill se loggen för alla åtgärder i modulen innan du försöker lösa den ofullständiga körningen kan du lösa den ofullständiga körningen från [!UICONTROL History] mapp:

1. Klicka på **[!UICONTROL History]** -fliken.
1. Leta reda på loggen för misslyckad körning för scenariot och klicka på **[!UICONTROL Details]**.
1. Öppna modulens logg där alla åtgärder i modulen visas.
1. Leta reda på den misslyckade åtgärden och klicka på **[!UICONTROL Resolve]**:

   ![](assets/resolve-btn-350x188.png)

## Alternativ för ofullständiga körningar

Följande alternativ i [!UICONTROL Scenario settings] avgör om och hur de ofullständiga körningarna lagras:

* Tillåt lagring av ofullständiga körningar
* Sekventiell bearbetning
* Aktivera dataförlust

Mer information om de här alternativen finns i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Fel som leder till ofullständiga körningar

Det finns flera typer av fel som leder till att ofullständiga körningar lagras. Dessa kan omfatta:

* Valideringsfel som uppstår på grund av ofullständiga eller felaktiga data, huvudsakligen på grund av att ett objekt saknas som förväntas bearbeta alla data som går igenom en modul.
* Fel som uppstod när det slutliga målet inte var tillgängligt på grund av tillfälligt eller långvarigt anslutningsfel (t.ex. vid anslutning till e-post eller fjärr-FTP-server).

Om ett fel inträffar på den första modulen i scenariot avbryts körningen omedelbart och ingen ofullständig körning sparas.

Om ett fel inträffar i någon annan modul och det inte finns någon kopplad felhanterarväg händer något av följande:

* Om feltypen är `ConnectionError`, `RateLimitError`, `OutOfSpaceError` eller `ModuleTimeoutError`, lagras en ofullständig körningspost med automatiskt återförsök.
* Om feltypen är `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, eller `MaxResultsExceededError`, lagras en ofullständig körningspost utan automatiskt återförsök.
* Om feltypen är något annat än ovanstående misslyckas körningen.
