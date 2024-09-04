---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Workfront Proof moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder  [!DNL Workfront Proof] samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 558ca6a1935d33e2c3c7ea3f4c1bd90a493ef8ff
workflow-type: tm+mt
source-wordcount: '2688'
ht-degree: 0%

---

# [!DNL Workfront Proof] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL Workfront Proof] samt ansluta det till flera tredjepartsprogram och -tjänster.

Detta är användbart om du behöver utföra uppgifter som för närvarande inte stöds för korrektur i [!DNL Workfront] eller [!DNL Workfront Proof], till exempel uppdatera korrektur baserat på vissa händelser och söka efter mottagare av ett korrektur.

[!DNL Workfront Proof]-kopplingen räknar inte med antalet aktiva appar som är tillgängliga för din organisation. Alla scenarier, även om de bara använder appen [!DNL Workfront Proof], räknas mot din organisations totala antal scenarier.

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
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
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

## Anslut [!DNL Workfront Proof] till [!DNL Workfront Fusion]

Du kan skapa en anslutning till ditt [!DNL Workfront Proof]-konto direkt inifrån en [!DNL Workfront Fusion]-modul.

1. Klicka på [!UICONTROL **Lägg till**] bredvid fältet [!UICONTROL Connection] i en [!DNL Workfront Fusion]-modul

2. Fyll i följande fält:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Ange ett namn för anslutningen</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Ange om det är en produktionsmiljö eller en icke-produktionsmiljö som Förhandsgranska eller Sandbox.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Ange om det här är ett tjänstkonto eller ett personligt konto.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Email / Username]</td>
                <td>Ange användarnamn för ditt [!DNL Workfront Proof]-konto.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Password]</td>
                <td>Ange lösenordet för ditt [!DNL Workfront Proof]-konto.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant ID]</td>
                <td><strong>Obs!</strong> Kunder som inte använder BYOK måste lämna det här fältet tomt. <p>Ange klientorganisations-ID för det här kontot. Kontakta Workfront kundsupport om du behöver hjälp med att hitta ditt klient-ID.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain Extension]</td>
                <td>Ange tillägget för den URL som du använder för att komma åt ditt konto. <p>Exempel: <code>com</code> eller <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Production, Preview, or Custom Environment]</td>
                <td>Välj en anslutning till en produktion, förhandsgranskning eller en anpassad miljö.</td>
            </tr>
        </tbody>
    </table>


3. Klicka på [!UICONTROL **Fortsätt**] för att spara anslutningen och återgå till modulen

## [!DNL Workfront Proof]-moduler och deras fält

När du konfigurerar [!DNL Workfront Proof] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL Workfront Proof] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

