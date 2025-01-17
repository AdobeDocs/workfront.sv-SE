---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Skapa ett scenario för övningsautomatisering i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1482'
ht-degree: 0%

---

# Skapa ett scenario för övningsautomatisering i [!DNL Adobe Workfront Fusion]

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

Automatiseringsscenarier automatiserar Workfront-processer, inklusive datamanipulering och -omvandling. I den här artikeln beskrivs hur du skapar ett scenario som söker efter ett projekt och sedan returnerar alla uppgifter som är kopplade till det projektet.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront</td>  
      <td>Alla</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-licens</td>  
      <td>
        Nytt: Standard<br>
        Eller<br>
        Aktuell: Arbete eller högre
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-licens</td>  
      <td> 
        Aktuell: Inga Workfront Fusion-licenser krävs.<br>
        Eller<br>
        Äldre: Alla
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Nytt: Välj eller Prime Workfront Plan: Din organisation måste köpa Adobe Workfront Fusion.<br>
        Ultimate Workfront Plan: Workfront Fusion ingår.<br>
        Eller<br>
        Aktuell: Din organisation måste köpa Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Skapa ett scenario för automatisering

[!DNL Adobe Workfront Fusion] hjälper dig att fokusera på viktiga uppgifter genom att automatisera repetitiva uppgifter. Det skapar scenarier som automatiskt hanterar data i olika program och tjänster.

Varje scenario består av moduler, som vägleder hur data behandlas i en app eller överförs mellan olika program och tjänster. Du kan till exempel skapa ett scenario i Fusion för att automatiskt hitta ett [!DNL Workfront]-projekt och visa dess uppgifter. På så sätt sparar Fusion tid och kraft genom att hantera rutinuppgifter.

Det här scenariot tar dig genom processen att skapa ett scenario som söker efter ett [!DNL Workfront]-projekt och returnerar aktiviteterna i projektet.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Innan du börjar

Skapa ett projekt med aktiviteter i förgrunden som du kan använda för den här övningen. Du behöver inte göra någon ytterligare konfiguration förutom att lägga till uppgifter i projektet.

Mer information om hur du skapar ett projekt i Workfornt finns i xxx.

### 1. Skapa och namnge scenariot

1. Logga in på ditt [!DNL Workfront Fusion]-konto.
1. Klicka på **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen.

   >[!NOTE]
   >
   >Om den vänstra navigeringspanelen eller dess ikoner inte visas klickar du på ikonen ![Meny](assets/main-menu-icon-left-nav.png) .

1. Klicka på ikonen **[!UICONTROL Add folder]** ![](assets/add-folder-icon.png) på panelen [!UICONTROL **Mappar**] och skriv sedan ett namn som &quot;Practice scenarios&quot; för den första mappen.

1. Öppna mappen och klicka sedan på **[!UICONTROL Create a new scenario]** i det övre högra hörnet på sidan.

1. För den här övningen väljer du appen **[!DNL Adobe Workfront]** och klickar sedan på **Sök** längst ned.


1. Markera platshållarnamnet **[!UICONTROL New scenario]** i det övre vänstra hörnet och skriv sedan ett namn som &quot;Practice scenarios 1&quot;.

   ![](assets/name-the-scenario.png)

