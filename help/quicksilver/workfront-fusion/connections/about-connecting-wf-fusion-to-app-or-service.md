---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Om att ansluta [!DNL Adobe Workfront Fusion] till en app eller tjänst
description: För de flesta program måste du skapa en anslutning genom vilken [!DNL Adobe Workfront Fusion] kan kommunicera med den angivna tredjepartstjänsten enligt inställningarna för det specifika scenariot.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Om att ansluta [!DNL Adobe Workfront Fusion] till en app eller tjänst

För de flesta program måste du skapa en anslutning genom vilken [!DNL Adobe Workfront Fusion] kan kommunicera med den angivna tredjepartstjänsten enligt inställningarna för det specifika scenariot.

Om du till exempel vill skapa ett scenario som hämtar information från [!DNL Workfront]måste du ge åtkomstbehörighet för [!DNL Workfront Fusion] för att få tillgång till [!DNL Workfront] konto.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Åtkomsträttigheter

För varje anslutning [!DNL Workfront Fusion] kräver endast de åtkomsträttigheter som är nödvändiga för att slutföra ett visst scenario. Om du till exempel skapar ett scenario för att lista dokument från [!DNL Google Docs], [!DNL Workfront Fusion] frågar inte efter tillstånd att hämta innehållet i dokumenten.

Tyvärr kan du inte begränsa åtkomsten till vissa uppgifter med alla tjänster. Därför [!DNL Workfront Fusion] måste kräva fullständig behörighet. Mer information om hur du begränsar [!DNL Workfront Fusion] åtkomst till ditt konto som är registrerat för dessa tjänster finns i den programspecifika dokumentationen.

## Administrera anslutningar

Du kan administrera alla anslutningar från [!UICONTROL Connections] område. Här kan du:

* Se vilka behörigheter som tilldelats [!DNL Workfront Fusion] för varje anslutning
* Byt namn på anslutningar
* Återauktorisera befintliga anslutningar
* Ta bort befintliga anslutningar
* Kontrollera att anslutningen till tjänsten har upprättats

Öppna [!UICONTROL Connections] område, klicka <b>[!UICONTROL Connections]</b> i den vänstra navigeringen.

## Förnya en anslutning

[!DNL Workfront Fusion] oftast får nyttjanderätt till en viss tjänst under en obegränsad tidsperiod. Detta är dock inte alltid fallet. För vissa tjänster måste åtkomstbehörigheten förnyas efter en viss tidsperiod. I dessa fall [!DNL Workfront Fusion] meddelar dig via e-post kort innan åtkomsträttigheterna upphör att gälla.

Så här förnyar du en anslutning:

1. Klicka på **[!UICONTROL Reauthorize]** i **[!UICONTROL Connections]** område.