* [Titta på korrektur](#watch-proofs)
* [Se PDF i korthet](#watch-for-pdf-summary)
* [[!UICONTROL Watch Proof Activity]](#watch-proof-activity)

#### [!UICONTROL Watch Proofs]

Denna schemalagda utlösarmodul verkställer ett scenario när någon skapar eller fattar ett beslut om ett bevis.

Modulen returnerar en lista över alla poster som hittas under den period du anger, tillsammans med deras typer. Den returnerar även värdena för de fält som du anger. Om modulen hittade beslut som fattats på korrekturet, innehåller den både det föregående och det aktuella värdet i separata fält. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Detta sker regelbundet enligt ett schema som du anger.

Du måste ha tillräcklig behörighet för att komma åt korrektur eller korrektur i [!DNL Workfront Proof] för att kunna hämta den här informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Posttyp</td> 
   <td>Välj den typ av [!DNL Workfront Proof]-post som du vill att modulen ska bevaka.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Utdata</td> 
   <td> <p>Välj den information som du vill inkludera i utdatapaketet för den här modulen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Gräns</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch for PDF Summary]

Den här snabbutlösarmodulen kör ett scenario när någon skapar en PDF-sammanfattning för ett korrektur.

En webkrok krävs i den här modulen.

Modulen returnerar alla standardfält som är associerade med korrekturet, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Den skapar också en ny händelseprenumeration för PDF-sammanfattningar och matar ut innehållet från det pdf_url-attribut som skickas i nyttolasten. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Du kan välja en befintlig webbkrok eller skapa en ny. Mer information finns i <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Proof Activity]

Den här utlösarmodulen kör ett scenario när en angiven aktivitet inträffar på ett korrekturbevis.

Modulen returnerar alla standardfält som är associerade med korrekturet, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Den skapar också en ny händelseprenumeration för PDF-sammanfattningar och matar ut innehållet från attributet `pdf_url` som skickas i nyttolasten. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activity type]</td> 
   <td>Välj om du bara vill se ett nytt beslut (inklusive [!UICONTROL proof] statusändringar) eller om den övergripande korrekturstatusen ska ändras.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [[!UICONTROL Create Proof]](#create-proof)
* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Download Proof]](#download-proof)
* [[!UICONTROL Read a Record]](#read-a-record)
* [[!UICONTROL Request PDF Summary]](#request-pdf-summary)
* [[!UICONTROL Update Proof]](#update-proof)
* [[!UICONTROL Upload File]](#upload-file)

#### [!UICONTROL Create Proof]

Denna åtgärdsmodul skapar ett nytt korrektur eller en ny version av ett korrektur i [!DNL Workfront Proof].

Du anger parametrarna för det nya korrekturet och källkorrekturet om du skapar en ny version.

Modulen returnerar ID:t för den nya korrektur- eller korrekturversionen. Du kan mappa informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Type]</td> 
   <td> <p>Ange om du vill att det skapade korrekturet ska ha ett grundläggande arbetsflöde eller en [!UICONTROL Automated Workflow].</p> <p>Fyll sedan i fälten som visas som korrekturtyp. Om du till exempel väljer [!UICONTROL Automated Workflow] fyller du i fältet <strong>[!UICONTROL Workflow Stages]</strong> för att konfigurera faserna.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Allow original file to be downloaded]</td> 
   <td>Välj om du vill tillåta att originalfilen som korrekturet skapades från hämtas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Ange om du använder det klassiska korrekturläsaren.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combine all files into single proof]</td> 
   <td>Aktivera det här alternativet om du vill kombinera alla filer till ett enda flersidigt korrektur.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create a new proof version]</td> 
   <td>Välj det här alternativet om du vill att modulen ska skapa en ny version av ett befintligt korrektur. Mappa eller ange ett unikt ID för korrekturet i fältet <strong>[!UICONTROL Existing Proof ID]</strong> som visas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link Label]</td> 
   <td>Ange eller mappa en etikett för den anpassade korrekturlänken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link URL]</td> 
   <td>Ange eller mappa URL:en för den anpassade länken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Ange ett av följande nummer för att ange vilka av följande standardinställningar för e-postmeddelanden som du vill använda för korrekturet som skapas.
    <ul>
     <li><strong>1</strong> - Alla nya kommentarer och svar</li>
     <li><strong>2</strong> - Besvarar mina kommentarer</li>
     <li><strong>3</strong> - Daglig sammanfattning</li>
     <li><strong>4</strong> - Sammanfattning varje timme</li>
     <li><strong>5</strong> - Endast beslut</li>
     <li><strong>9</strong> - Inaktiverad</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Excel Summary]</td> 
   <td>Välj om du vill inaktivera möjligheten att hämta korrekturkommentarer till en Excel-fil.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable PDF Summary]</td> 
   <td>Ange om du vill inaktivera möjligheten att hämta korrekturkommentarer till en PDF-fil.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Välj om du vill inaktivera e-postprenumerationen för det här korrekturet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Embed Player]</td> 
   <td>Välj om du vill aktivera den inbäddade spelaren för det här korrekturet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Välj om personer som inte är deltagare ska kunna prenumerera på beviset.<br>Om du väljer det här alternativet kan du även välja standardroll för prenumeranter, vilket beskrivs i den här tabellen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Välj om du vill aktivera e-postvalidering av prenumeration. Om detta är aktiverat måste prenumeranten klicka på en länk i ett e-postmeddelande för att få tillgång till ett korrektur.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Välj om du vill att det skapade beviset ska dölja eller visa team-URL:en.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">eller</span> [!UICONTROL File Hashes]</td> 
   <td>Lägg till ID:t för filen eller filerna som du vill skapa ett korrektur eller korrektur från.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Names]</td> 
   <td>Lägg till filnamnet eller namnen för korrekturet som skapas Detta är ett obligatoriskt fält.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Ange om du vill att det skapade korrekturet ska låsas när alla nödvändiga beslut har fattats.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notify recipients about this proof]</td> 
   <td>Välj ett alternativ som anger om du vill att mottagarna ska meddelas när korrekturet skapas.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof name]</td> 
   <td>Ange ett namn för korrekturet som skapas Detta är ett obligatoriskt fält. Använd en vertikalstreckssymbol (|) för att skilja namn på flera korrektur.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof owner ID]</td> 
   <td>Ange eller mappa ID:t för korrekturägaren. Om fältet lämnas tomt ställs korrekturägaren in på den aktuella användaren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference ID]</td> 
   <td>Ange referens-ID för korrekturet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require electronic signature]</td> 
   <td>Välj om du vill att en person som fattar ett beslut om ett bevis ska skicka en elektronisk signatur.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Ange om du vill att det skapade korrekturet ska kräva inloggning. </p> <p>Detta är samma som inställningen [!UICONTROL Login Required] som förklaras i <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] i [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>Ange ID:t för den upplösning som du vill använda för ditt korrektur. En lista med matchnings-ID:n finns i [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API-dokumentationen</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Ange typen av SWF-korrektur.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [objekt]</td> 
   <td>För varje objekt väljer du om du vill visa det i korrekturet.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Ange ID:t för den arbetsyta som du vill skapa korrekturet i. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recipients]</td> 
   <td>Lägg till e-postadresserna till de mottagare som du vill ha för korrekturet som skapas.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Ange den deadline du vill ha för korrekturet som skapas. Använd följande datumformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till API:t [!DNL Workfront Proof]. På så sätt kan du skapa en dataflödesautomatisering som inte kan utföras av de andra [!DNL Workfront Proof]-modulerna.

Modulen returnerar statuskod, rubriker och brödtext. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Method]</td> 
   <td>Ange åtgärden för API-anropet. Information om tillgängliga åtgärder finns i <a href="https://api.proofhq.com/">dokumentationen för korrektur-API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Download Proof]

