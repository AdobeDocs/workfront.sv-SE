---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud Libraries-moduler
description: Med [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Biblioteksmoduler. Du kan starta ett scenario när ett element eller bibliotek skapas eller uppdateras. Du kan också överföra, hämta, arkivera eller lista element, eller ringa ett samtal till [!DNL Adobe Creative Cloud Libraries] API.
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# Moduler för Adobe Creative Cloud Libraries

Med [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] kan du starta ett scenario när ett element eller bibliotek skapas eller uppdateras. Du kan också överföra, hämta, arkivera eller lista element, eller ringa ett samtal till [!DNL Adobe Creative Cloud Libraries] API.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] eller högre</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
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

## Förutsättningar

Används [!DNL Adobe Creative Cloud Libraries] moduler, du måste ha en [!UICONTROL Adobe Creative Cloud] konto.

## [!UICONTROL Adobe Creative Cloud Libraries] moduler och deras fält

När du konfigurerar [!UICONTROL Adobe Creative Cloud Libraries] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Creative Cloud Libraries] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Element](#elements)

* [Bibliotek](#libraries)

* [Övriga](#other)


### Element

* [[!UICONTROL Archive an Element]](#archive-an-element)

* [[!UICONTROL Get an Element]](#get-an-element)

* [[!UICONTROL List Elements]](#list-elements)

* [[!UICONTROL Upload an Element]](#upload-an-element)

* [!UICONTROL [Se nytt element i bibliotek]](#watch-new-element-in-library)

* [[!UICONTROL Watch Updated Elements]](#watch-updated-elements)


#### [!UICONTROL Archive an Element]

Denna åtgärdsmodul arkiverar ett element från ett bibliotek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Markera det bibliotek som innehåller elementet som du vill arkivera.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Markera elementet som du vill arkivera.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an Element]

Den här åtgärdsmodulen returnerar ett enskilt element från ett bibliotek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Markera det bibliotek som innehåller elementet som du vill hämta.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Ange eller mappa ID:t för elementet som du vill hämta.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Välj den typ av information som modulen returnerar. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Basdata</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alla tillgängliga data</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>En förenklad lista med resurser som är associerade med bibliotekselementet</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Elements]

Den här åtgärdsmodulen hämtar en lista med element i ett bibliotek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Välj det bibliotek som du vill lista element från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>Välj om du vill beställa resultat efter namn eller efter det senaste datum som elementet ändrades.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Ange en MIME-typ för att begränsa resultaten till element som identifieras med den angivna MIME-typen. Exempel: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Välj den typ av information som modulen returnerar. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Basdata</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alla tillgängliga data</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>En förenklad lista med resurser som är associerade med bibliotekselementet</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Upload an Element]

Denna åtgärdsmodul överför en liten filresurs till ett befintligt bibliotek. Största filstorlek är 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Välj det bibliotek som du vill lista element från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>Välj det bearbetningsläge som den här förfrågningsprocessen ska anropas med.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>API-anropet behandlas synkront. Svaret levereras när bearbetningen är slutförd (såvida inte samtalstiderna är slut).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>Svaret på den asynkrona övervakaren returneras omedelbart, och bearbetningen av begäran sker asynkront. Anropet ansvarar för avsökningen av slutpunkten tills det är klart.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Standard)</p>
            <p>Ett försök görs att synkronisera begäran. När bearbetningen sträcker sig över mer än 5 000 ms returneras det asynkrona skärmsvaret. URL:en för övervakaren bör avfrågas tills begäran är slutförd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Ange eller mappa MIME-typen för den överförda filen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch New Element in Library]

Denna utlösarmodul startar ett scenario när ett element läggs till i ett bibliotek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Välj det bibliotek som du vill bevaka för uppdaterade element.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Watch Updated Elements]

Den här utlösarmodulen startar ett scenario när ett element i ett bibliotek uppdateras.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Välj det bibliotek som du vill bevaka för nya element.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>

### Bibliotek

* [[!UICONTROL Watch New Libraries]](#watch-new-libraries)

* [[!UICONTROL Watch Updated Libraries]](#watch-updated-libraries)


#### [!UICONTROL Watch New Libraries]

Den här utlösarmodulen startar ett scenario när ett nytt bibliotek skapas.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch Updated Libraries]

Den här utlösarmodulen startar ett scenario när ett befintligt bibliotek uppdateras.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du ansluter [!DNL Adobe Creative Cloud] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>

### Övriga

#### [!UICONTROL Make an API Call]

Den här modulen gör ett anpassat API-anrop till [!DNL Adobe Creative Cloud Libraries] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt Adobe Creative Cloud-konto till Workfront Fusion finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe Workfront Fusion - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Ange en sökväg i förhållande till <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Exempel <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>Välj version av [!DNL Adobe Analytics] API som du vill ansluta till.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion lägger till auktoriseringsrubrikerna åt dig.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Upload a transient document]</td>
      <td>
      <p>Om du vill överföra ett tillfälligt dokument anger du källfilen för dokumentet som du vill överföra.</p>
      <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p>
    </td>
    </tr>

</tbody>
</table>
