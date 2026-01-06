---
product-previous: workfront-goals
navigation-topic: goal-management
title: Redigera mål i Adobe Workfront-mål
description: Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Redigera mål i Adobe Workfront-mål

<!--Audited for P&P only: 10/2025-->

Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.

## Åtkomstkrav

>[!NOTE]
>
>Ditt företag kan välja att fortsätta använda Adobe Workfront-mål om de tidigare har köpt det här paketet. Du måste prata med din kontorepresentant för mer information.
>
>Adobe Workfront-mål går inte längre att köpa.

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront package</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licens</td>
 <td>
 <p>Medarbetare eller högre</p>
<p>Begäran eller senare</p></td>
 </tr>
  <tr>
 <td role="rowheader">Åtkomstnivåkonfiguration</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektbehörigheter</td>
 <td>
  <div>
  <p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive systemadministratörer, måste tilldelas en layoutmall som innehåller området Mål på huvudmenyn. </p>  
</td>
  </tr>
</tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

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
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

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

{{step1-to-goals}}

En lista med mål visas.

1. Klicka på ett mål.\
   Målsidan visas.

   ![Målsida](assets/goal-page-unshimmed.png)

1. Gör något av följande om du vill redigera information för målet:
   * Klicka på fält som visas i målhuvudet för att uppdatera dem. Alla fält i rubriken kan inte redigeras.
   * Klicka på ikonen **Mer** ![Mer ](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Redigera**.
   * Klicka på **Målinformation** i den vänstra panelen och klicka på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) i det övre högra hörnet. Klicka sedan på **Redigera alla**. Börja uppdatera fält i delen Målinformation.

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
