---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] kan du skapa, läsa, uppdatera eller ta bort poster, lista alla poster av en viss typ, söka efter poster baserat på villkor som du anger eller utföra ett anpassat API-anrop till [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 43bd30c2db6219cd4e68380c1d9c0d1421f51592
workflow-type: tm+mt
source-wordcount: '1899'
ht-degree: 0%

---

# [!DNL Adobe Target] Moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Adobe Target], samt ansluta till flera tredjepartsprogram och -tjänster. [!DNL Adobe Target] kan du använda för att skapa, skapa, läsa, uppdatera eller ta bort poster, lista alla poster av en viss typ, söka efter poster baserat på villkor som du anger eller utföra ett anpassat API-anrop till [!DNL Adobe Target] API.


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
    </tr>
  </tbody>
</table>


Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Innan du kan använda [!DNL Adobe Target] måste du se till att följande krav uppfylls:

* Du måste ha en aktiv [!DNL Adobe Target] konto.

## Skapa en anslutning till [!DNL Adobe Target]

>[!IMPORTANT]
>
>Anslutningar som skapas efter den 3 juni 2024 kräver en Adobe Target Server-till-server-anslutning.
>
>* Befintliga anslutningar till tjänstkonton fortsätter att fungera till januari 2025. Du måste ersätta dina tjänstkontoanslutningar med Adobe Target Server-till-server-anslutningar senast i januari 2024.
>* Du måste vara utvecklare för att din organisation ska kunna skapa en Adobe Target Server-till-server-anslutning. Utvecklarrollen anges i Adobe Admin Console.

Skapa en anslutning för [!DNL Adobe Target] moduler:

1. Klicka **[!UICONTROL Add]** bredvid rutan Anslutning.

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
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>Ange om du skapar en anslutning till ett tjänstkonto eller en anslutning från Adobe Target Server till server.<p><b>VIKTIGT</b>: Anslutningar som skapas efter den 3 juni 2024 kräver en Adobe Target Server-till-server-anslutning. Befintliga anslutningar till tjänstkonton fortsätter att fungera till januari 2025. Du måste ersätta dina tjänstkontoanslutningar med Adobe Target Server-till-server-anslutningar senast i januari 2024.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Ange om du ansluter till en produktionsmiljö eller icke-produktionsmiljö.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Ange om du ansluter till ett tjänstkonto eller ett personligt konto.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Ange [!DNL Adobe] Klient-ID. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Ange [!DNL Adobe] Klienthemlighet. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Ange [!DNL Adobe] ID för tekniskt konto. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Ange [!DNL Adobe] Organisations-ID. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Logga in på [!DNL Adobe Experience Cloud], öppna [!DNL Target]och klickar på [!DNL Target] kort. Använd det klient-ID som anges i URL-underdomänen.</p>
          <p>Om din URL-adress till exempel är inloggad på [!DNL Adobe Target] är <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> blir ditt klient-ID"mincompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Retur <code>ent_marketing_sdk</code>       </td>
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

## [!DNL Adobe Target] moduler och deras fält

När du konfigurerar [!DNL Adobe Target] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Target] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)

