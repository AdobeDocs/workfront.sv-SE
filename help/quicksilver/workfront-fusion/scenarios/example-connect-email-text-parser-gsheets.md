---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Exempel på ett Adobe Workfront Fusion-scenario: Koppla e-post, Textparser och Google Sheets'
description: Med det här scenariot kan du skapa en logg över alla e-postmeddelanden och tagga dem för ytterligare åtgärder i ett kalkylblad. Den hämtar e-postinnehåll i två separata tabeller i ett kalkylblad med Reguljära uttryck (Regex) som sökmönster. Det första mönstret söker efter en fras och det andra söker efter samma fras och en e-postadress.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 0%

---

# Exempel på [!DNL Adobe Workfront Fusion]-scenario: Anslut e-post, [!UICONTROL Text Parser] och [!DNL Google Sheets]

Med det här scenariot kan du skapa en logg över alla e-postmeddelanden och tagga dem för ytterligare åtgärder i ett kalkylblad. Den hämtar e-postinnehåll i två separata tabeller i ett kalkylblad med Reguljära uttryck (Regex) som sökmönster. Det första mönstret söker efter en fras och det andra söker efter samma fras och en e-postadress.

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

## Förutsättningar

Den här självstudien kräver grundläggande kunskaper i reguljära uttryck. Mer information om Regex finns på [https://regexone.com](https://regexone.com/).

Lägg till den första modulen och konfigurera den

1. Sök efter e-post och välj **[!UICONTROL Watch emails]** som utlösare.

   >[!NOTE]
   >
   >Du kan ansluta ett [!DNL Google]-konto med epostmodulen, men du kan också använda en [!DNL Gmail]-modul.

1. Anslut antingen ett [!DNL Google]-konto eller någon annan IMAP-baserad e-postklient (till exempel [!DNL Outlook]).
1. När du är ansluten väljer du en mapp vars inkommande e-postmeddelanden du vill bevaka, till exempel [!UICONTROL Inbox].
1. Under [!UICONTROL Criteria] väljer du **[!UICONTROL All email]** (eller begränsa den till att läsa eller läsa olästa e-postmeddelanden).

   Du kan också markera hämtade e-postmeddelanden som lästa eller olästa.

1. Ange [!UICONTROL Maximum number of results] till 1.

   ![](assets/save-max-as-1-350x304.png)

   Du kan ändra detta baserat på den mängd meddelanden du får. Vi rekommenderar dock att du anger ett lågt värde och kör scenariot oftare.

1. Klicka på **[!UICONTROL Show advanced settings]** längst ned.

   ![](assets/show-adv-settings-350x332.png)

1. Filtrera e-postmeddelanden efter [!UICONTROL Sender address], [!UICONTROL Subject] och [!UICONTROL Phrase].

   Detta ger er möjlighet att endast titta på relevanta e-postmeddelanden. I det här exemplet har vi bara lagt till ett ämnesfilter och lämnat de andra två tomma.

   >[!NOTE]
   >
   >Vi ska lägga till en router för att söka efter fraser i ett e-postmeddelande med hjälp av iteratorn [!UICONTROL Match Pattern] och ett reguljärt uttryck (Regex) som sökmönster. Detta gör det även möjligt för oss att skapa ett flerfunktionsscenario.

1. När konfigurationen är klar och du uppmanas att ange var du vill börja titta på dina e-postmeddelanden klickar du på **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Fortsätt till [Sök efter [!UICONTROL Flow Control] och lägg till en [!UICONTROL Router]](#search-for-flow-control-and-add-a-router)

## Sök efter [!UICONTROL Flow Control] och lägg till en [!UICONTROL Router]

1. Lägg till en router efter en modul för att dela eller duplicera data innan du skickar dem till nästa modul.

   Här har vi använt en [!UICONTROL Router] för att skicka brödtexten för e-post till två separata tabeller i en [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Använd modulen [!UICONTROL Text Parser]

1. Lägg till en [!UICONTROL Match Pattern]-transformator om du vill söka efter en fras i ett e-postmeddelande.

   Vi söker efter frasen [!UICONTROL text parser module] i alla inkommande e-postmeddelanden för att fånga brödtexten och avsändarens namn på de som matchar frasen.

   1. Skriv mönstret som ett reguljärt uttryck:

      text\sparser\smodul

   1. (Valfritt) Använd något av de andra mönsteralternativen.

      ![](assets/pattern-350x318.png)

      Flera rader är användbara om texten innehåller flera rader och du behöver söka efter mönstret på varje rad. I den här självstudiekursen måste vi söka efter mönstret i hela brödtexten i e-postmeddelandet, så vi lämnar det omarkerat.

   1. Klicka på attributet **Textinnehåll** i listan i fältet [!UICONTROL Text].

      ![](assets/text-content-350x264.png)

      Det här är attributet som lagrar texten från e-postbrödtexten där vi ska söka efter mönstret.

1. Lägg till ytterligare [!UICONTROL Match Pattern] som söker efter samma fras och en e-postadress.

   Detta är särskilt användbart om du har kundkonton hos flera användare. Om du vill spara tid kan du klona modulen [!UICONTROL Text Parser] som du nyss skapade och länka den till routern.

   ![](assets/clone.png)

1. Redigera mönstret på följande sätt:

   text\sparser\smodul.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Det här mönstret söker efter frasen [!UICONTROL text parser module] och en e-postadress som john.doe@gmail.com och returnerar bara e-postadressen.

   >[!NOTE]
   >
   >Det är viktigt att du skriver regex i enlighet med specifikationen för de e-postadresser som du godkänner, men den ovan tar hand om de flesta vanliga e-postadresser.

   * Om du bara vill söka efter e-postadresser kan du använda regex nedan:

     ([\w.-]+@[\w.-]+)

   * Du kan också söka enbart efter telefonnummer med regex nedan:

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d,4}
Ovanstående mönster omfattar de vanligaste formaten där ett telefonnummer skrivs.

   Vi rekommenderar att du använder [[!DNL https://regex101.com]](https://regex101.com/) med [!DNL javascript] som Flash för att testa dina mönster.

   Resten av konfigurationen är densamma som den tidigare.

## Lägg till modulerna [!DNL Google Sheets]

För [!DNL Sheets] måste vi först skapa ett kalkylblad med de nödvändiga rubrikerna.

1. Skapa ett kalkylblad med de kolumner som du vill hämta användardata från. (Du kan använda en befintlig fil också).

   Skapa till exempel en som heter&quot;E-postdata: supportbiljett&quot; med avsändarens namn, avsändarens e-postinnehåll och e-postinnehåll som kolumner. Ge kalkylbladet namnet&quot;innehåller: textparsermodul.&quot;

1. Lägg till modulen [!UICONTROL Google Sheets] med **[!UICONTROL Add a row]** som åtgärd.

   ![](assets/add-a-row-350x174.png)

1. Anslut ditt [!DNL Google]-konto (om du inte redan har det). Välj den fil du skapade tidigare och välj sedan det kalkylblad i vilket du hämtar data.

   Din konfiguration bör se ut så här:

   ![](assets/connect-google-acct-350x279.png)

1. Mappa attributen i relevanta fält (kolumner) för att slutföra modulinställningarna.

   ![](assets/map-attributes-350x282.png)

1. Klona modulen som du nyss skapade och länka den till den andra [!UICONTROL Text Parser]-modulen.

   1. Gå till ditt kalkylblad, duplicera det kalkylblad du skapade tidigare och ge det ett namn.

      Ge den till exempel namnet&quot;innehåller: textanalysmodul och e-post&quot;.

   1. Lägg till en annan kolumn för att lagra e-postadressen som e-postbrödtexten innehåller.

      Ge det till exempel namnet&quot;E-postadress delad&quot;.

   1. Klicka på den klonade modulen [!DNL Google Sheets] för att konfigurera inställningarna.
   1. Ändra kalkylbladet till det nya som du just skapade.
   1. Mappa utdata från modulen [!UICONTROL Match Pattern] ($1) till den kolumn där du vill lagra e-postadressen (delad e-postadress).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Klicka på **[!UICONTROL OK]**, spara scenariot och ta det för en testkörning.

      Du måste skicka två separata e-postmeddelanden till den anslutna e-postadressen enligt följande:

      * Innehåller frasen [!UICONTROL text parser module] (och ingen e-postadress)

        ![](assets/text-parser-module-350x103.png)

      * Innehåller frasen ovan och en e-postadress

        ![](assets/above-phrase-and-email-350x106.png)

        Om det inte finns några fel i konfigurationen kommer du att se att det första kalkylbladet hämtar alla e-postmeddelanden som innehåller frasen [!UICONTROL text parser module], medan det andra kalkylbladet endast hämtar de som innehåller frasen [!UICONTROL text parser module] och en e-postadress. Se skärmbilderna nedan.

        Kalkylblad 1:

        ![](assets/worksheet-1-350x57.png)

        Kalkylblad 2:

        ![](assets/worksheet-2-350x41.png)

## Resurs

* [Kostnadsfria övningar](https://regexone.com/) om du vill veta mer om reguljära uttryck
* [Läs mer om matchning av telefonnummer](https://regexone.com/problem/matching_phone_numbers) med Regex
* [Läs mer om matchning av e-post](https://regexone.com/problem/matching_emails) med Regex
* [Testa reguljära uttryck](https://regex101.com/)
