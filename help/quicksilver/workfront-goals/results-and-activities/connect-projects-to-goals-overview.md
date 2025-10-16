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
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Lägg till projekt i mål i Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Du kan koppla projekt till mål för att ange hur målet fortskrider, baserat på projektets faktiska förlopp. Projektet blir en förloppsindikator för målet.

Genom att koppla projekt till mål kan du koppla organisationens strategiska planering (mål) till det arbete som medarbetarna utför och slutför varje dag (projekt).

>[!IMPORTANT]
>
>Mål på projektnivå som skapats i ett projekts Business Case-område är inte kopplade till strategiska mål som skapats i Workfront-mål. Mer information om projektmål för affärsärenden finns i [Skapa mål för affärsärenden](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


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

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* När du tar bort ett projekt som är kopplat till ett mål tas även projektet bort från målet.

  >[!CAUTION]
  >
  >Om målet var aktivt innan du tog bort projektet och det inte finns några andra förloppsindikatorer för målet, blir målet inaktivt.


## Lägg till projekt i mål

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) (utkast för Shell: eller klicka på **Huvudmeny** ![Huvudmenyrader](assets/three-line-main-menu-icon.png) i det övre vänstra hörnet, om det är tillgängligt.) och sedan på **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka på **Förloppsindikatorer** i den vänstra panelen.
1. Klicka på **Lägg till befintligt projekt** i den nedrullningsbara menyn **Ny förloppsindikator**.

   Rutan Lägg till projekt i mål visas.
1. (Valfritt) Uppdatera **vyn**, **filtret** eller **grupperingen** genom att klicka på respektive ikoner i det övre högra hörnet av listan för att ändra hur projektlistan visas.
1. (Valfritt) Klicka på ikonen **Sök** ![Sök](assets/search-icon.png) och börja skriva namnet på ett projekt för att snabbt hitta det i listan.
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
