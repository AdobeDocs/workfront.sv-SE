---
title: HubSpot CRM-moduler
description: The [!DNL Adobe Workfront Fusion] Med HUBspot CRM-modulerna kan du övervaka händelser, poster, kontakter, ärenden, fil- och formuläröverföringar eller skapa, hämta, uppdatera och ta bort poster, kontakter, ärenden, händelser eller filer i dina [!DNL HubSpot CRM] konto.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2049'
ht-degree: 0%

---

# [!DNL HubSpot CRM] moduler

The [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] Med -moduler kan du övervaka händelser, poster, kontakter, ärenden, fil- och formuläröverföringar eller skapa, hämta, uppdatera och ta bort poster, kontakter, ärenden, händelser eller filer i dina [!DNL HubSpot CRM] konto.

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

Används [!DNL HubSpot CRM] moduler, du måste ha en [!DNL HubSpot CRM] konto.

## Anslut [!DNL Adobe Workfront Fusion] till [!DNL HubSpot CRM]

Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se [Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] moduler och deras fält

När du konfigurerar [!DNL Hubspot CRM] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Hubspot CRM] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM-objekt](#crm-objects)
* [Register (avtal, kontakter och företag)](#records-deals-contacts-and-companies)
* [Kontakter](#contacts)
* [Erbjudanden](#deals)
* [Företag](#companies)
* [Filer](#files)
* [Biljetter](#tickets)
* [Göra ett API-anrop](#make-an-api-call)

### CRM-objekt

#### [!UICONTROL Search for CRM Objects]

Den här sökmodulen söker efter CRM-objekt efter anpassade egenskaper eller efter fråga. Om du vill söka efter produkter eller radobjekt använder du en speciell anslutning med ett nödvändigt anpassat omfång.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antalet objekt som modulen ska returnera i en körningscykel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type to Search]</td> 
   <td>Välj den typ av Hubspot CRM-objekt som du vill söka efter.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Markera de egenskaper som du vill ska visas i modulens utdata. Vilka fält som är tillgängliga beror på vilket objekt du har valt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by] </td> 
   <td> <p>Välj hur du vill filtrera sökningen</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Ange eller mappa frågan</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Ange grupper eller filter för sökningen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Klicka om du vill sortera resultaten. Om du väljer att sortera resultaten visas följande fält. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Property name]</strong> </p> <p>Välj den egenskap som du vill sortera resultaten efter</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Välj om du vill sortera resultaten i stigande eller fallande riktning.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Register (avtal, kontakter och företag)

* [[!UICONTROL Create a Record (Legacy)]](#create-a-record-legacy)
* [[!UICONTROL Get a Record]](#get-a-record)
* [[!UICONTROL Update a Record]](#update-a-record)
* [[!UICONTROL Delete a Record]](#delete-a-record)
* [[!UICONTROL Get a Record Property]](#get-a-record-property)
* [[!UICONTROL Watch Records]](#watch-records)

#### [!UICONTROL Create a Record (Legacy)]

Den här åtgärdsmodulen skapar kontakt, ett företag eller ett avtal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Välj den typ av post som du vill skapa</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fyll i alla egenskaper som du vill ange för posten. Vilka fält som är tillgängliga beror på vilken typ av post du vill skapa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record]

Den här åtgärdsmodulen hämtar information om en kontakt, ett företag eller ett avtal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Välj posttyp.</p> 
    <ul> 
     <li>[!UICONTROL Contact]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>Om du får en kontakt väljer du om du vill identifiera den med ID eller via e-postadress.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för den kontakt, det företag eller det avtal som du vill hämta. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Ange e-postadressen till den kontakt vars information du vill hämta. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Record]

Den här åtgärdsmodulen uppdaterar en kontakt, ett företag eller ett avtal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Välj den typ av post som du vill uppdatera.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>Om du får en kontakt väljer du hur du vill identifiera posten:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för den kontakt, det företag eller det avtal som du vill uppdatera. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Ange e-postadressen till den kontakt vars information du vill uppdatera. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fyll i alla egenskaper som du vill ange för posten. Vilka fält som är tillgängliga beror på vilken typ av post du vill skapa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Record]

Den här åtgärdsmodulen tar bort en kontakt, ett företag eller ett avtal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Välj den typ av post som du vill ta bort.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för den kontakt, det företag eller det avtal som du vill ta bort. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Record Property]

Den här åtgärdsmodulen hämtar metadata för en viss postegenskap med dess (interna) namn.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Välj den typ av post som har den egenskap som du vill hämta metadata för.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property Name]</td> 
   <td>Välj den egenskap som du vill hämta metadata för.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Vissa egenskaper har en uppsättning tillgängliga alternativ som en användare kan välja som egenskapsvärde. Ange ID:t för alternativet som representerar egenskapsvärdet som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Records]

Den här utlösarmodulen startar ett scenario när en kontakt, ett företag eller ett avtal har ändrats eller skapats under de senaste 30 dagarna. Utdata är begränsade till 10 000 poster.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Välj den typ av post som har den egenskap som du vill bevaka.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Välj om du vill se nyligen ändrade eller nyligen skapade poster.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Välj de egenskaper som du vill inkludera i modulens utdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kontakter

* [[!UICONTROL Create/Update a Contact (Legacy)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Create/Update a Group of Contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Add Contacts to a List]](#add-contacts-to-a-list)
* [[!UICONTROL Remove a Contact from a List]](#remove-a-contact-from-a-list)
* [[!UICONTROL Merge contacts]](#merge-contacts)
* [[!UICONTROL Search for Contacts]](#search-for-contacts)
* [[!UICONTROL List Contacts]](#list-contacts)
* [[!UICONTROL List Contacts of a Company]](#list-contacts-of-a-company)

#### [!UICONTROL Create/Update a Contact (Legacy)]

Skapar en kontakt om den inte redan finns i en portal, eller uppdaterar den med de senaste egenskapsvärdena om den finns i en portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Fyll i de egenskaper som du vill ange eller uppdatera för kontakten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Group of Contacts]

Skapar en grupp kontakter eller uppdaterar dem om de redan finns. Prestanda är bäst när gruppstorleken är begränsad till 100 kontakter eller färre. Ändringar som görs via den här slutpunkten bearbetas asynkront, så det kan ta flera minuter innan ändringar tillämpas på kontaktposter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch of Contacts to Create/Update] </td> 
   <td> <p>Lägg till gruppen med kontakter.</p> <p>Klicka <strong>[!UICONTROL Add item]</strong> för att lägga till en ny kontakt. I fönstret som visas anger eller mappar du följande information:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Välj hur du vill identifiera kontakten:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Ange ID:t för den kontakt som du vill skapa eller uppdatera. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Ange e-postadressen till den kontakt som du vill skapa eller uppdatera. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Fyll i alla egenskaper som du vill ställa in eller uppdatera för kontakten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Contacts to a List]

Den här modulen lägger till kontaktposter som redan har skapats i systemet i en kontaktlista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Markera ID:t för listan som du vill lägga till kontakten i. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>Välj hur du vill identifiera de kontakter som du vill lägga till i listan:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Lägg till ID:n för de kontakter som du vill lägga till i listan.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Lägg till e-postadresserna till kontakterna som du vill lägga till i listan.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove a Contact from a List]

Tar bort en kontakt från en kontaktlista.

>[!NOTE]
>
>Du kan inte ta bort kontakter manuellt från en dynamisk lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Markera ID:t för listan som du vill ta bort kontakten från. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>Ange ID:t för den kontakt du vill ta bort från listan. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Merge contacts]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Ange ID:t för den av kontakterna som du vill sammanfoga. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Ange ID:t för den andra kontakten som du vill sammanfoga.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search for Contacts]

Hämtar en lista med kontakter som använder sökfrågan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Ange sökfrågan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Ange eller mappa maximalt antal kontakter [!DNL Workfront Fusion] ska returneras under en körningscykel. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Contacts]

Returnerar alla kontakter som har skapats i portalen. Utdata är begränsat till 5 000 kontakter. Om du vill visa tidigare eller kommande kontakter kan du använda [!UICONTROL advanced] -parameter som ska förskjutas listan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Högsta antal kontakter [!DNL Workfront Fusion] ska returneras under en körningscykel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Markera de egenskaper som du vill ska visas i modulens utdata. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL List Contacts of a Company]

Hämtar en lista med kontakter i företaget. Utdata är begränsat till 5 000 kontakter. Om du vill visa tidigare eller kommande kontakter kan du använda [!UICONTROL advanced] -parameter som ska förskjutas listan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för det företag vars kontakter du vill visa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Högsta antal kontakter [!DNL Workfront Fusion] ska returneras under en körningscykel. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Watch contacts added to a list]

Den här utlösarmodulen startar ett scenario när en ny kontakt läggs till i en lista. Detta är endast tillgängligt för användare med ett betalt Marketing-konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Ange eller mappa ID:t för listan som innehåller de kontakter som du vill bevaka.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Välj de egenskaper som du vill inkludera i modulens utdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Erbjudanden

* [[!UICONTROL List Deal/Ticket Pipelines]](#list-dealticket-pipelines)
* [[!UICONTROL Get a Deal's CRM Pipeline]](#get-a-deals-crm-pipeline)

#### [!UICONTROL List Deal/Ticket Pipelines]

Returnerar alla erbjudanden och biljettledningar för en viss portal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Välj om du vill visa erbjudanden eller biljetter.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Deal's CRM Pipeline]

Returnerar en specifik avtalspipeline.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline ID] </td> 
   <td>Ange eller mappa ID:t för den pipeline du vill hämta information för. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Ange eller mappa ID:t för den scen som du vill hämta information för. </td> 
  </tr> 
 </tbody> 
</table>

### Företag

#### [!UICONTROL Search for Companies by domain]

Hämtar en lista över företag baserat på en exakt matchning av egenskapen domain.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Ange domänen för de företag du vill söka efter, till exempel <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Högsta antal företag [!DNL Workfront Fusion] ska returneras under en körningscykel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Markera de egenskaper som du vill ska visas i modulens utdata. </td> 
  </tr> 
 </tbody> 
</table>

### Filer

* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Delete a Folder]](#delete-a-folder)
* [[!UICONTROL Move a File]](#move-a-file)

#### [!UICONTROL Create a Folder]

Den här modulen skapar en mapp.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>Ange eller mappa ett namn för den nya mappen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Välj ID för den överordnade mappen för mappen som du skapar. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Folder]

Markerar en mapp som borttagen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för mappen som du vill ta bort.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File]

Flyttar en fil till en annan mapp.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Ange eller mappa ID:t för filen som du vill flytta. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Markera ID:t för mappen där du vill flytta filen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Ange ett namn för den flyttade filen.</td> 
  </tr> 
 </tbody> 
</table>

### Biljetter

#### [!UICONTROL Delete a Ticket]

Tar bort en befintlig biljett med dess ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange ID:t för biljetten som du vill ta bort. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call]

Gör att du kan utföra ett anpassat API-anrop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL HubSpot CRM] konto till [!DNL Workfront Fusion], se <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Ange en relativ sökväg till https://api.hubapi.com/. Till exempel /kontakter/v1/lists/all/contact/all</p> <p>En lista över tillgängliga slutpunkter finns i <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API-dokumentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Välj den HTTP-metod som du vill använda:</p> <p>[!UICONTROL GET]</p> <p>för att hämta information för ett tävlingsbidrag.</p> <p>[!UICONTROL POST]</p> <p>för att skapa ett nytt inlägg.</p> <p>[!UICONTROL PUT]</p> <p>om du vill uppdatera/ersätta en befintlig post.</p> <p>[!UICONTROL PATCH]</p> <p>för att göra en partiell postuppdatering.</p> <p>[!UICONTROL DELETE]</p> <p>om du vill ta bort en post.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Ange önskade begäranderubriker. Du behöver inte lägga till auktoriseringsrubriker; vi gjorde det redan för dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ange frågesträngen för begäran.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödtexten för API-anropet i form av ett standard-JSON-objekt. När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Följande API-anrop returnerar alla kontakter i [!DNL HubSpot] konto:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Metod**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Matchningar av sökningen finns i modulens utdata under [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL contacts].
>
>I vårt exempel returnerades tre kontakter:
>
>![](assets/hubspot-api-output.png)

## Skapa ett nytt program

1. Logga in på [!DNL HubSpot] utvecklarkonto.
1. Välj **[!UICONTROL Create an App]** alternativ.
1. Ange appnamnet och [!UICONTROL Save] dialogrutan.
1. Välj de omfattningar du behöver för din webkrok.

   Du kan till exempel lägga till kontaktomfattningar för att aktivera modulen när en ny kontakt skapas eller tas bort.

   The [!UICONTROL contacts scope] är allt du behöver för att kunna ta emot kontakter, erbjudanden och webbsajter för företagshändelser.

   >[!IMPORTANT]
   >
   >Fyll inte i [!UICONTROL Redirect URL] fält.
