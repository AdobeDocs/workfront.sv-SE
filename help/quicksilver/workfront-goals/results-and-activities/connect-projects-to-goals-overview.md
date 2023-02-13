---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Lägga till projekt i mål i Adobe Workfront-mål
description: Du kan koppla projekt till mål för att ange hur målet fortskrider, baserat på projektets faktiska förlopp. Projektet blir en förloppsindikator för målet.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Lägga till projekt i mål i Adobe Workfront-mål

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Du kan koppla projekt till mål för att ange hur målet fortskrider, baserat på projektets faktiska förlopp. Projektet blir en förloppsindikator för målet.

Genom att koppla projekt till mål kan du koppla organisationens strategiska planering (mål) till det arbete som medarbetarna utför och slutför varje dag (projekt).

>[!IMPORTANT]
>
>Mål på projektnivå som skapats i ett projekts Business Case-område är inte kopplade till strategiska mål som skapats i Workfront-mål. Mer information om projektmål för affärsärenden finns i [Skapa mål för affärsärenden](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Åtkomstkrav

<!--drafted for P&P release: replace the table below with this: 

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
   <td> <p>Redigera åtkomst till mål</p> <p><b>ANMÄRKNING</b>

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

Mer information om åtkomst till Workfront-mål finns på [Krav för att använda Workfront-mål](../goal-management/access-needed-for-wf-goals.md).

## Överväganden om att koppla projekt till mål

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

1. Klicka på **Huvudmeny** ![](assets/main-menu-icon.png) (draft this for Shell: eller klicka på **Huvudmeny** ![](assets/three-line-main-menu-icon.png) i det övre vänstra hörnet, om det är tillgängligt.) **Mål**.
1. Öppna målsidan genom att klicka på namnet på ett mål i mållistan.
1. Klicka **Förloppsindikatorer** i den vänstra panelen.
1. Från **Ny förloppsindikator** nedrullningsbar meny, klicka **Lägg till befintligt projekt**.

   Rutan Lägg till projekt i mål visas.
1. (Valfritt) Uppdatera **Visa**, **Filter**, eller **Gruppering** genom att klicka på respektive ikoner i det övre högra hörnet av listan för att ändra hur projektlistan visas.
1. (Valfritt) Klicka på **Sök** icon ![](assets/search-icon.png) och börja skriva namnet på ett projekt för att snabbt hitta det i listan.
1. Välj de projekt som du vill lägga till i målet och klicka sedan på **Lägg till**.

   De valda projekten läggs till i målet och visas i avsnittet med förloppsindikatorer på målsidan, under **Projekt** gruppering.

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
   <td>Faktisk status
   </td>
   <td> <p>Procent färdigt av projektet. Du kan inte uppdatera projektprocenten som har slutförts manuellt från målet. Workfront beräknar den automatiskt baserat på hur många procent av arbetsmomenten som har slutförts. </p>
   </td>
  </tr>
  <tr>
   <td>Förlopp
   </td>
   <td>Procent färdigt av projektet som representeras av ett fält. Om du ändrar procentandelen färdigt i projektet uppdateras automatiskt målförloppet såvida inte målet stängs.
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
