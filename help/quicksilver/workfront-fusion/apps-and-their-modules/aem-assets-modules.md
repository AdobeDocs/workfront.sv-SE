---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets-moduler
description: Med [!DNL Adobe Experience Manager Assets] anslutning för [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] konton, skapa, ladda upp och uppdatera resurser samt kopiera eller flytta mappar och resurser.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] moduler

Med [!DNL Adobe Experience Manager Assets] anslutning för [!DNL Adobe Workfront Fusion]kan du starta ett scenario baserat på händelser i [!DNL Adobe Experience Manager Assets] konton, skapa, ladda upp och uppdatera resurser samt kopiera eller flytta mappar och resurser.

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

## Förutsättningar

* Du måste ha en [!DNL Adobe Experience Manager Assets] för att använda dessa moduler.
* Du måste konfigurera [!UICONTROL Server-to-server] i [!DNL Adobe Developer console].

  Instruktioner om hur du konfigurerar [!UICONTROL Server-to-server] i [!DNL Adobe Developer console], se [Genererar åtkomsttoken för API:er på serversidan](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Skapa en anslutning för [!DNL Adobe Experience Manager Assets] moduler:

1. Klicka [!UICONTROL Add] bredvid [!UICONTROL Connection] box.

2. Välj den typ av anslutning som du skapar:

   * **[!DNL AEM Assets as a Cloud Service]**

     Den här konfigurationen kräver information från [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Den här konfigurationen kräver ett användarnamn och lösenord.

3. Fyll i fälten för den typ av anslutning som du skapar.

   För [!DNL AEM Assets as a Cloud Service], se [Konfigurera anslutningen för [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   För [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]), se [Konfigurera anslutningen för [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.


### Konfigurera anslutningen för [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>Informationen för dessa fält genereras som en del av konfigurationen [!UICONTROL Server-to-server] flödar på [!DNL Adobe Developer Console]. Dessa värden finns i JSON-tjänstens inloggningsinformation som genereras som en del av den konfigurationen.
>
>Instruktioner om hur du konfigurerar [!UICONTROL Server-to-server] flödar på [!UICONTROL Adobe Developer Console], se [Genererar åtkomsttoken för API:er på serversidan](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Connection name]</td>
                  <td>
                      <p>Ange ett namn för anslutningen</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                  <td>Ange URL:en för [!DNL Adobe Experience Manager] -instans. Ta inte med ett snedstreck <code>/</code> i slutet av URL:en.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Ange klient-ID som genereras i [!UICONTROL Server-to-server] konfiguration.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Ange den klienthemlighet som genererats i [!UICONTROL Server-to-server] konfiguration.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Technical account ID]</td>
                  <td>Ange ID för det tekniska kontot. Det här är[!UICONTROL id]" i JSON-filen för klientinloggningsuppgifter.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">Ange ID:t för din organisation. Det här är[!UICONTROL org]" i JSON-filen för klientinloggningsuppgifter.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta Scopes]</td>
                  <td>Ange de metaomfång som genereras i dialogrutan [!UICONTROL Server-to-server] konfiguration.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Private key]</td>
                  <td>Ange den privata nyckel som genererats för att vinna [!UICONTROL Server-to-server] konfiguration. Extrahera den privata nyckeln genom att klicka [!UICONTROL Extract]anger du sedan den fil som ska extraheras och lösenordet för filen.</td>
              </tr>
          </tbody>
      </table>


### Konfigurera anslutningen för [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Connection name]</td>
                <td>
                    <p>Ange ett namn för anslutningen</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                <td>Ange URL:en för [!DNL Adobe Experience Manager] -instans. Ta inte med ett snedstreck <code>/</code> i slutet av URL:en.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Ange användarnamn för [!DNL AEM Assets] konto som den här anslutningen använder.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Ange lösenordet för [!DNL AEM Assets] konto som den här anslutningen använder.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] moduler och deras fält

När du konfigurerar [!DNL Adobe Experience Manager Essentials] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Experience Manager Essentials] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copy a folder or asset]

