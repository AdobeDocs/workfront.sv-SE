---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktivera mål i Adobe Workfront-mål
description: När du skapar ett mål sparar Adobe Workfront Goals det med statusen Utkast. Ritade mål ingår inte i målhanteringen.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '489'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
  <p> Nytt produktkrav: Workfront</p>
 <p>eller</p>
  <p>Aktuellt produktkrav: Förutom en Workfront-licens måste du köpa en licens för Adobe Workfront Goals. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
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

+++

## Förutsättningar

Om du vill aktivera ett mål måste det vara associerat med en förloppsindikator som en aktivitet, ett resultat, ett projekt eller så är det justerat mot ett annat aktivt mål.

Gör minst något av följande för att kunna aktivera ett mål:

* Lägg till ett resultat till målet

  Mer information finns i [Lägga till resultat i mål i Adobe Workfront ](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Lägg till en aktivitet i målet

  Mer information finns i [Lägga till aktiviteter i mål i Adobe Workfront ](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

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
