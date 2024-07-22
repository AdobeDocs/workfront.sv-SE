---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Kom igång med resultat och aktiviteter i Adobe Workfront-mål
description: Du måste lägga till resultat, aktiviteter eller anpassade mål till ett mål för att det ska kunna aktiveras. Detta uppdaterar målstatusen från Utkast till Aktiv och börjar registrera förloppet för målet.
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Kom igång med resultat och aktiviteter i Adobe Workfront-mål

>[!IMPORTANT]
>
>Din organisation måste ha följande för att kunna använda de funktioner som beskrivs i den här artikeln:
>
>* För den nya planen och licensstrukturen:
>
>   * Den ultimata Workfront-planen
>    
>* För aktuell plan och licensstruktur:
>
>   * En plan för Pro eller senare Workfront
>   * En Adobe Workfront Goals-licens förutom en Workfront-licens.
>
>Kontakta er kontoansvarige på Workfront för att få veta mer om en Workfront Goals-licens.
> 
>Mer information om åtkomst till Workfront-mål finns i [Krav för att använda Workfront-mål](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

När du skapar ett mål har målet statusen Utkast. Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

Om du vill börja spela in ett måls förlopp måste du aktivera det. Om du vill aktivera ditt mål och ändra dess status till Aktiv måste du först lägga till följande i det:

* Resultat
* En aktivitet
* Ett projekt
* Ett justerat mål

När minst ett av dessa objekt har lagts till kan du aktivera målet. Du måste uppdatera resultaten och aktiviteterna för målen för att kunna visa hur målet utvecklas.


>[!IMPORTANT]
>
> Ett mål får inte innehålla mer än totalt 1 000 aktiviteter, resultat, projekt eller justerade mål.</span>

I den här artikeln finns en översikt över aktiviteter och resultat. Mer information om att justera mål finns i [Måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/goal-alignment.md). Mer information om att ansluta projekt till mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](../results-and-activities/connect-projects-to-goals-overview.md).

## Resultatöversikt

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

Resultaten mäter hur långt du kommit med ditt mål eller hur nära du uppnår det. Som målägare kan du även äga resultatet. Ett resultat för ditt mål kan även tilldelas en annan användare.

Mer information om hur du lägger till resultat i mål finns i [Lägga till resultat i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-results-to-goals.md).

Du kan lägga till resultat till dina egna mål eller mål som tillhör andra enheter i organisationen.

Tänk på följande när du arbetar med resultat:

* De svarar på frågan&quot;Hur vet jag när mitt mål är klart?&quot;
* De är mätindikatorer. Du kan välja mellan följande alternativ för att ange förloppet för resultatet:

  <!--
  this might change (jira, Salesforce, etc))
  -->

   * Valuta
   * Nummer
   * Procent

Mer information om resultat finns i listan över likheter mellan resultat och aktiviteter i avsnittet [Likheter mellan resultat, aktiviteter och projekt](#similarities-between-results-activities-and-projects) i den här artikeln.

## Översikt över aktiviteter

<!--
This will have additional types in the future - add another section for types?
-->

Aktiviteter, som resultat, är specifika och mätbara och innehåller vanligen en procentsiffra för slutförande. Som målägare kan du även äga aktiviteter som är kopplade till målet. En aktivitet på ditt mål kan även tilldelas en annan användare.

Mer information om hur du lägger till aktiviteter i mål finns i [Lägga till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

Tänk på följande när du associerar aktiviteter med dina mål:

* De svarar på frågan&quot;Vad ska jag uppnå när målet är klart?&quot;
* Aktiviteter är anpassade poster som du kan tänka på mer i termer av fullständiga eller ofullständiga. De måste uppdateras manuellt för att ange vilken procentandel av aktiviteten som har slutförts hittills.

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

Mer information om resultat och aktiviteter finns i listan över likheter mellan resultat och aktiviteter i avsnittet [Likheter mellan resultat, aktiviteter och projekt](#similarities-between-results-activities-and-projects) i den här artikeln.

## Likheter mellan resultat, aktiviteter och projekt {#similarities-between-results-activities-and-projects}

Resultat, aktiviteter och projekt är indikatorer för målframsteg.

Det finns vissa skillnader i hur du hanterar projekt jämfört med hur du hanterar resultat och aktiviteter. Mer information om hur du lägger till projekt i mål finns i [Lägga till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md). Mer information om projekt som är kopplade till mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

Förutom resultat, aktiviteter och projekt kan du även koppla underordnade mål till ett mål. Underordnade mål är också en typ av förloppsindikator för ett mål. Mer information finns i [Justera mål genom att ansluta dem i Adobe Workfront-mål](../goal-alignment/align-goals-by-connecting-them.md). Förloppet för det underordnade målets förloppsindikatorer driver också förloppet för det överordnade målet.

I följande tabell visas likheter och skillnader mellan resultat, aktiviteter och projekt som målindikatorer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>Funktion</p></b></td> 
   <td><b><p>Resultat</p></b></td> 
   <td><b><p>Verksamhet</p></b></td> 
   <td> <p><strong>Projekt</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">Du kan anpassa objektnamnet i Workfront-gränssnittet</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Du kan lägga till dem till tidigare mål.</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Du kan associera flera resultat, aktiviteter eller projekt med samma mål. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Du kan koppla en av dem till flera mål.</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Deras framsteg beaktas vid beräkning av målförloppet. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>De måste uppdateras manuellt i Workfront-mål</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>De är klara på målets slutdatum</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>De kan bara tilldelas till en användare, och inte till ett team, en grupp eller företaget. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>De är specifika och mätbara och innehåller vanligtvis inställda tal som anger deras förlopp. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>De erbjuder ett intervall av värden mellan start- och slutvärdena som visar hur nära du uppnår dem. Närheten till slutvärdet beräknar ett förloppsvärde för ditt mål. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
