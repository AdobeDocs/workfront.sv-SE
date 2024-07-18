---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft Word-mallmoduler
description: I ett Adobe Workfront Fusion-scenario kan du automatisera arbetsflöden som använder Microsoft Word-mallar samt ansluta dem till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# [!DNL Microsoft Word Template] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL Microsoft Word Templates] samt ansluta det till flera tredjepartsprogram och -tjänster.

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
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Om du vill använda [!DNL Miscrosoft Word Templates] med [!DNL Adobe Workfront Fusion] måste du ha ett [!DNL Office 365]-konto. Du kan skapa en på www.office.com.



## Ansluter tjänsten [!DNL Office] till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter ditt [!DNL Office]-konto till [!UICONTROL Workfront Fusion] finns i [Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
>
>Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.

## Använder [!DNL Microsoft Word Templates] moduler

Du kan använda en [!DNL Microsoft Word Template]-modul för att sammanfoga data från flera webbtjänster till ett [!DNL Microsoft Word]-dokument.

Du kan till exempel använda den här [!DNL Microsoft Word]-mallen:

![](assets/word-template-before-filled-350x62.png)

Så här skapar du det här dokumentet:

![](assets/word-template-exampled-filled-350x85.png)

## Om värdetaggar

En [!DNL Microsoft Word]-mall är ett vanligt [!DNL Microsoft Word]-dokument (.docx-fil) med särskilda taggar i texten som avgör var och hur data ska sammanfogas eller fyllas i. Det finns tre typer av taggar:

