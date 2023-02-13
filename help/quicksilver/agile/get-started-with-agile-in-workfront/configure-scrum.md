---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Konfigurera Scrum
description: Du kan konfigurera följande alternativ för Scrum-team under eller efter det att teamet har skapats.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1531'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Scrum]

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

>[!NOTE]
>
>Den här inställningen kan inte ändras om teamet har några pågående iterationer.

Du kan konfigurera artiklar att beräknas med hjälp av punkter eller timmar.

Så här konfigurerar du hur berättelser beräknas för ditt team:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!UICONTROL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.
1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.\
   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** i **[!UICONTROL Estimate Stories in]** väljer du om du vill använda punkter eller timmar för att beräkna artikelns storlek (arbetsbelastning). Om du väljer Punkter anger du hur många timmar som ska vara lika med 1 punkt. (Standardvärdet är 1 punkt = 8 timmar.) Detta är antalet planerade timmar som läggs till i artikeln.

   **Exempel:** Om du har valt att uppskatta artiklar i punkter och 1 punkt är lika med 8 timmar, och en artikel beräknas till 3 punkter, läggs 24 planerade timmar till artikeln.

1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera statuskolumner på den flexibla artikelpanelen

Du kan konfigurera vilka kolumner som ska visas på den flexibla artikelpanelen för alla iterationer som har tilldelats ditt team eller för ett visst projekt.

