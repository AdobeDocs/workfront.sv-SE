---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Inaktivera eller ta bort ett team
description: Du kan inaktivera team som du inte längre använder samtidigt som du behåller tillhörande historiska data. Adobe Workfront-administratörer kan återaktivera ett team när som helst från Teams-området i Setup.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Inaktivera eller ta bort ett team

Du kan inaktivera team som du inte längre använder samtidigt som du behåller tillhörande historiska data. [!DNL Adobe Workfront]-administratörer kan återaktivera ett team när som helst från Teams-området i installationsprogrammet. Om du inaktiverar ett team visas det inte längre inom följande områden:

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
     <li> <p>Nedrullningsbar meny för huvudval i området [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Assignments] typhuvud</p> </li> 
     <li> <p>[!UICONTROL Add to Kanban] leda dialog i ett projekt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Inaktiverade team visas inte när du söker efter ett team, men de visas fortfarande i [!UICONTROL Home Team] och andra team om användaren har tilldelats teamet före inaktiveringen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>
  </tr>
  <tr>
   <td>Konfigurationer på åtkomstnivå</td>
   <td><p>Inga konfigurationer krävs för att inaktivera ett team.</p>
   <p>Om du vill ta bort ett team måste du vara systemadministratör.</p></td>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inaktivera ett team

Alla arbeten som teamet tilldelats före inaktiveringen förblir tilldelade. Vi rekommenderar att du omformar arbetet innan du inaktiverar teamet.

>[!TIP]
>
>Du kan skapa en rapport som filtrerar efter uppgifter eller problem där det inaktiverade teamet fortfarande är tilldelat.

Om du inaktiverar ett team som tilldelats som standardteam i en routningsregel när du använder begärandeköer återstår teamet och begäranden dirigeras fortfarande till det inaktiverade teamet. Vi rekommenderar att du uppdaterar routningsregler med aktiva team innan du inaktiverar teamet.

{{step1-to-team}}

1. Klicka på ikonen **[!DNL Switch team]** och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Edit]**.

   ![](assets/edit-team-settings.png)

1. Avmarkera kryssrutan **[!UICONTROL Is Active]** i teaminställningarna.
1. Klicka på **[!UICONTROL Save changes]**.

## Kända begränsningar för att inaktivera ett team

Inaktiverade team visas inom följande områden:

* Ägarfältet i [!DNL Workfront Goals]. Detta kräver ytterligare en licens för [!DNL Adobe Workfront Goals]. Mer information finns i [Kom igång med [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Ta bort ett team

Det är bara en systemadministratör som kan ta bort ett team. Om du är teamägare (men inte administratör) och försöker ta bort ett team visas ett felmeddelande.

Så här tar du bort ett team:

{{step1-to-team}}

1. Klicka på ikonen **[!DNL Switch team]** och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Delete]**.

   ![](assets/edit-team-settings.png)

1. Klicka på [!UICONTROL **Bekräfta**] i bekräftelsemeddelandet om du vill ta bort teamet permanent. Borttagna team kan inte återställas.