* [Enkel värdetagg](#simple-value-tag)
* [Villkorstagg](#condition-tag)
* [Loop-tagg](#loop-tag)

### Enkel värdetagg {#simple-value-tag}

En enkel värdetagg ersätts med ett motsvarande värde. Taggens namn motsvarar fältets [!UICONTROL Key]-värde, som är placerat inom dubbla klammerparenteser, till exempel


<pre>{{name}}</pre>


.

**Exempel:** Om du vill skapa ett dokument med texten &quot;Hi, Petr!&quot; kan du använda en [!DNL Microsoft Word Template]-modul för att skapa följande mall:

<pre>&gt; Hej {{name}}!</pre>

Om du vill göra det ställer du in modulen enligt följande:

![](assets/word-template-simple-value-350x286.png)

### Villkorstagg {#condition-tag}

Du kan använda ett villkorsmärkord för att figursätta text som bara ska återges när vissa villkor uppfylls. Om du vill radbryta texten placerar du den mellan inledande och avslutande villkorstaggar, till exempel &quot;hasPhone&quot;, om villkoret är huruvida data innehåller ett telefonnummer eller inte. Namnet på en öppningstagg föregås av hash-tecknet #. Namnet på en avslutande tagg föregås av ett snedstreck /, vilket visas i exemplet nedan.

**Exempel:** Om du vill skapa ett dokument som innehåller en kunds telefonnummer om indata innehåller ett telefonnummer, men ingen e-postadress, kan du använda en [!DNL Microsoft Word Template]-modul och skapa följande mall:
<pre>&gt; {{#hasPhone}}Telefon: {{phone}} {{/hasPhone}}</pre><pre>&gt; {{#hasEmail}}E-post: {{email}} {{/hasEmail}}</pre>Om du vill göra det ställer du in modulen enligt följande:

![](assets/word-template-conditional-350x501.png)

I dokumentet visas telefonnumret så här:
<pre>&gt; Telefon: 444551234</pre>

### Loop-tagg {#loop-tag}

Du kan använda en loop-tagg, som också kallas avsnittstagg, för att upprepa ett textavsnitt. Radbryt texten genom att placera den mellan de inledande och avslutande looptaggarna. Namnet på en öppningstagg föregås av hash-tecknet #; namnet på en avslutande tagg föregås av ett snedstreck /.

* [Slinga taggen med Fyll i en dokumentmodul](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Loopa tagg med Fylla i en dokumentmodul {#loop-tag-with-fill-out-a-document-module}

**Exempel:** Om du vill skapa ett dokument med namn och telefonnummer för varje kontakt i en kundlista kan du använda en [!DNL Microsoft Word Template]-modul och skapa följande mall:

<pre>&gt; {{#contact}}</pre><pre>&gt;     {{name}}, {{phone}}</pre><pre>&gt; {{/contact}}</pre>

Om du vill göra det ställer du in modulen enligt följande:


![](assets/word-template-fill-out-a-document-350x732.png)

Modulen skulle skapa följande dokument:

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] moduler

Dessa moduler kräver ingen anslutning.

* [Fylla i ett dokument](#fill-out-a-document)
* [Fylla ett dokument med en datauppsättning](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Fill out a document] {#fill-out-a-document}

Med den här transformerarmodulen kan du fylla ett dokument med data som du anger. Den kan användas med enkla värdetaggar, villkorstaggar eller looptaggar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start delimiter of the text being replaced]</td> 
   <td> <p>Ange de tecken som du vill markera början av texten som ska ersättas. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Ange <code>[[</code> om du vill ersätta en text som liknar den här: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL End delimiter of the text being replaced]</p> </td> 
   <td> <p>Ange de tecken som du vill markera slutet av texten som ska ersättas. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Ange <code>]]</code> om du vill ersätta en text som liknar den här: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p> Mappa filen som du vill överföra från den tidigare modulen (t.ex. HTTP &gt; Hämta en fil eller Dropbox &gt; Hämta en filmodul). Eller ange datafilen manuellt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of filled out file]</td> 
   <td>Ange ett filnamn (inklusive filtillägg) för målutdatafilen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data source]</td> 
   <td> <p>Välj ett alternativ för att ange om de data du använder kommer från ett formulär eller från en samling rådata (obearbetade datordata).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Detta måste vara en array med samlingar där:</p> 
    <ul> 
     <li>Varje samling motsvarar en datapost och innehåller ett objekt <code>entry</code></li> 
     <li>Objektet <code>entry </code> innehåller en samling av <code>key </code>och <code>value</code></li> 
     <li>Objektet <code>key </code> innehåller taggens namn</li> 
     <li>objektet <code>value </code> innehåller taggens värde</li> 
    </ul> 
    <p>Så här lägger du till en post:</p>
    <ol> 
     <li> Klicka på <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Välj värdetyp för posten.</li> 
     <li>Lägg till namnet och värdet. Mer information finns i exemplet för den valda värdetypen i den här artikeln. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Enkel värdetagg</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Villkorstagg</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Loop-tagg</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fill a document with a batch of data] {#fill-a-document-with-a-batch-of-data}

Den här aggregeringsmodulen är användbar om dina datainmatningar kommer som separata paket. Med den här modulen kan du enkelt ställa in den struktur som krävs för fältet Värde och mappa objekt till varje värdeobjekt. Till skillnad från Fyll i en dokumentmodul tillåter fältet Värden i Fyll i ett dokument med en batch med data-modul endast en post som innehåller variabler.

Du kan också använda den här modulen om dina dataposter kommer som en array genom att använda modulen *Iterator* för att omvandla innehållet i arrayen till en serie paket.

De faktiska värdena skapas och fylls i för varje inkommande paket. Mallen skapas när alla indatapaket har bearbetats.

Den här aggregeringsmodulen är särskilt användbar när du vill skapa listor eller rapporter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Markera modulen som är textens källa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start delimiter of the text being replaced]</td> 
   <td> <p>Ange de tecken som du vill markera början av texten som ska ersättas. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Ange <code>[[</code> om du vill ersätta en text som liknar den här: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL End delimiter of the text being replaced]</p> </td> 
   <td> <p>Ange de tecken som du vill markera slutet av texten som ska ersättas. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Ange <code>]]</code> om du vill ersätta en text som liknar den här: <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td> Definiera ett uttryck som innehåller ett eller flera mappade objekt. De aggregerade data separeras under Grupper med samma uttrycksvärde. Varje grupp returnerar som ett separat paket som innehåller en nyckel med det utvärderade uttrycket och den aggregerade texten. På så sätt kan du använda Key (Nyckel) som ett filter i efterföljande moduler.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Aktivera det här alternativet om du vill stoppa bearbetningen när en aggregering inte innehåller några paket.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p> Mappa filen som du vill överföra från den tidigare modulen (t.ex. HTTP &gt; Hämta en fil eller Dropbox &gt; Hämta en filmodul). Eller ange datafilen manuellt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of filled out file]</td> 
   <td>Ange ett filnamn (inklusive filtillägg) för målutdatafilen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data source]</td> 
   <td> <p>Välj ett alternativ för att ange om de data du använder kommer från ett formulär eller från en samling rådata (obearbetade datordata).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Detta måste vara en array med samlingar där:</p> 
    <ul> 
     <li>Varje samling motsvarar en datapost och innehåller ett objekt <code>entry</code></li> 
     <li>Objektet <code>entry </code> innehåller en samling av <code>key </code>och <code>value</code></li> 
     <li>Objektet <code>key </code> innehåller taggens namn</li> 
     <li>objektet <code>value </code> innehåller taggens värde</li> 
    </ul> 
    <p>Så här lägger du till en post:</p>
    <ol> 
     <li> Klicka på <b>[!UICONTROL Add Item]</b>. </li> 
     <li>Välj värdetyp för posten.</li> 
     <li>Lägg till namnet och värdet. Mer information finns i exemplet för den valda värdetypen i den här artikeln. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Enkel värdetagg</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Villkorstagg</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Loop-tagg</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
