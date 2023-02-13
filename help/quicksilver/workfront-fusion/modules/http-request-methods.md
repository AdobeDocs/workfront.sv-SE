---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]
description: När du konfigurerar ett API-anrop i en modul måste du fylla i fältet för metoden för HTTP-begäran.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## HTTP-metoder

Använd någon av följande HTTP-metoder.

* **[!UICONTROL GET]**: Hämtar data från en webbserver baserat på dina parametrar. [!UICONTROL GET] begär en representation av den angivna resursen och tar emot en [!UICONTROL 200 OK] svarsmeddelande med begärt innehåll om det lyckas.
* **[!UICONTROL POST]**: Skickar data till en webbserver baserat på dina parametrar. [!UICONTROL POST] -begäranden innehåller åtgärder som att överföra en fil. Flera [!UICONTROL POST]s kan ge ett annat resultat än ett [!UICONTROL POST]var därför försiktig med att oavsiktligt skicka flera [!UICONTROL POST]s. Om en [!UICONTROL POST] har slutförts får du en [!UICONTROL 200 OK] svarsmeddelande.
* **[!UICONTROL PUT]**: Skickar data till en plats på webbservern baserat på dina parametrar. [!UICONTROL PUT] -begäranden innehåller åtgärder som att överföra en fil. Skillnaden mellan [!UICONTROL PUT] och [!UICONTROL POST] är att PUT är idealiskt, vilket innebär att resultatet av en enda framgång [!UICONTROL PUT] är samma som många identiska [!UICONTROL PUT]s. Om PUT lyckas får du ett svarsmeddelande från 200 (vanligen 201 eller 204).
* **[!UICONTROL PATCH]**: (Inte tillgängligt för vissa API-anropsmoduler) Tillämpar partiella ändringar på en resurs på en webbserver baserat på dina parametrar. [!UICONTROL PATCH] är inte idempotent, vilket innebär att resultatet av flera [!UICONTROL PATCH]Det kan få oväntade konsekvenser. Om en [!UICONTROL PATCH] om det lyckas får du ett 200-svarsmeddelande (vanligen 204).
* **[!UICONTROL DELETE]**: Tar bort den angivna resursen från webbservern baserat på dina parametrar (om resursen finns). Om en [!UICONTROL DELETE] när det är klart får du ett 200 OK-svarsmeddelande.
