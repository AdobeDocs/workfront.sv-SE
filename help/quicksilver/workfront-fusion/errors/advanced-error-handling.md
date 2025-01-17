---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Avancerad felhantering i  [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Avancerad felhantering i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Lägg till filtrering och kapsling i felhanteringsflöden](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/advanced-error-handling.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

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

## Filtrering

Det finns två sorters filtrering som kan ske i en felhanterarväg.

* [Lägga till ett filter i felhanterarflödet](#adding-a-filter-to-the-error-handler-route)
* [Lägga till en router följt av filter i felhanterarflödet](#adding-a-router-followed-by-filters-to-the-error-handler)

### Lägga till ett filter i felhanterarflödet

Du kan använda ett filter för att kontrollera vilka fel som hanteras av felhanterarvägen. På så sätt kan du bara bearbeta vissa typer av fel. Om ett fel inte skickas genom filtret behandlas det som om ingen felhanterarväg har definierats för den angivna modulen.

>[!INFO]
>
>**Exempel:**
>
>![](assets/filter-error-handling-350x238.png)

### Lägger till en [!UICONTROL Router] följt av filter i felhanteraren

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>I det här exemplet inträffar felet i modulen [!UICONTROL Create a folder] (A), som har en vanlig väg och en felhanterarväg. Den senare följs av en router med en rutt som har ett filter som definierar en viss typ av fel (datafel inträffar) och den andra som är standardvägen för alla andra fel. Den första vägen avslutas med direktivet [!UICONTROL Resume] som innehåller ersättningsvärden för scenariot som ska återupptas från modul A ([!UICONTROL Create a folder]), medan den andra vägen avslutas med direktivet [!UICONTROL Rollback] som omedelbart stoppar scenariokörningen.

Mer information om olika feltyper och om hur [!DNL Workfront Fusion] bearbetar och utvärderar dem finns i [Felbearbetning i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

### Exempelscenariot

Du kan ställa in det här exemplet för att förstå hur dessa filter fungerar för felhantering.

Använd en befintlig [!DNL Dropbox]-mapp för att överföra en fil i stället för att skapa en ny

Om du använder modulen [!UICONTROL Create a folder] på [!DNL Dropbox] och det redan finns en mapp med samma namn, kommer modulen att generera ett datafel enligt nedan:

![](assets/dropbox-350x276.png)

Det fullständiga scenariot:

![](assets/dropbox-scenario-350x190.png)

1. Modulen [!UICONTROL Tools] > [!UICONTROL Set Variable] innehåller mappnamnet
1. Modulen [!UICONTROL HTTP] >[!UICONTROL Get a file] hämtar filen som behöver överföras till mappen
1. Modulen [!UICONTROL Dropbox] >[!UICONTROL Create a folder] returnerar ett fel om det redan finns en mapp med samma namn som den som mappats i modulen
1. Felhanterarvägen (genomskinliga bubblor) innehåller en router som filtrerar felen
1. Den första vägen är för en angiven typ av fel med namnet Datafel som vi redan känner till:

   1. Om ett datafel inträffar och felinformationen skickas genom filtret, visar [!UICONTROL Dropbox] >[!UICONTROL List all files/subfolders in a folder module] alla mappar i [!DNL Dropbox]
   1. Det efterföljande filtret matchar mappnamnen
   1. Direktivet [!UICONTROL Resume] anger mapp-ID och mappsökväg för den befintliga mappen och scenariokörningen återupptas från modulen [!UICONTROL Dropbox] >[!UICONTROL Create a folder], men i stället för att försöka skapa en ny mapp använder den här gången värdena från direktivet [!UICONTROL Resume] för att flytta till nästa modul och överföra filen till den befintliga mappen

1. Den andra vägen är för alla andra fel och slutar med direktivet [!UICONTROL Rollback] som leder till att scenariot stoppas omedelbart

Nedan finns en detaljerad förklaring av den femte programsatsen:

Om du vill använda den befintliga mappen i efterföljande moduler ([!UICONTROL Upload a file] nedan) måste du lägga till en felhanterarväg till modulen och hämta mappsökvägen som ska mappas till [!UICONTROL Resume] -modulen enligt följande:

![](assets/add-error-handler-route-350x113.png)

Filtret på den första vägen är inställt på att endast hantera det specifika felet (datafel) som visas när det redan finns en mapp med samma namn:

![](assets/condition-350x327.png)

Modulen [!UICONTROL Dropbox] >[!UICONTROL List all files in a folder] har konfigurerats för att returnera alla mappar i målmappen. Följande filter skickar bara det som vi ursprungligen försökte skapa (mappnamnet lagras i mappen 33). Mappnamn):

![](assets/condition2-350x193.png)

Slutligen anger direktivet [!UICONTROL Resume] mappsökvägen som utdata för den felaktiga modulen. Observera att mapp-ID:t har lämnats tomt eftersom det inte behövs av modulen [!UICONTROL Upload a file]:

![](assets/flow-control-350x190.png)

## Kapsling

Oavsett var en modul finns kan felhanterarvägar skapas och implementeras på alla moduler, förutom routrar. Det är därför möjligt att skapa en felhanterarväg för en modul som redan är en del av en befintlig felhanterarväg som skapats för en annan modul.

Här är ett exempel på en kapslad felhanterarväg:

![](assets/nested-error-handling-route-350x174.png)

I det här scenariot kapslas den andra felhanterarvägen under den första felhanterarvägen. Om ett fel påträffas i [!UICONTROL Dropbox] >[!UICONTROL Create a folder module] flyttas körningen till rutt 1, och om filtret [!UICONTROL Data Error Takes Place] skickas, körs nästa modul följt av [!UICONTROL Resume] -modulen om ett fel inte inträffar med [!UICONTROL Dropbox] >[!UICONTROL List all files/subfolders] i en mappmodul.

Om ett fel inträffar med den här [!DNL Dropbox]-modulen flyttas körningen till felhanterarflöde 2 och avslutas med direktivet [!UICONTROL Ignore] . Modulen [!UICONTROL Resume directive] körs inte i det här fallet.

Det är en kombination av felhanterare för filtrering och kapsling.

