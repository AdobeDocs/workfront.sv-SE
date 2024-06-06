---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: connections-annd-webhooks
title: Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner
description: Många [!DNL Adobe Workfront Fusion] anslutningar kräver ingen anpassad konfiguration när en anslutning skapas. I den här artikeln beskrivs standardprocessen för att skapa anslutningar.
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
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
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Skapa en anslutning

Skapa en anslutning inuti en [!DNL Workfront Fusion] modul:

1. Klicka **[!UICONTROL Add]** bredvid [!UICONTROL Connection] för att öppna **[!UICONTROL Create a connection]** -panelen.
1. (Valfritt) Ändra standardinställningen **[!UICONTROL Connection name]**.
1. (Villkorligt) Om programmet kräver avancerade anslutningsinställningar, till exempel ett ID, en nyckel eller [!UICONTROL secret]anger du den informationen.

   Du kan behöva klicka **[!UICONTROL Show advanced settings]** om du vill visa fälten där du kan ange den här typen av information.

1. Klicka på **[!UICONTROL Continue]**.
1. I inloggningsfönstret som visas anger du dina inloggningsuppgifter för att logga in på appen om du inte redan har gjort det.
1. (Villkorligt) Om ett **[!UICONTROL Allow]** klickar du på knappen för att ansluta programmet till [!DNL Workfront Fusion].

   >[!NOTE]
   >
   >Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
   >
   >Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.