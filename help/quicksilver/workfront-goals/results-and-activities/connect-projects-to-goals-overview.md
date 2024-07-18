---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Lägg till projekt i mål i Adobe Workfront
description: Du kan koppla projekt till mål för att ange hur målet fortskrider, baserat på projektets faktiska förlopp. Projektet blir en förloppsindikator för målet.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 0%

---

# Lägg till projekt i mål i Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Du kan koppla projekt till mål för att ange hur målet fortskrider, baserat på projektets faktiska förlopp. Projektet blir en förloppsindikator för målet.

Genom att koppla projekt till mål kan du koppla organisationens strategiska planering (mål) till det arbete som medarbetarna utför och slutför varje dag (projekt).

>[!IMPORTANT]
>
>Mål på projektnivå som skapats i ett projekts Business Case-område är inte kopplade till strategiska mål som skapats i Workfront-mål. Mer information om projektmål för affärsärenden finns i [Skapa mål för affärsärenden](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


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
  <ul><li>En Ultimate-plan </li>
  eller
  <li>Ytterligare en licens för Adobe Workfront Goals för Prime- eller Select Adobe Workfront-planerna. </li></ul> </p>
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

## Att tänka på när du kopplar projekt till mål

* Du kan lägga till ett projekt som uppfyller följande villkor i ett mål:

   * Du måste ha minst behörighet att visa det.

     >[!NOTE]
     >
     >Om du förlorar din behörighet att visa projektet efter att du har kopplat projektet till målet, kan du fortfarande se projektinformation om målet, men du kan inte längre komma åt projektet.

   * Projektet får inte ha statusen Dead.

* Du kan associera flera projekt med ett mål.
* Du kan associera samma projekt med flera mål.
* Du kan inte uppdatera förloppet för ett projekt manuellt från målet som projektet är kopplat till. I stället beräknar Workfront hur stor procentandel av projektet som är färdigt och Workfront Target beräknar målförloppet med denna procentandel färdig. Detta uppdaterar målet i realtid efter att projektprocenten har uppdaterats.
* Projektets längd kan vara utanför tidsperioden för ett mål. Om ett projekt varar längre än målets deadline kan du fortfarande stänga målet och se det som slutfört, men målprocenten är inte 100 %. Procentandelen färdigt i projektet uppdateras inte längre för målet.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* När du tar bort ett projekt som är kopplat till ett mål tas även projektet bort från målet.

  >[!CAUTION]
  >
  >Om målet var aktivt innan du tog bort projektet och det inte finns några andra förloppsindikatorer för målet, blir målet inaktivt.


## Lägg till projekt i mål

1. Klicka på **huvudmenyn** ![](assets/main-menu-icon.png) (gör ett utkast för Shell: eller klicka på **huvudmenyn** ![](assets/three-line-main-menu-icon.png) i det övre vänstra hörnet, om det är tillgängligt.) och sedan på **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Klicka på **Lägg till befintligt projekt** i den nedrullningsbara menyn **Ny förloppsindikator**.

   Rutan Lägg till projekt i mål visas.
1. (Valfritt) Uppdatera **vyn**, **filtret** eller **grupperingen** genom att klicka på respektive ikoner i det övre högra hörnet av listan för att ändra hur projektlistan visas.
1. (Valfritt) Klicka på ikonen **Sök** ![](assets/search-icon.png) och börja skriva namnet på ett projekt för att snabbt hitta det i listan.
1. Markera de projekt som du vill lägga till i målet och klicka sedan på **Lägg till**.

   De valda projekten läggs till i målet och visas i avsnittet med förloppsindikatorer på målsidan, under grupperingen **Projekt**.

   När du har aktiverat målet uppdateras målets förlopp automatiskt när förloppet för ett projekt uppdateras. Mer information om hur du aktiverar ett mål finns i [Aktivera mål i Adobe Workfront-mål](../goal-management/activate-goals.md).

## Hitta projektinformation om mål

<p>
Följande projektinformation visas på målnivån i avsnittet Förloppsindikatorer på en målsida:

</p>

<table>
  <tr>
   <td>Projektnamn
   </td>
   <td>Alla ändringar i projektnamnet återspeglas också i det anslutna projektet.
   </td>
  </tr>
  <tr>
   <td>Projektägare
   </td>
   <td>Alla ändringar i projektägaren återspeglas också i det anslutna projektet.
   </td>
  </tr>
    <tr>
   <td>Faktiskt förlopp
   </td>
   <td> <p>Procent färdigt av projektet. Du kan inte uppdatera projektprocenten som har slutförts manuellt från målet. Workfront beräknar den automatiskt baserat på hur många procent av arbetsmomenten som har slutförts. </p>
   </td>
  </tr>
  <tr>
   <td>Förlopp
   </td>
   <td>Procent färdigt av projektet som representeras av en stapel. Om du ändrar procentandelen färdigt i projektet uppdateras automatiskt målförloppet såvida inte målet stängs.
   </td>
  </tr>

</table>

## Hitta målinformation i projekt

Följande målinformation visas i en projektlista eller -rapport:

| Målinformation | Beskrivning |
|---|---|
| Mål | En lista över alla mål som har ett projekt kopplat till sig. |
| Målhierarki | Hierarkin som ett mål tillhör. Endast målets överordnade och målet visas i det här fältet. Barnens mål visas inte. |
| Antal länkade mål | Antalet mål som är kopplade till ett projekt. |