* [Konfigurera statuskolumner för iterationer](#configure-status-columns-for-iterations)
* [Konfigurera statuskolumner för projekt](#configure-status-columns-for-projects)

### Konfigurera statuskolumner för iterationer {#configure-status-columns-for-iterations}

Du kan definiera de statusar som finns på artikeltavlan för det flexibla teamet. Det här är de enda statusvärdena som visas på artikelpanelen.

Så här definierar du de statusvärden som är tillgängliga för den artikelpanel som är kopplad till det flexibla teamet:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** -avsnittet, leta upp **[!UICONTROL Story Board]** område.

1. (Valfritt) Klicka på **[!UICONTROL Add Column]** om du vill lägga till ytterligare en statuskolumn på artikelpanelen.
1. (Valfritt) Dra en statuskolumn med dra och släpp-indikatorn för att ändra ordningen på statuskolumnerna på artikelpanelen. Den första kolumnen kan inte flyttas och du kan inte dra en annan kolumn framför den första kolumnen.

   ![Dra och släpp](assets/agile-story-card-drag-and-drop.png)

1. Välj både uppgifts- och utgivningsstatus. Uppgiftsstatus visas som kolumnrubrik för varje kolumn på artikelpanelen. De utgivningsstatusar du väljer är mappa till uppgiftsstatusvärdena. Det innebär att när du flyttar en utgåva till en annan kolumn på artikelpanelen, ändras utgåvans status till de utgivningsstatusar som visas här, inte till namnet på kolumnen på artikelpanelen (som återspeglar aktivitetens status).

   >[!IMPORTANT]
   >
   >Endast låsta systemomfattande statusar är tillgängliga för val; du kan inte välja gruppspecifika statusar. Den första kolumnens status motsvarar alltid **[!UICONTROL New]**.

   Du kan lägga till anpassade statusvärden om [!DNL Workfront] administratören har konfigurerat dem, anpassade statusvärden kan konfigureras enligt beskrivningen i [Skapa eller redigera en status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >När du väljer utgivningsstatus används alltid den tredje kolumnen som standard [!UICONTROL Closed]. Om du har fler än tre kolumner måste du uppdatera kolumnerna manuellt för att återspegla rätt status.

1. Klicka på **[!UICONTROL Save changes]**.

### Konfigurera statuskolumner för projekt {#configure-status-columns-for-projects}

Mer information om hur du konfigurerar statuskolumner för ett projekt finns i avsnittet [Skapa eller anpassa en [!UICONTROL Agile] visa](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) i artikeln [Skapa eller redigera vyer i [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!UICONTROL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I **[!UICONTROL Agile]** anger du ett fältnamn för att hitta det.

   ![Ytterligare fält](assets/agile-additional-fields-scrum.png)

1. Markera namnet på det fält som du vill lägga till.
1. Skriv **[!UICONTROL Display name]** för fältet som ska visas på artikeln eller utgivningskortet.
1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera hur färgindikatorer används för artiklar på den flexibla artikelpanelen

Som standard färgkodas plattor i en flexibel iteration enligt det projekt som artikeln är kopplad till. Varje projekt tilldelas godtyckligt en färg på artikelpanelen. Du kan ändra det här standardbeteendet för varje smidigt team. Färger för flexibla artiklar kan knytas till artikelprioritet, ägare och så vidare.

Så här ändrar du hur färger tilldelas artiklar för ett smidigt team:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.

1. Välj det flexibla team som du vill hantera.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.

   ![Redigera team](assets/edit-team-settings-350x205.png)

1. I [!UICONTROL Agile] i [!UICONTROL Associate Card Color to] väljer du bland följande alternativ:

   * **[!UICONTROL Project]**: Färger är kopplade till det projekt som artikeln är kopplad till. (När en artikel skapas måste den kopplas till ett projekt, vilket beskrivs i [Skapa en Agile Story](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Alla uppgifter från samma projekt visas med samma färg.
   * **[!UICONTROL Free Form]**: Alla kort visas som blå som standard tills användaren ändrar färgen manuellt enligt beskrivningen i [[!UICONTROL Categorize stories by color] på Scrum board](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priority]**: Färgerna kopplas till artikelprioriteten enligt följande:

      * Hög = röd
      * Medel = gul
      * Låg = Grön\

         Om systemadministratören har konfigurerat anpassade prioriteringar för din [!DNL Workfront] system, den högsta prioriteten är röd, den näst högsta är gul och den tredje högsta är grön.
   * **[!UICONTROL Task Owner]**: Alla artiklar med samma primära tilldelade färg har samma färg. Den primära tilldelaren är den användare som först tilldelades uppgiften.


1. Klicka på **[!UICONTROL Save changes]**.

## Konfigurera hur datum tillämpas när arbetsobjekt läggs till i en iteration

När du lägger till ett arbetsobjekt i en upprepning av en upprepning ändras som standard det planerade startdatumet och det planerade slutförandedatumet för arbetsobjektet så att de matchar iterationens start- och slutdatum. Du kan välja att behålla originaldatum för alla arbetsobjekt för teamet.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Teams]**.
1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   Endast teammedlemmar med antingen en [!UICONTROL Plan] eller [!UICONTROL Work] se det här alternativet.
1. I [!UICONTROL Agile] i [!UICONTROL When a Work Item is Added to an Iteration] väljer du bland följande alternativ:

   * **[!UICONTROL Modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: När arbetsobjekt läggs till i en iteration ändras arbetsuppgiftens datum till iteration-datum.\

      Mer information om hur datum ändras finns i avsnittet [Förstå hur inlagda artiklar påverkar aktivitetsdatum](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) i artikeln [Lägga till artiklar i en befintlig upprepning](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Do not modify the Planned Start Date and Planned Completion Date to match the iteration start and end dates]**: När arbetsobjekt läggs till i en iteration behåller arbetsobjekten sina ursprungliga datum.

   Om du ändrar datumalternativet justeras inte datum för arbetsobjekt som redan finns i upprepningen.

   Dessa alternativ kan påverka datum när team tilldelar arbetsobjekt till varandras iterationer. Team A ändrar till exempel datum för arbetsuppgift till upprepningsdatum och team B ändrar inte datum för arbetsuppgift. Om team B tilldelar en arbetsuppgift till team A:s iteration ändras arbetsartikelns datum. Om team A tilldelar ett arbetsobjekt till grupp B:s iteration ändras dock inte datumen.

1. Klicka på **[!UICONTROL Save changes]**.
