---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Inaktivera ett team
description: Du kan inaktivera team som du inte längre använder samtidigt som du behåller tillhörande historiska data. Adobe Workfront-administratörer kan återaktivera ett team när som helst från Teams-området i Setup.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Inaktivera ett team

Du kan inaktivera team som du inte längre använder samtidigt som du behåller tillhörande historiska data. [!DNL Adobe Workfront] administratörer kan återaktivera ett team när som helst från Teams-området i installationsprogrammet. Om du inaktiverar ett team visas det inte längre inom följande områden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Typsnittsfält i anpassade formulär</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Dialogrutan för delning av objekt</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Listrutan Huvudval i [!UICONTROL Teams] area</p> </li> 
     <li> <p>[!UICONTROL Assignments] typhuvud</p> </li> 
     <li> <p>[!UICONTROL Add to Kanban] leda dialog i ett projekt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Inaktiverade team visas inte när du söker efter ett team, men de visas fortfarande i [!UICONTROL Home Team] och andra team om användaren var tilldelad teamet före inaktiveringen.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Inaktivera ett team

Alla arbeten som teamet tilldelats före inaktiveringen förblir tilldelade. Vi rekommenderar att du omformar arbetet innan du inaktiverar teamet.

>[!TIP]
>
>Du kan skapa en rapport som filtrerar efter uppgifter eller problem där det inaktiverade teamet fortfarande är tilldelat.

Om du inaktiverar ett team som tilldelats som standardteam i en routningsregel när du använder begärandeköer återstår teamet och begäranden dirigeras fortfarande till det inaktiverade teamet. Vi rekommenderar att du uppdaterar routningsregler med aktiva team innan du inaktiverar teamet.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Teams]**.
1. Klicka på **[!DNL Switch team]** väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.

   ![](assets/edit-team-settings-350x205.png)

1. Rensa **[!UICONTROL Is Active]** kryssruta.
1. Klicka på **[!UICONTROL Save changes]**.

## Kända begränsningar

Inaktiverade team visas inom följande områden:

* Fältet Ägare i [!DNL Workfront Goals]. Detta kräver ytterligare licens för [!DNL Adobe Workfront Goals]. Mer information finns i [Kom igång med [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
