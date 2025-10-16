---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Lägga till resultat i mål i Adobe Workfront
description: Resultaten mäter förloppet för ett mål. Om du inte kopplar resultat, aktiviteter eller justerade mål till ett mål kan du inte aktivera målet och du kan inte registrera förloppet för det.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Lägga till resultat i mål i Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Resultaten mäter förloppet för ett mål. Om du inte kopplar resultat, aktiviteter eller justerade mål till ett mål kan du inte aktivera målet och du kan inte registrera förloppet för det.

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
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

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.
* Ett befintligt mål.

  Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Ett mål får inte innehålla mer än totalt 1 000 aktiviteter, resultat, projekt eller anpassade mål.

## Lägg till ett resultat i ett mål

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Klicka på ikonen Huvudmeny ![Huvudmeny](assets/main-menu-icon.png) och sedan på **Mål**.

1. Öppna målsidan genom att klicka på namnet på ett mål i **mållistan**.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Expandera den nedrullningsbara menyn **Ny förloppsindikator** och klicka sedan på **Skapa resultat**.

   Rutan Nytt resultat öppnas.

   ![Ny resultatruta](assets/new-result-box-unshimmed.png)

1. Ange ett namn för resultatet i fältet **Resultatnamn**. Detta är ett obligatoriskt fält.
1. (Valfritt) Ta bort ditt namn från fältet **Resultatägare** om du vill tilldela resultatet till en annan användare. Som standard är du ägare av en aktivitet som du skapar.

   >[!NOTE]
   >
   >Du kan inte tilldela ett team, en grupp eller företaget som resultatägare.

1. I **Hur vill du mäta resultatet?** anger du följande information:
   * **Värdetyp**: Detta anger hur du vill mäta förloppet för resultatet. Du kan mäta förloppet numeriskt, med ett procentvärde eller med ett valutabelopp.

     Välj en värdetyp bland alternativen i följande tabell:

     | Värdetyp | Beskrivning |
     |---------------------------------------------------------|------------------|
     | Nummer | Nummervärde |
     | % | Procentvärde |
     | CN¥,DKK,KR,Mex$, R, R$, zolika, £ ,¥ , € , ₹, ฿, MYR, ₪, $ | Valutavärden |

   * **Startvärde**: Det värde som resultatet har i början, innan förloppet har spelats in.
   * **Målvärde**: Det värde som resultatet ska uppnå när det anses vara slutfört.
1. Klicka på **Skapa resultat**.

   Resultatet visas i avsnittet Förloppsindikatorer på målsidan, under resultatgrupperingen.

   När du har aktiverat målet uppdateras målets förlopp automatiskt när du uppdaterar förloppet för ett resultat. Mer information om hur du aktiverar ett mål finns i [Aktivera mål i Adobe Workfront-mål](../goal-management/activate-goals.md).
