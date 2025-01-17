---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Skapa ett scenario för praktikintegrering i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '2062'
ht-degree: 0%

---

# Skapa ett scenario för praktikintegrering i Adobe Workfront Fusion

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Arbetsflöde för att skapa ett scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

I den här artikeln beskrivs hur du skapar ett integreringsscenario med Adobe Workfront Fusion. Integreringsscenarier kopplar samman olika appar så att data kan flöda genom olika program.

Om du vill skapa ett integreringsscenario måste din organisation ha en [!DNL Workfront Fusion for Work Automation and Integration]-licens.

Instruktioner om hur du skapar ett Workfront-specifikt automatiseringsscenario finns i [Skapa ett scenario för övningsautomatisering i Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Mer information om Workfront Fusion-licenser finns i [Adobe Workfront Fusion-licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Din organisation kanske inte tillåter åtkomst till Google Sheets. Om så är fallet kommer du inte att kunna konfigurera den här integreringen, men informationen som presenteras här kan användas som ett allmänt exempel på hur integreringsscenarier fungerar.

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

## Skapa ett övningsscenario

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera dina processer så att du kan koncentrera dig på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

Ett scenario består av en serie moduler som anger hur data ska omvandlas i en app eller överföras mellan program och webbtjänster.

För att förklara hur du skapar ett scenario och stärker de bästa metoderna när du lär dig att använda [!DNL Workfront Fusion], tar den här artikeln dig igenom processen steg för steg. Vi skapar ett scenario som skapar en ny post i [!DNL Workfront] för varje rad i ett [!DNL Google Sheets]-kalkylblad.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Ett scenario som detta skulle vara användbart om du hade ett kalkylbladsprojekt som du behöver arbeta med med projekt i [!DNL Workfront]. Scenariot kunde&quot;bevaka&quot; kalkylbladet för nya rader och lägga till ett nytt projekt i [!DNL Workfront] för var och en av dem.

Att skapa ett scenario består av flera huvuduppgifter:

## Välj program och ge scenariot ett namn

1. Hämta det här [kalkylbladet](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx) och överför det sedan till [!DNL Google Drive] för användning genom den här övningen.

   eller

   Skapa eller hitta ett eget enkelt [!DNL Google Sheets]-kalkylblad som liknar det här:

   ![](assets/spreadsheet-headers-350x55.png)

1. Logga in på ditt [!DNL Workfront Fusion]-konto.
1. Klicka på **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen.

   >[!NOTE]
   >
   >Om den vänstra navigeringspanelen eller dess ikoner inte visas klickar du på ikonen ![Meny](assets/main-menu-icon-left-nav.png) .

   I den grå [!UICONTROL Folders]-panelen som visas kan du ordna dina scenarier i mappar.

   Högst upp i huvudområdet till höger kan du visa **[!UICONTROL All]** scenarier som du har skapat, **[!UICONTROL Active Scenarios]**, **[!UICONTROL Inactive Scenarios]** och **[!UICONTROL Concepts]**, vilket är scenarier som behöver lite mer arbete innan [!DNL Workfront Fusion] kan klassificera dem som aktiva eller inaktiva.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Klicka på ikonen **[!UICONTROL Add folder]** ![](assets/add-folder-icon.png) på panelen [!UICONTROL Folders] och skriv sedan ett namn som &quot;Practice scenarios&quot; för den första mappen.

1. Öppna mappen och klicka sedan på **[!UICONTROL Create a new scenario]** i det övre högra hörnet på sidan.

   På landningssidan som visas kan du förhandsladda alla appar som du vill använda i det scenario som du tänker skapa.

1. Sök efter och välj appen **[!UICONTROL Google Sheets]** för den här övningen.
1. Klicka på **[!UICONTROL Continue]** i det övre högra hörnet.

   Scenarioredigeraren visas med en tom modul i mitten, den [!DNL Google Sheets]-app som du har förinläst och några alternativ i verktygsfältet längst ned.

<!--
   ![](assets/scenario-editor.png)
-->

När du börjar skapa ett nytt scenario är det en bra idé att börja med att skapa ett namn för det.

1. Markera platshållarnamnet **[!UICONTROL New scenario]** i det övre vänstra hörnet och skriv sedan ett namn som &quot;Practice scenarios 1&quot;.
1. Fortsätt med [Lägg till och konfigurera den första modulen](#add-and-configure-the-first-module) nedan.

## Lägg till och konfigurera den första modulen

Den tomma modulen med ett frågetecken representerar den utlösarmodul som du behöver lägga till. Modulen startar scenariot varje gång det körs. Klockikonen på den tomma modulen anger att det är en schemalagd modul.

![](assets/empty-module.png)

Den här modulen innehåller de data som du vill att scenariot ska bevakas för.

1. Klicka på den tomma modulen för att välja det program du vill välja en modul från.

   Appen som du förinstallerade visas bredvid den tomma modulen. Du kan lägga till andra appar som har moduler med rutan [!UICONTROL Search].

   ![](assets/pre-loaded-apps-350x139.png)

1. Klicka på **[!DNL Google Sheets]**.

   Listan ändras till att visa alla [!DNL Google Sheets] moduler som du kan använda som utlösarmodul.

1. Klicka på modulen **[!UICONTROL Watch for Records]**.

   Nu måste du upprätta en autentiserad anslutning till ditt Google-konto. Alla moduler som du lägger till i ett scenario måste ha en anslutning till dess program.

1. I rutan **[!DNL Google Sheets]**, under **[!UICONTROL Connection]**, klickar du på **[!UICONTROL Add]** och anger sedan ett namn för anslutningen, till exempel&quot;Olivias Google-konto&quot;. Klicka sedan på **[!UICONTROL Continue]**.
1. Autentisera anslutningen i fönstret som visas.

   Processen för att autentisera en anslutning kan variera lite mellan olika program. Du kan behöva logga in på appen. Du måste vanligtvis klicka på en **[!UICONTROL Allow]**-knapp. Om du behöver hjälp kan du läsa [Anslutningsöversikt](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Konfigurera den första modulen

När du har anslutit [!DNL Workfront Fusion] till ditt [!DNL Google Sheets]-konto kan du ange ett [!DNL Google Sheets]-kalkylblad som du har åtkomst till och de data där som du vill att den första modulen ska bearbeta.

1. Klicka på rutan **[!UICONTROL Spreadsheet]** och markera sedan kalkylbladet **[!UICONTROL Workfront Fusion practice scenario]#1** i listan som visas.

   Det här kalkylbladet innehåller 2 blad (flikar), så vi måste ange vilket blad som innehåller de data vi vill ha:

1. I listrutan **[!UICONTROL Sheet]** väljer du **[!UICONTROL Projects]**.

   Vårt kalkylblad innehåller rubriker och vi vill att modulen ska använda dem för att identifiera de data som vi vill bearbeta:

   ![](assets/spreadsheet-headers-350x55.png)

1. Låt **[!UICONTROL Yes]** vara markerat för **[!UICONTROL Table contains headers]**.

1. I rutan **[!UICONTROL Row with headers]** kan du ange ett radintervall som du vill ta med, men vi låter standardvärdet A1:Z1 vara kvar där för den här övningen.
1. Skriv 1 i rutan **[!UICONTROL Limit]**.

   På så sätt bearbetar modulen bara 1 rad i kalkylbladet varje gång du kör ett scenario. Detta är användbart när du vill förenkla testkörningarna medan du skapar scenariot.

1. Klicka på **[!UICONTROL OK]**.

   I rutan **[!UICONTROL Choose where to start]** uppmanas du att ange var i kalkylbladet du vill att modulen ska börja bearbeta.

1. Klicka på **[!UICONTROL Choose manually]**, välj det översta alternativet i listan som visas och klicka sedan på **[!UICONTROL OK]**.
1. Högerklicka på modulen, klicka på **[!UICONTROL Rename]**, skriv ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Se projektlistan&quot;) och klicka sedan på **[!UICONTROL OK]**.

   Namnet visas precis nedanför modulen. Under det finns en kort beskrivning av den typ av åtgärd som har utförts av modulen i [!DNL Workfront Fusion].

   ![](assets/module-renamed-350x388.png)

1. Fortsätt med [Lägg till och konfigurera den andra modulen](#add-and-configure-the-second-module).

## Lägg till och konfigurera den andra modulen

1. Klicka på den partiella cirkeln till höger om modulen till **[!UICONTROL Add another module]**.

   Den andra modulen måste vara en [!DNL Workfront]-modul, men appen [!DNL Workfront] lästes inte in i förväg.

1. Om du vill hitta appen [!DNL Workfront] börjar du skriva [!DNL Workfront] och klickar på appen när den visas.
1. Klicka på **[!UICONTROL Create Record]** i listan med [!DNL Workfront] moduler som visas.

1. Precis som du gjorde tidigare med Google Sheets-appen klickar du på **[!UICONTROL Add]** i rutan [!DNL Workfront] för att lägga till en anslutning mellan Workfront Fusion och Workfront.

   Nu ska vi börja specificera vad vi vill göra med data från kalkylbladet.

1. Klicka på **[!UICONTROL Record type]** och välj sedan **[!UICONTROL Project]** eftersom vi vill skapa ett projekt i [!DNL Workfront] med en rad från kalkylbladet.

   >[!TIP]
   >
   >Du kan hitta **[!UICONTROL Project]** i listan om du börjar skriva ordet [!UICONTROL project].

   Rutan expanderas och visar alla tillgängliga [!DNL Workfront]-projektfält där du kan skicka information som hittas av den första modulen.

   Vi ska använda fältet **[!UICONTROL Name]**: vi vill att den här modulen ska namnge varje projekt i [!DNL Workfront] med texten i motsvarande [!UICONTROL Google Sheets]-rad.

1. Sök och klicka på fältet **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F**([!DNL Windows] OS) för att snabbt hitta ett fält.

   Då öppnas en lista med variabler som du kan använda i fältet **[!UICONTROL Name]** för att definiera namnet på varje projekt som skapas i Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Observera att variablerna i den övre delen av listan motsvarar kolumnrubrikerna i kalkylbladet.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Klicka på variabeln **[!UICONTROL My Project Name (A)]** för att lägga till den i fältet **[!UICONTROL Name]**.

   Du har just mappat din första datadel för det här scenariot.

   Låt oss mappa ytterligare en datadel från kalkylbladet till [!DNL Workfront]: startdatumet för varje projekt.

1. Sök och klicka på fältet **[!UICONTROL Planned Start Date]** och klicka sedan på variabeln **[!UICONTROL Planned Begin Date (E)]** för att hämta data från den kolumnen i kalkylbladet.

1. Klicka på **[!UICONTROL OK]**.

   Nu har du ett fungerande scenario.

1. Ge den andra modulen ett namn som&quot;Skapa Workfront-projekt&quot; och fortsätt sedan med [Testa scenariot](#test-the-scenario).

## Testa scenariot

Innan du aktiverar ditt scenario är det viktigt att du testar det genom att köra det minst en gång och visa resultatet. Detta hjälper er att förstå hur data flödar genom scenariot och hitta eventuella fel.

Vi valde att låta 1 rad från kalkylbladet bearbetas för att skapa ett projekt i Workfront. Om du kör scenariot är det vad som ska hända.

1. Klicka på **[!UICONTROL Run once]** i det nedre vänstra hörnet i scenarioredigeraren.
1. När scenariot är klart klickar du på bubblan ovanför modulen [!DNL Google Sheets].

   ![](assets/click-bubble.png)

   I den ruta som visas kan du visa information om det datapaket som modulen har bearbetat, inklusive faktiska data som hämtats från kalkylbladet för raden som du började med.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Klicka på bubblan i körningskontrollen ovanför modulen [!DNL Workfront] för att visa indata och utdata, vilket är ID:t för det projekt som nu skapas i [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Du kan läsa mer om hur du läser information om körning av scenarier i följande artiklar:

   * Allmän information finns i [Körningsflöde för scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Mer information om bearbetade paket finns i [Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Gå till [!DNL Workfront] och sök efter &quot;soho downtown loft&quot; för att se projektet som scenariot skapade. Detta var den sista raden i kalkylbladet.
1. I [!DNL Workfront Fusion] klickar du på **[!UICONTROL Save]** ![](assets/save-icon.png) i det nedre vänstra hörnet för att spara förloppet för scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

## Slutför scenariot och testa det igen

Vi måste fortfarande konfigurera scenariot för att skapa projekt för alla andra rader i kalkylbladet.

1. Klicka på modulen **[!UICONTROL Watch Rows]** som du skapade för Google-blad.
1. Ändra **[!UICONTROL Limit]** till 100.

   Om du anger ett tal som är högre än det antal rader som du vet finns i kalkylbladet, innebär det att alla rader kommer att registreras.

1. Högerklicka på modulen **[!UICONTROL Watch Rows]**, klicka på **[!UICONTROL Choose where to start]**, klicka på **[!UICONTROL All]** och sedan på **[!UICONTROL OK]**.

1. Klicka på **[!UICONTROL Run once]** och se vad som händer i körningskontrollen.

   Modulen [!DNL Google] Blad **[!UICONTROL Watch Rows]** körs en gång för att läsa alla rader. Därefter körs Workfront **[!UICONTROL Create Record]**-modulen 20 gånger för att skapa ett projekt för var och en av de återstående 20 raderna i kalkylbladet.

1. Klicka på exekveringskontrollbubblan för modulen [!DNL Workfront] om du vill visa alla 20 åtgärder. Klicka sedan på en av åtgärderna om du vill visa information om det projekt som skapats.
1. Klicka på **[!UICONTROL Save]** ![](assets/save-icon.png) nära det nedre vänstra hörnet.
1. Gå till [!DNL Workfront] om du vill se de projekt som scenariot har skapat.

>[!TIP]
>
>Vi rekommenderar den valfria men användbara metoden att lägga till anteckningar om varje modul.
>
>1. Högerklicka på modulen [!DNL Workfront] och klicka sedan på **[!UICONTROL Add a note]**.
>1. Skriv en översikt för modulen i anteckningen som visas.
>
>    Detta är praktiskt eftersom du inte behöver öppna modulen hela tiden för att se vad den gör. Du kan skriva något som &quot;Skapar ett projekt med namnet, planerat startdatum och prioritet mappat från kalkylbladet&quot;.
>
>    För modulen [!UICONTROL Google Sheets] kan du skriva &quot;Bevakade projektlistor för nya rader/projekt som lagts till&quot;.
>
>    Du kan lägga till flera anteckningar för en modul.
>
>1. Stäng området **[!UICONTROL Notes]**.
>
>    När du har lagt till en anteckning i ett scenario visas en orange punkt på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) längst ned i scenarioredigeraren.
>
>1. Klicka på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) för att visa dina anteckningar.
>



## Aktivera scenariot

Om det här vore ett scenario som du skulle använda för verkliga data, skulle du först aktivera det. När du har aktiverat ett scenario körs det som standard var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta du vill att det ska köras.

Mer information om att aktivera scenarier finns i [Aktivera eller inaktivera ett scenario i Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Mer information om scheman finns i [Schemalägg ett scenario i Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
