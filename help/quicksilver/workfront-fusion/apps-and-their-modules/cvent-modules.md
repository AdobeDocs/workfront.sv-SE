---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Kundmoduler
description: I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder Event, samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# [!DNL Cvent] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Cvent], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Cvent] moduler, du måste ha en [!DNL Cvent] konto.

## Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>The [!DNL Cvent] -moduler fungerar genom [!UICONTROL SOAP] API. Skapa en anslutning till [!DNL Cvent]måste du se till följande:
>
>* Du har [!UICONTROL SOAP] åtkomst till [!DNL Cvent] API.
>* The [!DNL Workfront Fusion] IP-adresser har lagts till i din organisations tillåtelselista.
>
>  För en lista med [!DNL Workfront Fusion] IP-adresser, se [IP-adresser för åtkomst [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


Du kan skapa en anslutning till [!DNL Cvent] direkt inifrån [!DNL Cvent] -modul.

1. I alla [!DNL Cvent] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Markera det område som du vill ansluta till.

   * [!UICONTROL North America]
   * [!UICONTROL Europe]
   * [!UICONTROL Sandbox]

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Cvent] moduler och deras fält

När du konfigurerar [!DNL Cvent] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Cvent] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)
* [Sökningar](#searches)

### Åtgärder

* [[!UICONTROL Custom API Call]](#create-meeting-request)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Register Invitee]](#register-invitee)
* [[!UICONTROL Add Invitee]](#add-invitee)
* [[!UICONTROL Delete Contact]](#delete-contact)
* [[!UICONTROL Update Contact]](#update-contact)
* [[!UICONTROL Create meeting request]](#create-meeting-request)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Cvent] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Cvent] moduler.

När du konfigurerar den här modulen visas följande fält.

Modulen returnerar statuskoden, tillsammans med rubrikerna och brödtexten för API-anropet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtgärd</td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Brödtext (XML)</td> 
   <td> <p>Ange eller mappa innehållet i API-anropet. Detta får endast innehålla XML. Modulen kommer automatiskt att innehålla autentiseringshuvuden. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Den här åtgärdsmodulen läser information om en viss post.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td>Välj objekttypen för den post som du vill läsa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Ange eller mappa ID:t för objektet som du vill läsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Markera de fält som du vill inkludera i modulens utdata. Fälten är tillgängliga beroende på vilken objekttyp du har valt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Register Invitee]

Den här åtgärdsmodulen registrerar en inbjudan för en händelse.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Inbjudan-ID</p> </td> 
   <td> <p>Ange eller mappa ID:t för den inbjudne som du vill registrera för en händelse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Händelse-ID</td> 
   <td> <p>Ange eller mappa ID:t för händelsen som du vill registrera den inbjudne för.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Invitee]

Den här åtgärdsmodulen bjuder in en kontakt till en händelse.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för kontakten som du vill lägga till i en händelse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Ange eller mappa ID:t för händelsen som du vill lägga till kontakten i.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Contact]

Den här åtgärdsmodulen tar bort en enskild kontakt i Event.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
   <td> <p>Ange eller mappa ID:t för den kontakt du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update Contact]

Den här åtgärdsmodulen uppdaterar en befintlig kontakt med dess ID.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för den kontakt du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Markera de fält som du vill ange information för och fyll sedan i önskade värden för dessa fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> <p>Markera de fält som du vill ange information för och fyll sedan i önskade värden för dessa fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create meeting request]

Den här åtgärdsmodulen lägger till en mötesförfrågan till ditt konto.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för det formulär som du vill använda för att skapa den nya mötesförfrågan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting Request Fields]</td> 
   <td> <p>Markera de mötesförfrågningsfält som du vill ange information för och fyll sedan i önskade värden för dessa fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>Markera de fält för händelsebegäran som du vill ange information för och fyll sedan i önskade värden för dessa fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Välj begäran om förslagsfält som du vill ange information för och fyll sedan i önskade värden för dessa fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

#### [!UICONTROL List records]

Den här sökmodulen hämtar information om alla poster av en viss typ.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Cvent] konto till [!DNL Workfront Fusion], se <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Anslut [!DNL Cvent] till [!DNL Adobe Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td> <p>Välj den typ av post som du vill visa.</p> 
    <ul> 
     <li> <p>Alla evenemang från [!DNL Cvent] konto</p> </li> 
     <li> <p>Alla sessioner för en händelse</p> </li> 
     <li> <p>Alla inbjudna till en händelse</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Om du listar inbjudna eller sessioner anger eller mappar du ID:t för händelsen som de inbjudna eller sessionerna är kopplade till.</p> </td> 
  </tr> 
 </tbody> 
</table>
