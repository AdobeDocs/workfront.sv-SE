---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: http-modules
title: HTTP &gt; Skapa en modul för grundläggande auktoriseringsbegäran
description: Adobe Workfront Fusion kräver en Adobe Workfront Fusion-licens förutom en Adobe Workfront-licens.
author: Becky
feature: Workfront Fusion
exl-id: df8b53de-1af2-4026-b7dd-ff5133b4aac2
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL Make a Basic Authorization request] modul

Detta [!DNL Adobe Workfront Fusion] Med -modulen kan du konfigurera en HTTP-begäran med grundläggande HTTP-auktorisering och skicka den till en server. Det mottagna HTTP-svaret finns sedan i utdatapaketet.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Make a Basic Authorization request] modulkonfiguration

När du konfigurerar [!UICONTROL HTTP] >[!UICONTROL Make a Basic Authorization request] modul, [!DNL Adobe Workfront Fusion] visar fälten som listas nedan. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Välj den nyckel som innehåller dina grundläggande autentiseringsuppgifter eller klicka på <strong>[!UICONTROL Add]</strong> för att lägga till dina inloggningsuppgifter i en ny nyckel. </p> <p>Obs! Du kan lägga till fler autentiseringsuppgifter för att enkelt växla mellan olika anslutningar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx )] </td> 
   <td> <p>Använd det här alternativet om du vill konfigurera felhantering.</p> <p>Mer information finns i <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Felhantering i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Ange den URL som du vill skicka en begäran till, t.ex. en API-slutpunkt, webbplats osv.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.Till exempel <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ange önskade nyckelvärdepar för frågan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP-brödtexten är de databyte som skickas i ett HTTP-transaktionsmeddelande omedelbart efter rubrikerna om något ska användas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw-brödtexttypen är vanligtvis lämplig för de flesta HTTP-innehållsbegäranden, även i situationer där utvecklardokumentationen inte anger vilka data som ska skickas.</p> <p>Ange en form av tolkning av data i [!UICONTROL Content type] fält.</p> <p>Trots att innehållstypen är vald, anges data i vilket format som helst som anges eller krävs av utvecklardokumentationen.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Den här brödtypen är [!UICONTROL POST] data använda <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>För <code>[!UICONTROL application/x-www-form-urlencoded]</code>, innehåller HTTP-meddelandet som skickas till servern i stort sett en frågesträng. Tangenterna och värdena kodas i nyckelvärdepar avgränsade med <code>&amp;</code> och med <code>=</code> mellan nyckeln och värdet. </p> <p>Använd för binära data <code>multipart/form-data</code> i stället.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exempel: </b></span></span> 
       <p>Exempel på det resulterande formatet för HTTP-begäran:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>The [!UICONTROL Multipart/form-data] är en HTTP-multipart-begäran som används för att skicka filer och data. Det används ofta för att överföra filer till servern.</p> <p>Lägg till fält som ska skickas i begäran. Varje fält måste innehålla nyckelvärdepar.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Ange nyckeln och värdet som ska skickas i begärandetexten.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Ange nyckeln och ange den källfil som du vill skicka i begärandetexten.</p> <p>Mappa filen som du vill överföra från föregående modul (till exempel [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] eller [!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]eller ange filnamnet och fildata manuellt.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Aktivera det här alternativet för att automatiskt analysera svar och konvertera JSON- och XML-svar så att du inte behöver använda [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] eller [!UICONTROL XML] &gt; [!UICONTROL Parse XML] moduler.</p> <p>Innan du kan använda tolkat JSON- eller XML-innehåll kör du modulen en gång manuellt, så att modulen kan identifiera svarsinnehållet och mappa det i efterföljande moduler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Ange timeout för begäran i sekunder (1-300). Standardvärdet är 40 sekunder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> Aktivera det här alternativet om du vill dela cookies från servern med alla HTTP-moduler i ditt scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Överför ditt certifikat om du vill använda TLS med ditt självsignerade certifikat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>Aktivera det här alternativet om du vill avvisa anslutningar som använder overifierade TLS-certifikat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Aktivera det här alternativet om du vill följa URL-omdirigeringarna med 3xx-svar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>Aktivera det här alternativet om du vill följa URL-omdirigeringarna med alla svarskoder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>Som standard [!DNL Workfront Fusion] hanterar flera värden för samma URL-frågesträngsparameternyckel som arrayer. Till exempel: <code>www.test.com?foo=bar&amp;foo=baz</code> konverteras till <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Aktivera det här alternativet om du vill inaktivera den här funktionen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> Aktivera det här alternativet om du vill begära en komprimerad version av webbplatsen.</p> <p>Lägger till en <code>[!UICONTROL Accept-Encoding]</code> för att begära komprimerat innehåll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>Aktivera det här alternativet om du vill använda ömsesidig TLS i HTTP-begäran.</p> <p>Mer information om Ömsesidig TLS finns i <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Använd ömsesidig TLS i HTTP-moduler i  </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
