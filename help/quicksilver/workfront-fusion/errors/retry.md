---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Försök att hantera fel igen i  [!DNL Adobe Workfront Fusion]
description: I vissa fall kan det vara bra att köra en felande modul ett par gånger om det finns en möjlighet att orsaken till felet kan passera över tiden.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Försök igen med felhantering i [!DNL Adobe Workfront Fusion]

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

## Tillfälliga lösningar på direktivet [!UICONTROL Retry] för felhantering

[!UICONTROL Adobe Workfront Fusion] erbjuder för närvarande inte direktivet [!UICONTROL Retry] för felhantering, men två temporära lösningar kan användas för att efterlikna dess funktioner. Mer information finns i [Direktiv om felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Använd direktivet [!UICONTROL Break]

1. Aktivera alternativet **[!UICONTROL Allow storing of Incomplete Executions]** på panelen för scenarioinställningar.

   Mer information finns i [Panelen för scenarioinställningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Koppla en felhanterarväg till modulen, vilket beskrivs i [Felhantering i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Länka direktivet [!UICONTROL Break] till felhanterarvägen och konfigurera det.

   Mer information finns i [Direktiv om felhantering i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nackdelar

* Det minsta intervallet för återförsök är en minut.
* Om modulen bearbetar flera paket och bearbetningen av ett paket misslyckas, flyttas den partiella körningen (endast det paket som orsakade felet) till den ofullständiga körningsmappen och schemaläggs för nya försök enligt [!UICONTROL Break]-direktivets inställningar. Den aktuella körningen fortsätter dock och modulen fortsätter att bearbeta efterföljande paket. Du kan aktivera alternativet [!UICONTROL Sequential processing] i [!UICONTROL Scenario settings] om du vill förhindra att scenariot körs igen tills körningen i mappen Ofullständiga körningar har lösts.

  Mer information om ofullständiga körningar finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Använd modulen [!UICONTROL Repeater]

1. Distribuera modulen **[!UICONTROL Repeater]** och ställ in fältet **[!UICONTROL Repeats]** på maximalt antal försök.
1. Länka den modul som kan misslyckas till modulen **[!UICONTROL Repeater]**.
1. Koppla en felhanterarväg till modulen (se [Felhantering i [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Länka modulen **[!UICONTROL Tools]>[!UICONTROL Sleep]** till felhanterarvägen och ställ in fältet **[!UICONTROL Delay]** på antalet sekunder mellan försöken.

1. Länka direktivet **[!UICONTROL Ignore]** efter modulen **[!UICONTROL Tools]>[!UICONTROL Sleep]** (se [Direktiv om felhantering i Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Länka modulen **[!UICONTROL Tools]>[!UICONTROL Set variable]** efter den modul som kan misslyckas och konfigurera den så att den lagrar modulens resultat i en variabel som till exempel heter `Result`.

1. Länka modulen **[!UICONTROL Array aggregator]** efter **[!UICONTROL Tools]>[!UICONTROL Set variable]** och välj modulen **[!DNL Repeater]** i fältet Source-modul.

1. Länka modulen **[!UICONTROL Tools]>[!UICONTROL Get variable]** till modulen **[!UICONTROL Array aggregator]** och konfigurera den så att värdet för variabeln `Result` hämtas.

1. Infoga modulen **[!UICONTROL Tools]>[!UICONTROL Get variable]** mellan modulen **[!UICONTROL Repeater]** och den modul som kan misslyckas och konfigurera den så att värdet för variabeln `Result` hämtas.

1. Infoga ett filter mellan den här **[!UICONTROL Tools]>[!UICONTROL Get variable]**-modulen och den eventuellt felaktiga modulen så att den bara fortsätter om variabeln `Result` inte finns.

>[!INFO]
>
>**Exempel:** Här är ett exempel på scenario där modulen [!UICONTROL HTTP] >[!UICONTROL Make a request] representerar den modul som kan misslyckas:
>
>![](assets/http-make-request-350x116.png)
>
>Om resultatet av den eventuellt felaktiga modulen är för komplext för att lagras i en enkel variabel kan du använda ett datalager för att lagra/hämta resultatet. Datalagret skulle bara innehålla en post. Postens nyckel kan till exempel vara `Result`.
>
>Mer information om datalager finns i [Datalager i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Återställning

Den här lösningen kan se lite för komplex ut och är också mer krävande när det gäller åtgärder.
