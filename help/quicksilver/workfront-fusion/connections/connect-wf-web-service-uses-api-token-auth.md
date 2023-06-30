---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till en webbtjänst som använder API-tokenauktorisering
description: Vissa tjänster tillåter inte integreringslösningar som [!DNL Adobe Workfront Fusion] för att skapa en app som du enkelt kan använda i ditt scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till en webbtjänst som använder API-tokenauktorisering

Vissa tjänster tillåter inte integreringslösningar som [!DNL Adobe Workfront Fusion] för att skapa en app som du enkelt kan använda i ditt scenario.

Det finns en lösning på den här situationen. Du kan ansluta den önskade tjänsten (appen) till [!DNL Workfront Fusion] använda [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] -modul.

I den här artikeln beskrivs hur du ansluter nästan alla webbtjänster till [!DNL Workfront Fusion] med en API-nyckel/API-token.

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
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ansluta till en webbtjänst som använder en API-token

Proceduren för att ansluta tjänsten via en API-token liknar den för de flesta webbtjänster.

1. Skapa ett program på webbtjänstens webbplats, vilket förklaras i avsnittet [Skapa ett nytt program och hämta API-token](#create-a-new-application-and-obtain-the-api-token) i den här artikeln.
1. Hämta API-nyckeln eller API-token.
1. Lägg till [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL Make a Request] till ditt scenario.
1. Konfigurera modulen enligt webbtjänstens API-dokumentation och köra scenariot, vilket förklaras i avsnittet [Konfigurera [!UICONTROL HTTP] modul](#set-up-the-http-module) i den här artikeln.

>[!NOTE]
>
>Vi använder [!DNL Pushover] meddelandetjänst som ett exempel i den här artikeln.

## Skapa ett nytt program och hämta API-token

>[!NOTE]
>
>Det finns många olika sätt att skapa och distribuera API-nycklar eller API-tokens i webbtjänster. Instruktioner om hur du hämtar en API-nyckel och -token för den önskade webbtjänsten finns på tjänstens webbplats och söker efter &quot;API-nyckel&quot; eller &quot;API-token&quot;.
>
>Vi inkluderar instruktioner om hur du får en Pushover API-nyckel som exempel på vad du kan hitta.

1. Logga in på [!DNL Pushover] konto.
1. Klicka **[!UICONTROL Create an Application/API Token]** längst ned på sidan.
1. Fyll i programinformationen och klicka på **[!UICONTROL Create an Application]**.
1. Lagra den angivna API-token på en säker plats. Du behöver den för [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Make a Request] för att ansluta till önskad webbtjänst ([!DNL Pushover], i det här fallet).

## Konfigurera [!UICONTROL HTTP] modul

Ansluta en webbtjänst till [!DNL Workfront Fusion] scenario måste du använda [!UICONTROL HTTP] >[!UICONTROL Make a request] i scenariot och konfigurera modulen enligt webbtjänstens API-dokumentation.

1. Lägg till [!UICONTROL HTTP] >[!UICONTROL Make a Request] till ditt scenario.
1. Skicka ett meddelande med [!DNL Workfront Fusion]ställer du in HTTP-modulen enligt följande.

   >[!NOTE]
   >
   >Dessa modulinställningar motsvarar [!DNL Pushover] API-dokumentation för webbtjänst. Inställningarna kan vara annorlunda för andra webbtjänster. API-token kan till exempel infogas i [!UICONTROL Header] och inte [!UICONTROL Body] fält.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL-fältet innehåller slutpunkten som du hittar i webbtjänstens API-dokumentation.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>Vilken metod som används beror på motsvarande slutpunkt. Pushover-slutpunkten för push-meddelanden använder metoden POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Vissa webbtjänster kan använda rubriker för att ange API-tokenautentisering eller andra parametrar. Detta är inte fallet i vårt exempel eftersom Pushover-slutpunkten för push-meddelanden använder Body (se nedan) för alla typer av begäranden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Vissa webbtjänster kan använda en frågesträng för att ange andra parametrar. Detta är inte fallet i vårt exempel som [!DNL Pushover] webbtjänst använder [!UICONTROL Body] (se nedan) för alla typer av förfrågningar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Med den här inställningen kan du välja JSON-innehållstypen i [!UICONTROL Content Type] fält nedan.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON är den innehållstyp som krävs av [!UICONTROL Pushover] app. Detta kan skilja sig från andra webbtjänster.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Ange [!UICONTROL Body] begär innehåll i JSON-format. Du kan använda [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] modul enligt <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON-brödtext mappad med [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] modul</a> i den här artikeln. Du kan också ange JSON-innehållet manuellt enligt anvisningarna i <a href="#json-body-entered-manually" class="MCXref xref">JSON-brödtext har angetts manuellt</a> i den här artikeln.</p> <p>I webbtjänstens API-dokumentation finns information om vilka parametrar som krävs för den webbtjänsten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## JSON-brödtext har angetts manuellt

Ange parametrar och värden i JSON-format.

>[!INFO]
>
>**Exempel:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>Din USER_KEY. Det finns i [!DNL Pushover] kontrollpanel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Din API-token/API-nyckel som du skapade [!DNL Pushover] app.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>Textinnehållet i push-meddelandet som skickas till enheten/enheterna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Valfritt) Meddelandets titel. Om inget värde anges används appens namn. </p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-brödtext mappad med [!UICONTROL JSON] >[!UICONTROL Create JSON] modul

The [!UICONTROL Create JSON] gör det enklare att ange JSON. Du kan också definiera värden dynamiskt.

Mer information om JSON-modulerna finns i [JSON-moduler](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Ange eller mappa de värden som du vill skapa JSON från.

   ![](assets/json-values-350x288.png)

1. Anslut [!UICONTROL JSON] > [!UICONTROL Create JSON] till HTTP > Gör en begäran-modul.
1. Mappa JSON-strängen från [!UICONTROL Create JSON] till [!UICONTROL Request content] i [!UICONTROL HTTP] >[!UICONTROL Make a Request] -modul.

   När du kör scenariot skickas nu push-meddelandet till den enhet som har registrerats i din [!DNL Pushover] konto.
