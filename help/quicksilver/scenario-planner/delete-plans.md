---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Ta bort planer i scenarioplanen
description: Du kan ta bort planer som du har skapat. Du kan inte ta bort planer som delas med dig.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Ta bort planer i [!DNL Scenario Planner]

Du kan ta bort planer som du har skapat. Du kan inte ta bort planer som delas med dig.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Aktuell: [!UICONTROL Business] eller högre</p>
   <p>Nytt: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td> <p>Nytt: Ljus eller högre</p> 
   <p>Aktuell: [!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> 
   <p>För nuvarande Workfront-planer: </p>
   <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om åtkomst och behörigheter för [!DNL Workfront Scenario Planner] finns i <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst som behövs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Åtkomstnivå </td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort planer

>[!IMPORTANT]
>
>Du kan inte återställa borttagna planer.

Du kan ta bort en plan eller ta bort ett scenario i en plan.

* [Ta bort planer](#delete-plans)
* [Ta bort scenarier](#delete-scenarios)

### Ta bort planer

>[!IMPORTANT]
>
>Tänk på följande när du tar bort planer:
>
>* All information som rör planen tas också bort. Detta inkluderar alla scenarier och initiativ som är kopplade till planen, inklusive information om roller och kostnader för jobb. Denna information kan inte återställas.
>* Om planen innehåller ett publicerat scenario bevaras de projekt som är länkade till de borttagna initiativen och området [!DNL Scenario Planner] finns kvar i avsnittet [!UICONTROL Project Details].
>
>  Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom publicering i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Så här tar du bort en plan:

{{step1-to-scenario-planner}}

En lista över planer visas.

1. Klicka på namnet på en plan för att öppna den.
1. Klicka på **[!UICONTROL More menu]** ![](assets/more-menu.png) till höger om plannamnet och klicka sedan på **[!UICONTROL Delete]** > **[!UICONTROL Yes, delete it]**.

   Planen tas bort och du återgår till listan över planer.

### Ta bort scenarier {#delete-scenarios}

>[!IMPORTANT]
>
>Tänk på följande när du tar bort ett scenario:
>
>* Om du tar bort ett scenario tas alla initiativ och deras information bort från scenariot. Om de kopieras till andra scenarier fortsätter initiativen i de andra scenarierna.
>* När du tar bort ett scenario får det efterföljande scenariot samma nummer som det borttagna scenariot och inventeringsordningen bevaras. Om du till exempel tar bort scenario 4 blir scenario 5 scenario 4.
>* Om vissa initiativ för scenariot publiceras bevaras projektet som är kopplat till initiativet och området för scenarioplanering finns kvar i de länkade projekten
>* Om de publicerade initiativen finns i ett annat scenario finns de kvar i det scenariot, inklusive deras länk till projektet. När du publicerar dessa initiativ från andra scenarier uppdateras de länkade projekten med ny information från dessa scenarier.
>
>  Mer information om publicering av projekt finns i [Uppdatera eller skapa projekt genom publicering i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Så här tar du bort ett scenario:

1. Gå till planen som du vill ta bort ett scenario för.

   Som standard visas det inledande scenariot.

1. Klicka på **[!UICONTROL Compare scenarios]**.
1. Klicka på **[!UICONTROL More]**-menyn ![](assets/more-menu.png) i det övre högra hörnet av scenariokortet och klicka sedan på **[!UICONTROL Delete]**.

   Scenariot tas bort.

1. Klicka på **[!UICONTROL Save plan]** om du vill spara ändringarna.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


