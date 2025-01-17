---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Power BI-moduler
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 0%

---

# [!DNL Power BI] moduler

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Power BI-moduler](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/powerbi-modules.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

[!DNL Power BI] är ett program som gör att du kan visualisera och presentera data för dina intressenter. Den kan hämta data från en mängd olika källor.

>[!NOTE]
>
>[!DNL Workfront Fusion] är inte en datakälla. Även om [!DNL Workfront Fusion] kan skapa och använda datakällor lagras inte dina data.


## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
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

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Microsoft Power BI API-information

Microsoft Power BI-kontakten använder följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bas-URL</td> 
   <td> https://api.powerbi.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tagg</td> 
   <td>v1.0.2</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Power BI]-moduler och deras fält

När du konfigurerar [!DNL Power BI] visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En fetstilt titel i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kontrollpaneler](#dashboards)
* [Rapporter](#reports)
* [Datauppsättning](#dataset)
* [Appar](#apps)
* [Övriga](#other)

### Kontrollpaneler

* [Skapa en instrumentpanel](#create-a-dashboard)
* [Skaffa en instrumentpanel](#get-a-dashboard)
* [Skaffa en instrumentpanel](#get-a-dashboard-tile)
* [Visa panelpaneler](#list-dashboard-tiles)
* [Listinstrumentpaneler](#list-dashboards)

#### [!UICONTROL Create a Dashboard]

Den här åtgärdsmodulen skapar en ny kontrollpanel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Ange eller mappa ett namn för instrumentpanelen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för den grupp som ska äga den nya instrumentpanelen.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dashboard]

Den här åtgärdsmodulen hämtar metadata för en angiven instrumentpanel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Välj eller mappa alternativet för att välja den instrumentpanel som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Ange eller mappa ID:t för den kontrollpanel som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger kontrollpanelerna som du vill hämta metadata för.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dashboard Tile]

Den här åtgärdsmodulen hämtar metadata för en angiven instrumentpanelspanel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Välj eller mappa alternativet för att välja den instrumentpanelsinformation som du vill hämta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Ange eller mappa ID:t för den instrumentpanel som du vill hämta information för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Ange eller mappa ID:t för den [!DNL Power BI]-panel som du vill hämta information för.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger den platta som du vill hämta.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Dashboard Tiles]

Den här sökmodulen hämtar en lista med instrumentpanelsrutor.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
    <td>
      <p>Välj eller mappa alternativet för att välja den instrumentpanel vars rutor du vill visa.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Ange eller mappa ID:t för den instrumentpanel som innehåller de rutor som du vill visa.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Markera eller mappa ID:t för gruppen som äger kontrollpanelerna som innehåller de paneler som du vill visa.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL List Dashboards]

Den här sökmodulen hämtar en lista med instrumentpaneler.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Markera eller mappa ID:t för gruppen som äger de instrumentpaneler som du vill visa.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Rapporter

* [Kopiera en rapport](#copy-a-report)
* [Ta bort en rapport](#delete-a-report)
* [Hämta en rapport](#get-a-report)
* [Listrapporter](#list-reports)

#### [!UICONTROL Copy a Report]

Denna åtgärdsmodul kopierar en befintlig rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Välj eller mappa alternativet för att välja den rapport som du vill kopiera.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ange eller mappa ID:t för rapporten som du vill kopiera.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger rapporten som du vill kopiera.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL New Copied Report Name]</td>
      <td>Ange eller mappa ett namn för den nya rapporten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Report]

Den här åtgärdsmodulen tar bort en rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Markera eller mappa alternativet för att välja den rapport som du vill ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ange eller mappa ID:t för rapporten som du vill ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger rapporten som du vill ta bort.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Report]

Den här åtgärdsmodulen hämtar metadata för en angiven rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Välj eller mappa alternativet för att välja den rapport som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ange eller mappa ID:t för rapporten som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger rapporten som du vill hämta metadata för.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Reports]

Den här sökmodulen hämtar en lista med rapporter.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Markera eller mappa ID:t för den grupp som äger de rapporter som du vill visa.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>


### Datauppsättning

* [Lägga till/ta bort rader i en datauppsättningstabell](#add-or-delete-rows-in-a-dataset-table)
* [Skapa en datauppsättning](#create-a-dataset)
* [Ta bort en datauppsättning](#delete-a-dataset)
* [Hämta en datauppsättning](#get-a-dataset)
* [Visa datauppsättningar](#list-datasets)
* [Uppdatera en datauppsättning](#refresh-a-dataset)

#### [!UICONTROL Add or Delete Rows in a Dataset Table]

Den här åtgärdsmodulen lägger till eller tar bort rader i en angiven push-datamängdstabell.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a table]</td>
      <td>Markera eller mappa alternativet för att välja den datauppsättning som innehåller tabellen som du vill justera.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Ange eller mappa ID:t för datauppsättningen som innehåller raderna som du vill lägga till eller ta bort.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Ange eller mappa namnet på den tabell som innehåller raderna som du vill lägga till eller ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Ange eller mappa ID:t för gruppen som äger datauppsättningen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Select the Action]</td>
      <td>
        <p>Markera eller mappa åtgärden som du vill utföra.</p>
        <ul>
          <li>
            <p>[!UICONTROL Add rows]</p>
          </li>
          <li>
            <p>[!UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Lägg till radfälten.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Ange eller mappa nyckelnamnet.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
            </p>
            <p>Markera eller mappa fälttypen:</p>
            <ul>
              <li>
                <p>Boolean</p>
              </li>
              <li>
                <p>Datum</p>
              </li>
              <li>
                <p>Text</p>
              </li>
              <li>
                <p>Nummer</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Value]</p>
            <p>Ange eller mappa nyckelvärdet.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Create a Dataset]

Den här åtgärdsmodulen skapar en ny datauppsättning.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Ange eller mappa ett namn för datauppsättningen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för den grupp som ska äga den nya datauppsättningen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default Mode]</td>
      <td>
        <p>Välj eller mappa datamängdens standardläge:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: En datauppsättning med en direktanslutning till [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: En datauppsättning med en direktanslutning till tjänsten [!DNL On-premise Analysis]</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: En datauppsättning som ger programmatisk åtkomst till data i [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: En datauppsättning som stöder dataströmning och ger programmatisk åtkomst för att skicka data till [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: En datauppsättning som stöder dataströmning</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tables]</td>
      <td>Lägg till tabeller i datauppsättningen. För fält, se <a href="#Table" class="MCXref_0">Tabellfält</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Lägg till datakällorna. Mer information finns i <a href="#Data" class="MCXref_0">Datakällsfält</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Välj eller mappa den avsiktliga principen för datauppsättningen:</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Tabellfält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Ange eller mappa ett namn för tabellen.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>Lägg till kolumnerna:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Ange (mappa) ett kolumnnamn.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Markera eller mappa datatypen:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Ange (mappa) formatsträngen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Ange eller mappa radinformation.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>Lägg till måttet för tabellerna.</td>
    </tr>
  </tbody>
</table>

##### Datakällfält

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
      <td>
        <p>Ange eller mappa den databas som du vill använda.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Ange eller mappa namnet på den server som du vill använda.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Ange eller mappa den URL som du vill använda.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  Ange eller mappa ID:t för datakällan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source Type]  </td>
      <td>
        <p>Markera eller mappa datakälltypen. Exempel: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Ange eller mappa ID:t för den gateway som du vill använda.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Dataset]

Den här åtgärdsmodulen tar bort en datauppsättning.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Markera eller mappa alternativet för att välja den datauppsättning som du vill ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ange eller mappa ID:t för den datauppsättning som du vill ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger den datauppsättning som du vill ta bort.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get a Dataset]

Den här åtgärdsmodulen hämtar metadata för en angiven datauppsättning.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Välj eller mappa alternativet för att välja den rapport som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Ange eller mappa ID:t för den datauppsättning som du vill hämta metadata för.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger den datauppsättning som du vill hämta metadata för.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Datasets]

Sökmodulen hämtar en lista med datauppsättningar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Markera eller mappa ID:t för gruppen som äger rapporten som du vill hämta metadata för.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Ange eller mappa det maximala antalet poster som du vill att modulen ska [åtgärd] under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Refresh a Dataset]

Den här åtgärdsmodulen uppdaterar en angiven datauppsättning.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a dataset]</td>
      <td>Markera eller mappa alternativet för att välja den datauppsättning som du vill uppdatera.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Ange eller mappa ID:t för den datauppsättning som du vill uppdatera.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Ange eller mappa namnet på den tabell som innehåller raderna som du vill lägga till eller ta bort.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Ange eller mappa ID:t för gruppen som äger datauppsättningen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notify Option]  </td>
      <td>
        <p>Välj eller mappa alternativet för att meddela:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL No Notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Appar

* [Skaffa en app](#get-an-app)
* [Skaffa en apps Dashboard](#get-an-apps-dashboard)
* [Hämta en apprapport](#get-an-apps-report)
* [Visa appens instrumentpaneler](#list-apps-dashboards)
* [Visa apprapporter](#list-apps-reports)
* [Listappar](#list-apps)
* [Bevakade appar](#watch-apps)

#### [!UICONTROL Get an App]

Den här åtgärdsmodulen hämtar metadata för en angiven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Markera eller mappa ID:t för det program du vill hämta.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Dashboard]

Den här åtgärdsmodulen hämtar metadata för ett angivet programs kontrollpanel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Markera eller mappa ID:t för programmet som innehåller den instrumentpanel som du vill hämta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Markera eller mappa ID:t för den kontrollpanel som du vill hämta.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Get an App's Report]

Den här åtgärdsmodulen hämtar metadata för ett angivet programs rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Markera eller mappa ID:t för programmet som innehåller rapporten som du vill hämta.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Markera eller mappa ID:t för rapporten som du vill hämta.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List Apps]

Den här sökmodulen hämtar en lista över alla installerade program.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Dashboards]

Den här sökmodulen hämtar en lista med instrumentpaneler från en angiven app.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Markera eller mappa ID:t för programmet som du vill visa instrumentpaneler från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List App's Reports]

Den här sökmodulen hämtar en lista med alla rapporter från den angivna appen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Markera eller mappa ID:t för det program som du vill visa rapporter från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Watch Apps]

Den här utlösarmodulen startar ett scenario när en app uppdateras.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Övriga

#### [!UICONTROL Make an API Call]

Den här åtgärdsmodulen utför ett API-anrop till API:t [!DNL Power BI].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Power BI]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till Adobe [!DNL Workfront Fusion] - grundläggande instruktioner</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Ange en relativ sökväg till <code>https://api.powerbi.com</code>. Exempel: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>Välj den [!UICONTROL HTTP]-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i [!UICONTROL HTTP]-metoder för begäran.</p>
      </td>
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
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
