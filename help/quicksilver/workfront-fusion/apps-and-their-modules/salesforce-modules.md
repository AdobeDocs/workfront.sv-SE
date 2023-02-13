---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Salesforce-moduler
description: I ett Adobe Workfront Fusion-scenario kan du automatisera arbetsflöden som använder Salesforce och ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 0%

---

# [!DNL Salesforce] moduler

I ett Adobe Workfront Fusion-scenario kan du automatisera arbetsflöden som använder [!DNL Salesforce], samt ansluta till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Inte alla utgåvor av [!DNL Salesforce] har API-åtkomst. Mer information finns i informationen om [!DNL Salesforce] utgåvor med API-åtkomst på [!DNL Salesforce] Webbplats för communityn.
>* För information om specifika fel som returneras från [!DNL Salesforce] API, se [!DNL Salesforce] API-dokument. Du kan även kontrollera status för [!DNL Salesforce] API för eventuella tjänstavbrott.
>


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

## Förutsättningar

Används [!DNL Salesforce] moduler, du måste ha en [!DNL Salesforce] konto.

## Om att söka efter [!DNL Salesforce] objekt

När du söker efter objekt kan du antingen ange enskilda sökord eller skapa en mer komplex fråga med jokertecken och operatorer:

* Använd asteriskens jokertecken (\*) som ersättning för noll eller flera tecken. Om du till exempel söker efter Ca\* hittas objekt som börjar med Ca
* Använd frågetecken som jokertecken (?) som ersättning för ett enskilt tecken. Om du söker efter Jo?n hittas objekt med termen John eller Joan men inte Jon
* Använd operatorn för citattecken (&quot; &quot;) för att hitta en exakt frasmatchning. Till exempel: &quot;Månadsmöte&quot;

Mer information om sökmöjligheter finns i [!DNL Salesforce] utvecklardokumentation om SOQL och SOSL.

## [!DNL Salesforce] moduler och deras fält

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

* [[!UICONTROL Watch for Records]](#watch-for-records)
* [[!UICONTROL Watch Outbound Messages]](#watch-outbound-messages)
* [[!UICONTROL Watch a field]](#watch-a-field)

#### [!UICONTROL Watch for Records]

Den här utlösarmodulen kör ett scenario när en post i ett objekt skapas eller uppdateras. Modulen returnerar alla standardfält som är associerade med posten eller posterna, tillsammans med anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Välj typ av [!DNL Salesforce] spela in som du vill att modulen ska bevaka.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Fields]</td> 
   <td>Markera de fält som du vill att modulen ska bevaka. Vilka fält som är tillgängliga beror på posttypen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Ange om du vill att scenariot bara ska bevaka nya poster av den typ som du har valt, eller nya poster av den typ som du har valt och alla andra ändringar av poster av den typen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Outbound Messages]

Den här utlösarmodulen kör ett scenario när någon skickar ett meddelande. Modulen returnerar alla standardfält som är associerade med posten eller posterna, tillsammans med anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Den här modulen kräver extra inställningar:

1. Gå till [!DNL Salesforce] konfigurationssida.

   Om du vill komma åt installationssidan letar du upp och klickar på knappen &quot;[!UICONTROL Setup]&quot; i det övre högra hörnet av [!DNL Salesforce] konto. Från [!DNL Salesforce] konfigurationssida, leta upp[!UICONTROL Quick Find / Search]&quot; bar till vänster. Sök efter &quot;[!UICONTROL Workflow Rules].&quot;

1. Klicka på **[!UICONTROL Workflow Rules]**.
1. På [!UICONTROL Workflow Rules] sida som visas klickar du på **[!UICONTROL New Rule]** och välj den objekttyp som regeln ska gälla för (till exempel &quot;[!UICONTROL Opportunity]&quot; om du övervakar uppdateringar av säljprojektsposter).
1. Klicka på **[!UICONTROL Next]**.
1. Ange ett regelnamn, utvärderingskriterier och regelvillkor och klicka sedan på **[!UICONTROL Save]** och **[!UICONTROL Next]**.

1. Klicka på **[!UICONTROL Done]**.
1. Klicka på den nya arbetsflödesregeln **[!UICONTROL Edit]**..
1. I listrutan **[!UICONTROL Add Workflow Action]** väljer du **[!UICONTROL New Outbound Message]**.

1. Ange namn, beskrivning, slutpunkts-URL och fält som du vill inkludera i det nya utgående meddelandet och klicka sedan på **[!UICONTROL Save]**.

   The **[!UICONTROL Endpoint URL]** fältet innehåller den URL som finns på [!DNL Salesforce] [!UICONTROL Outbound Message] in [!DNL Workfront Fusion].

1. Konfigurera ett scenario som börjar med [!UICONTROL Outbound Message] -händelse.

1. Klicka på **&lt;/>** ikonen längst ned till höger och kopiera den angivna URL:en.
1. Återgå till **[!UICONTROL Workflow Rules]** söker du efter den nya regeln och klickar på **[!UICONTROL Activate]**.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Välj den webkrok som du vill använda för att bevaka utgående meddelanden. Om du vill lägga till en webkrok klickar du på <strong>[!UICONTROL Add]</strong> och ange webbhakens namn och anslutning.</p> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Välj typ av [!DNL Salesforce] registrera att du vill att modulen ska bevaka utgående meddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Markera de fält som du vill att modulen ska bevaka för utgående meddelanden. Vilka fält som är tillgängliga beror på posttypen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Watch a field]*

