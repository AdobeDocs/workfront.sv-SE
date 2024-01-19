---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Nivåresurser i  [!UICONTROL Gantt Chart]
description: Information om hur du jämnar ut resurser i Gantt-schemat.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '524'
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

Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] tillgång till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Översikt över resursutjämning

Om samma resurs tilldelas två olika uppgifter kan du använda resursutjämning för att justera tidslinjen för aktiviteterna så att de inte inträffar samtidigt.

Tänk på följande när du utjämnar resurser i ett projekt:

* Resursutjämning gäller endast ett projekt, så [!DNL Adobe Workfront] delar inte resurser över mer än ett projekt i taget.
* If **[!UICONTROL Effort Driven]** markeras som en **[!UICONTROL Duration Type]**, [!DNL Workfront] kommer inte att jämna ut resurserna.
* När flera användare tilldelas till samma uppgift avbryts utjämningen.
* Villkor för typen av **[!UICONTROL Task Constraint]** har företräde framför resursutjämning. Om **[!UICONTROL Fixed Dates]** är markerat som [!UICONTROL Task Constraint], kommer resursutjämning inte att ändra aktivitetsdatumen.
* Föregående relationer har företräde framför resursutjämning.
* **[!UICONTROL Resource Leveling]** måste anges till **[!UICONTROL Manual]** för projektet för att justera utjämningen i [!UICONTROL Gantt chart]. Om du har behörigheten Hantera för projektet kan du låta systemet automatiskt nivåindela resurser genom att justera den här inställningen i projektet och välja **[!UICONTROL Automatic]** i stället för **[!UICONTROL Manual]** i **[!UICONTROL Edit Project]** box.

  ![](assets/resource-leveling-mode-350x177.png)

* Som projektägare, eller tilldelad uppgift, kan du ange en nivåfördröjning för en aktivitet för att ange att det finns en stor risk att aktiviteten behöver extra tid. Mer information om hur du lägger till en nivåfördröjning för en uppgift finns i [Uppdatera nivåfördröjning för aktivitet](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Använd resursutjämning i [!UICONTROL Gantt Chart]

Du kan använda uppgiftslistan [!UICONTROL Gantt Chart] för att jämna ut era resurser.

1. Gå till det projekt som du vill nivåindela.
1. I **[!UICONTROL Tasks]** klickar du på **[!UICONTROL Gantt chart]** -ikon.

   Alla ändringar sparas automatiskt när **[!UICONTROL Autosave]** är aktiverat. Den är aktiverad som standard.

1. (Valfritt) Klicka på **[!UICONTROL Plan]läge** ikon och markera **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.

   >[!TIP]
   >
   >Du kan inte jämna ut resurser i  [!UICONTROL Gantt Chart] när [!UICONTROL Autosave] är aktiverat.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicka på **[!UICONTROL Level Resources]** listruta.

   ![Level_resources.png](assets/level-resouces.png)

1. Välj något av följande alternativ:

   * **[!UICONTROL Level Now]**: Använder resursutjämning för den markerade aktiviteten.
   * **[!UICONTROL Clear Leveling]**: Tar bort all resursutjämning från den valda aktiviteten.

   >[!NOTE]
   >
   >Resurserna kan vara överallokerade om de har tilldelats flera aktiviteter som inträffar under samma tidsram.

1. (Valfritt och villkorligt) Om du har inaktiverat alternativet Spara automatiskt klickar du på **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** ikoner om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar på [!UICONTROL Gantt Chart]:
   >
   >* [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] att göra om.
   >* Windows: Använd [!UICONTROL Ctrl + Z] för att ångra och [!UICONTROL Ctrl + Y] att göra om.


1. Klicka **[!UICONTROL Save]** i det övre högra hörnet av [!UICONTROL Gantt chart].

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
