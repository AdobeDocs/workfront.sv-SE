---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Felhantering i [!DNL Adobe Workfront Fusion]
description: När fel inträffar under körningen av ett scenario beror det oftast på att en tjänst inte är tillgänglig på grund av ett fel, att en tjänst svarar med oväntade data eller att valideringen av indata misslyckas.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Felhantering i [!DNL Adobe Workfront Fusion]

När fel inträffar under körningen av ett scenario beror det oftast på att en tjänst inte är tillgänglig på grund av ett fel, att en tjänst svarar med oväntade data eller att valideringen av indata misslyckas.

Om en modul genererar ett fel under scenariokörningen och det inte finns någon felhanteringsväg kopplad till modulen, körs standardfelhanteringslogiken enligt beskrivningen i [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Genom att lägga till en felhanterarväg till en modul kan du ersätta standardfelhanteringslogiken med din egen. [!DNL Adobe Workfront Fusion] erbjuder fem olika direktiv som kan infogas i slutet av felhanteringsrutterna.

Mer information finns i [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Felhanterarflöde

Så här lägger du till en felhanterarväg i en modul:

1. Högerklicka på modulen och välj **[!UICONTROL Add error handler]**:

   ![](assets/error-handler-route.png)

   I modulen visas en lista med direktiv samt de program som används i ditt scenario.

1. Om modulen som du har lagt till en felhanterare i är den sista modulen i ditt flöde väljer du ett av direktiven.

   eller

   Lägg till en eller flera moduler i felhanterarflödet.

   Om du lägger till fler moduler i flödet visas [!UICONTROL Ignore] -direktivet används som standard och om ett fel inträffar bearbetas efterföljande moduler på det flödet.


>[!INFO]
>
>I det här exemplet inträffar ett fel när [!UICONTROL Create a folder] -modulen [!UICONTROL Ignore] -direktivet tillämpas automatiskt och scenariot flyttas till nästa modul på felhanterarvägen.
>
>Om det inte finns något fel flyttas dock scenariot till [!UICONTROL List all files in a folder module] på den normala rutten.
>
>![](assets/if-there-is-no-error-350x234.png)

Observera att en felhanterarväg består av genomskinliga cirklar, medan en vanlig väg består av heldragna cirklar.

## Felhanteringsdirektiv

Direktiven förklaras kortfattat nedan. Mer information finns i [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Det finns totalt fem direktiv som kan grupperas i följande kategorier baserat på om ett scenario ska fortsätta eller inte.

Följande direktiv ser till att en scenariokörning fortsätter:

* **[!UICONTROL Resume]**: Gör att du kan ange ett ersättningsutvärde för modulen med felet. Scenariots körningsstatus har markerats som Slutfört
* **[!UICONTROL Ignore]**: ignorerar felet. Scenariots körningsstatus har markerats som Slutfört
* **[!UICONTROL Break]**: Sparar indata i kön för ofullständiga körningar. Scenariots körningsstatus är markerad som varning. Mer information finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Om en scenariokörning ska stoppas när ett fel inträffar, ska du använda något av följande direktiv:

* **[!UICONTROL Rollback]**: Stoppar scenariokörningen omedelbart och anger dess status som fel
* **[!UICONTROL Commit]**: Stoppar scenariokörningen omedelbart och anger att den har lyckats

Mer information om felhantering finns i:

* [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Avancerad felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)