Den här utlösarmodulen startar ett scenario när ett fält uppdateras i [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Välj den typ av post som innehåller fältet som du vill att modulen ska bevaka. Du måste välja en posttyp som har [!UICONTROL Field History] aktiverad [!DNL Salesforce] konfiguration. Mer information finns i <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Spårning av fälthistorik</a> i [!DNL Salesforce] dokumentation. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Markera de fält som du vill att modulen ska bevaka för ändringar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal fält som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [[!UICONTROL Create a Record]](#create-a-record)
* [[!UICONTROL Read a Record]](#read-a-record)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Upload Attachment/Document]](#upload-attachmentdocument)
* [[!UICONTROL Download Attachment/Document]](#download-attachmentdocument)

#### [!UICONTROL Create a Record]

Den här åtgärdsmodulen skapar en ny post i ett objekt.

I modulen kan du välja vilka av objektets fält som är tillgängliga i modulen. Detta minskar antalet fält som du måste bläddra igenom när du ställer in modulen.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Välj typ av [!DNL Salesforce] som du vill att modulen ska skapa. Fälten blir tillgängliga baserat på vilken typ av post som har valts i [!UICONTROL Record Type] fält. Dessa fält är baserade på [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Markera de fält som du vill att modulen ska konfigurera när den nya posten skapas. Obligatoriska fält visas högst upp i listan. </p> <p>Fälten som du väljer öppnas under det här fältet. Du kan nu ange värden i dessa fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a Record]

Den här åtgärdsmodulen läser data från ett enskilt objekt i [!DNL Salesforce].

Du anger postens ID.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Välj typ av [!DNL Salesforce] som du vill att modulen ska [åtgärd].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Record Fields]</td>
    <td>Markera de fält som du vill att modulen ska läsa. Du måste markera minst ett fält.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Ange eller mappa det unika [!DNL Salesforce] ID för den post som du vill att modulen ska läsa.</p> <p>Öppna [!DNL Salesforce] i webbläsaren och kopiera texten i slutet av URL:en efter det sista snedstrecket (/). Exempel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Record]

Den här åtgärdsmodulen tar bort en befintlig post i ett objekt.

Du anger postens ID.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Välj typ av [!DNL Salesforce] som du vill att modulen ska ta bort.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Ange eller mappa det unika [!DNL Salesforce] ID för den post som du vill att modulen ska ta bort.</p> <p>Öppna [!DNL Salesforce] i webbläsaren och kopiera texten i slutet av URL:en efter det sista snedstrecket (/). Exempel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Salesforce] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Salesforce] moduler.

Modulen returnerar följande:

* **[!UICONTROL Status Code]** (tal): Detta anger om HTTP-begäran lyckades eller misslyckades. Det här är standardkoder som du kan söka efter på Internet.
* **[!UICONTROL Headers]** (objekt): En mer detaljerad kontext för den svars-/statuskod som inte är relaterad till utdatatexten. Alla sidhuvuden som visas i en svarshuvud är inte svarshuvuden, så en del kanske inte är användbara för dig.

   Svarshuvuden beror på den HTTP-begäran du valde när du konfigurerade modulen.

