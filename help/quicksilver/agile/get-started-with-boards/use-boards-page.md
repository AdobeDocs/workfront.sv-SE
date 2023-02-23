---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Använda panelkontrollpanelen
description: The [!UICONTROL boards] På kontrollpanelen visas en lista med paneler som du har tillgång till, inklusive paneler som du har skapat och paneler som du har lagts till i.
author: Lisa
feature: Agile
exl-id: bb275f4f-efaf-4dcc-b184-40e015f089b6
source-git-commit: e27965502ef7943f901daecd12897a4d3428068e
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Använda panelkontrollpanelen

På panelpanelen visas en lista med paneler och samlingar som du har tillgång till, inklusive paneler som du har skapat och paneler som du har lagts till i. Enskilda anslagstavlor som du har åtkomst till som inte ingår i en samling visas först.

>[!NOTE]
>
>Samlingar är bara tillgängliga via tidiga funktioner för [!DNL Workfront] [!UICONTROL Boards].

På kontrollpanelen kan du göra följande för paneler och samlingar:

* Arkivera en anslagstavla (samlingar kan inte arkiveras)
* Filtrera listan över anslagstavlor
* Sortera listan efter styrelsens namn eller ändringsdatum
* Sök efter en anslagstavla eller samling
* Ta bort en anslagstavla eller samling

Mer information om hur du skapar en ny styrelse eller redigerar en befintlig styrelse finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md). Mer information om hur du skapar en ny samling finns i [Hantera samlingar](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Filterbord {#filter-boards}

Du kan filtrera panelernas kontrollpanel så att de visar aktiva paneler, arkiverade paneler eller alla paneler.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Klicka [!UICONTROL **Filter**] och markera **[!UICONTROL All]**, **[!UICONTROL Active boards]**, eller **[!UICONTROL Archived boards]**.

   När ett annat filter än standardfiltret används på kontrollpanelen visas en indikator på filterikonen ![[!UICONTROL Filter applied to] kontrollpanel](assets/boards-filterapplied-30x30.png).

## Sortera ritytor

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Om du vill sortera listan över ritytor klickar du på [!UICONTROL **Sortera**]. Standardsorteringsalternativet för sidan är **[!UICONTROL Date modified]**. Du kan också sortera sidan efter board **[!UICONTROL Name]**.

   Välj **[!UICONTROL Reverse order]** om du vill sortera ritytorna i omvänd ordning efter ändringsdatum eller namn. När pilen på sorteringsikonen pekar uppåt, används omvänd ordning. När pilen pekar nedåt används standardordningen.

   När en annan sortering än standardsorteringen används på kontrollpanelen visas en indikator på sorteringsikonen ![Sortering används](assets/sort-applied-boards.png).

## Söka efter en anslagstavla eller en samling

Du kan söka efter en viss anslagstavla i området för anslagstavlor eller söka efter en viss samling i området Samlingar.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Klicka [!UICONTROL **Sök**] och skriv ett sökord. Tryck sedan på Enter.

   Alla anslagstavlor som innehåller söktermen i titeln visas.

   Klicka på X för att rensa sökningen.

   ![Sök efter paneler på kontrollpanelen](assets/boards-searchbox.png)

## Arkivera en styrelse

När du arkiverar en anslagstavla skickas den till arkivet och du kan återställa den senare.

>[!NOTE]
>
>När du arkiverar en styrelse arkiveras den för alla styrelseledamöter.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) och väljer **[!UICONTROL Archive]**.

   An [!UICONTROL Archive] icon ![Arkiv](assets/archive-icon-spectrum-25x20.png) visas på anslagstavlan. Du kan inte redigera en arkiverad anslagstavla.

   Arkiverade paneler är dolda på panelens kontrollpanel såvida du inte använder ett filter för att visa dem. Mer information finns i [[!UICONTROL Filter boards]](#filter-boards) i den här artikeln.

1. Om du vill återställa en arkiverad anslagstavla klickar du på **[!UICONTROL More]** meny ![Menyikonen Mer](assets/more-icon-spectrum.png) ombord och väljer **[!UICONTROL Restore]**.

## Ta bort en anslagstavla eller en samling

När du tar bort en anslagstavla tas den bort permanent från [!DNL Workfront] och kan inte återställas. Alla kort som finns ombord tas också bort tillsammans med styrelsen.

Om du tar bort en samling tas alla ritytor i samlingen bort.

>[!NOTE]
>
>Du kan bara ta bort ritytor och samlingar som du har skapat, inte ritytor och samlingar som du har lagts till i.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Klicka på **[!UICONTROL More]** meny ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) ombord eller i samlingen, och **[!UICONTROL Delete]**.

   I en samling finns menyn till höger, bredvid [!UICONTROL **Visa samling**] -knappen.

1. Klicka **[!UICONTROL Delete board]** eller [!UICONTROL **Ta bort samling**] på bekräftelsemeddelandet.

## Flytta en anslagstavla till en samling

Du kan flytta en fristående anslagstavla till en samling eller flytta en anslagstavla från en samling till en annan.

>[!NOTE]
>
>Du kan bara flytta ritytor som du har skapat, inte ritytor som du har lagts till i.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Klicka på **[!UICONTROL More]** meny ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) och väljer [!UICONTROL **Flytta till samling**].
1. Välj vilken samling du vill lägga till i och klicka på [!UICONTROL **Flytta**].

   Styrelsen flyttas till samlingen och visas inte längre i [!UICONTROL Boards] område.
Om du inte har skapat någon samling än uppmanas du att skapa en som du kan flytta den till.