* [Sökningar](#searches)


### Åtgärder

* [[!UICONTROL Create a record]](#create-a-record)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)

* [[!UICONTROL Delete a record]](#delete-a-record)

* [[!UICONTROL Read a record]](#read-a-record)

* [[!UICONTROL Update a record]](#update-a-record)


#### [!UICONTROL Create a record]

Denna åtgärdsmodul skapar en AB- eller XT-aktivitet, ett erbjudande eller en målgrupp.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>
      <p>Välj den typ av post som du vill skapa.</p>
      <ul>
        <li>
        <b>Egenskap</b><p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Properties/operation/createProperty">Skapa en egenskap</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
        <b>Erbjudanderekommendation</b><p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Offers/operation/createOffer">Skapa ett nytt rabatterbjudande</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
          <b>[!UICONTROL Offer JSON]</b>
          <p>Fortsätt till <a href="#offer-fields" class="MCXref xref" >Erbjudandefält</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL Offer Content]</b>
          <p>Fortsätt till <a href="#offer-fields" class="MCXref xref" >Erbjudandefält</a>.</p>
        </li>
        <li>
        <b>Miljö</b><p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Environments/operation/createEnvironment">Skapa miljö</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
          <b>[!UICONTROL Audience]</b>
          <p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Audiences/operation/createAudience_1_1">Skapa målgrupper</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
          <b>[!UICONTROL AB Activity]</b>
          <p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Skapa AB-aktivitet</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
          <b>[!UICONTROL XT Activity]</b>
          <p>Fortsätt till <a href="#xt-activity-fields" class="MCXref xref" >XT Activity fields</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL AP Activity]</b>
          <p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_2">Skapa AP-aktivitet</a> i Adobe Target API-dokumentationen.</p>
        </li>
        <li>
          <b>[!UICONTROL Response Token]</b>
          <p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Response-tokens/operation/createResponseToken">Skapa svarstoken</a> i Adobe Target API-dokumentationen.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

<!--

##### AB Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mboxes]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selectors]</td>
      <td>
        <p>For each selector that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Selector]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience
</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.
</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td><p>For details on metrics, see <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Create AB activity</a> in the Adobe Target API documentation.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

##### XT Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Ange eller mappa ett namn för aktiviteten. Namnet får innehålla högst 250 tecken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>För varje alternativ som du vill lägga till i aktiviteten klickar du på <b>[!UICONTROL Add item]</b> och fylla i följande fält:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Ange eller mappa en sträng som ska användas för att spåra alternativet mellan API-begäranden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Ange eller mappa ett namn för alternativet. Namnet får innehålla högst 250 tecken.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Markera eller mappa erbjudandet som är kopplat till alternativet.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>För varje Mbox som du vill lägga till i aktiviteten klickar du på <b>[!UICONTROL Add item]</b> och fylla i följande fält:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>För varje publik som du vill lägga till i Mbox klickar du på <b>[!UICONTROL Add item]</b> och välj Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Ange eller mappa en sträng som ska användas för att spåra platsen mellan API-begäranden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Ange eller mappa ett namn för platsen. Namnet får innehålla högst 250 tecken.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>En lista över platser på sidan där innehållserbjudandet levereras. En plats innehåller följande:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Ange eller mappa upplevelsens ID</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Ange eller mappa namnet på upplevelsen

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>För varje publik som du vill se upplevelsen klickar du <b>[!UICONTROL Add item]</b> och ange publikens ID.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Ange eller mappa den procentandel besökare som tilldelats upplevelsen</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Ange eller mappa ett ID för att identifiera aktiviteten. Du kan välja detta ID. Detta ID får inte vara samma som en annan aktivitet och får inte vara längre än 250 tecken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Ange eller mappa datum och tid för att starta aktiviteten i formatet <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Ange eller mappa datum och tid för att avsluta aktiviteten i formatet <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Ange eller mappa aktivitetens tillstånd.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Ange ett tal som definierar aktivitetens prioritet. Högre tal har högre prioritet. Värdet måste vara mellan 0 och 999. Standardvärdet är 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Aktivera det här alternativet om du vill allokera trafik automatiskt. Automatisk allokering skickar mer trafik till en mer framgångsrik upplevelse.</p>
        <p>Välj eller mappa utvärderingskriterierna för att bedöma vilken upplevelse som blir mest framgångsrik.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Ange eller mappa arbetsytan som aktiviteten är kopplad till</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>För varje egenskap som du vill lägga till i aktiviteten klickar du på <b>[!UICONTROL Add item]</b> och markera eller mappa egenskapens ID.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>För varje rapportpublik som du vill lägga till i aktiviteten klickar du på [!UICONTROL Add item] och ange följande information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Ange eller mappa en sträng som ska användas för att spåra rapportens målgrupp över API-begäranden.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Ange eller mappa segmentet som ska användas vid rapportering</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Ange eller mappa en sträng som ska användas för att spåra mätvärden över API-begäranden.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Erbjudandefält

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Ange eller mappa ett namn för aktiviteten. Namnet får innehålla högst 250 tecken.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Ange eller mappa innehållet i erbjudandet som ska visas för användaren.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Ange eller mappa ID:t för den arbetsyta som är associerad med erbjudandet. Om inget anges kopplas erbjudandet till kontots standardarbetsyta. Den här funktionen gäller endast för [!DNL Target] Premiumkonton.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Ange eller mappa det datum och den tidpunkt då erbjudandet ändrades.</p>
      </td>
    </tr>
  </tbody>
</table>

<!--

##### Audience fields

>[!NOTE]
>
>Audiences created through Workfront Fusion can only be edit in Fusion or through the API. They cannot be edited from within Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Description]</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Origin]</td>
      <td>
        <p>Select whether this audience's origin is from Target or from the cloud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>[!UICONTROL Add item]</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Example 1:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p>Example 2</p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target Premium] accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

