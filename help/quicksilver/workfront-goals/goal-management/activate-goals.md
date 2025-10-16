---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktivera mål i Adobe Workfront-mål
description: När du skapar ett mål sparar Adobe Workfront Goals det med statusen Utkast. Ritade mål ingår inte i målhanteringen.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Aktivera mål i Adobe Workfront-mål

<!--Audited for P&P only: 4/2025-->

När du skapar ett mål sparar Adobe Workfront Goals det med statusen Utkast. Ritade mål ingår inte i målhanteringen.

Om du vill hålla reda på hur nära det är att uppnå ett mål genom att uppdatera dess förlopp måste du aktivera det. Detta ändrar dess status till Aktiv.

Mer information om hur du skapar ett mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Du måste aktivera ett mål innan du kan uppdatera förloppet för dess resultat och aktiviteter.


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
 <td role="rowheader">Konfigurationer på åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr>
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

## Förutsättningar

Om du vill aktivera ett mål måste det vara associerat med en förloppsindikator som en aktivitet, ett resultat, ett projekt eller så är det justerat mot ett annat aktivt mål.

Gör minst något av följande för att kunna aktivera ett mål:

* Lägg till ett resultat till målet

  Mer information finns i [Lägga till resultat i mål i Adobe Workfront &#x200B;](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Lägg till en aktivitet i målet

  Mer information finns i [Lägga till aktiviteter i mål i Adobe Workfront &#x200B;](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Koppla ett projekt till målet

  Mer information finns i [Lägga till projekt i mål i Adobe Workfront-mål](../results-and-activities/connect-projects-to-goals-overview.md).

* Justera ett annat mål mot det mål som du vill aktivera

  Mer information finns i [Justera mål genom att ansluta dem i Adobe Workfront-mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Aktivera mål

Du kan aktivera mål som du har skapat eller mål som du har behörighet att hantera.

1. Gå till ett mål som du vill aktivera. Målsidan öppnas.

1. Klicka på ikonen **Mer** ![Mer](../goal-management/assets/more-icon.png) till höger om målnamnet och klicka sedan på **Aktivera**.

   ![Mer meny utökad](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   Målstatusen ändras till Aktiv. Du kan nu följa förloppet för målet och se hur målet visas i incheckningsavsnittet. Du kan även se det i diagramavsnitten i Workfront-mål
