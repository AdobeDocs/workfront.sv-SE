---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: OpenAI-moduler (ChatGPT)
description: I ett Adobe Workfront Fusion-scenario kan du automatisera arbetsflöden som använder OpenAIT(ChatGPT) och ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
source-git-commit: a8bc882f393dcf17bca80da86c25c053272e27c9
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL OpenAI (ChatGPT & DALL-E)], samt ansluta till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Används [!DNL OpenAI (ChatGPT & DALL-E)] moduler, du måste ha en [!DNL OpenAI] konto, inklusive en API-nyckel och ett organisations-ID.

## Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]

Du kan skapa en anslutning till [!DNL OpenAI (ChatGPT & DALL-E)] direkt inifrån ett [!DNL OpenAI (ChatGPT & DALL-E)] -modul.

1. I alla [!DNL OpenAI (ChatGPT & DALL-E)] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Ange ett namn för den nya anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>Du hittar API-nyckeln i användarinställningarna för OpenAI.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Organization ID] </td> 
      <td>Du hittar ditt organisations-ID på sidan Organisationsinställningar i OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.


## [!DNL OpenAI (ChatGPT & DALL-E)] moduler och deras fält

När du konfigurerar [!DNL OpenAI (ChatGPT & DALL-E)] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL OpenAI (ChatGPT & DALL-E)] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Skapa en slutförd

Den här åtgärdsmodulen skapar ett slutförande för den angivna uppmaningen eller chatten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Ange eller mappa ID:t för modellen som ska användas. Du kan använda modulen Hämta modeller för att visa alla tillgängliga modeller. </td> 
  </tr> 
  <!--<tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>Mer information om de valfria avancerade inställningarna i den här modulen finns i informationen om hur du skapar slutföranden i <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">API-dokumentation för OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Skapa en moderering

Den här åtgärdsmodulen avgör om texten bryter mot OpenAI:s innehållspolicy.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> För varje textexempel som du vill ta med klickar du <b>Lägg till objekt</b> och ange eller mappa texten. Inkludera hela textexemplet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Ange eller mappa ID:t för modellen som ska användas. Du kan använda modulen Hämta modeller för att visa alla tillgängliga modeller. </td> 
  </tr> 
 </tbody> 
</table>

### Skapa en redigering

Den här åtgärdsmodulen returnerar en redigerad version av en fråga som du anger, enligt dina instruktioner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Ange eller mappa ID:t för modellen som ska användas. Du kan använda modulen Hämta modeller för att visa alla tillgängliga modeller. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Ange eller mappa texten som du vill redigera. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Instruction]</td> 
   <td> Ange eller mappa instruktionerna för redigeringen. Exempel:"Korrigera stavfel." </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>Mer information om de valfria avancerade inställningarna i den här modulen finns i informationen om hur du skapar redigeringar i <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">API-dokumentation för OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Skapa en inbäddning

Den här åtgärdsmodulen skapar en inbäddningsvektor som representerar indatatexten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Ange eller mappa ID:t för modellen som ska användas. Du kan använda modulen Hämta modeller för att visa alla tillgängliga modeller. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input text to embed]</td> 
   <td> Ange eller mappa texten som du vill bädda in. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> Ange eller mappa en unik identifierare som representerar din slutanvändare, vilket kan hjälpa OpenAI att övervaka och upptäcka missbruk </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Ange eller mappa det maximala antal redigeringar som du vill att modulen ska arbeta med under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Skapa chattslutförande

Om en lista med meddelanden beskriver en konversation returnerar åtgärdsmodulen ett svar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Ange eller mappa ID:t för modellen som ska användas. Du kan använda modulen Hämta modeller för att visa alla tillgängliga modeller. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>Meddelanden beskriver konversationen hittills. För varje meddelande du vill lägga till klickar du på <b>Lägg till objekt</b> och fylla i följande:
   <ul>
   <li> <b>Roll</b>: Välj rollen som författare till det här meddelandet.</li>
   <li> <b>Innehåll</b>: Ange eller mappa innehållet i meddelandet.</li>
   <li> <b>Namn</b>: Ange eller mappa namnet på meddelandets författare. Namnet kan innehålla versaler och gemener, siffror och understreck. Namnet får innehålla högst 64 tecken.</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>Mer information om de valfria avancerade inställningarna i den här modulen finns i informationen om hur du skapar chattkompletteringar i <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">API-dokumentation för OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Generera bilder

Den här åtgärdsmodulen genererar eller ändrar bilder med Dall-E-modeller.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text description of the desire image]</td> 
   <td> Ange eller mappa en beskrivning av den önskade bilden. Den maximala beskrivningslängden är 1 000 tecken. 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>Mer information om de valfria avancerade inställningarna i den här modulen finns i informationen om hur du skapar bilder i <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">API-dokumentation för OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Hämta modeller

I den här modulen visas och beskrivs de olika modeller som finns i OpenAI API:t.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Välj om du vill få en lista över alla modeller eller hämta en specifik modell.
    <ul>
    <li><p><b>Listmodeller </b></p><p>Den här åtgärden listar de modeller som är tillgängliga och ger grundläggande information om var och en av dem, till exempel ägare och tillgänglighet.</p></li>
    <li><p><b>Hämta modell </b></p><p>Ange eller mappa ID:t för modellen som du vill hämta. </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### Göra ett anpassat API-anrop

Den här åtgärdsmodulen är en anpassad HTTP-begäran till OpenAI API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Ange en sökväg i förhållande till <code>https://api.openai.com/v1/</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion lägger automatiskt till auktoriseringshuvuden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"name":"something-urgent"}</code></p> </td> 
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

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### Hantera filer

Den här åtgärdsmodulen visar, tar bort eller hämtar filer eller filinnehåll.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Välj den åtgärd som du vill utföra. 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> Om du tar bort en fil eller hämtar en fil eller ett filinnehåll anger eller mappar du filens ID. 
  </tr> 
</tbody>
</table>

### Hantera finjusteringar

Hantera finjusteringsjobb för att skräddarsy en modell efter era specifika utbildningsdata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL OpenAI (ChatGPT & DALL-E)] konto för Workfront Fusion, se <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Ansluter [!DNL OpenAI (ChatGPT & DALL-E)] till [!DNL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Välj den åtgärd som du vill utföra.
   <ul>
   <li><p>Finjustera en modell från en datauppsättning</p><p>Ange eller mappa en beskrivning för den önskade bilden.</p>
     <li><p>Hämta information om ett finjusteringsjobb</p><p>Ange eller mappa ID:t för jobbet.</p>
   <li><p>Avbryt ett finjusteringsjobb</p><p>Ange eller mappa ID:t för jobbet.</p>
   <li><p>Avbryt ett finjusteringsjobb</p><p>Ange eller mappa ID:t för jobbet.</p>
   <li><p>Hämta statusuppdateringar för ett finjusteringsjobb</p><p>Ange eller mappa ID:t för jobbet och välj om du vill strömma uppdateringarna.</p>
   <li><p>Ta bort en finjusterad modell</p><p>Ange eller mappa ID:t för modellen som du vill ta bort.</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> Om du tar bort en fil eller hämtar en fil eller ett filinnehåll anger eller mappar du filens ID. 
  </tr> 
</tbody>

