---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Felsöka scenarier med Adobe Workfront Fusion Devtool
description: Med Adobe Workfront Fusion Devtool kan du förstå och felsöka scenarier. Utvecklingsverktyget lägger till en extra panel i Chrome Developer Tools. Med den här felsökningspanelen kan du kontrollera alla manuella körningar av ditt scenario, granska alla utförda åtgärder och se information om alla API-anrop som utförs. Du kan se vilken modul, åtgärd eller enskilt svar som orsakade felet och använda den kunskapen för att förfina ditt scenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Felsökningsscenarier med [!DNL Adobe Workfront Fusion] Devtool

The [!DNL Adobe Workfront Fusion] Med Devtool kan du förstå och felsöka scenarier. Utvecklingsverktyget lägger till en extra panel i [!DNL Chrome Developer Tools]. Med den här felsökningspanelen kan du kontrollera alla manuella körningar av ditt scenario, granska alla utförda åtgärder och se information om alla API-anrop som utförs. Du kan se vilken modul, åtgärd eller enskilt svar som orsakade felet och använda den kunskapen för att förfina ditt scenario.

>[!NOTE]
>
>Loggning på felsökningspanelen kommer att vara begränsad eller otillgänglig för konfidentiella scenarier, automatiska körningar och framgångsrika åtgärder.

En videointroduktion och genomgång av verktyget Fusion Devtool finns på

