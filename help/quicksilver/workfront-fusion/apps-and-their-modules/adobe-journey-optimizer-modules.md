---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Journey Optimizer], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Moduler

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Journey Optimizer], samt ansluta till flera tredjepartsprogram och -tjänster. [!DNL Adobe Journey Optimizer] kan du skapa, läsa, uppdatera eller ta bort poster, eller utföra ett anpassat API-anrop till [!DNL Adobe Journey Optimizer] API.


Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table>
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

Innan du kan använda [!DNL Adobe Journey Optimizer] måste du se till att följande krav uppfylls:

* Du måste ha en aktiv [!DNL Adobe Journey Optimizer] konto.

## Skapa en anslutning till [!DNL Adobe Journey Optimizer]

Skapa en anslutning för [!DNL Adobe Journey Optimizer] moduler:

1. I alla [!DNL Adobe Journey Optimizer] modul, klicka på **[!UICONTROL Add]** bredvid rutan Anslutning.

1. Fyll i följande fält:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Ange ett namn för anslutningen.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client Secret]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Technical account ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID]</td>
          <td>Ange [!DNL Adobe] [!UICONTROL Organization ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes]</td>
          <td>
            Ange eventuella metaomfång som behövs för anslutningen.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Private key]</td>
          <td>
            <p>Ange den privata nyckel som skapades när dina autentiseringsuppgifter skapades i [!DNL Adobe Developer Console]. </p>
            <p>Så här extraherar du din privata nyckel eller ditt certifikat:</p>
            <ol>
              <li value="1">
                <p>Klicka på <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Välj vilken typ av fil du extraherar.</p>
              </li>
              <li value="3">
                <p>Markera filen som innehåller den privata nyckeln eller certifikatet.</p>
              </li>
              <li value="4">
                <p>Ange lösenordet för filen.</p>
              </li>
              <li value="5">
                <p>Klicka <b>[!UICONTROL Save]</b> för att extrahera filen och återgå till anslutningsinställningarna.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.

## [!DNL Adobe Journey Optimizer] moduler och deras fält

När du konfigurerar [!DNL Adobe Journey Optimizer] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Journey Optimizer] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)
* [Sökningar](#searches)

### Åtgärder

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Update a record]](#update-a-record)

#### [!UICONTROL Create a record]

Den här åtgärdsmodulen skapar ett erbjudande om placering, beslutsregler, tagg, personaliserat erbjudande, samling eller reserverbjudande.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Välj den typ av post som du vill skapa
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Fortsätt till <a href="#placement-fields" >[!UICONTROL Placement] fält</a>.</li>
        <li><b>[!UICONTROL Decision rule]</b>: Fortsätt till <a href="#decision-rule-fields" >[!UICONTROL Decision rule] fält</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: Fortsätt till <a href="#decision-fields" >[!UICONTROL Decision] fält</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: Fortsätt till <a href="#tag-fields" >[!UICONTROL Tag] fält</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: Fortsätt till <a href="#collection-fields" >[!UICONTROL Collection] fält</a>.</li>
        <li><b>[!UICONTROL Fallback offer]</b>: Fortsätt till <a href="#fallback-offer-fields" >[!UICONTROL Fallback offer] fält</a>.</li>
        <li><b>[!UICONTROL Personalized offer]</b>: Fortsätt till <a href="#personalized-offer-fields" >[!UICONTROL Personalized offer] fält</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Placement] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för placeringen.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Ange eller mappa en beskrivning för placeringen.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Decision rule] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för beskrivningsregeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Ange eller mappa en beskrivning för beslutsregeln.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Ange eller mappa villkoret för beslutsregeln.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decision] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för beskrivningsregeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Välj status för beslutet.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Ange eller mappa startdatumet för beslutet.</p><p>En lista över datumformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Ange eller mappa slutdatumet för beslutet.</p><p>En lista över datumformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Placements]</td>
      <td>Välj de placeringar som ska läggas till i det här beslutet
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Välj den erbjudandesamling som innehåller de erbjudanden som det här beslutet gäller.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fallback offer]</td>
      <td>Välj det reserverbjudande som ska presenteras för kunder som inte matchar reglerna för det här beslutet.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för taggen.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Collection] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för samlingen.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filter Type]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Markera de taggar som ska ingå i samlingen.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Fallback offer] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för reserverbjudandet.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Välj status för reserverbjudandet.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Ange eller mappa placeringen för reserverbjudandet.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Personalized offer] fält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Ange eller mappa ett namn för beskrivningsregeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Välj status för beslutet.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Placement</td>
      <td>Välj placering för det personaliserade erbjudandet.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Ange eller mappa startdatumet för det personaliserade erbjudandet.</p><p>En lista över datumformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Ange eller mappa slutdatumet för det personaliserade erbjudandet.</p><p>En lista över datumformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Decision rules]</td>
      <td>Välj de beslutsregler som ska läggas till i det här personliga erbjudandet.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Välj prioritet för erbjudandet. Prioriteten påverkar om detta erbjudande presenteras i stället för ett annat erbjudande.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Capping constraint]</td>
      <td>Ange eller mappa det antal gånger som erbjudandet ska presenteras.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a record]

Den här åtgärdsmodulen tar bort en enstaka post i [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Välj den typ av post som du vill ta bort
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Markera den post som du vill ta bort.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Make a custom API call]

Den här modulen gör ett anpassat API-anrop till [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Ange en sökväg i förhållande till {baseURL} börja med<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion lägger automatiskt till auktoriseringshuvuden och x-api-key-huvuden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Ange frågesträngen för begäran.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange det maximala antal resultat som du vill att modulen ska returnera i en körningscykel.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Record]

Den här åtgärdsmodulen tar bort en enstaka post i [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Välj den typ av post som du vill ta bort
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Markera den post som du vill ta bort.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Update a record]

Den här åtgärdsmodulen skapar ett erbjudande om placering, beslut, beslutsregler, tagg, personaliserat erbjudande, samling eller reserverbjudande.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Välj den typ av post som du vill uppdatera
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Markera den post som du vill uppdatera.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>För varje fält som du vill uppdatera:
      <ol>
      <li>Klicka på <b>[!UICONTROL Add]</b>.</li>
      <li>Välj om du vill lägga till, ersätta eller ta bort värden.</li>
      <li>Ange fältet som du vill uppdatera.</li>
      <li>Ange fältets nya värde.</li>
      </td>
    </tr>

</tbody>
</table>


### Sökningar

#### [!UICONTROL List records]

Den här sökmodulen visar poster av den valda typen och returnerar resultat baserat på villkor som du anger.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Journey Optimizer], se <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Journey Optimizer]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type]</p>
      </td>
      <td>
        <p>Välj den typ av post som du vill visa.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Välj en operator som ska användas på parametrar i frågan</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Om du vill begränsa sökningen till specifika fält anger du fälten. För varje fält som du vill begränsa sökningen till klickar du på [!UICONTROL Add item] och ange fältets namn.</p><p>Banuttryck är i form av punktavgränsade banor som <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>Ange eller mappa den egenskap som du vill beställa resultat med.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order direction]</td>
   <td>Välj om du vill sortera resultaten i stigande eller fallande riktning.
    </td>
     </tr>
  </tbody>
</table>
