---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Lägga till eller ta bort medlemmar från en styrelse
description: Personer måste läggas till i styrelsen som medlemmar innan de kan se styrelsen och tilldelas kort.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: bf8d566ba9d24310e75d2fbaf523fe5464bb6657
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Lägga till eller ta bort medlemmar från en anslagstavla

{{highlighted-preview}}

Personer och team måste läggas till i styrelsen som medlemmar innan de kan se styrelsen.

Den som har skapat en styrelse är som standard ägare. Styrelseledamot är den enda person som kan ta bort eller uppdatera brädans filter på panelen Konfigurera. <span class="preview">Det är bara en systemadministratör eller den aktuella kortägaren som kan ändra kortets ägare.</span>

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

## Lägga till medlemmar i en styrelse

{{step1-to-boards}}

1. Skapa en ny styrelse eller redigera en befintlig. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på ikonen **[!UICONTROL Add member]** ![Lägg till medlemmar](assets/boards-addmember-spectrum-25x25.png).
1. I rutan **[!UICONTROL Add members]** börjar du skriva ett namn och markerar det sedan när det visas i listan.

   Du kan välja en enskild medlem eller ett team. Om du väljer ett team läggs teamet till i styrelsen.

   >[!NOTE]
   >
   >En enskild användare måste ha alternativet **[!UICONTROL View]** eller **[!UICONTROL Edit]** angivet i sin åtkomstnivå för team, annars kan de inte visa styrelsen.


   ![Lägg till medlemmar i styrelsen](assets/boards-add-members.png)

## Ta bort medlemmar från en anslagstavla

{{step1-to-boards}}

1. Skapa en ny styrelse eller redigera en befintlig. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på ikonen **[!UICONTROL Add member]** ![Lägg till medlemmar](assets/boards-addmember-spectrum-25x25.png).
1. I rutan **[!UICONTROL Add members]** klickar du på X bredvid namnet på en person eller ett team för att ta bort dem från styrelsen.

   ![Ta bort medlem från anslagstavlan](assets/boards-remove-member-from-board-350x367.png)

   När du tar bort en medlem från en styrelse tas de inte bort från de kort som de har tilldelats. För anslutna kort uppdateras även tilldelningarna för aktiviteten eller utgåvan [!DNL Workfront].

   Medlemmar tas bara bort från den här styrelsen. De tas inte bort från andra styrelser som de tillhör.

   >[!NOTE]
   >
   >Du kan inte ta bort styrelsens ägare.

<div class="preview">

## Ändra styrelsens ägare

>[!NOTE]
>
>Det är bara en systemadministratör eller den aktuella styrelseledamöten som kan ändra styrelsens ägare. En styrelse kan bara ha en ägare.
>
>Möjligheten att ändra styrelsens ägare finns på grundbräden, retrospektiva och Kanban-tavlor, men inte dynamiska.

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]**-menyn ![Mer-menyn](assets/more-icon-spectrum.png) bredvid kortnamnet och välj sedan **[!UICONTROL Change board owner]**.
1. I dialogrutan Ändra ägare av rityta söker du efter och väljer den användare som du vill göra ägare till.

   Du kan inte söka efter användare som redan är medlemmar i styrelsen. Om du vill göra en befintlig medlem till ägare måste du först ta bort dem från styrelsen. Om en användare blir styrelsemedlem läggs de till i styrelsen.

   Endast en användare kan vara styrelsemedlemmar. Ett team kan inte vara ägare.

1. Klicka på [!UICONTROL **Uppdatera**].

</div>
