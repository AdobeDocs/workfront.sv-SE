---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma-moduler
description: Med  [!DNL Adobe Workfront Fusion] Figma-modulen kan du hämta listor med kommentarer, filer, filversioner eller projekt. Du kan också publicera en kommentar eller ringa ett anrop till Figma API.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# [!DNL Figma] moduler

Med modulerna [!DNL Adobe Workfront Fusion] [!DNL Figma] kan du hämta listor med kommentarer, filer, filversioner eller projekt. Du kan också publicera en kommentar eller ringa ett anrop till [!DNL Figma]-API:t.

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


Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Du måste ha ett [!DNL Figma]-konto för att kunna använda [!DNL Figma]-moduler.

## Information om Figma API

Figma-kopplingen använder följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bas-URL</td> 
   <td> https://api.figma.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-version</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tagg</td> 
   <td>v1.8.25</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Figma]-moduler och deras fält

När du konfigurerar [!DNL Figma] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL Figma] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kommentar](#comments)

* [Projekt och filer](#projects-and-files)

* [Komponenter och format](#components-and-styles)

* [Övriga](#other)


### Kommentar

* [Ta bort en kommentar](#delete-a-comment)

* [Visa kommentarer](#list-comments)

* [Publicera en kommentar](#post-a-comment)


#### [!UICONTROL Delete a comment]

Den här åtgärdsmodulen tar bort en enskild kommentar från en fil.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Ange eller mappa fil-ID:t för filen som du vill lägga till en borttagningskommentar från. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Ange texten för kommentaren som du vill ta bort.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL List comments]

I den här sökmodulen visas alla kommentarer som är kopplade till en enskild fil i [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Ange eller mappa fil-ID:t för filen som du vill hämta kommentarer för. </p>
        <ul>
          <li>
            <p>Om du inte känner till ID:t klickar du på <b>[!UICONTROL Find Files]</b> och anger eller mappar ID:t för projektet som filen är kopplad till. Markera sedan filen.</p>
          </li>
          <li>
            <p>Om du inte känner till projektets ID klickar du på <b>[!UICONTROL Find Projects]</b> och anger eller mappar ID:t för det team som äger projektet som filen är kopplad till. Markera sedan projektet och markera sedan filen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal kommentarer som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Post a comment]

Den här åtgärdsmodulen skickar en kommentar till en Figma-fil.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Ange eller mappa fil-ID:t för filen som du vill skicka en kommentar till. </p>
        <ul>
          <li>
            <p>Om du inte känner till filens ID klickar du på <b>[!UICONTROL Find Files]</b> och anger eller mappar ID:t för projektet som filen är kopplad till. Markera sedan filen.</p>
          </li>
          <li>
            <p>Om du försöker hitta filens ID och inte känner till projektets ID klickar du på <b>[!UICONTROL Find Projects]</b> och anger eller mappar ID:t för det team som äger projektet som filen är associerad med. Markera projektet och markera sedan filen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Ange texten för kommentaren.</td>
    </tr>
  </tbody>
</table>


### Projekt och filer

* [Hämta en fil eller bild](#get-a-file-or-image)

* [Lista filversionshistorik](#list-file-version-history)

* [Visa projektfiler](#list-project-files)

* [Visa projekt](#list-projects)


#### [!UICONTROL Get a file or image]

Den här åtgärdsmodulen hämtar en enda fil eller bild från ett Figma-bibliotek

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>
        <p>Välj den typ av objekt som du vill hämta.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>Modulen returnerar det dokument som refereras av [!UICONTROL Key] som ett JSON-objekt. Filnyckeln kan tolkas från en Figma-fils-URL.</p>
            <p>Mer information finns i <a href="#Get2" class="MCXref xref" >[!UICONTROL Get a file or image: File]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL File nodes]</b>
            </p>
            <p>Returnerar de noder som ID:n refererar till som ett JSON-objekt. Noderna hämtas från filen [!DNL Figma] som [!UICONTROL Key] refererar till.</p>
            <p>Mer information finns i <a href="#Get3" class="MCXref xref" >[!UICONTROL Get a file or image: File nodes]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>Modulen återger bilder från en fil.</p>
            <p>Mer information finns i <a href="#Get4" class="MCXref xref" >[!UICONTROL Get a file or image: Image]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image fills]</b>
            </p>
            <p>Modulen returnerar hämtningslänkar för alla bilder som finns i bildfyllningar i ett dokument. Bildfyllningar är så här [!DNL Figma] representerar eventuella användardefinierade bilder. När du drar en bild till [!DNL Figma] skapar [!DNL Figma] en rektangel med en enda fyllning som representerar bilden, och användaren kan omforma rektangeln (och egenskaperna för fyllningen).</p>
            <p>Mer information finns i <a href="#Get5" class="MCXref xref" >[!UICONTROL Get a file or image: Image fills]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Get a file or image: File]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Markera filen som du vill returnera JSON från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ange eller mappa den version av filen som du vill att modulen ska returnera. Lämna fältet tomt för den aktuella modulen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Om du bara vill returnera en delmängd av dokumentet anger du de noder som du vill att modulen ska returnera. Modulen returnerar noderna i listan, deras underordnade noder och allt som finns mellan rotnoden och noderna i listan.</p>
        <p>För varje nod som du vill returnera klickar du på <b>[!UICONTROL Add]</b> och anger texten för noden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Ange eller mappa ett heltal som representerar hur djupt in i dokumentträdet du vill returnera resultat för. </p>
        <div class="example"><span class="autonumber"><span><b>Exempel: </b></span></span>
          <ul>
            <li>
              <p>Om du bara vill returnera sidor anger du <code>1</code>.</p>
            </li>
            <li>
              <p>Om du vill returnera sidor och objekt på den översta nivån anger du <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Lämna fältet tomt om du vill returnera alla noder.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Ange <code>paths</code> om du vill returnera vektordata.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>En kommaavgränsad lista med plugin-ID:n och/eller strängen [!UICONTROL shared]. Alla data som finns i dokumentet som skrivs av dessa plugin-program inkluderas i resultatet i egenskaperna <code>pluginData</code> och <code>sharedPluginData</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>Aktivera det här alternativet om du vill returnera filialmetadata för den begärda filen. Om filen är en gren inkluderas huvudfilens nyckel i det returnerade svaret. Om filen innehåller grenar inkluderas deras metadata i det returnerade svaret. Standard: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Get a file or image: File nodes]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Markera filen som du vill returnera JSON från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Ange de noder som du vill att modulen ska returnera och konvertera</p>
        <p>För varje nod som du vill returnera klickar du på <b>[!UICONTROL Add]</b> och anger texten för noden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ange eller mappa den version av filen som du vill att modulen ska returnera. Lämna fältet tomt för den aktuella modulen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Ange eller mappa ett heltal som representerar hur djupt in i dokumentträdet du vill returnera resultat för. </p>
        <div class="example"><span class="autonumber"><span><b>Exempel: </b></span></span>
          <ul>
            <li>
              <p>Om du bara vill returnera sidor anger du <code>1</code>.</p>
            </li>
            <li>
              <p>Om du vill returnera sidor och objekt på den översta nivån anger du <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Lämna fältet tomt om du vill returnera alla noder.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Ange <code>paths</code> om du vill returnera vektordata.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>En kommaavgränsad lista med plugin-ID:n och/eller strängen "shared". Alla data som finns i dokumentet som skrivs av dessa plugin-program inkluderas i resultatet i egenskaperna pluginData och sharedPluginData.</td>
    </tr>
  </tbody>
</table>


##### Hämta en fil eller bild: Bild

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Markera filen som du vill returnera JSON från.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Ange de noder som du vill att modulen ska återge.</p>
        <p>För varje nod som du vill återge klickar du på <b>[!UICONTROL Add]</b> och anger texten för noden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Ange eller mappa skalningsfaktorn om du vill skalförändra bilden. Talet måste vara mellan 0,01 och 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Välj format för bildutdata.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Include ID]</td>
      <td>Aktivera det här alternativet om du vill inkludera ID-attribut för alla SVG-element. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplify Stroke]</td>
      <td>Aktivera det här alternativet om du vill förenkla inre/yttre linjer och använda linjeattribut om det är möjligt i stället för &lt;mask&gt;. Standard: [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Use absolute bounds]</td>
      <td>Aktivera det här alternativet om du vill använda nodens fullständiga dimensioner oavsett om den beskärs eller inte eller om utrymmet runt den är tomt. Använd detta om du vill exportera textnoder utan beskärning. Standard: [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Ange eller mappa den version av filen som du vill att modulen ska returnera. Lämna fältet tomt för den aktuella modulen.</td>
    </tr>
  </tbody>
</table>

##### Hämta en fil eller bild: Bildfyllningar

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Markera filen som du vill returnera JSON från.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL List file version history]

Denna sökmodul returnerar versionshistoriken för en enskild fil i [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Ange eller mappa fil-ID:t för filen som du vill hämta versionshistorik för. </p>
        <ul>
          <li>
            <p>Om du inte känner till filens ID klickar du på <b>[!UICONTROL Find Files]</b> och anger eller mappar ID:t för projektet som filen är kopplad till. Markera sedan filen.</p>
          </li>
          <li>
            <p>Om du försöker hitta filens ID och inte känner till projektets ID klickar du på <b>[!UICONTROL Find Projects]</b> och anger eller mappar ID:t för det team som äger projektet som filen är associerad med. Markera projektet och markera sedan filen.</p>
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

#### [!UICONTROL List project files]

Sökmodulen returnerar en lista med alla filer i det angivna projektet.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Ange eller mappa det projekt-ID som du vill hämta filer för. </p>
        <ul>
          <li>
            <p>Om du inte känner till projektets ID klickar du på <b>[!UICONTROL Find Projects]</b> och anger eller mappar ID:t för det team som projektet är kopplat till. Markera sedan projektet.</p>
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

#### [!UICONTROL List projects]

Sökmodulen returnerar en lista över alla projekt i det angivna teamet.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Ange eller mappa projekt-ID:t för projektet som du vill hämta filer för. Team-ID:t finns på webbadressen till teamets sida i Figma</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td>
    </tr>
  </tbody>
</table>


### Komponenter och format

#### [!UICONTROL Get a style or component]

Den här åtgärdsmodulen hämtar ett enskilt format eller en komponent, eller en uppsättning format eller komponenter.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object> key]</td>
      <td>Ange nyckeln (unik identifierare) för objektet som du vill hämta.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Ange eller mappa ID:t för det team som posten eller posterna är kopplade till.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Page Size]</td>
      <td>Ange eller mappa talet eller resultaten som ska returneras per sida. Standard: 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>Ange eller mappa numret på resultatet efter vilket du vill börja hämta resultaten. Detta kan kombineras med fältet [!UICONTROL Page Size] för att numrera resultaten.</p>
        <p>Detta värde motsvarar inte objekt-ID.</p>
        <p>Det här fältet kan inte användas i kombination med fältet [!UICONTROL Before].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>Ange eller mappa det antal resultat som du vill börja hämta resultat innan. Detta kan kombineras med fältet [!UICONTROL Page Size] för att numrera resultaten.</p>
        <p>Detta värde motsvarar inte objekt-ID.</p>
        <p>Det här fältet kan inte användas i kombination med fältet [!UICONTROL After].</p>
      </td>
    </tr>
  </tbody>
</table>


### Övriga

* [Anropa ett API](#make-an-api-call)

* [Se händelser](#watch-events)


#### [!UICONTROL Make an API call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till Figma API utan att behöva tänka igenom autentiseringen. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås med de andra Figma-modulerna.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Ange en relativ sökväg till <code>https://api.figma.com/v1/</code>.</p>
        <p>Exempel: <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metoder för HTTP-begäran i [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] lägger till auktoriseringsrubrikerna åt dig.</p>
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
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Watch events]

Den här utlösarmodulen startar ett scenario när någon av följande händelser inträffar för ett specifikt team i ditt [!DNL Figma]-teamspace

* Filuppdatering

* Uppdatering av filversion

* Filborttagning

* Publicera bibliotek

* Filkommentar

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Välj den webkrok som modulen tittar på.</p>
        <p>Så här lägger du till en ny webbkrok:</p>
        <ol>
          <li value="1">
            <p>Klicka på <b>[!UICONTROL Add]</b> bredvid fältet [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Välj den anslutning som du vill använda för den här webkroken. Instruktioner om hur du ansluter ditt [!DNL Figma]-konto till [!UICONTROL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - grundläggande instruktioner.</a></p>
          </li>
          <li value="3">
            <p>Välj händelsetypen som du vill att modulen ska bevaka.</p>
          </li>
          <li value="4">
            <p>Ange ID:t för det team vars händelser du vill att webbkroken ska bevaka.</p>
          </li>
          <li value="5">
            <p>Ange [!UICONTROL Status] eller [!UICONTROL Description] för händelser som du vill att webbkroken ska bevaka.</p>
          </li>
          <li value="6">
            <p>Klicka på <b>[!UICONTROL Save]</b> för att spara webkroken och återgå till modulen.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