Den här åtgärdsmodulen hämtar källfilen för ett visst bevis som du identifierar med dess ID.

Du anger korrekturens ID.

Modulen returnerar innehållet i källfilen som användes för att skapa korrekturet.Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du måste ha behörighet att komma åt posten i [!DNL Workfront Proof] för att kunna hämta informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Skriv det unika ID:t för beviset som finns på sidan [!UICONTROL Proof Details]. Mer information finns i <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Hantera korrekturinformation i [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a Record]

Den här åtgärdsmodulen läser data från ett enda korrektur i [!DNL Workfront Proof].

Du anger korrekturets ID och den information du vill ha från korrekturet.

Modulen returnerar värdena för fälten som du väljer för korrekturet, tillsammans med deras typer. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du måste ha behörighet att komma åt posten i [!DNL Workfront Proof] för att kunna hämta informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Välj om du vill läsa korrektur, korrekturkommentarer eller korrekturgranskare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Välj den information som du vill inkludera i utdatapaketet för den här modulen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Ange eller mappa det unika [!DNL Workfront Proof]-ID:t för posten som du vill att modulen ska läsa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Request PDF Summary]

Den här åtgärdsmodulen begär sammanfattningen PDF för ett visst korrektur i [!DNL Workfront Proof].

Du anger korrekturens ID.

Modulen returnerar sammanfattningsinformation för PDF. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du måste ha behörighet att komma åt posten i [!DNL Workfront Proof] för att kunna hämta informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Ange det unika [!DNL Workfront Proof]-ID:t för det korrektur som du vill begära en sammanfattning för PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Ange eller mappa URL:en dit du vill att sammanfattningen för PDF ska skickas.</td> 
  </tr> 
 </tbody> 
</table>

##### Möjligt fel

* **Fel**: [!UICONTROL You do not have privilege to perform this request. The stage must contain at least one recipient.]
* **Lösning**: Kontrollera att du inte är den enda som tilldelats till stegen i arbetsflödet. En annan användare måste vara tilldelad till stegen i arbetsflödet.

