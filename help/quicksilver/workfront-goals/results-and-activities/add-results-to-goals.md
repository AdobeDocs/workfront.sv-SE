---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Lägga till resultat i mål i Adobe Workfront
description: Resultaten mäter förloppet för ett mål. Om du inte kopplar resultat, aktiviteter eller justerade mål till ett mål kan du inte aktivera målet och du kan inte registrera förloppet för det.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Lägga till resultat i mål i Adobe Workfront

Resultaten mäter förloppet för ett mål. Om du inte kopplar resultat, aktiviteter eller justerade mål till ett mål kan du inte aktivera målet och du kan inte registrera förloppet för det.

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
 <td role="rowheader"><p>Åtkomstnivå</p></td>
 <td> <p>Redigera åtkomst till mål</p>  </td>
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

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

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

1. Klicka på huvudmenyn ![](assets/main-menu-icon.png) och sedan på **Mål**.

1. Öppna målsidan genom att klicka på namnet på ett mål i **mållistan**.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Expandera den nedrullningsbara menyn **Ny förloppsindikator** och klicka sedan på **Skapa resultat**.

   Rutan Nytt resultat öppnas.

   ![](assets/new-result-box-unshimmed.png)

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
