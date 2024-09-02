---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Redigera gruppinställningar
description: Workfront-administratörer och användare med en plan- eller arbetslicens kan redigera teaminställningar.
author: Lisa
feature: People Teams and Groups
exl-id: b6761188-8630-446e-bc70-70fe272881ce
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Redigera teaminställningar

Som [!DNL Adobe Workfront]-administratör eller en användare med en [!UICONTROL Standard]-, [!UICONTROL Plan]- eller [!UICONTROL Work]-licens kan du redigera [!UICONTROL Team Settings].

Du kan lägga till användare i ett team, ange teamlayoutmallen och ange hur status ska registreras när arbetsobjekten slutförs av ett team.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Arbete eller högre</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Redigera teaminställningar

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** ![Byt ikon för team](assets/switch-team-icon.png) och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.

1. Klicka på **[!UICONTROL More]**-menyn ![](assets/more-icon.png) och välj sedan **[!UICONTROL Edit]**.

   Endast teammedlemmar med antingen en [!UICONTROL Plan]- eller [!UICONTROL Work]-licens kan se det här alternativet.

   Om du vill ha alternativet [!UICONTROL Edit] men inte ser det ber du Workfront-administratören att kontrollera att [!UICONTROL Team Settings] visas i layoutmallen för [!UICONTROL Scrum Team], [!UICONTROL Kanban Team] eller [!UICONTROL Waterfall Team].

   ![](assets/edit-team-settings-1.png)

1. I gruppinställningarna kan du göra följande typer av ändringar:

   * Ändra teamnamnet
   * Inaktivera teamet
   * Associera teamet med en grupp

     >[!NOTE]
     >
     >När ett team tilldelas till en grupp eller undergrupp kan alla gruppadministratörer i den gruppen eller undergruppen hantera teamet utan att vara medlem i det. Gruppadministratörer kan gå till Teams-området från huvudmenyn och klicka på [!UICONTROL Switch Teams]-pilen ![Byt team-ikonen](assets/switch-team-icon.png) för att lista alla team som har tilldelats de grupper som de hanterar.

     Du kan kontrollera att du associerar rätt grupp med gruppen genom att hålla markören över den och klicka på informationsikonen ![](assets/info-icon.png) som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.

   * Ange teamets ägare
   * Lägg till och ta bort teammedlemmar
   * Lägg till en beskrivning av teamet
   * Använda en layoutmall i teamet

     Mer information om hur du använder en anpassad layoutmall för ett team finns i avsnittet Använda en anpassad mall för ett team i Ändra [!UICONTROL My Work]- och [!UICONTROL Work Requests]-områdena med layoutmallar.

   * Bestäm om teamet är ett smidigt team genom att välja alternativet **[!UICONTROL This is an Agile Team]**.

     Mer information om flexibla team och hur du hanterar arbete i ett smidigt team finns i [Skapa ett smidigt team](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * Ändra knappen [!UICONTROL Work On It] till en [!UICONTROL Start]-knapp. Mer information om hur du konfigurerar knappen [!UICONTROL Start] finns i [Ersätt knappen Arbeta med med med en [!UICONTROL Start]-knapp](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Anpassa knappen **[!UICONTROL Done]**. Mer information om hur du anpassar knappen [!UICONTROL Done] finns i:

      * [Konfigurera knappen [!UICONTROL Done] för aktiviteter](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
      * [Konfigurera knappen [!UICONTROL Done] för problem](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

1. Klicka på **[!UICONTROL Save Changes]**.
