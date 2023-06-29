---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Skapa en metod för automatisering i [!DNL Adobe Workfront Fusion]
description: I den här artikeln beskrivs hur du skapar ett automatiseringsscenario med Adobe Workfront Fusion. Automatiseringsscenarier automatiserar Workfront-processer, inklusive datamanipulering och -omvandling. Det här exemplet tar dig genom processen att skapa ett scenario som söker efter ett projekt och sedan returnerar alla uppgifter som är kopplade till det projektet.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# Skapa en metod för automatisering i [!DNL Adobe Workfront Fusion]

I den här artikeln beskrivs hur du skapar ett automatiseringsscenario med Adobe Workfront Fusion. Automatiseringsscenarier automatiserar Workfront-processer, inklusive datamanipulering och -omvandling. Det här exemplet tar dig genom processen att skapa ett scenario som söker efter ett projekt och sedan returnerar alla uppgifter som är kopplade till det projektet.

Instruktioner om hur du skapar ett integreringsscenario som ansluter separata program finns i [Skapa ett scenario för praktikintegrering i Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Mer information om vilka funktioner som finns för respektive Workfront Fusion-licens finns i [Adobe Workfront Fusion-licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

## Skapa ett övningsscenario

Rollen för [!DNL Adobe Workfront Fusion] är att automatisera processerna så att ni kan koncentrera er på nya uppgifter i stället för att upprepa samma uppgifter om och om igen. Det fungerar genom att länka åtgärder inom och mellan program och tjänster för att skapa ett scenario som överför och omvandlar data automatiskt. Scenariot du skapar letar efter data i en app eller tjänst och bearbetar data för att ge det resultat du vill ha.

Ett scenario består av en serie moduler som anger hur data ska omvandlas i en app eller överföras mellan program och webbtjänster.
Det här exemplet tar dig igenom processen att skapa ett scenario som söker efter en [!DNL Workfront] och returnerar uppgifterna i projektet.

![](assets/create-practice-scenario-wf-only-350x157.png)

Att skapa ett scenario består av flera huvuduppgifter:

## Välj program och ge scenariot ett namn

1. Logga in på [!DNL Workfront Fusion] konto.
1. Klicka **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen.

   >[!NOTE]
   >
   >Om den vänstra navigeringspanelen eller dess ikoner inte visas klickar du på menyn ![Meny](assets/main-menu-icon-left-nav.png) ikon.

   I grått [!UICONTROL Folders] som visas kan du ordna dina scenarier i mappar.

   Överst i huvudområdet till höger kan du visa **[!UICONTROL All]** scenarier du har skapat, **[!UICONTROL Active Scenarios]**, **[!UICONTROL Inactive Scenarios]** och **[!UICONTROL Concepts]**. Koncept är scenarier som kräver mer arbete innan [!DNL Workfront Fusion] kan klassificera dem som aktiva eller inaktiva.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. I [!UICONTROL Folders] klickar du på **[!UICONTROL Add folder]** icon ![](assets/add-folder-icon.png)skriver du sedan in ett namn som&quot;Practice scenarios&quot; för den första mappen.

1. Öppna mappen och klicka sedan på **[!UICONTROL Create a new scenario]** i det övre högra hörnet på sidan.

   På landningssidan som visas kan du förhandsladda alla appar som du vill använda i det scenario som du tänker skapa.

1. Sök efter och välj **[!DNL Workfront]** app.
1. Klicka **[!UICONTROL Continue]** i det övre högra hörnet.

   Scenarioredigeraren visar, som innehåller en tom modul i mitten, [!DNL Workfront] som du har förinstallerat och vissa alternativ i verktygsfältet längst ned.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

När du börjar skapa ett nytt scenario är det en bra idé att börja med att skapa ett namn för det.

1. Välj **[!UICONTROL New scenario]** platshållarnamn i det övre vänstra hörnet och skriv sedan ett namn som &quot;Practice scenarios 1.&quot;
1. Fortsätt med [Lägg till och konfigurera den första modulen](#add-and-configure-the-first-module) nedan.

## Lägg till och konfigurera den första modulen

Den tomma modulen med ett frågetecken representerar den utlösarmodul som du behöver lägga till. Modulen startar scenariot varje gång det körs. Klockikonen på den tomma modulen anger att det är en schemalagd modul.

![](assets/empty-module.png)

Den här modulen innehåller de data som du vill att scenariot ska bevakas för.

I det här exemplet använder vi inte någon utlösarmodul. I stället börjar det här scenariot med en sökning.

1. Klicka på den tomma modulen för att välja det program du vill välja en modul från.

   Programmet som du förinstallerade visas bredvid den tomma modulen. Du kan lägga till andra appar som har moduler med [!UICONTROL Search] box.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Klicka på **[!DNL Workfront]**.

   Listan ändras och visar alla [!DNL Workfront] moduler som du kan använda som utlösarmodul.

1. Klicka på modulen Sök **[!UICONTROL Search]**.

   Nu måste du skapa en autentiserad anslutning till [!DNL Workfront] konto. Alla moduler som du lägger till i ett scenario måste ha en anslutning till dess program.

1. I **[!DNL Workfront]** ruta, under **[!UICONTROL Connection]**, klicka **[!UICONTROL Add]** och skriv sedan ett namn för anslutningen, till exempel&quot;Olivias Workfront-konto&quot;, och klicka sedan på **[!UICONTROL Continue]**.
1. Autentisera anslutningen i fönstret som visas.

   Processen för att autentisera en anslutning kan variera lite mellan olika program. Följande process är specifik för [!DNL Workfront], men processen liknar många program.

   1. Ange [!DNL Workfront] domän, klicka sedan på **[!UICONTROL Continue]**.
   1. Logga in [!DNL Workfront].
   1. Undersök åtkomsten som [!DNL Workfront Fusion] begär och klickar sedan på **[!UICONTROL Allow Access]**.

   Om du behöver hjälp, se [Om att ansluta [!DNL Adobe Workfront Fusion] till en app eller tjänst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Konfigurera den första modulen

När du har anslutit [!DNL Workfront Fusion] till [!DNL Workfront] kan du ange ett [!DNL Workfront] begärandekö som du har åtkomst till och de data där som du vill att den första modulen ska bearbeta.

1. I [!UICONTROL Record Type] ruta, markera **[!UICONTROL Project]**. Detta ställer in modulen så att endast projekt söks igenom.

   >[!TIP]
   >
   >Du kan hitta **[!UICONTROL Project]** i listan om du börjar skriva ordet[!UICONTROL project].&quot;

1. I **[!UICONTROL Result Set]** ruta, markera **[!UICONTROL First Matching Record]**. Detta ställer in modulen så att endast den första posten som uppfyller villkoren returneras. I det här exemplet behöver bara en post returneras.
1. I **[!UICONTROL Search criteria]** ska vi skapa ett filter för att returnera det specifika projektet.

   1. I den första rutan under [!UICONTROL Search Criteria]markerar du det fält som du vill söka i. I det här exemplet väljer du **[!UICONTROL Name]**.
   1. För operatorn väljer du [!UICONTROL Contains (case insensitive)]. Detta gör att modulen kan hitta projekt med de valda orden i namnet, även om du inte anger hela namnet eller anger namnet med fel skiftläge (till exempel versaler).
   1. I det sista fältet under [!UICONTROL Search Criteria], anger du ett ord eller en fras som du vet finns i namnet på det projekt du söker efter.

1. I **[!UICONTROL Outputs]** markerar du de fält som du vill att utgåvan ska visa. I det här exemplet väljer du **[!UICONTROL ID]** och **[!UICONTROL Name]** fält.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F** ([!DNL Windows] OS) för att snabbt hitta ett fält.

1. Klicka på **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Endast information) Eftersom det här inte är en utlösarmodul väljer du inte var den ska startas. När du använder en utlösarmodul väljer du nu var den ska startas.
   >
   >
   >Mer information finns i [Välj var en utlösarmodul ska börja i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Högerklicka på modulen och klicka på **[!UICONTROL Rename]** skriver du ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Sök efter projekt&quot;) och klickar sedan på **[!UICONTROL OK]**.

   Namnet visas precis nedanför modulen. Under den, [!DNL Workfront Fusion] innehåller en kort beskrivning av den typ av åtgärd som modulen utför.

   ![](assets/module-renamed-wf.png)

1. Fortsätt med [Lägg till och konfigurera den andra modulen](#add-and-configure-the-second-module).

## Lägg till och konfigurera den andra modulen

1. Klicka på den partiella cirkeln till höger om modulen för att **[!UICONTROL Add another module]**.
1. Välj [!DNL Workfront] i listan över program och välj sedan sökmodulen **[!UICONTROL Read Related Records]**.
1. Du har redan skapat en anslutning till [!DNL Workfront] för föregående modul. Du behöver inte skapa den igen här, men du måste se till att den här modulen använder samma anslutning som den föregående modulen.\
   I **[!UICONTROL Connection]** markerar du anslutningen som du skapade för föregående modul.
1. Klicka **[!UICONTROL Record type]** väljer **[!UICONTROL Project]**, eftersom vi vill läsa poster som hör till ett projekt.

   >[!TIP]
   >
   >Du kan hitta **[!UICONTROL Project]** i listan om du börjar skriva ordet &quot;project&quot;.

1. Klicka på **[!UICONTROL Parent Record ID]** fält. Det här fältet kräver Workfront-id:t för det projekt som du vill returnera uppgifter från.

   När du klickar på fältet öppnas en lista med variabler som du kan använda i **[!UICONTROL Parent Record ID]** för att identifiera projektet i Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klicka på variabeln **[!UICONTROL ID]** för att lägga till den i **[!UICONTROL Parent Record ID]** fält. Detta gör att det ID som returneras från den första modulen kan användas som identifierare för det projekt som du vill arbeta med i den andra modulen, vilket ser till att de returnerade uppgifterna tillhör det projektet.
1. I **[!UICONTROL Collections]** fält, markera **[!UICONTROL Tasks]**. Detta anger att modulen ska returnera uppgifter som är kopplade till det valda projektet.
1. Klicka på **[!UICONTROL OK]**

   Nu har du ett fungerande scenario.

1. Ge den andra modulen ett namn som&quot;Returuppgifter associerade med projekt&quot; och fortsätt sedan med [Testa scenariot](#test-the-scenario).

## Testa scenariot

Innan du aktiverar ditt scenario är det viktigt att testa det genom att köra det minst en gång och visa resultatet. Detta hjälper er att förstå hur data flödar genom scenariot och hitta eventuella fel.

Vi valde att få 1 projekt tillbaka, liksom de uppgifter som är kopplade till det projektet. Om du kör scenariot är det vad som ska hända.

1. Klicka **[!UICONTROL Run once]** i det nedre vänstra hörnet av scenarioredigeraren.
1. När scenariot är klart klickar du på bubblan ovanför den första modulen.

   ![](assets/click-bubble.png)

   I rutan som visas kan du visa information om det datapaket som modulen har bearbetat, inklusive faktiska data som hämtats från projektet som modulen returnerade.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klicka på exekveringspanelen ovanför den andra modulen för att visa indata och utdata, som är en samling uppgifter som finns i projektet.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Du kan läsa mer om hur du läser information om körning av scenarier i följande artiklar:

   * Allmän information finns i [Scenariokörningsflöde i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Mer information om bearbetade paket finns i [Körning av scenarier, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. I [!DNL Workfront Fusion], klicka **[!UICONTROL Save]** ![](assets/save-icon.png) nära det nedre vänstra hörnet för att spara dina framsteg i scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

>[!TIP]
>
>Vi rekommenderar den valfria men användbara metoden att lägga till anteckningar om varje modul.
>
>1. Högerklicka på en [!DNL Workfront] och sedan klicka på **[!UICONTROL Add a note]**.
>1. Skriv en översikt för modulen i anteckningen som visas.
>
>    Du kan lägga till flera anteckningar för en modul.
>
>1. Stäng **[!UICONTROL Notes]** område.
>
>     När du har lagt till en anteckning i ett scenario visas en orange punkt på **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) längst ned i scenarioredigeraren.
>
>1. Klicka på **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) för att visa dina anteckningar.
>



## Aktivera scenariot

Det här exempelscenariot har ingen utlösarmodul. Om detta vore ett scenario som du skulle använda för riktiga data skulle det börja med en utlösarmodul, och det sista du skulle göra är att aktivera den. När du har aktiverat ett scenario körs det som standard var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta du vill att det ska köras.

Mer information om att aktivera scenarier finns i [Aktivera eller inaktivera ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Mer information om scheman finns i [Schemalägg ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
