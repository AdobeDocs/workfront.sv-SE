---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-förfrågningsmetoder i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [HTTP-förfrågningsmetoder](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

När du konfigurerar ett API-anrop i en modul måste du fylla i fältet för metoden för HTTP-begäran.

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

## HTTP-metoder

Använd någon av följande HTTP-metoder.

* **[!UICONTROL GET]**: Hämtar data från en webbserver baserat på dina parametrar. [!UICONTROL GET] begär en representation av den angivna resursen och tar emot ett [!UICONTROL 200 OK]-svarsmeddelande med det begärda innehållet om det lyckas.
* **[!UICONTROL POST]**: Skickar data till en webbserver baserat på dina parametrar. [!UICONTROL POST] begäranden innehåller åtgärder som att överföra en fil. Flera [!UICONTROL POST] kan resultera i ett annat resultat än en enskild [!UICONTROL POST], så var försiktig med att oavsiktligt skicka flera [!UICONTROL POST]. Om [!UICONTROL POST] lyckas får du ett [!UICONTROL 200 OK] -svarsmeddelande.
* **[!UICONTROL PUT]**: Skickar data till en plats på webbservern baserat på dina parametrar. [!UICONTROL PUT] begäranden innehåller åtgärder som att överföra en fil. Skillnaden mellan [!UICONTROL PUT] och [!UICONTROL POST] är att PUT är idempotent, vilket innebär att resultatet av en [!UICONTROL PUT] som lyckades är detsamma som många identiska [!UICONTROL PUT]. Om PUT lyckas får du ett svarsmeddelande från 200 (vanligen 201 eller 204).
* **[!UICONTROL PATCH]**: (Inte tillgängligt för vissa API-anropsmoduler) Tillämpar partiella ändringar på en resurs på en webbserver baserat på dina parametrar. [!UICONTROL PATCH] är inte idempotent, vilket innebär att resultatet av flera [!UICONTROL PATCH]-objekt kan få oönskade konsekvenser. Om [!UICONTROL PATCH] lyckas får du ett 200-svarsmeddelande (vanligen 204).
* **[!UICONTROL DELETE]**: Tar bort den angivna resursen från webbservern baserat på dina parametrar (om resursen finns). Om [!UICONTROL DELETE] lyckas får du ett 200 OK-svarsmeddelande.
