---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Skapa eller redigera en anslagstavla
description: Från [!UICONTROL boards] kan du skapa en ny panel eller redigera en befintlig panel.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Skapa eller redigera en anslagstavla

Från [!UICONTROL boards] kan du skapa en ny panel eller redigera en befintlig panel.

Information om hur du lägger till en anslagstavla i ett arbetsflöde finns i [Hantera arbetsflöden](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

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

## Skapa en ny anslagstavla

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Om du vill skapa en fristående anslagstavla klickar du på **[!UICONTROL Add board]** i [!UICONTROL Boards] område. Information om hur du lägger till en anslagstavla i ett arbetsflöde finns i [Hantera arbetsflöden](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. Välj en mall för styrelsen.

   | Mall | Beskrivning |
   |---------|----------|
   | Grundläggande bräde | Tre standardkolumner finns på ritytan. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Tre standardkolumner finns på ritytan. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. |
   | Kanban-tavla | Följande kolumner finns på styrelsen: Eftersläpning, Nytt, Pågår, Fullständigt och Väntande. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna.<p>Om du vill använda eftersläpningen måste du ställa in filter för inloppskolumnen. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Om du vill granska standardreglerna för varje kolumn klickar du på [!UICONTROL **Mer** meny] i en kolumn och markera [!UICONTROL **Redigera**]. Du kan ändra vilken profil som helst av dessa förinställda profiler. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospektivkort | Följande kolumner finns på styrelsen: Vad gick bra? Vad kan förbättras? Vem ska vi fira? Vad kan vi göra för att gå fortare? Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Inga kolumnprinciper används. |
   | Dynamiskt kort | Följande kolumner finns på styrelsen: Avmarkerad, Ny, Pågår, Väntande och Slutförd. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. (Kolumnen Omarkerad kan byta namn men inte tas bort. Den här kolumnen innehåller alla kort med en status som inte matchar någon av de andra kolumnstatusarna.) <p>Standardkolumnprinciperna tilldelar kort till kolumner baserat på deras status. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. För ett dynamiskt kort följer du stegen i installationsguiden:

   1. Sök efter och markera [!DNL Workfront] [!UICONTROL **Projekt**] för att lägga in uppgifter och frågor i styrelsen.
   1. Sök efter och markera [!UICONTROL **Uppdrag**] för att lägga in uppgifter och frågor i styrelsen.

      Alla objekt visas på kortet som anslutna kort.

      The [!UICONTROL **Kort som läggs till**] räknaren visar hur många kort som kommer att finnas ombord. Om du till exempel markerar ett projekt med 100 uppgifter och ärenden visas 100 i räknaren. Om du lägger till en användartilldelning och den personen tilldelas till 5 uppgifter i projektet visas 5 i räknaren.

   1. (Valfritt) Välj [!UICONTROL **Inkludera slutfört arbete**] för att inkludera färdiga kort ombord.

      >[!NOTE]
      >
      >Om det här alternativet inte är markerat kommer kort i andra statusar att&quot;ramla av&quot; och inte längre visas.

   1. (Valfritt) Klicka på [!UICONTROL **Använd avancerade filter**] om du vill visa ytterligare filteralternativ.

      Detta är samma process som när du skapar ett filter för en inloppskolumn. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. När du har lagt till filtren klickar du på [!UICONTROL **Skapa anslagstavla**].

1. Ange ett namn för styrelsen i **[!UICONTROL Board]** och tryck på Retur.
1. Konfigurera styrelsen efter behov.

   Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](../../agile/get-started-with-boards/add-members-to-board.md), [Hantera kortkolumner](../../agile/get-started-with-boards/manage-board-columns.md), [Lägga till ett ad hoc-kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md)och [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klicka **[!UICONTROL All Boards]** för att gå tillbaka till panelernas kontrollpanel.

   Du kan också hitta den nedrullningsbara menyn som är märkt med namnet på aktuell anslagstavla och klicka på den för att växla till en annan anslagstavla.

   ![Förteckning över styrelser](assets/boards-button-list-of-boards-350x188.png)

## Redigera en befintlig styrelse

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. På kontrollpanelen väljer du den panel som ska öppnas.
1. Redigera styrelsen efter behov. Du kan klicka på styrelsens namn för att byta namn på det.

   Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](../../agile/get-started-with-boards/add-members-to-board.md), [Hantera kortkolumner](../../agile/get-started-with-boards/manage-board-columns.md)och [Lägg till ett kort till en anslagstavla](../../agile/get-started-with-boards/add-card-to-board.md).

1. Klicka **[!UICONTROL All Boards]** för att gå tillbaka till panelernas kontrollpanel.

   Du kan också hitta den nedrullningsbara menyn som är märkt med namnet på aktuell anslagstavla och klicka på den för att växla till en annan anslagstavla.
