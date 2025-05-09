---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Justera mål genom att koppla dem till Adobe Workfront mål
description: Om du är en enskild deltagare som har ett personligt mål kanske du vill anpassa det till teamets mål för att effektivt visa hur ditt eget mål utvecklas i ett större sammanhang i organisationens strategi.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Justera mål genom att koppla dem till Adobe Workfront mål

<!--Audited P&P only: 04/2025-->

Om du är en enskild deltagare som har ett personligt mål kanske du vill anpassa det till teamets mål för att effektivt visa hur ditt eget mål utvecklas i ett större sammanhang i organisationens strategi.

När alla i organisationen har sina mål anpassade till organisationens mål kan de tydligt se hur deras individuella bidrag och teamsatsningar bidrar till att föra nålen framåt på större prioriteringar på företagsnivå. Mer information om de bästa sätten att justera mål finns i [Översikt över måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Det finns två sätt att koppla samman mål i Adobe Workfront-mål:

* Du kan skapa justering mellan mål genom att koppla samman mål med varandra.

* Du kan justera två mål manuellt eller konvertera resultat och aktiviteter för ett befintligt mål till ett annat mål. Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet.

>[!IMPORTANT]
>
>Ett mål kan innehålla totalt 1 000 resultatindikatorer.

I den här artikeln beskrivs hur du kan justera mål genom att koppla dem till varandra. Mer information om hur du justerar mål genom att konvertera resultat och aktiviteter till mål finns i [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

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
 <p>Aktuell licens: Begär eller högre</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
  <p> Nytt produktkrav: Workfront</p>
  eller
  <p>Aktuellt produktkrav: Förutom en Workfront-licens måste du köpa en licens för Adobe Workfront Goals. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Åtkomstnivå</td>
 <td> <p>Redigera åtkomst till mål</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objektbehörigheter</td>
 <td>

<p>Visa eller högre behörigheter för målet för att visa det</p>
  <p>Hantera behörigheter till målet för att redigera det</p>
  <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p>
   </td>
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

## Justera mål genom att koppla dem till varandra

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![Align to another goal](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![Aligned cards](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![Align icon](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Skapa två mål som du vill justera. Mer information om att skapa mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).
1. (Valfritt) Aktivera de mål som du vill justera. Du kan justera mål som har statusen Utkast, Aktiv eller Inaktiv. Mer information om hur du aktiverar mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).
1. Gå till målet som du vill justera (underordnat mål) mot ett annat mål (överordnat mål) och klicka på namnet för att öppna målsidan.

   >[!INFO]
   >
   >Om du till exempel vill att mål 2 ska påverka förloppet för mål 1 måste du gå till mål 2.

1. Klicka på **Målinformation** i den vänstra panelen.

1. Klicka på **Lägg till** i fältet **Överordnat mål** i området **Överordnad målinformation** om det inte finns något överordnat mål,

   eller

   Klicka på namnet på det överordnade målet och välj ett annat.

1. Börja skriva namnet på ett befintligt mål i fältet **Överordnat mål** och markera det sedan när det visas i listan. Endast mål från samma eller kommande perioder visas i listan.

1. Klicka på **Spara ändringar**.

   Målet som du började med (mål 2) är nu det underordnade målet för det överordnade målet som du justerade det mot (mål 1).\
   De justerade målen visas i avsnittet Måljustering med mål 2 som sekundärt till mål 1.
Det underordnade målet visas i avsnittet Förloppsindikatorer för det överordnade målet när förloppet uppdaterar förloppet för det överordnade målet.

   ![Justerade kort](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Valfritt) Om du vill visa målen i avsnittet Måljustering går du till målområdet i Workfront och klickar sedan på avsnittet **Måljustering** i den vänstra panelen. Mer information om avsnittet Måljustering finns i [Navigera i avsnittet Måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Valfritt) Lägg till aktiviteter och resultat i något av målen för att ange deras framsteg. Mer information om hur du lägger till aktiviteter och resultat finns i följande artiklar:

   * [Lägg till aktiviteter i mål i Adobe Workfront-mål](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Lägga till resultat i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Valfritt) Ta bort justeringen mellan två mål när du anser att det inte längre är relevant för organisationens övergripande strategi. Mer information om hur du tar bort justering mellan mål finns i [Ta bort måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

