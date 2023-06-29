---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Försök att hantera fel igen i [!DNL Adobe Workfront Fusion]
description: I vissa fall kan det vara bra att köra en felande modul ett par gånger om det finns en möjlighet att orsaken till felet kan passera över tiden.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Försök att hantera fel igen i [!DNL Adobe Workfront Fusion]

I vissa fall kan det vara bra att köra en felande modul igen om det finns en möjlighet att orsaken till felet kan passera över tiden.

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
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

## Tillfälliga lösningar [!UICONTROL Retry] felhanteringsdirektiv

[!UICONTROL Adobe Workfront Fusion] för närvarande inte erbjuder [!UICONTROL Retry] felhanteringsdirektiv, men två temporära lösningar kan användas för att efterlikna dess funktionalitet. Mer information finns i [Direktiv om felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Använd [!UICONTROL Break] direktiv

1. Aktivera alternativet **[!UICONTROL Allow storing of Incomplete Executions]** alternativ.

   Mer information finns i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Koppla en felhanterarväg till modulen enligt beskrivningen i [Felhantering i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Länka [!UICONTROL Break] -direktivet till felhanterarvägen och konfigurera den.

   Mer information finns i [Direktiv om felhantering i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nackdelar

* Det minsta intervallet för återförsök är en minut.
* Om modulen bearbetar flera paket och bearbetningen av ett paket misslyckas, flyttas den partiella körningen (endast det paket som orsakade felet) till den ofullständiga körningsmappen och schemaläggs för nya försök enligt [!UICONTROL Break] -inställningar. Den aktuella körningen fortsätter dock och modulen fortsätter att bearbeta efterföljande paket. Du kan aktivera[!UICONTROL Sequential processing]&quot; i [!UICONTROL Scenario settings] för att förhindra att scenariot körs igen tills körningen i mappen Ofullständiga körningar har åtgärdats.

  Mer information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Använd [!UICONTROL Repeater] modul

1. Använd **[!UICONTROL Repeater]** och ange dess **[!UICONTROL Repeats]** till maximalt antal försök.
1. Länka den eventuellt felaktiga modulen till **[!UICONTROL Repeater]** -modul.
1. Koppla en felhanterarväg till den här modulen (se [Felhantering i [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Länka **[!UICONTROL Tools]>[!UICONTROL Sleep]** till felhanterarvägen och ange dess **[!UICONTROL Delay]** till antalet sekunder mellan försöken.

1. Länka **[!UICONTROL Ignore]** efter **[!UICONTROL Tools]>[!UICONTROL Sleep]** modul (se [Direktiv om felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Länka **[!UICONTROL Tools]>[!UICONTROL Set variable]** modulen efter den eventuellt felaktiga modulen och konfigurera den för att lagra modulens resultat i en variabel som till exempel heter `Result`.

1. Länka **[!UICONTROL Array aggregator]** modulen efter **[!UICONTROL Tools]>[!UICONTROL Set variable]** och väljer **[!DNL Repeater]** i fältet Källmodul.

1. Länka **[!UICONTROL Tools]>[!UICONTROL Get variable]** till **[!UICONTROL Array aggregator]** och konfigurera den för att få fram värdet för `Result` variabel.

1. Infoga **[!UICONTROL Tools]>[!UICONTROL Get variable]** modulen mellan **[!UICONTROL Repeater]** och den modul som kan misslyckas och konfigurera den för att få fram värdet för `Result` variabel.

1. Infoga ett filter mellan detta **[!UICONTROL Tools]>[!UICONTROL Get variable]** och den eventuellt felaktiga modulen bara fortsätter om `Result` variabeln finns inte.

>[!INFO]
>
>**Exempel:** Här är ett exempel på ett scenario där [!UICONTROL HTTP] >[!UICONTROL Make a request] representerar den modul som kan misslyckas:
>
>![](assets/http-make-request-350x116.png)
>
>Om resultatet av den eventuellt felaktiga modulen är för komplext för att lagras i en enkel variabel kan du använda ett datalager för att lagra/hämta resultatet. Datalagret skulle bara innehålla en post. Postens nyckel kan till exempel vara `Result`.
>
>Mer information om datalager finns i [Datalager i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Återställning

Den här lösningen kan se lite för komplex ut och är också mer krävande när det gäller åtgärder.
