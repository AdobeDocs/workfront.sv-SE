---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Nivåresurser i [!UICONTROL Gantt Chart]
description: Information om hur du jämnar ut resurser i Gantt-schemat.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Nivåresurser i [!UICONTROL Gantt Chart]

Att fördela resurser i ett projekt har två syften:

* Justera automatiskt överallokering av tid för tilldelningar.
* Skapa automatiskt ett realistiskt aktivitetsschema för ett projekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] behörighet till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] tillgång till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Översikt över resursutjämning

Om samma resurs tilldelas två olika uppgifter kan du använda resursutjämning för att justera tidslinjen för aktiviteterna så att de inte inträffar samtidigt.

Tänk på följande när du utjämnar resurser i ett projekt:

* Resursutjämning gäller endast ett projekt, så [!DNL Adobe Workfront] nivåjusterar inte resurser över flera projekt åt gången.
* Om **[!UICONTROL Effort Driven]** väljs som **[!UICONTROL Duration Type]** kommer [!DNL Workfront] inte att jämna ut resurserna.
* När flera användare tilldelas till samma uppgift avbryts utjämningen.
* Villkoren för typen av **[!UICONTROL Task Constraint]** har företräde framför resursutjämningen. Om till exempel **[!UICONTROL Fixed Dates]** väljs som [!UICONTROL Task Constraint] ändras inte aktivitetsdatumen vid resursutjämning.
* Föregående relationer har företräde framför resursutjämning.
* **[!UICONTROL Resource Leveling]** måste anges till **[!UICONTROL Manual]** för projektet för att justera utjämningen i [!UICONTROL Gantt chart]. Om du har behörigheten Hantera för projektet kan du låta systemet automatiskt nivåindela resurser genom att justera den här inställningen för projektet och välja **[!UICONTROL Automatic]** i stället för **[!UICONTROL Manual]** i rutan **[!UICONTROL Edit Project]**.

  ![Resursutjämningsläge](assets/resource-leveling-mode-350x177.png)

* Som projektägare, eller tilldelad uppgift, kan du ange en nivåfördröjning för en aktivitet för att ange att det finns en stor risk att aktiviteten behöver extra tid. Mer information om hur du lägger till en nivåfördröjning för en aktivitet finns i [Uppdatera aktivitetens nivåfördröjning](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Använd resursutjämning i [!UICONTROL Gantt Chart]

Du kan använda uppgiftslistan [!UICONTROL Gantt Chart] för att jämna ut dina resurser.

1. Gå till det projekt som du vill nivåindela.
1. Klicka på ikonen **[!UICONTROL Gantt chart]** i området **[!UICONTROL Tasks]**.

   Alla ändringar sparas automatiskt när alternativet **[!UICONTROL Autosave]** aktiveras. Den är aktiverad som standard.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Plan]mode** och välj **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.

   >[!TIP]
   >
   >Du kan inte nivåindela resurser i [!UICONTROL Gantt Chart] när alternativet [!UICONTROL Autosave] är aktiverat.

   ![Manuell inställning har aktiverats](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicka på listrutan **[!UICONTROL Level Resources]**.

   ![Level_resources.png](assets/level-resouces.png)

1. Välj något av följande alternativ:

   * **[!UICONTROL Level Now]**: Resursutjämning används för den valda aktiviteten.
   * **[!UICONTROL Clear Leveling]**: Tar bort all resursutjämning från den valda aktiviteten.

   >[!NOTE]
   >
   >Resurserna kan vara överallokerade om de har tilldelats flera aktiviteter som inträffar under samma tidsram.

1. (Valfritt och villkorligt) Om du har inaktiverat alternativet Spara automatiskt klickar du på ikonerna **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar i [!UICONTROL Gantt Chart]:
   >
   >* [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] för att göra om.
   >* Windows: Använd [!UICONTROL Ctrl + Z] för att ångra och [!UICONTROL Ctrl + Y] för att göra om.


1. Klicka på **[!UICONTROL Save]** i det övre högra hörnet av [!UICONTROL Gantt chart].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
