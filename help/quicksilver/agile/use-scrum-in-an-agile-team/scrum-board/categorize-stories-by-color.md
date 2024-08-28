---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Kategorisera artiklar efter färg på skärmanslaget
description: Standardfärgassociationen för Scrum board-artiklar varierar beroende på om artikelpanelen finns på en iteration eller i ett projekt.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Kategorisera artiklar efter färg på [!UICONTROL Scrum]-ritytan

## Ändra standardfärgassociationen för artiklar

Standardfärgassociationen för artiklar varierar beroende på om artikelpanelen finns på en iteration eller i ett projekt:

* **[!UICONTROL Iteration]**: På en iteration färgkodas artikelpaneler enligt det projekt som artikeln är kopplad till. (Varje projekt tilldelas godtyckligt en färg på artikelpanelen.) Du kan ändra det här standardbeteendet för varje smidigt team. Färger för flexibla artiklar i en iteration kan knytas till projektet (standard), artikelprioritet, ägare eller frihandsfigur. Mer information finns i [Konfigurera hur färgindikatorer används för artiklar på den flexibla artikelpanelen](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) i artikeln [Konfigurera surrning](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Project]**: I ett projekt matchar alla underaktiviteter färgen för den överordnade aktiviteten, så att färgerna för alla artiklar i ett givet simfält är desamma. Färger tilldelas slumpmässigt till aktiviteter när de skapas om aktiviteten inte har några underaktiviteter eller inte har någon överordnad aktivitet. Du kan ändra det här standardbeteendet genom att ändra den flexibla vyn. Färger för flexibla artiklar i ett projekt kan kopplas till den överordnade artikeln (standard), artikelprioritet, ägare eller frihandsfigur. Mer information finns i [Skapa eller anpassa en [!UICONTROL Agile] vy ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) i [Vyöversikt i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändra färgen på artiklar när du använder frihandsform

Om de flexibla gruppinställningarna har konfigurerats så att alternativet [!UICONTROL Associate Card Color to] är inställt på [!UICONTROL Free Form] kan användare ändra färgen på enskilda artikelrutor manuellt. Detta kan vara användbart för att kommunicera andra typer av information som är viktig för teamet eller organisationen:

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.
1. Håll pekaren över den färgade banderollen högst upp i artikelrutan.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Klicka på **[!UICONTROL Change color]** och välj önskad färg.

   ![](assets/agile-story-color2-nwe-350x138.png)
