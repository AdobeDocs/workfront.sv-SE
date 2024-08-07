---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Använda grupper på en anslagstavla
description: Du kan gruppera kort på en anslagstavla per tilldelad eller tagg. När du väljer ett alternativ att gruppera efter visas korten i ett simbaneformat.
author: Lisa
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
source-git-commit: 3cb62cb00bb6c13a0b03203bda1840bce8a4d7a7
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Använda grupper på en anslagstavla

Du kan gruppera kort på en anslagstavla per tilldelad eller tagg. När du väljer ett alternativ att gruppera efter visas korten i ett simbaneformat. Ej tilldelade kort eller kort utan taggar visas i sina egna simbanor.

>[!NOTE]
>
>Eventuella kort i inloppskolumnen ingår inte i en grupp och inloppskolumnen döljs när en grupp används. Mer information om intagskolumnen finns i [Lägga till en intag-kolumn på en bräda](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Gruppera kort ombord

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Boards]**.
1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Group]** för att öppna grupppanelen till vänster om ritytan.

   >[!NOTE]
   >
   >Standardinställningen att gruppera efter är **[!UICONTROL None]**. Du kan när som helst markera det här alternativet om du vill ta bort en grupp och bara visa kolumnerna på ritytan.

1. Om du vill gruppera korten väljer du **[!UICONTROL Assignees]** eller **[!UICONTROL Tags]**.

   Korten grupperas automatiskt. Klicka på pilen bredvid gruppnamnet för att komprimera och expandera gruppen.

   ![Grupperade kort på en anslagstavla](assets/group-by-assignee.png)

1. Välj vad som ska hända när ett kort flyttas till en annan grupp.

   * **[!UICONTROL Add on assignees]/ [!UICONTROL Add on tags]:** Tilldelningarna eller taggarna i den nya gruppen läggs till i den befintliga listan med tilldelningar eller taggar på kortet.
   * **[!UICONTROL Override assignees]/ [!UICONTROL Override tags]:** Tilldelningarna eller taggarna i den nya gruppen åsidosätter alla andra tilldelningar eller taggar och blir de enda tilldelningarna eller taggarna på kortet.

   ![[!UICONTROL Group by options]](assets/group-by-rail.png)

1. Klicka på **[!UICONTROL Hide groups]** om du vill dölja grupppanelen och visa hela gruppen.
