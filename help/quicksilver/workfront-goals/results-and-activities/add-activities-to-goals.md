---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Lägga till aktiviteter i mål i Adobe Workfront
description: Verksamheter mäter hur ett mål utvecklas. Utan associerade resultat, aktiviteter eller anpassade mål kan ett mål inte aktiveras och förloppet kan inte registreras på det.
author: Alina
feature: Workfront Goals
exl-id: 4d6ef324-4b5c-402b-b64d-b1a2a7d2ab57
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Lägga till aktiviteter i mål i Adobe Workfront

Verksamheter mäter hur ett mål utvecklas. Om du inte associerar resultat, aktiviteter, projekt eller anpassade mål kan du inte aktivera ett mål och du kan inte registrera förloppet för det.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> 
   <p>För den nya planen och licensstrukturen:
  <ul><li>En Ultimate-plan </li></ul>
   </p>
<p>För aktuell plan och licensstruktur: 
<ul><li> En Pro eller högre </li>
  <li>En Adobe Workfront Goals-licens förutom en Workfront-licens.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens*</td>
 <td>
 <p>Ny licens: Medarbetare eller högre</p>
 eller
 <p>Aktuell licens: Begär eller högre</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Nytt produktkrav, något av följande: </p>
<ul>
<li>A Select- eller Prime Adobe Workfront-plan och en extra licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå*</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Du måste ha ett befintligt mål för att lägga till aktiviteter i det.

Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Ett mål får inte innehålla mer än totalt 1 000 aktiviteter, resultat eller anpassade mål.

Mer information om aktiviteter finns i [Kom igång med resultat och aktiviteter i Adobe Workfront-mål](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md).

## Lägg till en aktivitet i ett mål

<!--
Adding activities to goals differs depending on which environment you use.

### Add an activity to a goal in the Production environment

1. Go to the goal for which you want to add an activity and click the name to open the **Goal Details** panel.
1. Click **Add activities**.

   ![Add activity inside goal](assets/add-activity-inside-goal-details-highlighted-350x152.png)

1. From the **Activity Type** drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select **Manual progress bar** or **Project**. Manual progress bar is the default selection. 
1. (Conditional) Depending on which activity type you selected, do the following:

   1. If you selected **Manual progress bar**:

      1. Start typing a name for your activity in the **Activity** field. 
      1. (Optional) If you want to set the activity owner as someone other than yourself, click your name in the **Owner** field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.

         >[!NOTE]
         >
         >You cannot assign a team or group as an activity owner.

         When you update the progress of an activity, the progress of the goal automatically updates.

   1. If you selected **Project**:

      1. Click the **Connect projects** field.

         Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. 
      
      1. Click the name of a project to add it as an activity to the goal. You can select several projects at one time.

         Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal.

         For more information about associating projects with goals, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

         >[!TIP]
         >
         >   
         >   * The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. 
         >   * You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in Workfront this also updates the connected project in Workfront Goals including the percent complete of the goal. 
         >   
         >

1. Click **Save**.

   The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

-->


1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) och sedan på **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Klicka på **Skapa aktivitet** i listrutan Ny förloppsindikator.

   Rutan Ny aktivitet öppnas.

   ![Ny aktivitetsruta](assets/new-activity-box-unshimmed.png)

1. Ange ett namn för aktiviteten i fältet för aktivitetsnamn. Detta är ett obligatoriskt fält.
1. (Valfritt) Ta bort ditt namn från fältet **Aktivitetsägare** om du vill tilldela aktiviteten till en annan användare. Som standard är du ägare av en aktivitet som du skapar.

   >[!NOTE]
   >
   >Du kan inte tilldela ett team, en grupp eller företaget som aktivitetsägare.

1. Klicka på **Skapa aktivitet** för att spara den och lägga till den i det valda målet.

   Aktiviteten visas i avsnittet Förloppsindikatorer på målsidan, under aktivitetsgrupperingen.





