---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Avancerad felhantering i [!DNL Adobe] Workfront Fusion
description: Bland de avancerade felhanteringsteknikerna finns filtrering och kapsling.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Avancerad felhantering i [!DNL Adobe Workfront Fusion]

Bland de avancerade felhanteringsteknikerna finns filtrering och kapsling.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
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

## Filtrering

Det finns två sorters filtrering som kan ske i en felhanterarväg.

* [Lägga till ett filter i felhanterarflödet](#adding-a-filter-to-the-error-handler-route)
* [Lägga till en router följt av filter i felhanterarflödet](#adding-a-router-followed-by-filters-to-the-error-handler)

### Lägga till ett filter i felhanterarflödet

Du kan använda ett filter för att kontrollera vilka fel som hanteras av felhanterarvägen. På så sätt kan du bara bearbeta vissa typer av fel. Om ett fel inte skickas genom filtret behandlas det som om det inte finns någon felhanterarväg definierad för den angivna modulen.

>[!INFO]
>
>**Exempel:**
>
>![](assets/filter-error-handling-350x238.png)

### Lägga till en [!UICONTROL Router] följt av filter till felhanteraren

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>I det här exemplet inträffar felet på [!UICONTROL Create a folder] modul (A), som har ett vanligt flöde och en felhanterarväg. Den senare följs av en router med en rutt som har ett filter som definierar en viss typ av fel (datafel inträffar) och den andra som är standardvägen för alla andra fel. Den första rutten slutar med [!UICONTROL Resume] som innehåller ersättningsvärden för scenariot som ska återupptas från modul A ([!UICONTROL Create a folder]), medan den andra sträckan slutar med [!UICONTROL Rollback] -direktiv som avbryter scenariokörningen omedelbart.

Se [Fel vid bearbetning av [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) för mer information om olika feltyper och om hur [!DNL Workfront Fusion] bearbetar och utvärderar dem.

### Exempelscenariot

Du kan ställa in det här exemplet för att förstå hur dessa filter fungerar för felhantering.

Använd en befintlig [!DNL Dropbox] mapp för att överföra en fil i stället för att skapa en ny

Om du använder [!UICONTROL Create a folder] modul på [!DNL Dropbox] och det redan finns en mapp med samma namn, kommer modulen att generera ett datafel enligt nedan:

![](assets/dropbox-350x276.png)

Hela scenariot:

![](assets/dropbox-scenario-350x190.png)

1. The [!UICONTROL Tools] > [!UICONTROL Set Variable] modulen innehåller mappnamnet
1. The [!UICONTROL HTTP] >[!UICONTROL Get a file] hämtar filen som behöver överföras till mappen
1. The [!UICONTROL Dropbox] >[!UICONTROL Create a folder] ett fel uppstår om det redan finns en mapp med samma namn som den som mappats i modulen
1. Felhanterarvägen (genomskinliga bubblor) innehåller en router som filtrerar felen
1. Den första vägen är för en angiven typ av fel med namnet Datafel som vi redan känner till:

   1. Om ett datafel inträffar och felinformationen skickas genom filtret visas [!UICONTROL Dropbox] >[!UICONTROL List all files/subfolders in a folder module] visar alla mappar i [!DNL Dropbox]
   1. Det efterföljande filtret matchar mappnamnen
   1. The [!UICONTROL Resume] -direktivet anger mapp-ID och mappsökväg för den befintliga mappen och scenariokörningen återupptas från [!UICONTROL Dropbox] >[!UICONTROL Create a folder] i stället för att försöka skapa en ny mapp, använder den här gången värdena från [!UICONTROL Resume] -direktiv för att gå till nästa modul och överföra filen till den befintliga mappen

1. Den andra vägen gäller alla andra fel och slutar med [!UICONTROL Rollback] -direktiv som leder till att scenariot stoppas omedelbart

Nedan finns en detaljerad förklaring av den femte programsatsen:

För att kunna använda den befintliga mappen i efterföljande moduler ([!UICONTROL Upload a file] nedan) måste du lägga till en felhanterarväg till modulen och hämta mappsökvägen som ska mappas till [!UICONTROL Resume] -modul som följer:

![](assets/add-error-handler-route-350x113.png)

Filtret på den första vägen är inställt på att endast hantera det specifika felet (datafel) som visas när det redan finns en mapp med samma namn:

![](assets/condition-350x327.png)

The [!UICONTROL Dropbox] >[!UICONTROL List all files in a folder] är konfigurerad för att returnera alla mappar i målmappen. Följande filter skickar bara det som vi ursprungligen försökte skapa (mappnamnet lagras i mappen 33). Mappnamnsobjekt):

![](assets/condition2-350x193.png)

Så småningom [!UICONTROL Resume] -direktivet anger mappsökvägen som utdata för den felaktiga modulen. Observera att mapp-ID har lämnats tomt eftersom det inte behövs av[!UICONTROL Upload a file]&#39;:

![](assets/flow-control-350x190.png)

## Kapsling

Oavsett var en modul finns kan felhanterarvägar skapas och implementeras på alla moduler, förutom routrar. Det är därför möjligt att skapa en felhanterarväg för en modul som redan är en del av en befintlig felhanterarväg som skapats för en annan modul.

Här är ett exempel på en kapslad felhanterarväg:

![](assets/nested-error-handling-route-350x174.png)

I det här scenariot kapslas den andra felhanterarvägen under den första felhanterarvägen. Så om [!UICONTROL Dropbox] >[!UICONTROL Create a folder module] påträffar ett fel, flyttar körningen till flöde 1, om [!UICONTROL Data Error Takes Place] -filtret skickas, nästa modul körs följt av [!UICONTROL Resume] om ett fel inte inträffar med [!UICONTROL Dropbox] >[!UICONTROL List all files/subfolders] i en mappmodul.

Men om ett fel inträffar med detta [!DNL Dropbox] flyttar körningen till Error Handler Route 2 och avslutas med [!UICONTROL Ignore] -direktivet. The [!UICONTROL Resume directive] -modulen körs inte i det här fallet.

Det är en kombination av felhanterare för filtrering och kapsling.

