---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive för företag-moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder  [!DNL Microsoft OneDrive for Business] samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL Microsoft OneDrive for Business] samt ansluta det till flera tredjepartsprogram och -tjänster.

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

Om du vill använda [!DNL Microsoft OneDrive for Business] med [!DNL Adobe Workfront Fusion] behöver du ett [!DNL Microsoft]-konto.

Instruktioner om hur du ansluter ditt [!DNL OneDrive for Business]-konto till [!DNL Workfront Fusion] finns i [Skapa en anslutning till Adobe [!DNL Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)



## Ansluter tjänsten [!DNL Microsoft OneDrive for Business] till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter ditt [!DNL Microsoft OneDrive for Business]-konto till [!UICONTROL Workfront Fusion] finns i [Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
>
>Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.

## [!DNL Microsoft OneDrive for Business]-moduler och deras fält

När du konfigurerar [!DNL Microsoft OneDrive for Business] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL Microsoft OneDrive for Business] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)

### Utlösare

* [[!UICONTROL Watch files]](#watch-files)
* [[!UICONTROL Watch folders]](#watch-folders)

#### [!UICONTROL Watch files]

Den här utlösarmodulen aktiveras när en ny fil läggs till eller uppdateras i en mapp som bevakas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Välj den enhet som du vill titta på.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Markera mappen som du vill bevaka. I ett scenario kan du bara övervaka en mapp.</p> <p>Tips! Om du vill hålla reda på flera mappar skapar du ett oberoende scenario för var och en av dem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>Välj om du endast vill titta på nya filer och alla ändringar, eller nya filer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> Ange det maximala antalet resultat som [!DNL Workfront Fusion] ska arbeta med under en cykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch folders]

Den här utlösarmodulen aktiveras när en ny mapp läggs till i den mapp som bevakas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Välj den enhet som du vill titta på.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Markera mappen som du vill bevaka. I ett scenario kan du bara övervaka en mapp.</p> <p>Tips! Om du vill hålla reda på flera mappar skapar du ett oberoende scenario för var och en av dem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>Välj om du endast vill bevaka nya mappar och alla ändringar, eller nya mappar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> Ange det maximala antalet resultat som [!DNL Workfront Fusion] ska arbeta med under en cykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [[!UICONTROL Upload a file]](#upload-a-file)
* [[!UICONTROL Delete a file]](#delete-a-file)
* [[!UICONTROL Get a file]](#get-a-file)
* [[!UICONTROL Create a folder]](#create-a-folder)
* [[!UICONTROL Delete a folder]](#delete-a-folder)
* [[!UICONTROL Get a sharing link]](#get-a-sharing-link)

#### [!UICONTROL Upload a file]

Den här åtgärdsmodulen överför en binär fil eller textfil till en angiven mapp

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Välj den enhet som du vill överföra en fil till.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Markera mappen på enheten.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL If the file with the same name exists]</td> 
   <td> <p> Välj vad du vill göra om det redan finns en fil med samma namn som den fil du försöker överföra.</p> 
    <ul> 
     <li>[!UICONTROL Replace the existing file]</li> 
     <li>[!UICONTROL Rename the new file]</li> 
     <li>[!UICONTROL End with an error]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a file]

Denna åtgärdsmodul flyttar den angivna filen till papperskorgen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Markera den enhet som du vill ta bort en fil från.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Ange ID:t för filen som du vill ta bort. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a file]

Den här åtgärdsmodulen hämtar filen med det angivna ID:t.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Välj den enhet som du vill hämta en fil från.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Ange ID:t för filen som du vill hämta. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a folder]

Skapar en mapp i den angivna överordnade mappen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Drive ID]</strong> </td> 
   <td> <p>Välj den enhet där du vill skapa en ny mapp.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>Markera mappen som du vill skapa en ny mapp i.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder name]</strong> </td> 
   <td>Ange eller mappa ett namn för den nya mappen.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a folder]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Markera den enhet som du vill ta bort en fil från.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td> <p>Ange eller mappa ID:t för mappen som du vill ta bort. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a sharing link]

Den här modulen hämtar en länk som du kan dela för att ge åtkomst till den angivna filen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Välj den enhet som du vill överföra en fil till.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>Välj om du vill välja en fil med fil-ID:t eller filsökvägen. Ange fil-ID eller sökväg i fältet som visas.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permission type]</p> </td> 
   <td> <p>Välj om du vill att personer som tar emot länken ska ha läs-/skrivbehörighet eller skrivbehörighet.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope]</td> 
   <td> <p> Välj om du vill att filen ska vara tillgänglig för alla som har länken eller bara är tillgängliga för medlemmar i organisationen.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
