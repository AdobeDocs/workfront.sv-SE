---
product-area: projects
navigation-topic: manage-projects
title: Kopiera ett projekt
description: Du kan kopiera ett projekt i stället för att skapa ett från början. Du kan bara kopiera ett projekt åt gången. Du kan inte kopiera projekt i grupp.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 93db334537b5ec12dc0c77d51f8b2d83d8348f3d
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Kopiera ett projekt

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

Du kan kopiera ett projekt från ett befintligt projekt i stället för att skapa ett från början, vilket sparar tid.

Observera att du inte kan kopiera projekt i grupp.

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
>* Budgeterade timmar
>
>Följande objekt kopieras alltid från ett befintligt projekt till ett nytt:
>
>* Uppgifter
>* Mall
>* Risker
>* Information om köinställningar
>* Portfolio och Program
>* Styrkort
>* Standardinformation för uppgift (Standardprocess för godkännande av uppgift, Anpassad Forms för standarduppgift)
>
> Datumen för det ursprungliga projektets uppgifter kopieras till det nya projektet. Du måste ändra start- eller slutdatumet för projektet (beroende på schemaläge) för att kunna uppdatera aktivitetsdatumen. Aktivitetsbegränsningar kan hindra dig från att ändra datum i projektet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.
Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td>  
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens</p> </td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
      </td> 
  </tr> 
     <td>Konfigurationer på åtkomstnivå </td> 
   <td> <p>Redigera åtkomst till projekt med möjlighet att skapa och kopiera projekt</p> </td> 
  </tr>

<td> <p>Objektbehörigheter </p> </td> 
   <td> <p>Visa behörigheter eller högre till projektet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Överväganden

* Bearbetningsgränsen är fem minuter vid kopiering av ett projekt. Om projektet har ett stort antal bifogade dokument och inte kan kopieras, kan du behöva ta bort en del av dokumenten och försöka igen.

## Kopiera ett enstaka projekt

När du kopierar ett projekt kopieras även viss information från det ursprungliga projektet till det nya projektet. Du kan också ange vilka objekt som inte ska kopieras till det nya projektet under kopieringsprocessen.

Kopiera ett projekt:

{{step1-to-projects}}

1. Välj det projekt som du vill kopiera från projektlistan och klicka sedan på ikonen **Mer** ![Mer meny](assets/more-icon.png) till höger om projektnamnet.

   eller

   Gå till en projektlista eller rapport och välj ett projekt och klicka sedan på ikonen **Mer** ![Mer meny](assets/more-icon.png) överst i listan.

1. Klicka på **Kopiera** i listrutan **Mer**. Dialogrutan **Kopiera av [projektnamn]** visas.

1. (Valfritt) Uppdatera **projektnamnet**. Som standard är det nya namnet **Kopia av [det ursprungliga projektnamnet]**.

   ![Kopiera projektruta](assets/copy-of-project-box.png)

1. Välj en **status**. Som standard är det ursprungliga projektets status valt.

1. (Valfritt) Avmarkera de objekt som du inte vill kopiera till det nya projektet. I följande tabell beskrivs vad som händer när du avmarkerar objekten:


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Markera alla</td> 
      <td> <p>Markerar alla alternativ och rensar alla fält och objekt som listas i det nya projektet. </p>

   <p> Om du avmarkerar det här alternativet avmarkeras alla objekt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td>Tar bort alla projekt- och aktivitetstilldelningar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förlopp</td> 
      <td>Tar bort förloppet för alla uppgifter och visar dem som Nytt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anpassade data</td> 
      <td> <p>Tar bort informationen från det anpassade formuläret i projektet, samt informationen om anpassade formulär som är kopplade till följande objekt:</p> 
       <ul> 
        <li>Uppgifter</li> 
        <li>Utgifter</li> 
        <li> Dokument</li> 
       </ul> 
      <p>De anpassade formulären förblir kopplade till uppgifter, utgifter, dokument och projekt, men informationen i formulärets anpassade fält kopieras inte till det nya projektet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td> <p>Tar bort allt på fliken Dokument, inklusive dokumentversioner, länkade dokument och mappar.</p> <p>Som standard kan dokumentkorrektur och godkännanden inte kopieras till ett annat projekt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alla föregående</td> 
      <td> <p>Tar bort alla föregående relationer mellan aktiviteterna i projektet. </p> <p>

   Föregångare som arbetar med flera projekt överför aldrig till det nya projektet, oavsett om det är markerat eller inte. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Budgeterade timmar</td> 
      <td> <p>Tar bort de timmar som har budgeterats i resursplaneringsområdet för projektets affärsärende från det kopierade projektet.</p> 
    <p>
   Timmar som har budgeterats med scenarioplaneraren kopieras aldrig till det nya projektet eftersom det nya projektet inte är länkat till något projekt i scenarioplaneraren. Mer information finns i <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budgetresurser i affärsärendet med scenarioplaneraren</a></p>
   </tr></td>
    <tr> 
      <td role="rowheader">Ekonomisk information</td> 
      <td> <p>Tar bort informationen i följande områden: </p> 
       <ul> 
        <li>Projektets finansieringsunderflik</li> 
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

1. Klicka på **Kopiera projekt**. Det kopierade projektet skapas.
