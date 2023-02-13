---
product-previous: workfront-goals
navigation-topic: goal-management
title: Redigera mål i Adobe Workfront-mål
description: Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Redigera mål i Adobe Workfront-mål

Du kan redigera befintliga mål när som helst under en viss period och med vilken status som helst.

## Åtkomstkrav

<!--drafted - for P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>
-->

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Goals för att få tillgång till de funktioner som beskrivs i den här artikeln. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mål eller högre</p> <p><b>ANMÄRKNING</b>

<p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Hantera behörigheter för målet</p> 
     <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.
* Du har skapat de mål som du vill redigera eller så har du behörigheten Hantera för dem.

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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)och sedan klicka **Mål**.\
   En lista med mål visas.
1. Klicka på ett mål.\
   Målsidan visas.

   ![](assets/goal-page-unshimmed.png)

1. Gör något av följande om du vill redigera information för målet:
   * Klicka på fält som visas i målhuvudet för att uppdatera dem. Alla fält i rubriken kan inte redigeras.
   * Klicka på **Mer-ikon** ![](assets/more-icon.png) till höger om målnamnet och klicka sedan på **Redigera**.
   * Klicka **Målinformation** i den vänstra panelen och klicka på **Ikonen Redigera** ![](assets/edit-icon.png) i det övre högra hörnet och klicka sedan på **Redigera alla**. Börja uppdatera fält i delen Målinformation.

      >[!IMPORTANT]
      >
      >Alla fält som visas i de områden som nämns ovan kan inte redigeras. Workfront beräknar några av fälten och de är skrivskyddade.

1. (Villkorligt) Beroende på vad du valde i det föregående steget ska du uppdatera följande information om målet:

   * Uppdatera följande information i målrubriken och tryck sedan på Retur för att spara ändringarna:
      * **Målnamn**: Klicka på målets namn och börja skriva ett nytt namn.
      * **Ägare**: Klicka på namnet på ägaren och börja skriva namnet på en användare, ett team, en grupp eller ditt företag. Markera sedan namnet när det visas i listan. Du kan bara ha en ägare för ett mål.
   * Uppdatera följande information i rutan Redigera mål och klicka sedan på **Spara**:
      * **Målnamn**
      * **Period**: Klicka för att uppdatera tidsperioden för målet\
         eller\
         Välj **Aktivera anpassade datum** för att ange datum för målets **Starta** och **Slutdatum**.

         >[!TIP]
         >
         >Avmarkera **Aktivera anpassade datum** för att återgå till den ursprungliga tidsperioden för målet.

      * **Målägare**
      * **Beskrivning**: Lägg till eller uppdatera information om målet.
   * Uppdatera eller granska information i avsnittet Målinformation. Mer information finns i [Uppdatera mål i avsnittet Målinformation i Adobe Workfront-mål](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Valfritt) Klicka på **Förloppsindikatorer** i den vänstra panelen för att lägga till resultat, aktiviteter eller projekt till målet. Genom att lägga till förloppsindikatorer kan du se till att du kan spåra målets framsteg.
Mer information finns i följande artiklar:
   * [Lägga till aktiviteter i mål i Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Lägg till resultat i mål i Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Lägga till projekt i mål i Adobe Workfront-mål](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
