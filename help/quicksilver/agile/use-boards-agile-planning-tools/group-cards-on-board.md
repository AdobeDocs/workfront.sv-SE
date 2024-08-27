---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Använd grupper på en anslagstavla
description: Du kan gruppera kort på en anslagstavla per tilldelad eller tagg. När du väljer ett alternativ att gruppera efter visas korten i ett simbaneformat.
author: Lisa
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Använda grupper på en anslagstavla

Du kan gruppera kort på en anslagstavla per tilldelad eller tagg. När du väljer ett alternativ att gruppera efter visas korten i ett simbaneformat. Ej tilldelade kort eller kort utan taggar visas i sina egna simbanor.

>[!NOTE]
>
>Eventuella kort i inloppskolumnen ingår inte i en grupp och inloppskolumnen döljs när en grupp används. Mer information om intagskolumnen finns i [Lägga till en intag-kolumn på en bräda](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> 
   <p>Nytt: [!UICONTROL Contributor] eller senare</p> 
   <p>eller</p>
   <p>Aktuell: [!UICONTROL Request] eller högre</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppera kort ombord

{{step1-to-boards}}

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
