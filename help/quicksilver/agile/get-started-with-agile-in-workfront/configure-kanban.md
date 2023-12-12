---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Konfigurera Kanban
description: Du skapar ett kanban- eller Scrum-team i [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Kanban]

Du kan skapa ett smidigt team i [!DNL Adobe Workfront] enligt beskrivning i [Skapa ett smidigt team](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). När ni skapar ett smidigt team kan ni välja den metod som teamet använder för att slutföra arbetet. Du kan välja mellan följande alternativ:

* Scrum
* Kanban

I den här artikeln beskrivs hur du konfigurerar inställningarna för ett Kanban-team. När du har skapat ett smidigt team och valt Kanban-metod kan du uppdatera följande inställningar i den här artikeln:

* Om artiklarna beräknas i antal poäng eller timmar
* Statuskolumnerna på den flexibla artikelpanelen
* Ytterligare fält att visa på artikelkort på den flexibla artikelpanelen
* Gränsen för pågående arbete (PIA)
* Så här lägger du automatiskt till artiklar från eftersläpningen
* Hur långa kort stannar på Kanban-tavlan

Mer information om hur du konfigurerar ett Scrum-team finns i [Konfigurera Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

*Om du vill veta vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Konfigurera om artiklar ska beräknas i punkter eller timmar

Du kan konfigurera artiklar att beräknas med hjälp av punkter eller timmar.

Så här konfigurerar du hur berättelser beräknas för ditt team:

{{step1-to-team}}

1. Klicka på **[!UICONTROL Switch Teams]** icon ![](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökrutan.
1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** meny ![](assets/more-menu.png) väljer **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.\
   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** i **[!UICONTROL Estimate Stories in]** väljer du om du vill använda punkter eller timmar för att beräkna artikelns storlek (arbetsbelastning). Om du väljer Punkter anger du hur många timmar som ska vara lika med 1 punkt. (Standardvärdet är 1 punkt = 8 timmar.) Detta är antalet planerade timmar som läggs till i artikeln.

   **Exempel:** Om du har valt att uppskatta artiklar i punkter och 1 punkt är lika med 8 timmar, och en artikel beräknas till 3 punkter, läggs 24 planerade timmar till artikeln.

1. Klicka på **[!UICONTROL Save Changes]**.

## Konfigurera statuskolumner på den flexibla artikelpanelen

Du kan definiera de statusar som finns på artikeltavlan för det flexibla teamet. Det här är de enda statusvärdena som visas på artikelpanelen.

Så här definierar du de statusvärden som är tillgängliga för den artikelpanel som är kopplad till det flexibla teamet:

{{step1-to-team}}

1. Klicka på **[!UICONTROL Switch Teams]** icon ![Ikonen Byt team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** -avsnittet, leta upp **[!UICONTROL Story Board]** område.

1. (Valfritt) Klicka på **[!UICONTROL Add Column]** om du vill lägga till ytterligare en statuskolumn på artikelpanelen.
1. (Valfritt) Dra en statuskolumn med dra och släpp-indikatorn för att ändra ordningen på statuskolumnerna på artikelpanelen. Den första kolumnen kan inte flyttas och du kan inte dra en annan kolumn framför den första kolumnen.

   ![Dra och släpp](assets/agile-story-card-drag-and-drop.png)

1. Välj uppgiftsstatus.

   >[!IMPORTANT]
   >
   >Det går bara att välja låsta statusvärden som omfattar hela systemet. Du kan inte välja gruppspecifika statusar. Status för den första kolumnen motsvarar alltid **[!UICONTROL New]**.

   Du kan lägga till anpassade statusvärden om [!DNL Workfront] administratören har konfigurerat dem. Mer information finns i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicka på **[!UICONTROL Save Changes]**.

## Konfigurera ytterligare fält som ska visas på artikelkort på den flexibla artikelpanelen

När du lägger till fält i artikelkort är fälten skrivskyddade och visas endast när fältet fylls i.

Som standard visas följande typer av data på artikelkortet för uppgifter och problem:

* Artikelnamn med en länk direkt till uppgiften eller utgåvan
* Projektnamnet med en länk direkt till projektet
* Den här länken visas endast för artiklar, inte för underaktiviteter
* Uppgiften eller utgivningsbeskrivningen
* Aktuellt åtagande
* Visa och redigera procentandelen antingen genom att justera själva procentandelen eller genom att justera antalet punkter eller timmar som ska slutföras
* Tilldelade användare

Du kan visa ytterligare data (inklusive anpassade data) på artikelkort. Du kan visa ytterligare fält på artikelkort av någon anledning. Du kan till exempel visa kund-ID:t om du arbetar med artiklar för flera kunder i iteration, eller om du vill visa projektets startdatum eller projektavslutsdatum.

>[!NOTE]
>
>Om du använder ett anpassat fält på ett artikelkort kan det inte innehålla en punkt (eller punkt) i namnet.

Så här konfigurerar du artikelkort som tilldelats det flexibla teamet så att ytterligare fält visas:

{{step1-to-team}}

1. Klicka på **[!UICONTROL Switch Teams]** icon ![Ikonen Byt team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** anger du ett fältnamn för att hitta det.

   ![Ytterligare fält](assets/agile-additional-fields-kanban.png)

1. Markera namnet på det fält som du vill lägga till.
1. Skriv **[!UICONTROL Display name]** för fältet som ska visas på artikeln eller utgivningskortet.
1. Klicka på **[!UICONTROL Save Changes]**.

## Konfigurera PIA-gränsen (Work in Progress)

När du definierar PIA-gränsen för ett Kanban-team kan du kontrollera antalet objekt teamet arbetar med genom att begränsa antalet uppgifter som kan visas i [!UICONTROL New] eller [!UICONTROL In Progress] kolumn på [!UICONTROL Kanban] bräda.

När du har konfigurerat PIA-gränsen för ett Kanban-team kan du visa PIA-gränsen och uppdatera den från [!UICONTROL Kanban] Flexibel artikelpanel, enligt beskrivningen i [Hantera PIA-gränsen på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Så här begränsar du PIA för ditt Kanban-team:

{{step1-to-team}}

1. Klicka på **[!UICONTROL Switch Teams]** icon ![Ikonen Byt team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det Kanban-team som du vill hantera.
1. Klicka på **[!UICONTROL More]** meny ![](assets/more-menu.png)väljer **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** i **[!UICONTROL Methodology]** kontrollerar du att Kanban är markerat.

1. I **[!UICONTROL Story Board]** i **[!UICONTROL WIP Limit]** anger du maximalt antal tillåtna objekt i varje kolumn i [!UICONTROL Kanban] flexibel artikelpanel. Du kan ange olika gränser för varje kolumn. Den maximala gräns du kan ange för varje kolumn är 100.\
   När inställningen är angiven visas ett varningsmeddelande på [!UICONTROL Kanban] Anpassa artikelpanelen när som helst när gränsen överskrids för en kolumn på artikelpanelen. Det här varningsmeddelandet visas bara första gången som PIA-gränsen överskrids. Det här varningsmeddelandet visas inte i kolumner som har en status som är lika med [!UICONTROL Complete].\
   Begränsningen för PIA är bara en visuell varning och förhindrar inte teamet från att ha fler objekt i en enda kolumn än den gräns som du anger.

   ![PIA-gräns](assets/wip-limit-350x193.png)

1. Klicka **Spara ändringar**.

## Konfigurera automatiskt att lägga till artiklar från eftersläpningen

<!-- this functionality needs to be verified-->

Du kan konfigurera artiklar från en eftersläpning så att de automatiskt läggs till i den första kolumnen på [!UICONTROL Kanban] kort omedelbart efter att ett objekt har flyttats från den kolumnen.

{{step1-to-team}}

1. Klicka på **[!UICONTROL Switch Teams]** icon ![Ikonen Byt team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det Kanban-team som du vill hantera.
1. Klicka på **[!UICONTROL More]** meny ![](assets/more-menu.png)väljer **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. Välj **[!UICONTROL Automatically add next story from backlog]** för att konfigurera att nästa objekt från eftersläpningen automatiskt läggs till i **[!UICONTROL New]** kolumn när ett objekt flyttas ut från **[!UICONTROL In Progress]** kolumn.

   Användarna måste aktivera **Visa eftersläpning** på [!UICONTROL Kanban] för att denna funktionalitet ska träda i kraft. När användare aktiverar [!UICONTROL Show Backlog] på [!UICONTROL Kanban Board], utförs följande funktionalitet:

   När en artikel flyttas från [!UICONTROL In Progress] i en kolumn på artikelpanelen som representerar en [!UICONTROL Complete] status (eller en status som är lika med [!UICONTROL Complete]) flyttas en artikel från kolumnen Backlog automatiskt till [!UICONTROL New] kolumn i [!UICONTROL Kanban Board].
När artikeln läggs till från eftersläpningen läggs artikeln med högst prioritet till på artikelpanelen.

1. Klicka på **[!UICONTROL Save Changes]**.

## Konfigurera hur länge kort ska vara på [!UICONTROL Kanban] board

Du kan välja hur länge färdiga kort ska vara kvar på [!UICONTROL Kanban] bräda. Uppgifter som faller utanför [!UICONTROL Kanban] styrelsen fortfarande är tillgänglig i sitt ursprungliga projekt.

{{step1-to-team}}

1. (Valfritt) Klicka på **[!UICONTROL Switch Teams]** icon ![Ikonen Byt team](assets/switch-team-icon.png)väljer du sedan ett nytt Kanban-team i listrutan eller söker efter ett team i sökfältet.
1. Välj Kanban-teamet.
1. Klicka på **[!UICONTROL More]** meny ![](assets/more-menu.png) väljer **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Number of days Completed cards stay on the Kanban board]** väljer du ett värde.

   Du kan välja mellan 1 och 30 dagar.
1. Klicka på **[!UICONTROL Save Changes]**.