#### [!UICONTROL Update Proof]

Denna åtgärdsmodul uppdaterar ett befintligt korrektur i [!DNL Workfront Proof].

Du anger korrekturets ID och posttyp samt vilka fält som ska inkluderas i utdata.

Modulen returnerar alla standardfält som är associerade med posten, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du måste ha behörighet att komma åt posten i [!DNL Workfront Proof] för att kunna hämta informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Skriv det unika ID:t för beviset som finns på sidan [!UICONTROL Proof Details]. Mer information finns i <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Hantera korrekturinformation i [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Ange den deadline du vill ha för korrekturet som skapas. Använd följande datumformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Välj vilken av följande standardinställningar för e-postmeddelanden som du vill använda för korrekturet som skapas.
    <ul>
     <li> [!UICONTROL All new comments and replies]</li>
     <li>[!UICONTROL Replies to my comments]</li>
     <li>[!UICONTROL Daily summary]</li>
     <li> [!UICONTROL Hourly summary]</li>
     <li> [!UICONTROL Decisions only]</li>
     <li> [!UICONTROL Disabled]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default Role]</td> 
   <td>Välj standardroll för korrekturet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Välj om du vill inaktivera e-postprenumerationen för det här korrekturet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Välj om personer som inte är deltagare ska kunna prenumerera på beviset.<br>Om du väljer det här alternativet kan du även välja [!UICONTROL Default Role] för prenumeranter, vilket beskrivs i den här tabellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Välj om du vill aktivera e-postvalidering av prenumeration. Om detta är aktiverat måste prenumeranten klicka på en länk i ett e-postmeddelande för att få tillgång till ett korrektur.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Välj om du vill att det skapade beviset ska dölja eller visa team-URL:en.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Ange om du vill att det skapade korrekturet ska låsas när alla nödvändiga beslut har fattats.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>Skriv eller mappa ett meddelande som du vill bifoga korrekturet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID] </td> 
   <td>Ange eller mappa ID:t för det korrektur som du vill uppdatera.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td>Ange eller mappa namnet på det korrektur som du vill uppdatera.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Ange om du vill att det skapade korrekturet ska kräva inloggning. </p> <p>Detta är samma som inställningen [!UICONTROL Login Required] som förklaras i <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] i [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show Versions Like]</td> 
   <td>Välj om du vill visa en länk till andra versioner av det här korrekturet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Ange eller mappa korrekturens ämne</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload File]

Den här åtgärdsmodulen överför en fil för användning med modulen [!UICONTROL Create Proof] i [!DNL Workfront Proof].

Modulen returnerar ett hash-ID för den överförda filen. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

* [[!UICONTROL List Workflow Templates]](#list-workflow-templates)
* [[!UICONTROL Search]](#search)

#### [!UICONTROL List Workflow Templates]

I den här sökmodulen visas alla tillgängliga arbetsflödesmallar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Välj den information som du vill inkludera i utdatapaketet för den här modulen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet mallar som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search]

Den här sökmodulen söker efter poster i ett objekt i [!DNL Workfront Proof] som matchar den sökfråga du anger.

Modulen returnerar korrekturets ID om den söker efter ett korrektur. Eller returnerar mottagarens användar-ID, e-post, namn, befattningar och e-postalias om den söker efter mottagare. Du kan mappa den här informationen i efterföljande moduler i scenariot.

Du måste ha behörighet att komma åt posten i [!DNL Workfront Proof] för att kunna hämta informationen.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Workfront Proof]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sök efter</td> 
   <td> <p>Se[!UICONTROL ]Välj den typ av post som du vill att modulen ska söka efter.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Ange korrekturnamnet för det korrektur som du vill söka efter.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Ange e-postadressen till mottagaren som du vill söka efter.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Ange om modulen ska söka efter <strong>[!UICONTROL All Matching Records]</strong> eller bara <strong>[!UICONTROL First Matching Record]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort By]</td> 
   <td>Markera det fält som du vill sortera resultaten efter.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sorting Direction]</td> 
   <td> <p>Välj om du vill sortera resultaten stigande eller fallande.</p> </td> 
  </tr> 
 </tbody> 
</table>