* **[!UICONTROL Body]** (objekt): Beroende på vilken HTTP-begäran du valde när du konfigurerade modulen kan du få tillbaka data. Dessa data, till exempel data från en [!UICONTROL GET] request, finns i det här objektet.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ange en sökväg som är relativ till<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>En lista över tillgängliga slutpunkter finns i <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Utvecklarhandbok för Salesforce REST API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.Till exempel <code>{"Content-type":"application/json"}</code>. Workfront Fusion lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt. Till exempel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Följande API-anrop returnerar listan över alla användare i [!DNL Salesforce] konto:
>
>* **URL**: `query`
>
>* **Metod**: [!UICONTROL GET]
>
>* **Frågesträng**:
>
>* **Nyckel**: `q`
>
>* **Värde**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Matchningar av sökningen finns i modulens utdata under **[!UICONTROL Bundle]> [!UICONTROL Body] >[!UICONTROL records]**.
>
>I vårt exempel returnerades sex användare:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Upload Attachment/Document]

Den här åtgärdsmodulen överför en fil och bifogar den till en post som du anger, eller överför ett dokument.

Modulen returnerar ID:t för den bifogade filen eller dokumentet och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type of Upload]</td> 
   <td>Välj om du vill att modulen ska överföra en bifogad fil eller ett dokument.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Ange eller mappa ID:t för objektet som du vill överföra en bifogad fil till.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Markera den mapp som innehåller den fil som du vill att modulen ska överföra. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download Attachment/Document]

Den här åtgärdsmodulen hämtar ett dokument eller en bifogad fil från en post.

Du anger postens ID och vilken typ av hämtning du vill använda.

Modulen returnerar ID:t för den bifogade filen eller dokumentet och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type of Download]</td>
    <td> <p>Ange vilken typ av fil du vill hämta från Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (Detta är ett dokument som har överförts till ett bibliotek i [!DNL Saleforce CRM Content] eller [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Ange eller mappa det unika [!DNL Salesforce] ID för den post som du vill att modulen ska hämta.</p> <p>Öppna [!DNL Salesforce] i webbläsaren och kopiera texten i slutet av URL:en efter det sista snedstrecket (/). Exempel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Update a Record]

Den här åtgärdsmodulen redigerar en post i ett objekt.

I modulen kan du välja vilka av objektets fält som är tillgängliga i modulen. Detta minskar antalet fält som du måste bläddra igenom när du ställer in modulen.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Ange eller mappa ID:t för den post som du vill uppdatera.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Välj typ av [!DNL Salesforce] som du vill att modulen ska uppdatera. Fälten blir tillgängliga baserat på vilken typ av post som har valts i fältet Posttyp. Dessa fält är baserade på [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Markera de fält som du vill att modulen ska konfigurera när den nya posten skapas. Obligatoriska fält visas högst upp i listan. </p> <p>Fälten som du väljer öppnas under det här fältet. Du kan nu ange värden i dessa fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

#### [!UICONTROL Search with Query]

Den här sökmodulen söker efter poster i ett objekt i [!DNL Salesforce] som matchar den sökfråga du anger. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>Välj den typ av sökning som du vill att modulen ska utföra:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Om du valde den enkla söktypen väljer du typ av [!DNL Salesforce] poster som du vill att modulen ska söka efter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Ange frågan som du vill söka efter.</p> <p>Mer information om SOSL finns på <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> i [!DNL Salesforce] dokumentation.</p> <p>Mer information om SOQL finns i <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> i [!DNL Salesforce] dokumentation.</p> <p>Obs! Observera att värdet på parametern <code>RETURNING </code>påverkar modulens utdata. Om du använder <code>LIMIT</code>, [!DNL Fusion] kommer att ignorera inställningarna i [!UICONTROL Maximal count of records] fält. Om du inte anger någon gräns infogar Fusion värdet [!UICONTROL LIMIT = Maximal count of records].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search]

Den här åtgärdsmodulen hämtar alla poster som uppfyller ett visst villkor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter [!DNL Salesforce] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till[!DNL  Adobe Workfront Fusion] - Grundläggande instruktioner</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Välj den typ av objekt som du vill söka efter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Markera fältet som du vill söka efter, operatorn som du vill använda i frågan och värdet som du söker efter i fältet. Du kan koppla frågor med AND eller OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de fält som du vill inkludera i modulens utdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Välj om du vill att modulen ska returnera alla matchande poster eller endast den första matchande posten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska hämta under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>
