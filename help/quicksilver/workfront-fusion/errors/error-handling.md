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
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# Felhantering i [!DNL Adobe Workfront Fusion]

När fel inträffar under körningen av ett scenario beror det oftast på att en tjänst inte är tillgänglig på grund av ett fel, att en tjänst svarar med oväntade data eller att valideringen av indata misslyckas.

>[!NOTE]
>
>Om en modul genererar ett fel under scenariokörningen och det inte finns någon felhanteringsväg kopplad till modulen, körs en standardfelhanteringslogik enligt beskrivningen i [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Genom att lägga till en felhanterarväg till en modul kan du ersätta standardfelhanteringslogiken med din egen. [!DNL Adobe Workfront Fusion] erbjuder fem olika direktiv, som alla kan infogas i slutet av felhanteringsrutterna. Mer information finns i [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Om du vill lägga till en felhanterarväg till en modul (vi kallar den Modul X) högerklickar du på modulen och väljer **[!UICONTROL Add error handler]**:

![](assets/error-handler-route.png)

I modulen visas en lista med direktiv samt de program som används i ditt scenario. Om modul X är den sista modulen i din väg måste du välja ett av direktiven. Du kan också fortsätta med att lägga till en eller flera moduler på vägen. I det här fallet [!UICONTROL Ignore] -direktivet tillämpas som standard på modul X och, i händelse av ett fel, kommer efterföljande moduler på den vägen att bearbetas.

![](assets/directives-350x426.png)

Om ett fel inträffar när [!UICONTROL Create a folder] -modulen [!UICONTROL Ignore] -direktivet tillämpas automatiskt och scenariot flyttas till nästa modul på felhanterarvägen om filtret&quot;Datafel inträffar&quot; returnerar ett eller flera paket.

Om det inte finns något fel flyttas dock scenariot till [!UICONTROL List all files in a folder module] på den normala rutten.

![](assets/if-there-is-no-error-350x234.png)

För att skilja en felhanterarväg från en vanlig rutt består den första av genomskinliga cirklar enligt ovan.

## Felhanteringsdirektiv

Direktiven förklaras kortfattat nedan. Mer information finns i [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Det finns sammanlagt fem direktiv som kan grupperas i följande kategorier baserat på om ett scenario-utförande ska fortsätta eller inte:

Följande direktiv ser till att en scenariokörning fortsätter:

* **[!UICONTROL Resume]** gör att du kan ange en ersättningsutmatning för modulen med felet och scenariokörningsstatusen markeras som lyckad
* **[!UICONTROL Ignore]** ignorerar bara felet och scenariokörningsstatusen markeras som lyckad
* **[!UICONTROL Break]** lagrar indata till kön för ofullständiga körningar och scenariokörningsstatusen markeras som varning. Mer information finns i [Visa och lösa ofullständiga körningar i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Om en scenariokörning å andra sidan ska stoppas måste du använda något av följande direktiv:

* **[!UICONTROL Rollback]** stoppar scenariokörningen omedelbart och markerar dess status som fel
* **[!UICONTROL Commit]** stoppar scenariokörningen omedelbart och anger att den har lyckats

## Ytterligare resurser

* [Direktiv om felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Avancerad felhantering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (innehåller konfiguration av det Dropbox-scenario som det hänvisas till ovan)
