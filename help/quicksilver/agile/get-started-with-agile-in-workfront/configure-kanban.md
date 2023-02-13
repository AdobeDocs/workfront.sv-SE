---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Konfigurera Kanban
description: Du kan konfigurera följande alternativ för Kanban-team under eller efter att teamet har skapats.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Kanban]

Du kan konfigurera följande alternativ för flexibla team under eller efter det att teamet har skapats. Du skapar ett rörligt team (Kanban eller Scrum) i [!DNL Adobe Workfront] enligt beskrivning i [Skapa ett smidigt team](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Konfigurera om artiklar ska beräknas i punkter eller timmar

Du kan konfigurera artiklar att beräknas med hjälp av punkter eller timmar.

Så här konfigurerar du hur berättelser beräknas för ditt team:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.
1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.\
   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** i **[!UICONTROL Estimate Stories in]** väljer du om du vill använda punkter eller timmar för att beräkna artikelns storlek (arbetsbelastning). Om du väljer Punkter anger du hur många timmar som ska vara lika med 1 punkt. (Standardvärdet är 1 punkt = 8 timmar.) Detta är antalet planerade timmar som läggs till i artikeln.

   **Exempel:** Om du har valt att uppskatta artiklar i punkter och 1 punkt är lika med 8 timmar, och en artikel beräknas till 3 punkter, läggs 24 planerade timmar till artikeln.

1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera statuskolumner på den flexibla artikelpanelen

Du kan definiera de statusar som finns på artikeltavlan för det flexibla teamet. Det här är de enda statusvärdena som visas på artikelpanelen.

Så här definierar du de statusvärden som är tillgängliga för den artikelpanel som är kopplad till det flexibla teamet:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!UICONTROL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

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
   >Endast låsta systemomfattande statusar är tillgängliga för val; du kan inte välja gruppspecifika statusar. Den första kolumnens status motsvarar alltid **[!UICONTROL New]**.

   Du kan lägga till anpassade statusvärden om [!DNL Workfront] administratören har konfigurerat dem, anpassade statusvärden kan konfigureras enligt beskrivningen i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera ytterligare fält som ska visas på artikelkort på den flexibla artikelpanelen

När du lägger till fält i artikelkort är fälten skrivskyddade och skrivskyddade när fältet fylls i.

Som standard visas följande typer av data på artikelkortet för uppgifter och ärenden:

* Artikelnamn med en länk direkt till uppgiften eller utgåvan
* Projektnamnet med en länk direkt till projektet
* Den här länken visas endast för artiklar, inte för underaktiviteter
* Uppgiften eller utgivningsbeskrivningen
* Aktuellt åtagande
* Visa och redigera procentandelen antingen genom att justera själva procentandelen eller genom att justera antalet punkter eller timmar som är klara
* Tilldelade användare

Du kan visa ytterligare data (inklusive anpassade data) på artikelkort. Du kan visa ytterligare fält på artikelkort av någon anledning. Du kan till exempel visa kund-ID:t om du arbetar med artiklar för flera kunder i iteration, eller om du vill visa projektets startdatum eller projektavslutsdatum.

>[!NOTE]
>
>Om du använder ett anpassat fält på ett artikelkort kan det inte innehålla en punkt/punkt i namnet.

Så här konfigurerar du artikelkort som tilldelats det flexibla teamet så att ytterligare fält visas:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** anger du ett fältnamn för att hitta det.

   ![Ytterligare fält](assets/agile-additional-fields-kanban.png)

1. Markera namnet på det fält som du vill lägga till.
1. Skriv **[!UICONTROL Display name]** för fältet som ska visas på artikeln eller utgivningskortet.
1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera PIA-gränsen (Work in Progress)

Kanban in [!DNL Workfront] kan du styra mängden arbete teamet arbetar med genom att begränsa antalet uppgifter som kan visas i [!UICONTROL In Progress] kolumn på [!UICONTROL Kanban] bräda.

När PIA-gränsen har konfigurerats kan du visa PIA-gränsen eller till och med uppdatera den från [!UICONTROL Kanban] Flexibel artikelpanel, enligt beskrivningen i [Hantera PIA-gränsen på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Så här begränsar du PIA för ditt Kanban-team:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det Kanban-team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** i **[!UICONTROL Methodology]** kontrollerar du att Kanban är markerat.

1. I **[!UICONTROL Story Board]** i **[!UICONTROL WIP LIMIT]** anger du maximalt antal tillåtna objekt i varje kolumn i [!UICONTROL Kanban] flexibel artikelpanel. Du kan ange olika gränser för varje kolumn. Den maximala gräns du kan ange för varje kolumn är 100.\
   När inställningen är angiven visas ett varningsmeddelande på [!UICONTROL Kanban] Anpassa artikelpanelen när som helst när gränsen överskrids för en kolumn på artikelpanelen. Det här varningsmeddelandet visas bara första gången som PIA-gränsen överskrids. Det här varningsmeddelandet visas inte för kolumner som har en status som är lika med [!UICONTROL Complete].\
   Begränsningen för PIA är bara en visuell varning och förhindrar inte teamet från att ha fler objekt i en enda kolumn än den gräns som du anger.

   ![PIA-gräns](assets/wip-limit-350x193.png)

1. Klicka **Spara ändringar**.

## Konfigurera artiklar som automatiskt ska läggas till från eftersläpningen

Du kan konfigurera artiklar från en eftersläpning så att de automatiskt läggs till i den första kolumnen på [!UICONTROL Kanban] kort omedelbart efter att ett objekt har flyttats från den kolumnen.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det Kanban-team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. Välj **[!UICONTROL Automatically add next story from backlog]** för att konfigurera artiklar som automatiskt ska läggas till från eftersläpningen till den första kolumnen på [!UICONTROL Kanban] artikelpanel.

   Detta inträffar när en artikel flyttas till en kolumn på artikelpanelen som representerar statusen Fullständig (en status som motsvarar Fullständig). När artikeln läggs till från en eftersläpning läggs den med högst prioritet till på artikelpanelen.Välj det här alternativet om du vill konfigurera nästa objekt från eftersläpningen så att det automatiskt läggs till i **[!UICONTROL In Progress]** kolumn när ett objekt flyttas ut från **[!UICONTROL In Progress]** kolumn.

1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera hur länge kort ska vara på [!UICONTROL Kanban] board

Du kan välja hur länge de färdiga korten ska vara kvar på [!UICONTROL Kanban] bräda. Uppgifter som faller utanför [!UICONTROL Kanban] styrelsen fortfarande är tillgänglig i sitt ursprungliga projekt.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Kanban-team i listrutan eller söker efter ett team i sökfältet.
1. Välj Kanban-teamet.
1. Klicka på **[!UICONTROL More]** väljer du **Edit**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Number of days Completed cards stay on the Kanban board]** väljer du ett värde.
1. Klicka på **[!UICONTROL Save changes]**.