-->

#### [!UICONTROL Make a custom API call]

Den här modulen gör ett anpassat API-anrop till [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Bas-URL]</td>
      <td>Ange eller mappa [!DNL Target] bas-URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Ange en sökväg i förhållande till {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] lägger automatiskt till auktoriseringsrubriker och x-api-key-rubriker.</p>
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
  </tbody>
</table>

#### [!UICONTROL Delete a record]

Den här åtgärdsmodulen tar bort en enstaka AB-aktivitet, XT-aktivitet, erbjudande eller publik.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Välj den typ av post som du vill ta bort.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Ange eller mappa ID:t för den post som du vill ta bort.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Read a record]

Den här åtgärdsmodulen hämtar data för en aktivitet, ett erbjudande, en målgrupp, en egenskap eller en rapport.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Välj den typ av post som du vill läsa.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Ange eller mappa ID:t för den post som du vill läsa.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Update a record]

Den här åtgärdsmodulen uppdaterar en post i Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>
        <p>Välj den typ av post som du vill uppdatera.</p>
       </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Field names]</td>
      <td>Markera de fält som du vill uppdatera. Fälten visas nedan.
          <p>Mer information om fält finns i <a href="https://developer.adobe.com/target/administer/admin-api/">Adobe Target API-dokumentation</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

### Sökningar

* [[!UICONTROL Get records]](#get-records)

* [[!UICONTROL Search]](#search)


#### [!UICONTROL Get records]

Den här sökmodulen hämtar en lista med poster av den valda typen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Välj den typ av post som du vill uppdatera.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sort by]</td>
      <td>För varje fält som du vill sortera efter klickar du på <b>[!UICONTROL Add item]</b> och markerar fältet och om de returnerade resultaten ska vara stigande eller fallande.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts At]</td>
      <td>
        <p>Ange det tidigaste datum som du vill hämta poster för. </p>
        <p>En lista över vilka datum- och tidsformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends At]</td>
      <td>
        <p>Ange det senaste datum som du vill hämta poster för. </p>
        <p>En lista över vilka datum- och tidsformat som stöds finns på <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Search]

Den här sökmodulen söker efter aktiviteter, erbjudanden eller målgrupper baserat på kriterier som du anger.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Target], se <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Target]</a> i den här artikeln.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>Välj den typ av post som du vill uppdatera.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Sort by]</td>
    <td>För varje fält som du vill sortera efter klickar du på <b>[!UICONTROL Add item]</b> och markerar fältet och om de returnerade resultaten ska vara stigande eller fallande.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>För varje regel som du vill ställa in markerar du fältet, operatorn och värdet. Klicka <b>[!UICONTROL Add AND rule]</b> om du vill skapa ytterligare regler.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Ange numret på det första svar som du vill att modulen ska returnera. Det första returnerade svaret har en förskjutning på <code>0</code>. Använd det här fältet tillsammans med [!UICONTROL Maximum number of returned results] för att numrera svaren.</p>
      <p>Om du till exempel vill se den tredje sidan med svar, när varje sida har tio svar, anger du [!UICONTROL Offset] till 20 och [!UICONTROL Maximum number of returned] resultatet blir 10.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]</td>
    <td>
      <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario. Använd det här fältet tillsammans med [!UICONTROL Offset] för att numrera svaren.</p>
      <p>Om du till exempel vill se den tredje sidan med svar, när varje sida har tio svar, anger du [!UICONTROL Offset] till 20 och [!UICONTROL Maximum number of returned] resultatet blir 10.</p>
    </td>
  </tr>
</tbody>
</table>
