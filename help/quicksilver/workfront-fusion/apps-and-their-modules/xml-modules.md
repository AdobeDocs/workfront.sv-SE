---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: Med XML-appen kan du tolka en XML-formaterad text via XML-&get; Tolka XML-modulen och konvertera den till ett paket för att göra data tillgängliga för andra moduler. Du kan även konvertera ett paket till en XML-formaterad text via XML-&gt; Skapa XML-modul
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 1%

---

# XML

The [!UICONTROL XML] kan du tolka XML-formaterad text via [!UICONTROL XML] > [!UICONTROL Parse XML] och konvertera till ett paket för att göra data tillgängliga för andra moduler. Du kan också konvertera ett paket till en XML-formaterad text via [!UICONTROL XML] > [!UICONTROL Create XML] modul

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

## [!UICONTROL Parse XML]

The [!UICONTROL XML] > [!UICONTROL Parse XML] tolkar en XML-formaterad text och genererar ett enda paket som innehåller all information som extraheras från XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>Datastrukturen beskriver XML-strukturen så att modulens utdata blir tillgängliga på mappningspanelen för följande moduler.</p> <p>Om du har ett exempel på den XML som du vill analysera kan du använda den för att generera datastrukturen:</p> 
    <ol> 
     <li value="1">Klicka på <strong>[!UICONTROL Add]</strong> -knappen.</li> 
     <li value="2">Klicka på <strong>[!UICONTROL Generator]</strong> -knappen.</li> 
     <li value="3">Kopiera och klistra in XML-exemplet i <strong>[!UICONTROL Sample data]</strong> fält.</li> 
     <li value="4">Klicka på <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Kontrollera att datastrukturen har skapats.</li> 
     <li value="6"> <p>Klicka på <strong>[!UICONTROL Save]</strong> för att spara datastrukturen.</p> <p>Du kan hoppa över steg 2-5 för att tillhandahålla en tom datastruktur. Om datastrukturen är tom är modulens utdata inte tillgängliga på mappningspanelen förrän modulen har körts minst en gång.</p> </li> 
    </ol> <p>Mer information finns i <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datastrukturer i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve numbers as text]</td> 
   <td>Aktivera det här alternativet för att säkerställa att tal förblir som textvärden (strängvärden). I annat fall byts tal ut mot talvärden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Ange eller mappa den XML-formaterade text som du vill analysera.</p> <p>Om du använder en formel måste du se till att dess resultatvärdetyp är (eller kan tvingas till automatiskt) [!UICONTROL Text] datatyp. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Om resultatvärdetypen är [!UICONTROL Buffer] (binära data) använder du <code>toString()</code> för att konvertera den till datatypen Text. Mer information finns i <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a> och <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Artikeldatatyper i [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Så här hämtar du en XML-fil från en URL och tolkar innehållet i den:
>
>1. Skapa ett nytt scenario.
>1. Infoga [!UICONTROL HTTP] > [!UICONTROL Get a file] modul
>1. Öppna modulens konfiguration och konfigurera den enligt följande:
>
>   **URL**: XML-filens URL (t.ex. `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Klicka **[!UICONTROL OK]**&#x200B; att spara och stänga modulens konfiguration.
1. Lägg till [!UICONTROL XML] > [!UICONTROL Parse XML] ansluter du den efter [!UICONTROL HTTP] > [!UICONTROL Get a file] och konfigurera den enligt följande:
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Data structure]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Klicka på <strong>[!UICONTROL Add]</strong> -knappen.</li> 
&gt;        <li value="2">Klicka på <strong>[!UICONTROL Generator]</strong> -knappen.</li> 
&gt;        <li value="3">Öppna en ny flik eller ett nytt fönster i webbläsaren.</li> 
&gt;        <li value="4">Placera den URL du använde i det tredje steget i adressfältet och hämta XML-filen.</li> 
&gt;        <li value="5">Markera all XML-text och kopiera den till Urklipp.</li> 
&gt;        <li value="6">Stäng fliken eller fönstret och gå tillbaka till ditt scenario.</li> 
&gt;        <li value="7">Klistra in den kopierade XML-texten i datafältet Exempel.</li> 
&gt;        <li value="8">Klicka på <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">Kontrollera att datastrukturen har skapats.</li> 
&gt;        <li value="10">Klicka <strong>[!UICONTROL Save]</strong> för att spara datastrukturen.</li> 
&gt;       </ol> <p>Du kan hoppa över steg 2 till 9 för att tillhandahålla en tom datastruktur. Om datastrukturen är tom är modulens utdata inte tillgängliga på mappningspanelen förrän modulen har körts minst en gång.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Mappa <code>Data </code>från utdata från [!UICONTROL HTTP] &gt; [!UICONTROL Get a file] i fältet. Använd <code>toString()</code> funktionen för att konvertera dess värde från [!UICONTROL Buffer] (binära data) typ till [!UICONTROL Text] datatyp.</p> <p>Du kan kopiera och klistra in formelns kod i fältet: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Mer information om datatyperna Buffer och Text finns i <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Objektdatatyper i Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Parsing XML attributes]

Som standard är [!UICONTROL XML] > [!UICONTROL Parse XML] för att placera attribut i en särskild samling `_attributes` som underordnad nod till noden som har dessa attribut. Om noden är en textnod och har attribut läggs två specialegenskaper till: `_attributes` för attribut och `_value` för nodens textinnehåll.

>[!INFO]
>
**Exempel:** Denna XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

konverteras till det här paketet:

![](assets/xml-converted-to-bundle.png)

## Skapa XML

The [!UICONTROL XML] > [!UICONTROL Create XML] i konverteras ett paket till en XML-formaterad text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>Datastrukturen beskriver strukturen för den resulterande XML-filen. Om du har ett exempel på den XML som du vill skapa kan du använda den för att generera datastrukturen:</p> 
    <ol> 
     <li value="1">Klicka på <strong>[!UICONTROL Add]</strong> -knappen.</li> 
     <li value="2">Klicka på <strong>[!UICONTROL Generator]</strong> -knappen.</li> 
     <li value="3">Kopiera och klistra in XML-exemplet i datafältet Exempel.</li> 
     <li value="4">Klicka på <strong>[!UICONTROL Save]</strong> -knappen.</li> 
     <li value="5">Kontrollera att datastrukturen har skapats.</li> 
     <li value="6">Klicka <strong>[!UICONTROL Save]</strong> för att spara datastrukturen.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Root element name]</td> 
   <td>Ange namnet på XML-filens rotelement. Standardvärdet är <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Ange filnamnet som ska användas i<code> !DOCTYPE SYSTEM</code> deklaration</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Ange filnamnet som ska användas i<code> !DOCTYPE PUBLIC</code> deklaration</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Declaration]</td> 
   <td>Aktivera det här alternativet för att ta bort XML-deklarationen <code>&lt;?xml ... ?&gt;</code> och <code>&lt;!DOCTYPE ... &gt;</code>och lämna bara XML-rotelementet och dess innehåll.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Exempel:**
>
Ett typiskt exempel är att omvandla data från en [!DNL Google] >kalkylblad till XML.
>
1. Placera [!DNL Google Sheets] > [!UICONTROL Select rows] i ditt scenario för att hämta data. Konfigurera modulen för att hämta rader från din [!DNL Google] kalkylblad. Ange &#x200B;**[!UICONTROL Maximum number of returned rows]** till ett litet tal, men större än ett för testningsändamål (exempel, tre). Kör [!DNL Google Sheets] genom att högerklicka och välja &quot;**[!UICONTROL Run this module only]**.&quot; Kontrollera modulens utdata.
1. Anslut [!UICONTROL Array Aggregator] modulen efter [!DNL Google Sheets] -modul. Välj [!DNL Google Sheets] i **[!UICONTROL Source node]** fält. Låt de andra fälten vara som de är för tillfället.
1. Anslut [!UICONTROL XML] > [!UICONTROL Create XML] modulen efter [!UICONTROL Array Aggregator] -modul.
>
Modulens konfiguration kräver en datastruktur som beskriver strukturen för XML-utdata. Klicka på **[!UICONTROL Add]** för att öppna datastrukturinställningarna. Det enklaste sättet att skapa den här datastrukturen är att generera den automatiskt från ett XML-exempel.
>
1. Klicka på **[!UICONTROL Generator]** och klistra in XML-exemplet i [!UICONTROL Sample data] fält:
>
![](assets/sample-data-field-350x146.png)
>
1. Klicka på **[!UICONTROL Save]**. Fältet Specifikation i datastrukturen innehåller nu den genererade strukturen.
1. Ändra namnet på datastrukturen till något mer specifikt och klicka på **[!UICONTROL Save]**. Ett fält som motsvarar rotarrayattributet visas som ett mappningsbart fält i JSON-modulens inställningar.
1. Klicka på **[!UICONTROL Map]** intill fältet och mappa `Array[]` objekt från [!UICONTROL Array aggregator] till den:
1. Klicka **[!UICONTROL OK]** för att stänga XML-modulens inställningar.
1. Öppna inställningarna för [!UICONTROL Array Aggregator] -modul. Ändra **[!UICONTROL Target structure]** från Anpassad till ett fält i en XML-modul som motsvarar det överordnade XML-elementet.Mappa objekt från [!DNL Google Sheets] till lämpliga fält.
1. Klicka **[!UICONTROL OK]** för att stänga inställningarna för modulen Array Aggregator.
1. Kör scenariot.
>
XML-modulen matar ut rätt XML-fil.
>
1. Öppna inställningarna för [!DNL Google Sheets] och öka [!UICONTROL Maximum number of returned rows] talet vara större än antalet rader i kalkylbladet för att bearbeta alla data.
>
Resultatet kan sparas i [!DNL Dropbox], skickas som en bifogad fil via e-post, överförs via FTP till en server och så vidare.

## Lägga till XML-attribut

Om du vill lägga till attribut i en komplex nod (en nod som ska innehålla andra noder) måste du lägga till en samling med namnet `_attributes` för den komplexa anteckningen i din anpassade datastruktur. Samlingen mappas till nodattribut. Om du vill lägga till attribut i en textnod (till exempel: `<node attr="1">abc</node>`) måste du lägga till en samling `_attributes` för attribut och en text-egenskap `_value` för nodvärdet för den här noden i din anpassade datastruktur.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Felsökning: Det går inte att mappa data från [!UICONTROL Parse XML] modul

Kontrollera att datastrukturen är korrekt definierad. Du kan också använda en tom datastruktur och köra modulen minst en gång för att bearbeta en XML-inmatning.
