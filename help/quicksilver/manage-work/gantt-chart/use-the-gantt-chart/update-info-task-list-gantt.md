---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Uppdatera information i Gantt-schema för uppgiftslista
description: I Gantt-schemat för uppgiftslistan visas information om aktiviteter som finns i ett projekt eller en mall.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: e2f6eada24b4e48bce58189ec16447eda89f4a09
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Uppdatera information i uppgiftslistan [!UICONTROL Gantt Chart]

Uppgiftslistan [!UICONTROL Gantt Chart] innehåller information om aktiviteter som finns i ett projekt eller en mall.

I en mall återspeglar uppgiftslistan [!UICONTROL Gantt Chart] uppdateringar som gjorts i mallens uppgiftslista på aktivitetsnivå. Du kan inte redigera [!UICONTROL Gantt chart] som är associerad med en mall.

I ett projekt kan du uppdatera aktivitetsinformation direkt i uppgiftslistan [!UICONTROL Gantt Chart].

I den här artikeln beskrivs följande åtgärder som du kan utföra direkt i uppgiftslistan [!UICONTROL Gantt Chart]:

* Ändra aktivitetsvaraktighet
* Skapa eller ta bort tidigare relationer
* Ändra start- och slutdatum för aktivitet
* Procent av uppdatering klar
* Projektresurser på nivå

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
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till projekt och uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] tillgång till projektet och uppgifter </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Ändra aktivitetsvaraktighet

1. Gå till det projekt som du vill ändra.
1. Klicka på **[!UICONTROL Tasks]** i den vänstra panelen.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Klicka på ikonen **[!UICONTROL Gantt chart]**.

   ![Klicka på Gantt-schemaikonen](assets/click-gantt-chart-icon.png)

   Alla ändringar sparas automatiskt när alternativet **[!UICONTROL Autosave]** aktiveras. Den är aktiverad som standard.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Plan mode]** och välj **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Håll pekaren över tidslinjen för en uppgift och dra tidslinjen till ett annat datum.
1. Släpp indikatorn när du har nått rätt nya slutförandedatum för uppgiften.
1. (Valfritt och villkorligt) Om du har valt att spara ändringarna manuellt klickar du på ikonerna **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar i Gantt-schemat:
   >
   >   
   >   
   >   * [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] för att göra om.
   >   * [!DNL Windows]: Använd [!UICONTROL Ctrl + Z] för att ångra och [!UICONTROL Ctrl + Y] för att göra om.
   >   
   >

1. Klicka på **[!UICONTROL Save]** i det övre högra hörnet av [!UICONTROL Gantt chart].

## Skapa eller ta bort tidigare relationer

1. Gå till det projekt som du vill ändra.
1. Klicka på ikonen **[!UICONTROL Gantt chart]** i området **[!UICONTROL Tasks]**.

   Alternativet **[!UICONTROL Autosave]** är markerat som standard. I så fall sparas alla ändringar automatiskt.

   ![Klicka på Gantt-schemaikonen](assets/click-gantt-chart-icon.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Plan mode]** och välj **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Om du vill skapa en föregående relation klickar du på startpunkten för en uppgift och drar den till slutpunkten för uppgiften.
1. Om du vill ta bort en föregående relation klickar du på en föregående rad som ansluter två åtgärder för att markera den och trycker sedan på **[!UICONTROL Delete]** på tangentbordet.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Valfritt och villkorligt) Om du valde att spara ändringarna manuellt klickar du på ikonerna **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar i Gantt-schemat:
   >
   >   
   >   
   >   * [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] för att göra om.
   >   * [!DNL Windows]: [!UICONTROL Use Ctrl + Z] att ångra och [!UICONTROL Ctrl + Y] att göra om.
   >   
   >

1. Klicka på **[!UICONTROL Save]** .

## Ändra start- och slutdatum för aktivitet