* [Fusion Development Tool](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Utvecklargenomgång](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
  <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

## Åtkomst till Workfront Fusion Devtool

Åtkomsten till utvecklingsverktyget skiljer sig åt beroende på om du använder Fusion i [!DNL Adobe Unified Experience].

* [Öppna utvecklingsverktyget i [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Få åtkomst till utvecklingsverktyget i klassiska [!DNL Fusion] upplevelse](#access-the-devtool-in-the-classic-fusion-experience)

### Öppna utvecklingsverktyget i [!DNL Adobe Unified Experience] eller nya Fusion

Om du använder Fusion i Adobe Unified Shell, eller har uppdaterat till den nya Fusion-upplevelsen, kan du komma åt Dev-verktyget från Scenarioredigeraren.

1. Klicka på **Hjälpverktyg** ![Hjälpverktyg](assets/debugger-icon.png) -ikonen längst ned på skärmen.

Eller:

1. Gå till Scenarioredigeraren för det scenario som du vill felsöka.

   Information om hur du hittar Scenarioredigeraren finns i [Scenarioredigerare](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Högerklicka i ett tomt område på sidan (inte i en modul).
1. Välj **Open Devtool**.

### Få åtkomst till utvecklingsverktyget i klassiska [!DNL Fusion] upplevelse

Så här använder du utvecklingsverktyget i klassiska [!DNL Fusion] måste du installera en [!DNL Chrome] tillägg. Du kan sedan använda det här tillägget från [!DNL Chrome] Utvecklarverktyg.

* [Installera installationsfilen [!DNL Chrome] Devtool-tillägg](#install-the-chrome-devtool-extension)
* [Leta reda på [!DNL Workfront Fusion] Devtool](#locate-the-workfront-fusion-devtool)

#### Installera [!DNL Chrome] Devtool-tillägg

Du kan lägga till [!DNL Workfront Fusion] Utveckla för [!DNL Chrome] via [!UICONTROL [!DNL Chrome] Web Store].

1. Klicka [den här länken](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) för att gå till [!DNL Workfront Fusion] Devtool på [!UICONTROL [!DNL Chrome] Web Store].
1. Klicka på **[!UICONTROL Add to [!DNL Chrome]]**.
1. Granska behörigheter i det fönster som öppnas. Om du godkänner behörigheterna klickar du på **[!UICONTROL Add Extension]**.

The [!DNL Workfront Fusion] Utvecklingsverktyget läggs till i [!DNL Chrome] tillägg.


#### Leta reda på [!DNL Workfront Fusion] Devtool

Använd [!DNL Workfront Fusion] Devtool, du måste lägga till [!DNL Workfront Fusion] Utveckla tillägg till [!DNL Chrome] webbläsare, enligt beskrivning i [Installera tillägget Chrome Devtool](#install-the-chrome-Devtool-extension).

1. Öppna [!DNL Workfront Fusion] scenario.
1. Öppna [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Cmd + Alt + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Skift + I</p> <p> eller </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Vi rekommenderar att du dockar [!DNL Chrome Developer Console] längst ned för att få en bättre bild av dina moduler.

1. Klicka på **[!DNL Workfront Fusion]** tabba in [!DNL Chrome Dev Tools].

## Använd [!DNL Workfront Fusion] Devtool

Workfront Fusion Devtool är uppdelat i tre huvudavsnitt. De finns i den vänstra panelen i fönstret Utvecklare.

* [Live Stream](#live-stream)
* [Scenariofelsökning](#scenario-debugger)
* [verktyg](#tools)

### Live Stream

Live Stream visar vad som händer i bakgrunden när du klickar på Kör en gång i ditt scenario.

1. Klicka på **[!UICONTROL Live Stream]** icon ![](assets/live-stream-icon.png) för att öppna Live Stream-avsnittet.
1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Åtgärd</th> 
      <th>Instruktioner</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa begärandeinformation</td> 
      <td> <p>Du kan visa följande information för varje modul i ditt scenario</p> 
       <ul> 
        <li> <p>Begäranrubriker (API-slutpunkts-URL, http-metod, tid och datum då begäran anropades, begäranrubriker och frågesträng)</p> </li> 
        <li> <p>Begärandetext</p> </li> 
        <li> <p>Svarshuvuden</p> </li> 
        <li> <p>Svarstext</p> </li> 
       </ul> <p>Om du vill visa den här informationen klickar du på lämplig flik i den högra panelen i dialogrutan [!DNL Workfront Fusion] Devtool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Sök efter förfrågningar och svar</p> </td> 
      <td> <p>Ange söktermen i sökfältet i den vänstra panelen i dialogrutan [!DNL Workfront Fusion] Utvecklingsverktyget om du bara vill visa begäranden som innehåller söktermen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ta bort listan med begäranden </p> </td> 
      <td> <p>Klicka på papperskorgsikonen i det övre högra hörnet av utvecklingsverktygets vänstra panel för att rensa listan över begäranden som spelats in av [!DNL Workfront Fusion] Devtool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Aktivera konsolloggning</p> </td> 
      <td> <p>Klicka på datorikonen <img src="assets/console-computer-icon.png"> i det övre högra hörnet av utvecklingsverktygets vänstra panel.</p> <p>Inloggning på konsolen aktiveras när datorikonen är grön.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Hämta begäran i Raw JSON-format eller cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Råformat JSON</strong> </p> <p>Klicka <strong>[!UICONTROL Copy RAW]</strong> i det övre högra hörnet av utvecklingsverktygets högra ruta.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Klicka <strong>[!UICONTROL Copy cURL]</strong> i det övre högra hörnet av utvecklingsverktygets högra ruta.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Scenariofelsökning

Scenariofelsökaren är användbar för mer komplexa scenarier. Den visar historiken för scenariot som körs och gör att du kan söka efter moduler efter namn eller ID.

1. Klicka på **[!UICONTROL Scenario Debugger]** icon ![](assets/scenario-debugger-icon.png) för att öppna Scenario Debugger.
1. (Valfritt) Ange söktermen (namn eller modul-ID) i sökfältet i den vänstra rutan i [!DNL Workfront Fusion] Utvecklingsverktyget i [!UICONTROL Scenario Debugger] -avsnitt.
1. Dubbelklicka på modulens namn för att öppna dess inställningar i scenarioredigeraren.
1. Visa information om begäran genom att klicka på önskad åtgärd.

### verktyg

The [!DNL Workfront Fusion] Utvecklingsverktyg har verktyg som gör det enklare att konfigurera ditt scenario.

1. Klicka på **[!UICONTROL Tools]** icon ![](assets/console-tools-icon.png) för att öppna verktygen.
1. Välj det verktyg som du vill använda
1. Konfigurera fälten enligt nedan.
1. Klicka på **[!UICONTROL Run]**.

Verktyg och deras fält:

* [Fokusera på en modul](#focus-a-module)
* [Sök efter moduler efter mappning](#find-modules-by-mapping)
* [Hämta appmetadata](#get-app-metadata)
* [Kopiera mappning](#copy-mapping)
* [Kopiera filter](#copy-filter)
* [Växla anslutning](#swap-connection)
* [Växla variabel](#swap-variable)
* [Byt app](#swap-app)
* [Bas 64](#base-64)
* [Kopiera modulnamn](#copy-module-name)
* [Mappa om källa](#remap-source)
* [Markera app](#highlight-app)
* [Migrera GS](#migrate-gs)

#### [!UICONTROL Focus a Module]

Öppnar inställningarna för den angivna modulen efter ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Ange ID:t för modulen som du vill öppna inställningar för.</td>
    </tr>
</table>

#### [!UICONTROL Find Modules by Mapping]

Gör att du kan söka efter modulernas värden för en angiven term. Utdata innehåller ID:n för moduler som innehåller den term du har sökt efter.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Ange den term som du vill söka efter. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>Aktivera det här alternativet om du bara vill söka i modulfältets värden.</p> <p>Inaktivera det här alternativet om du även vill söka i modulfältens namn.</p> <p>Sökningen utförs med parametrarna name och label.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get App Metadata]

Hämtar metadata för programmet utifrån dess modulnamn eller ID. Detta är användbart när du behöver veta vilken version av programmet som används i ditt scenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Markera modulen som du vill hämta metadata för.</td>
    </tr>
</table>

#### [!UICONTROL Copy Mapping]

Kopierar värden från källmodulen till målmodulen.

>[!CAUTION]
>
>Kontrollera att du har angett rätt käll- och målmoduler. Om du väljer en annan typ av modul tas värdena i målmodulen bort.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Markera modulen eller ange ID:t för modulen som du vill kopiera fältvärden från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Markera modulen eller ange ID:t för modulen som du vill infoga källmodulens värden i.</p> <p>Viktigt: Värdena i målmodulen skrivs över.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Filter]

Kopierar filterinställningarna från källmodulen till målmodulen.

>[!NOTE]
>
>Kopieringsåtgärden utförs på filtret till vänster om den valda modulen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Markera modulen eller ange ID:t för modulen som du vill kopiera filtervärden från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Markera modulen eller ange ID:t för modulen där du vill infoga filtervärdena från källmodulen.</p> <p>Viktigt: Värdena i målmodulen skrivs över.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>Källfiltret anges som reservflöde. Aktivera det här alternativet om du även vill ange att målfiltret ska anges som reservflöde.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap Connection]

Duplicerar en anslutning från källmodulen till varje modul i scenariot för samma program.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Markera modulen eller ange ID:t för modulen som du vill duplicera anslutningen från.</td>
    </tr>
</table>

#### [!UICONTROL Swap Variable]

Söker efter angivna variabler i scenariot och ersätter dem med en ny variabel.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> Leta reda på variabeln som du vill ersätta från modulen i ditt scenario och kopiera den till det här ([!UICONTROL Variable to Find]). I fältet visas det med dubbla klamrar. Exempel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Leta reda på variabeln som du vill ersätta variabeln med från modulen i ditt scenario och kopiera den till det här ([!UICONTROL Variable to Find]). I fältet visas det med dubbla klamrar. Exempel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Markera den modul i vilken du vill ersätta variabeln. Om ingen modul är markerad ersätts variabeln i hela scenariot.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Swap App]

Ersätter den valda programversionen i ditt scenario med en annan programversion.

Detta kan till exempel användas för att uppgradera Gmail- och Email-apparnas moduler till den senaste versionen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> Välj det program som du vill ersätta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>Välj det program som du vill ersätta det med.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Gör att du kan koda angivna data till Base64 eller avkoda Base64. Vissa begäranden kodas till Base64. Det här verktyget kan vara användbart när du vill söka efter vissa data i den kodade begäran.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Välj om du vill koda data från [!UICONTROL Raw Data] till Base64 eller avkoda Base64 till Raw-data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Ange de data som du vill koda till Base64, eller Base64 om du vill avkoda till rådata, beroende på vilket alternativ som har valts i dialogrutan [!UICONTROL Operation] ovanför.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy Module Name]

Kopierar namnet på den valda modulen till Urklipp.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Markera modulen som du vill kopiera namnet på.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remap Source]

Gör att du kan ändra mappningskällan från en modul till en annan.

Du måste först lägga till den modul som du vill använda som källmodul i flödet i ditt scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Markera den modul som du vill ersätta som mappningskälla för andra moduler i ditt scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Markera modulen som du vill använda som en ny mappningskälla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>Markera modulen som du vill ändra mappningen för om du inte vill ändra mappningen i hela scenariot. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Highlight App]

Markerar moduler för den angivna appen i ditt scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> Välj det program som du vill ska markeras i ditt scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Välj den version av programmet som du vill markera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> Ange färghexten som du vill använda för markeringsmoduler.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrate GS]

Det här verktyget är särskilt utformat för att uppgradera [!DNL Google Sheets] (äldre) moduler till de senaste [!DNL Google Sheets] version. En ny version av modulen läggs till precis efter den äldre versionen av modulen i scenarioflödet.

Du behöver inte ange några parametrar för den här modulen.
