---
product-previous: workfront-goals
navigation-topic: goal-management
title: Redigera mål i Adobe Workfront-mål
description: Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Redigera mål i Adobe Workfront-mål

Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.

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
<li>A Select- eller Prime Adobe Workfront-plan och ytterligare licens för Adobe Workfront Goals.</li>
<li>En Ultimate Workfront-plan som innehåller Workfront-mål som standard. </li></ul>
 <p>eller</p>
 <p>Aktuellt produktkrav: En Workfront-plan och ytterligare licens för Adobe Workfront-mål. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
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

## Att tänka på när du redigerar mål

* Du kan inte redigera mål med statusen Stängd.
* Du kan redigera mål från vilken tidsperiod som helst.

  Du kan redigera följande information för ett tidigare mål:

   * Namn
   * Tidsperiod
   * Status

     >[!TIP]
     >
     >Om målet är stängt beräknas förloppsprocenten som är slutförd om när du öppnar det igen. Du kan inte redigera ett stängt mål.

   * Beskrivning
   * Resultat och verksamhet

## Redigera mål

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) och sedan på **Mål**.\
   En lista med mål visas.
1. Klicka på ett mål.\
   Målsidan visas.

   ![](assets/goal-page-unshimmed.png)

1. Gör något av följande om du vill redigera information för målet:
   * Klicka på fält som visas i målhuvudet för att uppdatera dem. Alla fält i rubriken kan inte redigeras.
   * Klicka på ikonen **Mer** ![](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Redigera**.
   * Klicka på **Målinformation** i den vänstra panelen och klicka på ikonen **Redigera** ![](assets/edit-icon.png) i det övre högra hörnet. Klicka sedan på **Redigera alla**. Börja uppdatera fält i delen Målinformation.

     >[!IMPORTANT]
     >
     >Alla fält som visas i de områden som nämns ovan kan inte redigeras. Workfront beräknar några av fälten och de är skrivskyddade.

1. (Villkorligt) Beroende på vad du valde i det föregående steget ska du uppdatera följande information om målet:

   * Uppdatera följande information i målrubriken och tryck sedan på Retur för att spara ändringarna:
      * **Målnamn**: Klicka på målets namn och börja skriva ett nytt namn.
      * **Ägare**: Klicka på ägarnamnet och börja skriva namnet på en användare, grupp, grupp eller ditt företag. Markera sedan namnet när det visas i listan. Du kan bara ha en ägare för ett mål.
   * Uppdatera följande information i rutan Redigera mål och klicka sedan på **Spara**:
      * **Målnamn**
      * **Period**: Klicka för att uppdatera tidsperioden för målet\
        eller\
        Välj **Aktivera anpassade datum** om du vill ange datum för målets **start**- och **slutdatum**.

        >[!TIP]
        >
        >Avmarkera **Aktivera anpassade datum** om du vill återgå till den ursprungliga tidsperioden för målet.

      * **Målägare**
      * **Beskrivning**: Lägg till eller uppdatera information om målet.
   * Uppdatera eller granska information i avsnittet Målinformation. Mer information finns i [Uppdatera mål i avsnittet Målinformation i Adobe Workfront-mål](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Valfritt) Klicka på **Förloppsindikatorer** i den vänstra panelen för att lägga till resultat, aktiviteter eller projekt i målet. Genom att lägga till förloppsindikatorer kan du se till att du kan spåra målets framsteg.
Mer information finns i följande artiklar:
   * [Lägga till aktiviteter i mål i Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Lägg till resultat i mål i Adobe Workfront ](../results-and-activities/add-results-to-goals.md).
   * [Lägg till projekt i mål i Adobe Workfront-mål](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
