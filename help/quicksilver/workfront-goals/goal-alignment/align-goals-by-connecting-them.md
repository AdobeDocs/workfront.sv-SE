---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Justera mål genom att koppla dem till Adobe Workfront mål
description: Om du är en enskild deltagare som har ett personligt mål kanske du vill anpassa det till teamets mål för att effektivt visa hur ditt eget mål utvecklas i ett större sammanhang i organisationens strategi.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Justera mål genom att koppla dem till Adobe Workfront mål


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

<!--drfated for the P&P release: 

You must have the following:

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

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Justera mål genom att koppla dem till varandra

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Skapa två mål som du vill justera. Mer information om hur du skapar mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).
1. (Valfritt) Aktivera de mål som du vill justera. Du kan justera mål som har statusen Utkast, Aktiv eller Inaktiv. Mer information om hur du aktiverar mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).
1. Gå till målet som du vill justera (underordnat mål) mot ett annat mål (överordnat mål) och klicka på namnet för att öppna målsidan.

   >[!INFO]
   >
   >Om du till exempel vill att mål 2 ska påverka förloppet för mål 1 måste du gå till mål 2.

1. Klicka **Målinformation** i den vänstra panelen.

1. I **Överordnad målinformation** område, klicka **Lägg till** i **Överordnat mål** fält om det inte finns något överordnat mål,

   eller

   Klicka på namnet på det överordnade målet och välj ett annat.

1. Börja skriva namnet på ett befintligt mål i **Överordnat mål** markerar du det när det visas i listan. Endast mål från samma eller kommande perioder visas i listan.

1. Klicka **Spara ändringar**.

   Målet som du började med (mål 2) är nu det underordnade målet för det överordnade målet som du justerade det mot (mål 1).\
   De justerade målen visas i avsnittet Måljustering med mål 2 som sekundärt till mål 1.
Det underordnade målet visas i avsnittet Förloppsindikatorer för det överordnade målet när förloppet uppdaterar förloppet för det överordnade målet.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Valfritt) Om du vill visa målen i avsnittet Måljustering går du till målområdet i Workfront och klickar på **Måljustering** i den vänstra panelen. Mer information om måljustering finns i [Navigera i avsnittet Måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Valfritt) Lägg till aktiviteter och resultat i något av målen för att ange deras framsteg. Mer information om hur du lägger till aktiviteter och resultat finns i följande artiklar:

   * [Lägga till aktiviteter i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Lägg till resultat i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Valfritt) Ta bort justeringen mellan två mål när du anser att det inte längre är relevant för organisationens övergripande strategi. Mer information om hur du tar bort justeringen mellan mål finns i [Ta bort måljustering i Adobe Workfront-mål](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

