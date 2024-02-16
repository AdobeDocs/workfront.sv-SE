---
product-area: agile-and-teams
navigation-topic: iterations
title: Skapa en iteration
description: Iterationer är en nyckelkomponent för Scrum-team när det gäller att planera arbetskapaciteten. [!DNL Adobe Workfront] Med kan Scrum smidiga team hantera sitt arbete genom att skapa flera iterationer för att tillgodose teamets behov.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Skapa en iteration

Iterationer är en nyckelkomponent för Scrum-team när det gäller att planera arbetskapaciteten. [!DNL Adobe Workfront] Med kan Scrum smidiga team hantera sitt arbete genom att skapa flera iterationer för att tillgodose teamets behov.

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
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Lägga till en upprepning

Använd [!UICONTROL Add Iteration] för att snabbt skapa en iteration och lägga till uppgifter och problem senare.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. På **[!UICONTROL Iterations]** flik, klicka **[!UICONTROL Add Iteration]**.\
   ![](assets/add-iteration-adobe-350x275.png)

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
      <td><p>Ange det datum då iterationen ska sluta. [!DNL Workfront] rekommenderar att du anger ett slutdatum som inte är längre än fyra veckor från startdatumet.</p><p>Tips! Välj en arbetsdag som slutdatum. Nedbrytningsdiagrammet använder bara arbetsdagar i sina beräkningar.<br>Som standard används standardschemat för att definiera arbetsdagar (enligt beskrivningen i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>). Eller, för att inkludera teamspecifika lediga dagar, kan rörliga team välja att använda ett alternativt schema (enligt beskrivningen i"Definiera ett alternativt teamschema för nedladdningsscheman" i <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Skapa ett smidigt team</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Ange upprepningens kapacitet. Det här är antalet poäng eller timmar som ditt team kan uppnå i iterationen. Talet som du anger måste vara lika med eller större än antalet punkter eller timmar från summan av alla artiklar i iterationen.<br>[!DNL Workfront] förifyller det här fältet med 50 kapacitet som standard. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Ange fokusprocenten för teamet. Om alla teammedlemmar fokuserar helt på detta projekt blir fokus 100 %.<br>[!DNL Workfront] fyller i det här fältet automatiskt med 100 %. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Submit]**. Nu när du har skapat en upprepning måste du lägga till artiklar. Mer information finns i [Lägga till artiklar i en befintlig upprepning](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planera en iteration på [!UICONTROL Backlog] tab

Använd [!UICONTROL Plan Iteration] för att skapa en upprepning med uppgifter i din eftersläpning.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Välj **[!UICONTROL Backlog]** till vänster. Klicka sedan på **[!UICONTROL Plan Iteration]**.

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
      <td><p>Ange det datum då iterationen ska sluta. [!DNL Workfront] rekommenderar att du anger ett slutdatum som inte är längre än fyra veckor från startdatumet.</p><p>Tips! Välj en arbetsdag som slutdatum. Nedbrytningsdiagrammet använder bara arbetsdagar i sina beräkningar.<br>Som standard används standardschemat för att definiera arbetsdagar (enligt beskrivningen i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>). Eller, för att inkludera teamspecifika, icke-arbetsrelaterade dagar, kan rörliga team välja att använda ett alternativt schema (enligt beskrivningen i <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Använd ett alternativt teamschema för nedladdningsscheman</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Ange fokusprocenten för teamet. Om alla teammedlemmar fokuserar helt på detta projekt blir fokus 100 %.<br>[!DNL Workfront] fyller i det här fältet automatiskt med det genomsnittliga värdet från teamets tidigare iterationer. Om det här är teamets första upprepning är fältvärdet 0 som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Ange upprepningens kapacitet. Det här är antalet poäng eller timmar som ditt team kan uppnå i iterationen. Talet som du anger måste vara lika med eller större än antalet punkter eller timmar från summan av alla artiklar i iterationen.<br>[!DNL Workfront] fyller i det här fältet automatiskt med det genomsnittliga värdet från teamets tidigare iterationer. Om det här är teamets första upprepning är fältvärdet 0 som standard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Ange ett mål för upprepningen. Detta fält är inte obligatoriskt.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Välj artiklar om du vill lägga till dem i iterationen nu eller hoppa över det här steget och lägga till artiklar i en iteration vid ett senare tillfälle. Artikeln högst upp i efterloggen har högre prioritet. Artiklar markeras med grönt när de passar in i kapaciteten. De markeras med rött om de inte gör det.\
   Du kan lägga till både uppgifter och ärenden i en enda iteration:

   * **Så här lägger du till uppgifter i iterationen:** På **[!UICONTROL Backlog]** -fliken kontrollerar du att **[!UICONTROL Stories]** -fliken är markerad (den här fliken är markerad som standard när du visar eftersläpningen). Markera de artiklar som du vill lägga till i iterationen.\

     När du lägger till uppgifter i en iteration beräknas startdatumet för uppgiften enligt beskrivningen i [[!UICONTROL Understand] hur startdatum för uppgift beräknas när de läggs till i en iteration](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Så här lägger du till problem i iterationen:** På **[!UICONTROL Backlog]** klickar du på **[!UICONTROL Issues]** -fliken. Markera de problem som du vill lägga till i iterationen.

1. Klicka på **[!UICONTROL Save].**
iterationen skapas.

1. (Valfritt) Mer information om hur du lägger till artiklar i en befintlig iteration finns i [Lägga till artiklar i en befintlig upprepning](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Förstå hur startdatum för aktiviteter beräknas när de läggs till i en iteration {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

När du lägger till en uppgift som en artikel i en iteration visas [!UICONTROL Must Finish On task] -begränsning används för varje artikel. I de flesta fall beräknas det planerade startdatumet för aktiviteten utifrån följande formel:

[!UICONTROL Iteration End Date] minus (-) [!UICONTROL Task Duration] är lika med (=) [!UICONTROL Task Planned Start Date]

The [!UICONTROL Project End Date] används i stället för om projektets startdatum är efter upprepningens startdatum och projektets slutdatum är efter upprepningens slutdatum.

Du kan konfigurera enskilda Scrum-team så att de använder projektdatum som standard, i stället för upprepningsdatum. Mer information finns i avsnittet [Konfigurera hur datum tillämpas när arbetsobjekt läggs till i en iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) i artikeln [Konfigurera Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
