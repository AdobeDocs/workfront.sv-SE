---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Konfigurera hur information visas i [!UICONTROL Gantt]-diagrammet
description: Du kan konfigurera vilken information som ska visas både i Gantt-schemat för uppgiftslistor och i Gantt-schemat för projektlistor.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Konfigurera hur information visas på [!UICONTROL Gantt Chart]

Du kan konfigurera vilken information som ska visas i både aktivitetslistan [!UICONTROL Gantt Chart] och projektlistan [!UICONTROL Gantt Chart].

## Åtkomstkrav

Du måste ha följande för att kunna följa stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL View] eller bättre åtkomst till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förstå visningsalternativ

Följande tabell visar visningsalternativen för [!UICONTROL Gantt chart]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actual Dates]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date] och [!UICONTROL Actual Completion Date] visas med en triangelikon. Om [!UICONTROL Actual Completion Date] är null visas bara [!UICONTROL Actual Start Date].</p> <p>Mer information om start- och slutdatum finns i <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Översikt över projektet [!UICONTROL Actual Completion Date] </a> och <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Översikt över projektet [!UICONTROL Actual Start Date] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="tilldelningar_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Visar tilldelningar av uppgifter. För musen över länken <strong>[!UICONTROL Details]</strong> bredvid namnet på en tilldelad för att se mer detaljerad information om dem, inklusive procentandelen av deras allokering till uppgiften.</p> <p>Tilldelningar visas inte på [!UICONTROL Gantt chart] när [!UICONTROL Gantt chart] exporteras till PDF. När [!UICONTROL Gantt chart] exporteras till PDF visas endast tilldelningar i uppgiftslistan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baslinjer_sandbox_gantt.png"> </td> 
   <td> <p>En ögonblicksbild av ett projekt som representerar viktiga data om projektet som ingår i den ursprungliga projektplanen. Baslinjer kan tas under hela projektets löptid. När du aktiverar att visa baslinjer i [!UICONTROL Gantt chart], väljer du vilken baslinje du vill visa. Du kan bara visa en baslinje på [!UICONTROL Gantt chart] åt gången, och den visas i form av ett grått fält.</p> <p>Mer information om baslinjer finns i <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Skapa projektbaslinjer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>Det datum som en tilldelad anger som sitt åtagande när uppgiften ska slutföras visas med en markör i [!UICONTROL Gantt chart]. </p> <p>Mer information om implementeringsdatum finns i <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] översikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  Procentandelen av uppgiften som är slutförd visas på aktivitetsraden.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critical Path]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>De uppgifter som skulle kunna påverka tidslinjen i projektet betraktas som en del av den kritiska sökvägen och markeras tydligt i rött. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Diamanter</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="millestone_diamonds.png"> </td> 
   <td> <p>En diamantikon visas efter uppgiften som är associerad med en milstolpe. För musen över en milstolpe för att visa namn och datum för milstolpen. Administratören [!DNL Workfront] bestämmer färgen på varje milstolpe-romb.</p> <p>Mer information om milstolpar finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Skapa en milstolpe-sökväg</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Linjer</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="millestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>En rad visas efter uppgiften som är associerad med en milstolpe. För musen över en milstolpe för att visa namn och datum för milstolpen. Administratören [!DNL Workfront] bestämmer färgen på varje milstolpe.</p> <p> Mer information om milstolpar finns i  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Skapa en milstolpe-sökväg</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>En rad från en aktivitet till en annan som visar den föregående relationen mellan de två aktiviteterna. Om du vill markera en enskild föregående linje för du musen över den. Klicka på den för att behålla den markerad. Du kan bara markera en föregående rad åt gången.</p> <p>En <strong>[!UICONTROL Predecessor]</strong>-ikon visas bredvid en aktivitet som har en föregående relation som sträcker sig över flera sidor i Gantt-diagrammet eller för en aktivitet som har en föregående aktivitet mellan flera projekt.</p> <p>Klicka på ikonen <strong>[!UICONTROL Predecessor]</strong> om du vill visa alla föregående och efterföljande aktiviteter samt information om varje aktivitet, till exempel aktivitetsnamn, typ av föregående relation och nyckeldatum.</p> <p>Obs! [!UICONTROL Gantt Chart] i en lista med projekt visar information om föregångare mellan projekt. Mer information om hur du skapar föregångarrelationer mellan olika projekt finns i <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Skapa föregångare mellan projekt</a></p> <p>Mer information om föregångare finns i <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Tvinga föregångare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__Oct._2017.png"></p> <p>[!UICONTROL Behind]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind_okt._2017.png"></p> <p>[!UICONTROL At Risk]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Sena        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>Status för det aktuella förloppet för en viss uppgift. </p> <p>Mer detaljerad information om varje [!UICONTROL Progress Status]-typ finns i <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref"> Åtgärdsöversikt [!UICONTROL Progress Status]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projected Dates]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projicerade_datum.png" style="width: 272;height: 152;"> </td> 
   <td> <p>Förväntad projicerad tidslinje som markerar [!UICONTROL Projected Start] och [!UICONTROL Completion dates] baserat på det arbete som har slutförts, plus återstående arbete. </p> <p>Mer information om planerade slutförandedatum finns i <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Översikt över [!UICONTROL Projected Completion Date] för projekt, uppgifter och problem</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera visningsalternativ

1. Gå till aktivitetslistan [!UICONTROL Gantt Chart] eller projektlistan [!UICONTROL Gantt Chart].\
   Mer information om var [!UICONTROL Gantt chart] finns finns i [Kom igång med [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Valfritt) Välj inställningen **[!UICONTROL Switch to Projected Dates]** om du vill visa aktiviteterna efter [!UICONTROL Projected Dates]. Som standard visas uppgifter av deras [!UICONTROL Planned Dates] i [!UICONTROL Gantt chart].
1. Klicka på alternativikonen för att visa dialogrutan **[!UICONTROL Options]**.\
   ![Alternativ.png](assets/options-350x129.png)

1. Välj de konfigurationsalternativ som du vill visa i [!UICONTROL Gantt chart].

   >[!NOTE]
   > Alla konfigurationsalternativ är inte tillgängliga i projektlistan [!UICONTROL Gantt Chart].

1. Klicka någonstans i [!UICONTROL Gantt chart] för att stänga dialogrutan **[!UICONTROL Options]**.
