---
product-area: projects
navigation-topic: manage-projects
title: Kopiera ett projekt
description: Du kan kopiera ett projekt i stället för att skapa ett från början. Du kan bara kopiera ett projekt åt gången. Du kan inte kopiera projekt i grupp.
author: Alina
feature: Work Management
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 5e0e1425f45886a805726de49357c43b0aecb7f4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Kopiera ett projekt

<!--some areas are drafted for the 23.2 release story-->

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Du kan kopiera ett projekt i stället för att skapa ett från början. Du kan bara kopiera ett projekt åt gången. Du kan inte kopiera projekt i grupp.

>[!IMPORTANT]
>
>Följande objekt kopieras aldrig från ett befintligt projekt till ett nytt:
>
>* Problem
>* Faktureringstaxor
>* Faktureringsposter
>* Anteckningar
>* Timmar
>* Föregångare mellan projekt
>* Budgeterade timmar <!-- drafted for release 23.2: take this out and move it to the one below IF there is no UI component for the story that allows you to check/uncheck this information as you copy the project. If there is a UI component, take this out of here and just add it to the new screen shot below. -->
>
>Följande objekt kopieras alltid från ett befintligt projekt till ett nytt:
>
>* Uppgifter
>* Mall
>* Risker
>* Information om köinställningar
>* Portfolio och programmet
>* Styrkort
>* Standardinformation för uppgift (Standardprocess för godkännande av uppgift, Anpassad Forms för standarduppgift)
>


## Åtkomstkrav

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>Redigera åtkomst till projekt med möjlighet att skapa <span>och kopiera</span> projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>Visa behörigheter eller högre till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Kopiera ett enstaka projekt

När du kopierar ett projekt kopieras även viss information från det ursprungliga projektet till det nya projektet. Du kan också ange vilka objekt som inte ska kopieras till det nya projektet under kopieringsprocessen.

Så här kopierar du ett projekt:

1. Gå till projektet som du vill kopiera och klicka på **Mer** icon ![](assets/qs-more-menu.png) till höger om projektnamnet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   eller

   Gå till en projektlista eller rapport och välj ett projekt och klicka sedan på **Mer** icon ![](assets/qs-more-menu.png) högst upp i listan.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Klicka **Kopiera**.

1. Uppdatera namnet på det nya projektet.

   Som standard är det nya namnet **Kopia av `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Välj **Status** för det nya projektet.

   Som standard är **Status** matchar originalets egenskaper.

1. (Valfritt) Avmarkera de objekt som du inte vill kopiera till det nya projektet. I följande tabell beskrivs vad som händer när du avmarkerar objekten:

   <!--drafted for story for the 23.2 release: add another line in the table below for "Budgeted hours" and add this information to that row:
      Removes the hours budgeted in the Resource Planning area of the project's Business Case from the copied project. 
      <b>NOTE</b>
      Hours budgeted using the Scenario Planner are never copied to the new project because the new project is not linked to an initiative in the Scenario Planner. For more information, see <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budget resources in the Business Case using the Scenario Planner</a>
      -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Markera alla</td> 
      <td> <p>Markerar alla alternativ och rensar alla fält och objekt som listas i det nya projektet.</p> <p><b>TIPS</b>

   Avmarkera <strong>Markera alla</strong> avmarkerar alla objekt. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td>Tar bort alla projekt- och uppgiftstilldelningar</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förlopp</td> 
      <td>Tar bort förloppet för alla uppgifter och visas som Nytt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassade data</td> 
      <td> <p>Tar bort informationen från det anpassade formuläret i projektet, samt informationen om anpassade formulär som är kopplade till följande objekt:</p> 
       <ul> 
        <li>Uppgifter</li> 
        <li>Utgifter</li> 
        <li> Dokument</li> 
       </ul> <p><b>ANMÄRKNING</b>

   De anpassade formulären förblir kopplade till uppgifter, utgifter, dokument och projektet, men informationen i de anpassade fälten i formulären kopieras inte till det nya projektet. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td> <p>Tar bort allt på dokumentfliken, inklusive dokumentversioner, länkade dokument och mappar.</p> <p>Som standard kan dokumentkorrektur och godkännanden inte kopieras till ett annat projekt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alla föregående</td> 
      <td> <p>Tar bort alla föregående relationer mellan aktiviteterna i projektet. </p> <p>Tips: Föregångare som arbetar med flera projekt överför aldrig till det nya projektet, oavsett om det är markerat eller inte. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ekonomisk information</td> 
      <td> <p>Tar bort informationen i följande områden: </p> 
       <ul> 
        <li>Projektets underflik Ekonomi</li> 
        <li> Planerad förmån i affärsärendet</li> 
        <li>Ekonomisk information från alla uppgifter<br></li> 
       </ul> <p>Mer information om underfliken Projektfinansiering finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Hantera information i projektfinansieringsdelen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandeprocess</td> 
      <td>Tar bort alla godkännanden som är associerade med aktiviteterna eller projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td> Tar bort de påminnelsemeddelanden som är associerade med aktiviteterna eller projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td>Tar bort utgifter som är associerade med aktiviteterna eller projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Behörigheter</td> 
      <td> Tar bort behörigheter till alla användare för aktiviteterna eller projektet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Kopiera** för att skapa en kopia av projektet.

   Detta skapar ett nytt projekt som liknar det projekt du kopierade.

   Du kan börja göra ändringar i det nya kopierade projektet, som att granska aktivitetstilldelningar eller justera tidslinjer.
