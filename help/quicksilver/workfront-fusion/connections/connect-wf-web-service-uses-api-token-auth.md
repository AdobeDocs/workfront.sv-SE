---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till en webbtjänst som använder API-tokenauktorisering
description: Vissa tjänster tillåter inte integreringslösningar som  [!DNL Adobe Workfront Fusion]  för att skapa en app som du enkelt kan använda i ditt scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till en webbtjänst som använder API-tokenauktorisering

Vissa tjänster tillåter inte integreringslösningar som [!DNL Adobe Workfront Fusion] att skapa en app som du enkelt kan använda i ditt scenario.

Det finns en lösning på den här situationen. Du kan ansluta den önskade tjänsten (appen) till [!DNL Workfront Fusion] med hjälp av [!UICONTROL HTTP]-modulen för [!DNL Workfront Fusion].

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

## Ansluta till en webbtjänst som använder en API-token

Proceduren för att ansluta tjänsten via en API-token liknar den för de flesta webbtjänster.

1. Skapa ett program på webbtjänstens webbplats, enligt beskrivningen i avsnittet [Skapa ett nytt program och hämta API-token](#create-a-new-application-and-obtain-the-api-token) i den här artikeln.
1. Hämta API-nyckeln eller API-token.
1. Lägg till [!DNL Workfront Fusion]-modulen [!UICONTROL HTTP] > [!UICONTROL Make a Request] i ditt scenario.
1. Konfigurera modulen enligt webbtjänstens API-dokumentation och kör scenariot, vilket förklaras i avsnittet [Konfigurera [!UICONTROL HTTP] modulen ](#set-up-the-http-module) i den här artikeln.

>[!NOTE]
>
>Vi kommer att använda meddelandetjänsten [!DNL Pushover] som ett exempel i den här artikeln.

## Skapa ett nytt program och hämta API-token

>[!NOTE]
>
>Det finns många olika sätt att skapa och distribuera API-nycklar eller API-tokens i webbtjänster. Instruktioner om hur du hämtar en API-nyckel och -token för den önskade webbtjänsten finns på tjänstens webbplats och söker efter &quot;API-nyckel&quot; eller &quot;API-token&quot;.
>
>Vi inkluderar instruktioner om hur du får en Pushover API-nyckel som exempel på vad du kan hitta.

1. Logga in på ditt [!DNL Pushover]-konto.
1. Klicka på **[!UICONTROL Create an Application/API Token]** längst ned på sidan.
1. Fyll i programinformationen och klicka på **[!UICONTROL Create an Application]**.
1. Lagra den angivna API-token på en säker plats. Du behöver det för modulen [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Make a Request] för att ansluta till önskad webbtjänst ([!DNL Pushover], i det här fallet).

## Konfigurera modulen [!UICONTROL HTTP]

Om du vill ansluta en webbtjänst till ditt [!DNL Workfront Fusion]-scenario måste du använda modulen [!UICONTROL HTTP] >[!UICONTROL Make a request] i scenariot och konfigurera modulen enligt webbtjänstens API-dokumentation.

1. Lägg till modulen [!UICONTROL HTTP] >[!UICONTROL Make a Request] i ditt scenario.
1. Om du vill skicka ett meddelande med [!DNL Workfront Fusion] ställer du in HTTP-modulen enligt följande.

   >[!NOTE]
   >
   >De här modulinställningarna motsvarar API-dokumentationen för webbtjänsten [!DNL Pushover]. Inställningarna kan vara annorlunda för andra webbtjänster. API-token kan till exempel infogas i [!UICONTROL Header] och inte i fältet [!UICONTROL Body].

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
      <td> <p>Vissa webbtjänster kan använda en frågesträng för att ange andra parametrar. Detta är inte fallet i vårt exempel eftersom webbtjänsten [!DNL Pushover] använder [!UICONTROL Body] (se nedan) för alla typer av förfrågningar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Med den här inställningen kan du välja JSON-innehållstypen i fältet [!UICONTROL Content Type] nedan.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON är den innehållstyp som krävs av appen [!UICONTROL Pushover]. Detta kan skilja sig från andra webbtjänster.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Ange [!UICONTROL Body]-begärandeinnehållet i JSON-format. Du kan använda modulen [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] enligt beskrivningen i <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref"> JSON-brödtext som har mappats med [!UICONTROL JSON] &gt; [!UICONTROL Create JSON]-modulen </a> i den här artikeln. Du kan också ange JSON-innehållet manuellt, vilket förklaras i <a href="#json-body-entered-manually" class="MCXref xref">JSON-brödtext som har angetts manuellt</a> i den här artikeln.</p> <p>I webbtjänstens API-dokumentation finns information om vilka parametrar som krävs för den webbtjänsten.</p> </td> 
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
   <td> <p>Din USER_KEY. Detta finns på din [!DNL Pushover]-instrumentpanel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Din API-token/API-nyckel som genererades när du skapade din [!DNL Pushover]-app.</p> </td> 
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

## JSON-brödtext mappad med modulen [!UICONTROL JSON] >[!UICONTROL Create JSON]

Modulen [!UICONTROL Create JSON] gör det enklare att ange JSON. Det ger dig också möjlighet att definiera värden dynamiskt.

Mer information om JSON-modulerna finns i [JSON-moduler](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Ange eller mappa de värden som du vill skapa JSON från.

   ![](assets/json-values-350x288.png)

1. Anslut modulen [!UICONTROL JSON] > [!UICONTROL Create JSON] till HTTP > Gör en begäran-modul.
1. Mappa JSON-strängen från modulen [!UICONTROL Create JSON] till fältet [!UICONTROL Request content] i modulen [!UICONTROL HTTP] >[!UICONTROL Make a Request].

   När du kör scenariot skickas nu push-meddelandet till enheten som har registrerats i ditt [!DNL Pushover]-konto.
