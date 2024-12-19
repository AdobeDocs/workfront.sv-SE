---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Använd cURL för att lägga till en HTTP-modul
description: Du kan klistra in en cURL-begäran i ditt scenario, så skapar Fusion en HTTP-modul som konfigurerats från cURL-begäran.
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Använd cURL för att lägga till en HTTP-modul

Du kan klistra in en cURL-begäran i ditt scenario, så skapar Fusion en HTTP-modul som konfigurerats från cURL-begäran.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront</td>  
      <td>Alla</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-licens</td>  
      <td>
        Nytt: Standard<br>
        Eller<br>
        Aktuell: Arbete eller högre
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-licens</td>  
      <td> 
        Aktuell: Inga Workfront Fusion-licenser krävs.<br>
        Eller<br>
        Äldre: Alla
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Nytt: Välj eller Prime Workfront Plan: Din organisation måste köpa Adobe Workfront Fusion.<br>
        Ultimate Workfront Plan: Workfront Fusion ingår.<br>
        Eller<br>
        Aktuell: Din organisation måste köpa Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Skapa en HTTP-modul från en cURL-begäran


Så här skapar du en HTTP-modul med cURL:

1. Skapa texten i cURL-begäran utanför Fusion, till exempel i en textredigerare.

   >[!IMPORTANT]
   >
   >Om du använder Fusion på en Windows-dator får din cURL-begäran inte innehålla radbrytningar.
1. Kopiera cURL-begäran till Urklipp.
1. Klicka på fliken **[!UICONTROL Scenario]** i den vänstra panelen.
1. Välj det scenario där du vill skapa modulen.
1. Klicka någonstans i scenariot för att öppna Scenarioredigeraren.
1. Högerklicka på ett tomt utrymme i scenarioredigeraren och välj **Klistra in**.

   eller

   Tryck på Ctrl + V (Windows) eller Cmd + V (Mac).


   En HTML-modul skapas.
1. Dra modulen för att ansluta den till ditt scenario.

## Felsökning

Om din cURL inte klistras in i ditt scenario kontrollerar du följande:

* Kontrollera webbläsarens inställningar för att se till att inklistring från Urklipp är aktiverad.
* Om du kör Windows bör du kontrollera att cURL-begäran inte innehåller radbrytningar.