1. Fortsätt med [Anslut den första modulen](#2-connect-the-first-module) nedan.

### 2. Anslut den första modulen

Nu måste du upprätta en autentiserad anslutning till ditt [!DNL Workfront]-konto. Alla moduler som du lägger till i ett scenario måste ha en anslutning till dess program.

1. I rutan **[!DNL Workfront]**, under **[!UICONTROL Connection]**, klickar du på **[!UICONTROL Add]** och anger sedan ett namn för anslutningen, till exempel&quot;Olivias Workfront-konto&quot;. Klicka sedan på **[!UICONTROL Continue]**.
1. Autentisera anslutningen i fönstret som visas.

   Processen för att autentisera en anslutning kan variera lite mellan olika program. Följande process är specifik för [!DNL Workfront], men processen liknar många appar:

   1. Ange din [!DNL Workfront]-domän och klicka sedan på **[!UICONTROL Continue]**.
   1. Logga in på [!DNL Workfront].
   1. Undersök den åtkomst som [!DNL Workfront Fusion] begär och klicka sedan på **[!UICONTROL Allow Access]**.

   Om du behöver hjälp kan du läsa [Anslutningsöversikt](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Konfigurera den första modulen

När du har anslutit [!DNL Workfront Fusion] till ditt [!DNL Workfront]-konto kan du ange ett [!DNL Workfront]-projekt som du har åtkomst till och de data som du vill att den första modulen ska bearbeta.

1. Välj **[!UICONTROL Project]** i rutan [!UICONTROL Record Type]. Detta anger att modulen endast ska söka efter projekt.

   >[!TIP]
   >
   >Du kan hitta **[!UICONTROL Project]** i listan om du börjar skriva ordet [!UICONTROL project].

1. Välj **[!UICONTROL First Matching Record]** i rutan **[!UICONTROL Result Set]**. Detta ställer in modulen så att endast den första posten som uppfyller villkoren returneras. I det här exemplet behöver bara en post returneras.
1. I området **[!UICONTROL Search criteria]** skapar vi ett filter som returnerar det specifika projektet:

   | Fält | Åtgärd |
   |--------|-------------|
   | Sökkriteriefält | Markera fältet som du vill söka efter värdena i. I det här exemplet väljer du **[!UICONTROL Name]**. |
   | Sökvillkor | Välj **[!UICONTROL Name]** i den första listrutan. |
   | Grundläggande operatorer | Välj [!UICONTROL Contains (case insensitive)] i den andra listrutan. Detta gör att modulen kan hitta projekt med de valda orden i namnet, även om du inte anger hela namnet eller anger namnet med fel skiftläge (till exempel versaler). |
   | Textruta | Ange ett ord eller en fras som du vet finns i namnet på det projekt du söker efter. |

+++ Expandera om du vill visa ett exempel på skärmen.
   ![](assets/search-name.png)
+++

1. I listan **[!UICONTROL Outputs]** markerar du de fält som du vill att modulen ska visa. I det här exemplet väljer du fälten **[!UICONTROL ID]** och **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Du kan använda **Cmd+F** ([!DNL Mac] OS) eller **Ctrl-F** ([!DNL Windows] OS) för att snabbt hitta ett fält.

1. Klicka på **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Eftersom det här inte är en utlösarmodul väljer du inte var den ska startas. När du använder en utlösarmodul väljer du nu var den ska startas.
   >
   >
   >Mer information finns i [Välja var en utlösarmodul ska börja i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Högerklicka på modulen, klicka på **[!UICONTROL Rename]**, skriv ett namn som beskriver vad du vill att modulen ska göra (till exempel&quot;Sök efter projekt&quot;) och klicka sedan på **[!UICONTROL OK]**.

   Namnet visas precis nedanför modulen. Under det finns en kort beskrivning av den typ av åtgärd som har utförts av modulen i [!DNL Workfront Fusion].

   ![](assets/module-renamed-wf.png)

1. Fortsätt med [Lägg till och konfigurera den andra modulen](#add-and-configure-the-second-module).

### 4. Lägg till och konfigurera den andra modulen

1. Klicka på den partiella cirkeln till höger om modulen till **[!UICONTROL Add another module]**.
1. Välj [!DNL Workfront] i listan med program och välj sedan sökmodulen **[!UICONTROL Read Related Records]**.
1. I rutan **[!UICONTROL Connection]** markerar du anslutningen som du skapade för den tidigare modulen. Du måste se till att den här modulen använder samma anslutning som den tidigare modulen.
1. Klicka på **[!UICONTROL Record type]** och välj sedan **[!UICONTROL Project]** eftersom vi vill läsa poster som är relaterade till ett projekt.

   >[!TIP]
   >
   >Du kan hitta **[!UICONTROL Project]** i listan om du börjar skriva ordet &quot;project&quot;.

1. Klicka på fältet **[!UICONTROL Parent Record ID]**. Det här fältet kräver Workfront-id:t för det projekt som du vill returnera uppgifter från.

   När du klickar på fältet öppnas en lista med variabler som du kan använda i fältet **[!UICONTROL Parent Record ID]** för att identifiera projektet i Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klicka på variabeln **[!UICONTROL ID]** för att lägga till den i fältet **[!UICONTROL Parent Record ID]**. Detta gör att det ID som returneras från den första modulen kan användas som identifierare för det projekt som du vill arbeta med i den andra modulen, vilket ser till att de returnerade uppgifterna tillhör det projektet.
1. Välj **[!UICONTROL Tasks]** i fältet **[!UICONTROL Collections]**. Detta anger att modulen ska returnera uppgifter som är kopplade till det valda projektet.
1. I fältet **[!UICONTROL Outputs]** väljer du **[!UICONTROL Id]** och **[!UICONTROL Name]**.
1. Klicka på **[!UICONTROL OK]**

   Nu har du ett fungerande scenario.

1. Ge den andra modulen ett namn som&quot;Returnera aktiviteter som är associerade med projektet&quot; och fortsätt sedan med [Testa scenariot](#test-the-scenario).

## Testa scenariot

Innan du aktiverar ditt scenario är det viktigt att du testar det genom att köra det minst en gång och visa resultatet. Detta hjälper er att förstå hur data flödar genom scenariot och hitta eventuella fel.

Vi valde att få 1 projekt tillbaka, liksom de uppgifter som är kopplade till det projektet. Om du kör scenariot är det vad som ska hända.

1. Klicka på **[!UICONTROL Run once]** i det nedre vänstra hörnet i scenarioredigeraren.
1. När scenariot är klart klickar du på bubblan ovanför den första modulen.

   ![](assets/click-bubble.png)

   I rutan som visas kan du visa information om det datapaket som modulen har bearbetat, inklusive faktiska data som hämtats från projektet som modulen returnerade.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klicka på exekveringspanelen ovanför den andra modulen för att visa indata och utdata, som är en samling uppgifter som finns i projektet.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Du kan läsa mer om hur du läser information om körning av scenarier i följande artiklar:

   * Allmän information finns i [Körningsflöde för scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Mer information om bearbetade paket finns i [Scenariokörning, cykler och faser i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. I [!DNL Workfront Fusion] klickar du på **[!UICONTROL Save]** ![](assets/save-icon.png) i det nedre vänstra hörnet för att spara förloppet för scenariot.

   >[!IMPORTANT]
   >
   >Spara ofta när du finslipar ett scenario.

>[!TIP]
>
>Vi rekommenderar den valfria men användbara metoden att lägga till anteckningar om varje modul.
>
>1. Högerklicka på en [!DNL Workfront]-modul och klicka sedan på **[!UICONTROL Add a note]**.
>1. Skriv en översikt för modulen i anteckningen som visas.
>
>    Du kan lägga till flera anteckningar för en modul.
>
>1. Stäng området **[!UICONTROL Notes]**.
>
>     När du har lagt till en anteckning i ett scenario visas en orange punkt på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) längst ned i scenarioredigeraren.
>
>1. Klicka på ikonen **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) för att visa dina anteckningar.
>

## Aktivera scenariot

Det här exempelscenariot har ingen utlösarmodul. Om detta vore ett scenario som du skulle använda för riktiga data skulle det börja med en utlösarmodul, och det sista du skulle göra är att aktivera den. När du har aktiverat ett scenario körs det som standard var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta du vill att det ska köras.

Mer information om att aktivera scenarier finns i [Aktivera eller inaktivera ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Mer information om scheman finns i [Schemalägg ett scenario i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
