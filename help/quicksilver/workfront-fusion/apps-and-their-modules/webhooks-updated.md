---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# Webhooks



>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artiklarna:
>
>* [Webhooks](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/webhooks-updated.html)
>* [Konfigurera en webkrok för en webbtjänst utan anslutning](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

En webkrok är ett HTTP-anrop som aktiveras av en händelse. Du kan använda webhooks för att aktivera snabbutlösarmoduler. Alla program som är anslutna till Internet och som tillåter HTTP-begäranden kan skicka webbböcker till Adobe Workfront Fusion.

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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Använd en webkrok i [!DNL Workfront Fusion]

>[!NOTE]
>
>Om du vill anropa en webkrok från en annan leverantör (en utgående webkrok) använder du en av HTTP-modulerna. Mer information finns i [HTTP-moduler](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Så här använder du en webkrok för att ansluta en app till [!DNL Workfront Fusion]:

1. Lägg till **[!UICONTROL Webhooks]** >**[!UICONTROL Custom Webhook]**-modulen för snabbutlösare i ditt scenario.

1. Klicka på **[!UICONTROL Add]** bredvid Webkrok-fältet och ange ett namn för den nya webkroken.
1. (Valfritt) Klicka på **[!UICONTROL Advanced Settings]**.
1. I fältet **[!UICONTROL IP restrictions]** anger du en kommaavgränsad lista över IP-adresser som modulen kan ta emot data från.
1. Klicka på **[!UICONTROL Save]**

När du har skapat en webbkrok visas en unik URL. Det här är adressen som webbhoven skickar data till. Workfront Fusion validerar de data som skickas till den här adressen och skickar dem sedan för behandling i scenariot.

>[!NOTE]
>
>När du har skapat en webkrok kan du använda den i fler än ett scenario åt gången.

### Konfigurera webbhakens datastruktur {#configure-the-webhook-s-data-structure}

[!DNL Workfront Fusion] tolkar exempeldata som du skickar till den visade adressen för att identifiera datastrukturen för den inkommande nyttolasten. Du kan ange exempeldata genom att göra en ändring i tjänsten eller appen som får tjänsten eller appen att anropa webbkroken. Du kan till exempel ta bort en fil.

Du kan också följa stegen nedan för att skicka exempeldata via modulen [!UICONTROL HTTP] > [!UICONTROL Make a request].

1. Skapa ett nytt scenario med modulen **[!UICONTROL HTTP]** > **[!UICONTROL Make a request]**

1. Konfigurera modulen med följande värden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Ange webbkrokens URL. Du hittar den här URL:en i modulen [!UICONTROL Webhooks] som du har använt för att konfigurera webkroken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request content]</td> 
      <td><p>Rå JSON förväntades i webkroken</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Öppna scenariot med modulen [!UICONTROL Webhooks] på en separat webbläsarflik eller i ett separat fönster.
1. Klicka på **[!UICONTROL Redetermine data structure]** i webbmodulen.

   Du behöver inte bryta länken till andra moduler från webbhooks-modulen.

1. Växla till scenariot med modulen [!UICONTROL HTTP] och kör det.
1. Växla tillbaka till scenariot med modulen Webhooks.

   Ett [!UICONTROL Successfully determined]-meddelande betyder att modulen har fastställt datastrukturen.

   ![](assets/successfully-determined-350x175.png)

1. Klicka på **[!UICONTROL OK]** om du vill spara datastrukturen.

   Webkrokens objekt är nu tillgängliga på mappningspanelen för användning med efterföljande moduler i scenariot.

## Webkrok-kön

Om en webkrok tar emot data och det inte finns något aktivt scenario som förväntar sig dessa data, lagras data i kön. När du har aktiverat scenariot bearbetas alla paket som väntar i kön sekventiellt.

>[!IMPORTANT]
>
>Webkrokköer delas mellan scenarier som använder samma webkrok. Om ett av scenarierna är inaktiverat hålls alla inkommande data i kön.

## Inkommande dataformat som stöds

[!DNL Workfront Fusion] stöder 3 inkommande dataformat: [!UICONTROL Query String], [!UICONTROL Form Data] och [!UICONTROL JSON].

[!DNL Workfront Fusion] validerar alla inkommande data mot den valda datastrukturen. Beroende på inställningarna för scenariot lagras data antingen i kön för bearbetning eller bearbetas omedelbart.

Om någon del av data inte godkänns vid valideringen returnerar [!DNL Workfront Fusion] en HTTP-statuskod på 400 och anger, i HTTP-svarets brödtext, varför inkommande data misslyckades vid valideringskontrollerna. Om valideringen av inkommande data lyckas returnerar Workfront Fusion statusen [!UICONTROL 200 Accepted].

* [[!UICONTROL Query String]](#query-string)
* [[!UICONTROL Form Data]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Query String]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Form Data]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Multipart-formulärdata

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

För att kunna ta emot filer som är kodade med `multipart/form-data` måste du konfigurera en datastruktur med ett `collection`-typfält som innehåller de kapslade fälten `name`, `mime` och `data`. Fältet `name` är av typen `text` och innehåller namnet på den överförda filen. `mime` är en `text`-typ och innehåller en fil i MIME-format. Fältet `data` är av typen `buffer` och innehåller binära data för filen som överförs.

Mer information om MIME-format finns i [MIME-moduler](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Om du vill komma åt det ursprungliga JSON-objektet aktiverar du JSON-direktanslutningen när du konfigurerar webkroken.
>
>1. Klicka på **[!UICONTROL Add]** om du vill lägga till en ny webbkrok.
>1. Klicka på **[!UICONTROL Show advanced settings]**.
>1. Klicka på **[!UICONTROL JSON pass-through]**.
>

## Webkrohuvuden

Aktivera Hämta begäranderubriker när du konfigurerar webkroken om du vill få åtkomst till webbhakens sidhuvuden.

1. Klicka på **[!UICONTROL Add]** om du vill lägga till en ny webbkrok.
1. Klicka på **[!UICONTROL Show advanced settings]**.
1. Klicka på **[!UICONTROL Get request headers]**.

Du kan extrahera ett visst rubrikvärde med kombinationen av funktionerna `map()` och `get()`.

>[!INFO]
>
>**Exempel:**
>
>I exemplet nedan visas en formel som extraherar värdet för huvudet `authorization` från arrayen `Headers[]`. Formeln används i ett filter som jämför det extraherade värdet med den angivna texten för att skicka endast webhooks om det finns en matchning.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Mer information om hur du hämtar en arrays element med en viss nyckel finns i [Mappa en arrays element med en viss nyckel](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) i artikeln [Mappa information från en modul till en annan i Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Svara på webhooks

Standardsvaret på ett webkrok-anrop är texten&quot;Godkänd&quot;. Svaret returneras till appen som anropade webkroken när den anpassade webkrosmodulen kördes.

* [Testa svaret på en webkrok](#test-the-response-to-a-webhook)
* [Exempel på HTML-svar](#html-response-example)
* [Exempel på omdirigering](#redirect-example)

### Testa svaret på en webkrok

1. Inkludera modulen **[!UICONTROL Custom Webhook]** i ditt scenario.
1. Lägg till en ny webbkrok i modulen.
1. Kopiera webkroks-URL:en till Urklipp.
1. Kör scenariot.

   Blixtikonen i modulen [!UICONTROL Custom Webhook] ändras till snurrande punkter. Detta visar att modulen nu väntar på webkrok-anropet.

1. Öppna ett nytt webbläsarfönster, klistra in den kopierade URL:en i adressfältet och tryck på **[!UICONTROL Enter]**.

   Modulen [!UICONTROL Custom Webhook] aktiveras och webbläsaren visar en ny sida.

Om du vill anpassa webkroks svar ska du använda modulen Webkrok Response.

Modulens konfiguration innehåller två fält: [!UICONTROL Status] och [!UICONTROL Body].

* Fältet [!UICONTROL Status] innehåller HTTP-svarsstatuskoder som 2xx för Slutfört (till exempel `200` för OK), 3xx för Omdirigering (till exempel `307` för tillfällig omdirigering), 4xx för klientfel (till exempel `400` för Felaktig begäran) och så vidare.

* Fältet [!UICONTROL Body] innehåller allt som accepteras av webkrockens anrop. Det kan vara enkel text, HTML, XML, JSON och så vidare.

  >[!TIP]
  >
  >Vi rekommenderar att du ställer in rubriken `Content-Type` på motsvarande MIME-typ: `text/plain` för oformaterad text, `text/html` för HTML, `application/json` för JSON, `application/xml` för XML och så vidare. Mer information om MIME-typer finns i [MIME-moduler](../../workfront-fusion/apps-and-their-modules/mime.md).

Tidsgränsen för att skicka ett svar är 40 sekunder. Om svaret inte är tillgängligt inom den perioden returnerar Workfront Fusion statusen&quot;200 Accepted&quot;.

### Exempel på svar från HTML

>[!INFO]
>
>**Exempel:**
>
>Konfigurera modulen [!UICONTROL Webhook Response] enligt följande:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>2xx lyckad HTTP-statuskod, t.ex. 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Nyckel</strong>: Innehållstyp</li> 
&gt;     <li><strong>Värde</strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Detta ger ett svar från HTML som visas i en webbläsare:
>
>![](assets/html-response-350x70.png)

### Exempel på omdirigering

>[!INFO]
>
>**Exempel:** Konfigurera modulen [!UICONTROL Webhook Response] enligt följande:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>3 x omdirigerings-HTTP-statuskod, t.ex. 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Plats</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: Den URL som du vill omdirigera till.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webkroks-inaktivering

Webhooks inaktiveras automatiskt om något av följande gäller:

* Webbkroken har inte varit ansluten till något scenario på mer än fem dagar
* Webkroken används bara i inaktiva scenarier, som har varit inaktiva i mer än 30 dagar.

Inaktiverade webhooks tas bort och avregistreras automatiskt om de inte är anslutna till några scenarier och har inaktiverats i över 30 dagar.


## Felsökning

### Saknade objekt på mappningspanelen

Om några objekt saknas i mappningspanelen i inställningarna för modulerna efter modulen [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] klickar du på modulen **[!UICONTROL Webhooks]>[!UICONTROL Custom Webhook]** för att öppna dess inställningar och sedan på **[!UICONTROL Re-determine data structure]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Följ sedan de steg som beskrivs i avsnittet [Konfigurera webkrockens datastruktur](#configure-the-webhook-s-data-structure) i den här artikeln.
