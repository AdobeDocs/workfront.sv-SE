---
product-area: agile-and-teams
navigation-topic: iterations
title: Skapa en iteration
description: Iterationer är en nyckelkomponent för Scrum-team när det gäller att planera arbetskapaciteten.Med  [!DNL Adobe Workfront] kan Scrum-team hantera sitt arbete genom att skapa flera iterationer för att tillgodose teamets behov.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 9a3ec953ca1c7989be292f1747a052ed5cc7c74b
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 0%

---

# Skapa en iteration

Iterationer är en nyckelkomponent för Scrum-team när det gäller att planera arbetskapaciteten. Med [!DNL Adobe Workfront] kan Scrum-team hantera sitt arbete genom att skapa flera iterationer för att passa teambehov.

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
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Light] eller senare</p> 
   eller
   <p>Aktuell: [!UICONTROL Review] eller högre</p> </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägga till en upprepning

Du kan lägga till en iteration i listan för att snabbt skapa en iteration och lägga till uppgifter och problem senare.

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. Klicka på **[!UICONTROL Add iteration]** på fliken **[!UICONTROL Iterations]**.

   ![Klicka på Lägg till upprepning](assets/click-add-iteration.png)

1. Ange följande:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Ange namnet på iterationen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Lägg till de mål du har för iterationen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td>Ange det datum då iterationen ska börja.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong></td> 
      <td><p>Ange det datum då iterationen ska sluta. [!DNL Workfront] rekommenderar att du anger ett slutdatum som inte är längre än fyra veckor från startdatumet.</p><p>Tips! Välj en arbetsdag som slutdatum. Nedbrytningsdiagrammet använder bara arbetsdagar i sina beräkningar.<br>Som standard används standardschemat för att definiera arbetsdagar (enligt beskrivningen i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>). Om du vill inkludera teamspecifika, icke-arbetsrelaterade dagar kan rörliga team välja att använda ett alternativt schema (enligt beskrivningen i Definiera ett alternativt teamschema för nedladdningsscheman i <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Skapa ett smidigt team</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Ange upprepningens kapacitet. Det här är antalet poäng eller timmar som ditt team kan uppnå i iterationen. Talet som du anger måste vara lika med eller större än antalet punkter eller timmar från summan av alla artiklar i iterationen.<br>[!DNL Workfront] fyller i det här fältet automatiskt med 50-kapacitet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Ange fokusprocenten för teamet. Om alla teammedlemmar fokuserar helt på detta projekt blir fokus 100 %.<br>[!DNL Workfront] fyller i fältet automatiskt med 100 % som standard. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Add iteration]**. Nu när du har skapat en upprepning måste du lägga till artiklar. Mer information finns i [Lägga till artiklar i en befintlig iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planera en iteration på fliken [!UICONTROL Backlog]

Använd funktionen [!UICONTROL Plan Iteration] för att skapa en iteration med uppgifter på din eftersläpning.

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. Välj **[!UICONTROL Backlog]** på den vänstra panelen. Klicka sedan på **[!UICONTROL Plan Iteration]**.

1. Ange följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Ange ett namn för iterationen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td> Ange det datum då iterationen ska starta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong> </td> 
      <td><p>Ange det datum då iterationen ska sluta. [!DNL Workfront] rekommenderar att du anger ett slutdatum som inte är längre än fyra veckor från startdatumet.</p><p>Tips! Välj en arbetsdag som slutdatum. Nedbrytningsdiagrammet använder bara arbetsdagar i sina beräkningar.<br>Som standard används standardschemat för att definiera arbetsdagar (enligt beskrivningen i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>). Om du vill inkludera teamspecifika, icke-arbetsrelaterade dagar kan rörliga team välja att använda ett alternativt schema (enligt beskrivningen i <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Använd ett alternativt teamschema för nedladdningsscheman</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Ange fokusprocenten för teamet. Om alla teammedlemmar fokuserar helt på detta projekt blir fokus 100 %.<br>[!DNL Workfront] fyller i det här fältet i förväg med det genomsnittliga värdet från ditt teams tidigare iterationer. Om det här är teamets första upprepning är fältvärdet 0 som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Ange upprepningens kapacitet. Det här är antalet poäng eller timmar som ditt team kan uppnå i iterationen. Talet som du anger måste vara lika med eller större än antalet punkter eller timmar från summan av alla artiklar i iterationen.<br>[!DNL Workfront] fyller i det här fältet i förväg med det genomsnittliga värdet från ditt teams tidigare iterationer. Om det här är teamets första upprepning är fältvärdet 0 som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Ange ett mål för upprepningen. Detta fält är inte obligatoriskt.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Välj artiklar om du vill lägga till dem i iterationen nu eller hoppa över det här steget och lägga till artiklar i en iteration vid ett senare tillfälle. Artikeln högst upp i efterloggen har högre prioritet. Artiklar markeras med grönt när de passar in i kapaciteten. De markeras med rött om de inte gör det.
Du kan lägga till både uppgifter och ärenden i en enda iteration:

   * **Om du vill lägga till uppgifter i iterationen:** På fliken **[!UICONTROL Backlog]** kontrollerar du att fliken **[!UICONTROL Stories]** är markerad (den här fliken är markerad som standard när du visar eftersläpningen). Markera de artiklar som du vill lägga till i iterationen.

     När du lägger till uppgifter i en iteration beräknas startdatumet för aktiviteten enligt beskrivningen i [[!UICONTROL Understand] hur startdatum för aktiviteten beräknas när de läggs till i en iteration ](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Om du vill lägga till problem i iterationen:** Klicka på fliken **[!UICONTROL Backlog]** på fliken **[!UICONTROL Issues]**. Markera de problem som du vill lägga till i iterationen.

1. Klicka på **[!UICONTROL Save].**
iterationen skapas.

1. (Valfritt) Mer information om hur du lägger till artiklar i en befintlig iteration finns i [Lägga till artiklar i en befintlig iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Förstå hur startdatum för aktiviteter beräknas när de läggs till i en iteration {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

När du lägger till en uppgift som en artikel i en iteration används begränsningen [!UICONTROL Must Finish On task] för varje artikel. I de flesta fall beräknas det planerade startdatumet för aktiviteten utifrån följande formel:

[!UICONTROL Iteration End Date] minus (-) [!UICONTROL Task Duration] är lika med (=) [!UICONTROL Task Planned Start Date]

[!UICONTROL Project End Date] används i stället för   om projektets startdatum är efter upprepningens startdatum och projektets slutdatum är efter upprepningens slutdatum.

Du kan konfigurera enskilda Scrum-team så att de använder projektdatum som standard, i stället för upprepningsdatum. Mer information finns i avsnittet [Konfigurera hur datum ska användas när arbetsobjekt läggs till i en iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) i artikeln [Konfigurera repet](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