1. Gå till det projekt som du vill ändra.
1. Klicka på ikonen **[!UICONTROL Gantt chart]** i området **[!UICONTROL Tasks]**.

   Alla ändringar sparas automatiskt när alternativet **[!UICONTROL Autosave]** aktiveras. Den är aktiverad som standard.

   ![Klicka på Gantt-schemaikonen](assets/click-gantt-chart-icon.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Plan mode]** och välj **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Håll muspekaren över mitten av uppgiften och leta upp pilen som löper i flera riktningar.
1. Klicka och dra aktiviteten till önskat datum.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Om du ändrar aktivitetsdatumet på ett sätt som påverkar aktivitetsbegränsningen klickar du på **[!UICONTROL Accept]** för att bekräfta ändringen av aktivitetsbegränsningen.

   >[!NOTE]
   >
   >Om aktiviteten har någon av följande begränsningar uppdateras [!UICONTROL Task Constraint] till [!UICONTROL Start No Earlier], om projektet är schemalagt från [!UICONTROL Start Date] eller [!UICONTROL Finish No Later Than] om projektet är schemalagt från [!UICONTROL Completion Date]:
   >
   >   
   >   
   >   * [!UICONTROL As Soon As Possible]
   >   * [!UICONTROL As Late As Possible]
   >   * [!UICONTROL Earliest Available Time]
   >   * [!UICONTROL Latest Available Time]
   >   
   >   
   >I vissa fall kan de föregående relationerna hindra aktiviteterna från att starta tidigare och det är inte tillåtet att flytta aktiviteten.

1. (Valfritt och villkorligt) Om du har valt att spara ändringarna manuellt klickar du på ikonerna **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar i [!UICONTROL Gantt chart]:
   >
   >   
   >   
   >   * [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] för att göra om.
   >   * [!DNL Windows]: Använd [!UICONTROL Ctrl + Z] för att ångra och [!UICONTROL Ctrl + Y] för att göra om.
   >   
   >

1. Klicka på **[!UICONTROL Save]**.

## Procent av uppdatering klar

1. Gå till det projekt som du vill ändra.
1. Klicka på ikonen **[!UICONTROL Gantt chart]** i området **[!UICONTROL Tasks]**.

   ![Klicka på Gantt-schemaikonen](assets/click-gantt-chart-icon.png)

   Alla ändringar sparas automatiskt när alternativet **[!UICONTROL Autosave]** aktiveras. Den är aktiverad som standard.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Plan mode]** och välj **[!UICONTROL Manual save Standard]** eller **[!UICONTROL Timeline Planning]** om du vill spara ändringarna manuellt.
1. Dubbelklicka på procenttalet i uppgiften och ange numret.

   >[!IMPORTANT]
   >
   >Du måste ha markerat [!UICONTROL % Complete] i dialogrutan [!UICONTROL Options] för att kunna uppdatera procent färdigt. Om du vill göra det klickar du på ikonen **[!UICONTROL Options]** och väljer **[!UICONTROL % Complete]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Valfritt och villkorligt) Om du valde att spara ändringarna manuellt klickar du på ikonerna **[!UICONTROL Undo]** eller &#x200B;**[!UICONTROL Redo]** om du vill avbryta eller duplicera någon av ändringarna.

   >[!TIP]
   >
   >Du kan använda följande kortkommandon för att ångra eller göra om ändringar i [!UICONTROL Gantt chart]:
   >
   >   
   >   
   >   * [!DNL Mac]: Använd [!UICONTROL Command + Z] för att ångra och [!UICONTROL Command + Shift + Z] för att göra om.
   >   * [!DNL Windows]: Använd [!UICONTROL Ctrl + Z] för att ångra och [!UICONTROL Ctrl + Y] för att göra om.
   >   
   >

1. Klicka på **[!UICONTROL Save]** i det övre högra hörnet av [!UICONTROL Gantt chart].

## Nivå projektresurser

Du kan använda uppgiftslistan [!UICONTROL Gantt Chart] för att jämna ut dina resurser.

Mer information om att jämna ut resurser i [!UICONTROL Gantt chart] finns i [Nivåresurser i [!UICONTROL Gantt Chart]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
