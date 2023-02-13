---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Kategorisera artiklar efter färg på Scrum board
description: Standardfärgassociationen för Scrum board-artiklar varierar beroende på om artikelpanelen finns på en iteration eller i ett projekt.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Kategorisera artiklar efter färg på [!UICONTROL Scrum] board

## Ändra standardfärgassociationen för artiklar

Standardfärgassociationen för artiklar varierar beroende på om artikelpanelen finns på en iteration eller i ett projekt:

* **[!UICONTROL Iteration]**: På en iteration färgkodas artikelpaneler enligt det projekt som artikeln är kopplad till. (Varje projekt tilldelas godtyckligt en färg på artikelpanelen.) Du kan ändra det här standardbeteendet för varje smidigt team. Färger för flexibla artiklar i en iteration kan knytas till projektet (standard), artikelprioritet, ägare eller frihandsfigur. Mer information finns i [Konfigurera hur färgindikatorer används för artiklar på den flexibla artikelpanelen](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) i artikeln [Konfigurera Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Project]**: I ett projekt matchar alla underaktiviteter färgen för den överordnade uppgiften, så att färgerna för alla artiklar i en viss simbana är desamma. Färger tilldelas slumpmässigt till aktiviteter när de skapas om aktiviteten inte har några underaktiviteter eller inte har någon överordnad aktivitet. Du kan ändra det här standardbeteendet genom att ändra den flexibla vyn. Färger för flexibla artiklar i ett projekt kan kopplas till den överordnade artikeln (standard), artikelprioritet, ägare eller frihandsfigur. Mer information finns i [Skapa eller anpassa en [!UICONTROL Agile] visa](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Översikt över vyer i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Ändra färgen på artiklar när du använder frihandsform

Om de flexibla teaminställningarna har konfigurerats så att [!UICONTROL Associate Card Color to] option is set to [!UICONTROL Free Form]kan användare ändra färgen på enskilda artikelrutor manuellt. Detta kan vara användbart för att kommunicera andra typer av information som är viktig för teamet eller organisationen:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Välj **[!UICONTROL Iterations]** om du vill välja en viss upprepning, eller markera **[!UICONTROL Current Iteration]**.
1. Håll pekaren över den färgade banderollen högst upp i artikelrutan.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Klicka **[!UICONTROL Change color]** väljer du sedan önskad färg.

   ![](assets/agile-story-color2-nwe-350x138.png)
