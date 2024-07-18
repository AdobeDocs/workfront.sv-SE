---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Skapa ett smidigt team
description: Med Adobe Workfront kan smidiga team slutföra arbetet på ett inkrementellt och organiserat sätt.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---

# Skapa ett smidigt team

<!--Audited: 01/2024-->

Med [!DNL Adobe Workfront] kan team slutföra arbetet på ett inkrementellt och organiserat sätt.

Alla användare i organisationen kan se det flexibla teamet och se alla flexibla komponenter för teamet, inklusive eftersläpning, iterationer, artikelanslagstavla och individuella berättelser. Det är dock bara medlemmar i teamet som har [!UICONTROL Edit] behörighet att arbeta som kan ändra det arbete som tilldelats teamet.

[!DNL Workfront] har stöd för följande flexibla metoder:

* **[!UICONTROL Scrum]**: Team har en eftersläpning av arbete som måste utföras. När teamet är redo att arbeta med en viss del av arbetet flyttas arbetet från eftersläpningen till en upprepning. Mer information om hur du hanterar ett Scrum-team finns i [Scrum i ett rörligt team](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Team flyttar arbete i Kanban-vyn över förbestämda statusar. Standardstatusvärdena är: eftersläpning, pågående och slutförd. Mer detaljerad information om hur du hanterar ett Kanban-team finns i [Kanban i ett rörligt team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Nytt: Standard</p>
   Aktuell: 
   <ul><li><p>[!UICONTROL Plan] skapa ett nytt smidigt team</p></li> 
   <li><p>[!UICONTROL Work] eller högre för att konvertera ett team till ett smidigt team</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan eller licenstyp du har.

+++

## Bestäm en flexibel metod

Du kan använda en Scrum- eller Kanban-flexibel metod för ditt mobila team. Varje metod ger olika fördelar. Det sätt ditt flexibla team arbetar på avgör vilken flexibel metod du väljer att använda.

Med både Scrum- och Kanban-flexibla metoder i [!DNL Workfront] kan du flytta artiklar över en artikelpanel för att ange en statusändring och artikelstatus.

Scrum- och Kanban-flexibla metoder i [!DNL Workfront] skiljer sig på följande sätt:

### Fördelar med att använda Kanban i [!DNL Workfront]

Med den [!DNL Kanban] flexibla metoden i [!DNL Workfront] kan du enklare flytta artiklar mellan olika artikelpaneler samtidigt som du begränsar mängden pågående arbete. Det finns inga start- och slutdatum när den flexibla metoden [!DNL Kanban] används.

Följande funktionalitet stöder den här metoden:

* Visa eftersläpningen på den [!DNL Kanban] flexibla artikelpanelen.\
   Mer information finns i [Lägg till eftersläpning på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Konfigurera objekt på eftersläpningen så att de automatiskt läggs till på den [!UICONTROL Kanban] mobila artikelpanelen när andra objekt flyttas till en status som motsvarar fullständig.\
   Mer information finns i avsnittet [Konfigurera artiklar som ska läggas till automatiskt från eftersläpningen](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) i artikeln [Konfigurera Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Konfigurera en PIA-gräns (Work In Progress) som ska visas på den [!UICONTROL Kanban] mobila artikelpanelen.\
   Mer information finns i [Hantera gränsen för pågående arbete (PIA) på Kanban-tavlan](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Fördelar med att använda Scrum i [!DNL Workfront]

Med den flexibla metoden Scrum i [!DNL Workfront] kan du lägga till en uppsättning artiklar i en flexibel iteration och skapa en artikelpanel för den upprepningen. iterationen baseras på de start- och slutdatum som du anger.

Följande funktionalitet stöder den här metoden:

* Inkludera problem på [!UICONTROL Scrum]-artikelpanelen
* Inkludera problem i eftersläpningen i ett smidigt team
* Underaktiviteter kan visas på [!UICONTROL Scrum]-artikelpanelen
* Visa ett nedladdningsbart diagram för att se förloppet mot artiklar under upprepningen\
   Mer information finns i [Översikt över Agile-nedladdningsdiagram](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Skapa ett smidigt team

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch Teams]** ![Byt ikon för team](assets/switch-team-icon.png) och klicka sedan på **[!UICONTROL Create new team]**.

   ![Välj Skapa nytt team.](assets/create-new-team-350x198.png)

   Rutan Nytt team visas.

1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Skriv ett namn för det nya flexibla teamet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Välj det här alternativet om du vill konfigurera det nya teamet så att det blir ett smidigt team.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>Välj det här alternativet om du vill aktivera teamet. Inaktiva team är inte synliga för andra användare att tilldela till arbete. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Börja skriva namnet på en grupp som ska läggas till i teamet och markera sedan namnet när det visas i listrutan.</p> <p><b>ANMÄRKNING</b></p> <p> När ett team tilldelas till en grupp eller undergrupp kan alla gruppadministratörer i gruppen eller undergruppen hantera teamet utan att vara medlem i gruppen. Gruppadministratörer kan gå till området [!UICONTROL Teams] från [!UICONTROL Main Menu] och klicka på pilen [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Byt ikon för team"> för att lista alla team som är tilldelade de grupper som de hanterar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Börja skriva namnet på en användare som ska vara med i teamet och markera sedan namnet när det visas i listrutan.<br>Upprepa den här processen om du vill lägga till flera användare i teamet.<br>Eftersom användare kan finnas i fler än ett team kan de finnas i både flexibla och icke-flexibla team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Skriv en beskrivning för teamet.</p> <p>Beskrivningen visas längst upp till höger i området [!UICONTROL Teams] när teamet har valts.</p>
      <p>Om beskrivningen är lång kan du klicka på den för att visa den fullständiga beskrivningen i ett popup-fönster. Om du har tillgång till att redigera [!UICONTROL team settings] kan du även redigera beskrivningen direkt i popup-fönstret.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create]**.

   Mer information om hur du konfigurerar ett Agile-team finns i följande artiklar:

   * [Konfigurera [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurera [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Konvertera ett befintligt team till ett smidigt team

Du kan konvertera ett befintligt team till ett smidigt team:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront] och klicka sedan på **[!UICONTROL Teams]**.
1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.

1. Välj det team som du vill konvertera till ett smidigt team.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Edit]**.\
   Endast teammedlemmar med antingen en [!UICONTROL Plan]- eller [!UICONTROL Work]-licens kan se det här alternativet.\
   ![](assets/edit-team-settings-350x205.png)

1. Välj **[!UICONTROL This is an Agile Team]** i avsnittet **[!UICONTROL Agile]**.

1. I avsnittet **[!UICONTROL Methodology]** väljer du om teamet ska använda en **[!UICONTROL Scrum]** eller **[!UICONTROL Kanban]** flexibel metod.

1. Klicka på **Spara ändringar.**

   Teamet sparas som ett Agile-team. Du kan konfigurera det nya teamet som ett Scrum- eller Kanban-team när du redigerar teamet.

   Mer information finns i följande artiklar:

   * [Konfigurera [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurera [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