Den här åtgärdsmodulen kopierar en mapp eller en resurs till en annan plats i ditt Adobe Experience Manager Resurser-konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill kopiera en mapp eller en resurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>Markera eller mappa mappen eller resursen som du vill kopiera.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Markera eller mappa sökvägen till platsen för den nya mappen eller resursen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of copied folder] / [!UICONTROL asset]</td> 
   <td>Ange ett namn för den nya mappen eller resursen. Mappnamnet som visas i [!DNL Adobe Experience Manager Assets] är samma som det ursprungliga namnet. Namnet som anges här visas i URL:en för den nya mappen eller resursen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy children]</td> 
   <td>Aktivera det här alternativet om du vill kopiera alla undermappar eller resurser i mappen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Aktivera det här alternativet om du vill skriva över mappar eller resurser på målplatsen som har samma namn som mappen eller resursen som kopieras.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a record]

Den här åtgärdsmodulen skapar en mapp eller en resurskommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object type]</td> 
   <td> <p>Välj om du vill skapa en mapp eller en kommentar för en resurs.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Fyll i följande fält:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Ange ett namn för mappen. Det här namnet visas i filsökvägen, så det får inte innehålla blanksteg eller andra tecken. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Ange en rubrik för mappen, som kan visas i stället för namnet.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset comment]</p> <p>Fyll i följande fält:</p> 
      <ul> 
       <li> <p>[!UICONTROL Asset selection]</p> <p>Markera eller mappa ID:t för resursen som du vill lägga till en kommentar i.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>Ange texten för kommentaren.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a record]

Den här åtgärdsmodulen tar bort en mapp, en resurs eller en återgivning.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill ta bort en mapp, en resurs eller en återgivning.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Markera mappen som ska tas bort genom att markera mapparna i sökvägen.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Markera resursen genom att markera mapparna i sökvägen och sedan den resurs du vill ta bort.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Markera återgivningen genom att markera mapparna i sökvägen.</p> <p>Ange eller mappa återgivningens namn.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a folder listing]

Den här åtgärdsmodulen hämtar en representation av en befintlig mapp och av dess underordnade enheter (mappar eller resurser).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Markera eller mappa mappen som du vill hämta. Om du vill lägga till undermappar i sökvägen klickar du på plusikonen och väljer undermappen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make a custom API call]

Den här åtgärdsmodulen gör ett anpassat API-anrop till [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ange en relativ sökväg till [!DNL Adobe Experience Manager] bas-URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] lägger till auktoriseringshuvuden automatiskt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Ange frågesträngen för begäran. För varje nyckel/värde-par klickar du på <b>[!UICONTROL Add item]</b> och anger [!UICONTROL Key] och [!UICONTROL Value].</p> </td> 
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

### [!UICONTROL Move a folder or asset]

Den här åtgärdsmodulen flyttar resursen eller mappen på den angivna sökvägen till en ny plats.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill flytta en mapp eller en resurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>Markera eller mappa mappen eller resursen som du vill flytta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Markera eller mappa sökvägen till den plats där du vill flytta mappen eller resursen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of moved folder] / [!UICONTROL asset]</td> 
   <td>Ange ett nytt namn för den flyttade mappen eller resursen. Mappnamnet som visas i [!DNL Adobe Experience Manager Assets] är samma som det ursprungliga namnet. Namnet som anges här visas i URL:en för den flyttade mappen eller resursen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Aktivera det här alternativet om du vill skriva över mappar eller resurser på målplatsen som har samma namn som mappen eller resursen som kopieras.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a record]

Den här åtgärdsmodulen uppdaterar en befintlig post.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill ta bort metadata för resursen eller en resursåtergivning.</p> 
    <ul> 
     <li> <p>[!UICONTROL Asset metadata]</p> 
      <ul> 
       <li> <p>Välj den resurs som du vill uppdatera metadata för.</p> </li> 
       <li> <p>Ange resursens nya namn.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset rendition]</p> 
      <ul> 
       <li> <p>Välj den resurs som du vill uppdatera återgivningen för.</p> </li> 
       <li> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Upload an asset]

Den här åtgärdsmodulen överför en resurs till din [!DNL Adobe Experience Manager Assets] konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Adobe Experience Manager Assets] konto till [!DNL Workfront Fusion], se <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Adobe Experience Manager Assets] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination]</td> 
   <td> <p>Välj den mapp där du vill överföra en resurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Ange eller mappa källfilens namn och data.</td> 
  </tr> 
 </tbody> 
</table>
