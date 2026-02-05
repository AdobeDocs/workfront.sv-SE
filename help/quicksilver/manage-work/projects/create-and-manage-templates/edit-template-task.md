---
product-area: templates
keywords: uppgift,standard,automatisera,skapa
navigation-topic: templates-navigation-topic
title: Redigera mallaktivitet
description: När du har skapat en mall kan du redigera information om malluppgifterna. Den information som du uppdaterar för en malluppgift kopplas till projektuppgifter när du har använt mallen för att skapa ett projekt eller bifogat mallen till ett projekt.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: c9fa6d97607990710e6c2a74f3b373d06201d721
workflow-type: tm+mt
source-wordcount: '7460'
ht-degree: 0%

---

# Redigera malluppgifter

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<div class="preview">

Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner är också tillgängliga i produktionsmiljön för alla kunder från och med en vecka från förhandsversionen.

Mer information finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

När du har skapat en mall kan du redigera informationen för malluppgifterna. Den information som du uppdaterar för en malluppgift kopplas till projektuppgifter när du har använt mallen för att skapa ett projekt eller bifogat mallen till ett projekt.

Mer information om hur du skapar en mall finns i [Skapa en projektmall](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Du kan redigera en malluppgift åt gången eller redigera flera malluppgifter samtidigt.

>[!NOTE]
>
>Du kan inte redigera malluppgifter som tillhör olika mallar samtidigt. Du kan bara redigera malluppgifter som tillhör samma mall.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till mallar</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter </td> 
   <td> <p>Hantera behörigheter för en mall. </p> <p>Du kan inte dela en malluppgift. </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Innan du börjar måste du

* Skapa en mall.

  Mer information om hur du skapar en mall finns i [Skapa en projektmall](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Redigera malluppgifter

Redigeringen av malluppgifter skiljer sig åt beroende på vilken miljö du väljer att redigera uppgifterna.

### Redigera malluppgifter i produktionsmiljön

>[!NOTE]
>
><span class="preview">Vissa kunder kan redigera malluppgifter i sina produktionsmiljöer på samma sätt som de redigerar dem i sin förhandsvisningsmiljö.</span>
>
><span class="preview">Mer information om hur du redigerar uppgifter i förhandsvisningsmiljön finns i avsnittet [Redigera malluppgifter i förhandsvisningsmiljön](#edit-template-tasks-in-the-preview-environment) i den här artikeln. </span>


Du kan redigera en malluppgift med området Redigera malluppgift eller Malluppgiftsinformation.

{{step1-to-templates}}

1. Klicka på namnet på en mall för att öppna den.
1. Klicka på **Malluppgifter** i den vänstra panelen.
1. Klicka på namnet på en malluppgift i listan för att öppna malluppgiften.
1. Så här redigerar du begränsad information om mallaktiviteten:
   1. (Valfritt) Klicka på **Uppdateringar** i den vänstra panelen för att lägga till uppdateringar i mallaktiviteten. Uppdateringar av malluppgifter överförs inte till projektaktiviteter när mallen används för att skapa ett projekt.
   1. (Valfritt) Klicka på **Dokument** i den vänstra panelen för att lägga till dokument i mallåtgärden. Dokumenten överförs till projektuppgifterna när du använder mallen för att skapa projektet.
   1. (Villkorligt) Om du vill redigera begränsad information om en malluppgift klickar du på **Information om malluppgift** i den vänstra panelen. Gå sedan till områdena i detaljavsnittet för att redigera information för varje område.
   1. (Valfritt) Gör något av följande:
      * Klicka på ikonen **Komprimera alla** ![Komprimera alla ](assets/collapse-all-icon.png) om du vill komprimera alla områden.
      * Klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) och välj sedan något av områdena nedan. Du kan också klicka på **Redigera alla** om du vill redigera information i alla områden:

         * Översikt
         * Anpassad Forms
Namnen på tullformulär visas bara om det finns anpassade formulär kopplade till malluppgiften.
         * Ekonomi

        >[!TIP]
        >
        >Om du vill ha information om alla fält som visas i området Detaljer kan du fortsätta redigera alla fält med rutan Redigera malluppgift, som beskrivs nedan.

   1. (Valfritt) Klicka på avsnittet **Underaktiviteter** i den vänstra panelen för att lägga till underordnade för malluppgiften. Att lägga till underaktiviteter för malluppgifter liknar att lägga till underaktiviteter för projektaktiviteter. Mer information finns i avsnittet Skapa underaktiviteter från avsnittet Underaktiviteter för aktiviteter i artikeln [Skapa underaktiviteter](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Valfritt) Klicka på **Utgifter** i den vänstra panelen och lägg till utgifter i malluppgifterna. Malluppgiftsutgifter överförs till framtida projektaktiviteter när mallen används för att skapa ett projekt.
   1. (Valfritt) Klicka på **Godkännanden** i den vänstra panelen för att skapa godkännanden eller koppla globala godkännanden eller godkännanden på gruppnivå till mallåtgärderna. Godkännandena överförs till framtida projektaktiviteter.
   1. (Valfritt) Klicka på avsnittet **Föregående** i den vänstra panelen för att lägga till föregående för malluppgifterna. Att lägga till malluppgiftsföregångare liknar att lägga till föregångare för projektaktiviteter. Mer information finns i [Skapa en föregående relation med området Föregående användare](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Valfritt) Om du vill redigera flera malluppgifter samtidigt markerar du flera malluppgifter och klickar sedan på **Redigera** överst i malllistan.
1. (Villkorligt) Om du vill redigera all information om mallaktiviteten eller om flera åtgärder samtidigt klickar du för att markera dem i en lista och sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) längst upp i listan.

   Rutan **Redigera mallaktivitet** visas i den nya upplevelsen.

   ![Ny upplevelse för aktiviteten Redigera mall](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Du kan också välja en malluppgift i en lista och sedan klicka på **Redigera** till höger om malluppgiftens namn i sidhuvudet för att öppna rutan **Redigera malluppgift** .

   Fortsätt redigera mallaktiviteten enligt beskrivningen i avsnittet [Redigera en malluppgift med den nya funktionen](#edit-a-template-task-using-the-new-experience) i den här artikeln.

1. (Valfritt) Klicka på **Byt tillbaka till den gamla versionen** längst ned i rutan **Redigera mallaktivitet** för att öppna rutan **Redigera mallaktivitet** i den gamla versionen.

   ![Redigera malluppgift](assets/edit-template-tasks-box-classic-350x356.png)

1. Det kan vara bra att ange information i följande avsnitt:

   * [Översikt](#overview)
   * [Ekonomi](#finance)
   * [Inställningar](#settings)
   * [Uppdrag](#assignments)
   * [Anpassad Forms](#custom-forms)
   * [Kommentar](#comment)

1. Fortsätt redigera mallaktiviteten enligt beskrivningen i avsnittet [Redigera en malluppgift med den gamla funktionen](#edit-a-template-task-using-the-old-experience) i den här artikeln.

#### Redigera en malluppgift med den gamla funktionen

##### Översikt {#overview}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Översikt**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Namn</strong> </td> 
      <td>Ange ett namn för mallaktiviteten. Det här fältet visas inte när malluppgifter redigeras samtidigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Lägg till ytterligare information om mallaktiviteten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Ange en webblänk som relaterar till informationen om mallaktiviteten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet</strong> </td> 
      <td> <p>Det här är en visuell flagga som gör att du kan prioritera mallåtgärder. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ingen</strong> </p> </li> 
        <li> <p><strong>Låg</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>Hög</b> </p> </li> 
        <li> <p><b>Brådskande</b> </p> </li> 
       </ul> <p>Beroende på vilka projektinställningar du har valt av Workfront-administratören kan prioritetsnamnen vara olika för dig. Mer information om redigeringsprioriteringar finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Skapa och anpassa prioriteringar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Varaktighetstyp</strong> </td> 
      <td> <p>Den framtida uppgift som skapas från den här mallen kommer att ha den här varaktighetstypen. <br>Varaktighetstyp identifierar relationen mellan följande:</p> <p>- antal resurser som tilldelats en aktivitet</p> <p>- den totala arbetsinsats som krävs för att slutföra uppgiften</p> <p>- uppgiftens totala varaktighet. </p> <p>Med varaktighetstyper kan du ange konsekventa resurstilldelningar baserat på uppgiftens behov. Mer information om varaktighetstypen för en aktivitet finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>.</p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Beräknad tilldelning</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Beräknat arbete</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Ansträngningsstyrd</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Enkel</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Varaktighet</strong> </td> 
      <td> <p>Ange varaktigheten för framtida uppgifter i minuter, timmar, dagar, veckor eller månader. Den framtida uppgift som skapas från den här mallen har den varaktighet som anges här.</p> <p>Som standard mäter Workfront Varaktighet i dagar. Det här är den tid som du tillåter att aktiviteten förblir ofullständig innan den måste slutföras. Du kan inte ange varaktigheten för en aktivitet när aktivitetens <strong>Varaktighetstyp</strong> är <strong>Enkel</strong> eller när <strong>Aktivitetsbegränsning</strong> är <strong>Fasta datum</strong>.</p> <p><b>VIKTIGT</b></p> <p>Varaktighet är vanligtvis den tid som förflyter mellan planerad start och planerad slutförandetid för en mallaktivitet, och av den anledningen påverkar den mallens tidslinje. Detta avgör tidslinjen för det framtida projekt som skapas från mallen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planerade timmar</strong> </td> 
      <td> <p>Ange antalet planerade timmar för den framtida aktiviteten i det projekt som skapas med den här mallen. Detta är den faktiska tid det skulle ta för uppgiftens tilldelare att slutföra den. Du kan bara ange antalet planerade timmar för en aktivitet när varaktighetstypen <strong>är inställd på </strong>Beräknat uppdrag<strong>.</strong> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Aktivitetsbegränsning</strong> </td> 
      <td> <p>Aktiviteten i projektet som skapas från den här mallen har den här begränsningen. Uppgiftsbegränsningar identifierar när en uppgift måste slutföras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li><strong>Fasta datum</strong>. Ange en <strong>planerad start</strong> och ett <strong>planerat slutförandedatum.</strong></li> 
        <li><strong>måste börja </strong>. Ange ett <strong>planerat startdatum.</strong></li> 
        <li><strong>Måste avslutas </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Så snart som möjligt</strong> </li> 
        <li><strong>Så sent som möjligt</strong> </li> 
        <li style="font-weight: bold;"><strong>Tidigaste tillgängliga tid</strong> </li> 
        <li style="font-weight: bold;"><strong>Senaste tillgängliga tid</strong> </li> 
        <li>Börja inte senare än. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Starta inte tidigare än </strong>. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Slutför inte senare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Slutför inte tidigare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
       </ul> <p>Mer information om uppgiftsbegränsning finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Startdag</span><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange startdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul> 
        <li>Måste börja på</li> 
        <li>Starta tidigast</li> 
        <li>Starta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar det datum inom tidslinjen för det framtida projektet då aktiviteten startar. För alla andra begränsningar beräknas startdagen i Workfront baserat på föregående beroende mellan uppgifterna. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Slutförandedag</strong><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange slutdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Måste avslutas</li> 
        <li>Avsluta tidigast</li> 
        <li>Avsluta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar datumet inom tidslinjen för det framtida projektet när aktiviteten ska slutföras. För alla andra begränsningar beräknar Workfront Slutförandedagen baserat på Varaktighet och föregående beroende. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

##### Ekonomi {#finance}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Ekonomi**.

   ![edit_task_Finance.png](assets/edit-task-finance-350x216.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Kostnadstyp</strong> </td> 
      <td> <p>Ange kostnadstyp för den framtida aktiviteten. Detta avgör hur Kostnaden för aktiviteten beräknas, baserat på antalet timmar för aktiviteterna. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Ingen kostnad</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Korrigerad timme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Användartimme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Roll varje timme</span> </p> </li> 
       </ul> <p>Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Intäktstyp</strong> </td> 
      <td> <p>Ange intäktstyp för den framtida aktiviteten. Det här avgör hur Intäkten för uppgiften beräknas, baserat på antalet timmar för uppgifterna.</p> <p style="font-weight: normal;">Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Ej fakturerbar</p> </li> 
        <li> <p style="font-weight: normal;">Användare per timme</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis</p> </li> 
        <li> <p style="font-weight: normal;">Fast en timme</p> </li> 
        <li> <p style="font-weight: normal;">Användartimme med versaler</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis med ändpunkt</p> </li> 
        <li> <p style="font-weight: normal;">Användarens timma plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Fast intäkt</p> </li> 
       </ul> <p>Mer information om att spåra intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

##### Inställningar {#settings}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Inställningar**.

   ![Redigera inställningar för mallaktivitet](assets/edit-template-tasks-settings-classic-350x231.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milstolpe</b></p></strong> </td> 
      <td> <p>Välj en milstolpe som ska associeras med den valda malluppgiften.</p>

   <p><b>VIKTIGT</b></p>
   <p>Du måste associera en milstolpe-sökväg med en mall för att det här fältet ska kunna visas. Mer information finns i <a href="../create-and-manage-templates/edit-templates.md">Redigera projektmallar</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Spårningsläge</strong> </td> 
      <td> <p>Ange hur förloppsstatusen för den framtida aktiviteten ska spåras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Användaren måste uppdatera</strong> </p> </li> 
        <li> <p><strong>Anta i tid</strong> </p> </li> 
        <li> <p><strong>Ignorera sena varningar</strong> </p> </li> 
        <li> <p><strong>Komplettera automatiskt</strong> </p> </li> 
        <li> <p><strong>Föregående</strong> </p> </li> 
       </ul> <p>Mer information om spårningsläget för uppgifter finns i <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Översikt över spårningsläget för aktiviteter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Godkännandeprocess</strong> </td> 
      <td> <p>Välj den godkännandeprocess som du vill associera med malluppgiften. Workfront-administratören måste definiera processer för godkännande av uppgifter på systemnivå innan du kan koppla dem till malluppgifter. <span>En användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.</span> Mer information om hur du skapar godkännandeprocesser finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Skapa en godkännandeprocess för arbetsobjekt</a>.</p> <p>Tänk på följande när du lägger till godkännandeprocesser: </p> 
       <ul> 
       <li>Endast aktiva godkännandeprocesser visas i listan. </li> 
       <li> <p>Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. Godkännandeprocesser som är kopplade till en annan grupp än mallens visas inte i listan.</p> <p>Viktigt: Om gruppen som är kopplad till mallen ändras blir den gruppspecifika godkännandeprocessen en godkännandeprocess för enstaka användning. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>. </p> </li> 
       <li> <p>Om du har lagt till en godkännandeprocess för en enstaka användning visas den som &lt;Anpassad&gt; i det här fältet. Mer information finns i <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associera en ny eller befintlig godkännandeprocess med arbete</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>När malluppgifter gruppredigeras finns följande scenarier:</p> 
       <ul> 
       <li> <p>När du väljer malluppgifter från samma mallgrupp visas både godkännandeprocesser på system- och gruppnivå i det här fältet.</p> </li> 
       <li> <p>När du väljer malluppgifter från olika mallgrupper visas endast godkännandeprocesser på systemnivå i det här fältet.</p> </li> 
       <li> <p>När någon av malluppgifterna har en enda godkännandeprocess, ersätts den av den process på systemnivå <span>eller på gruppnivå</span> som du väljer. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Påminnelsemeddelanden</strong> </td> 
      <td> <p>Välj vilka påminnelsemeddelanden som du vill bifoga till malluppgiften. De kommer att bifogas till de framtida aktiviteterna i projektet som skapas från den här mallen. Systemadministratören måste konfigurera påminnelsemeddelanden innan du kan välja dem för en uppgift. Mer information om hur du konfigurerar påminnelsemeddelanden finns i <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Konfigurera påminnelsemeddelanden</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

##### Uppdrag {#assignments}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Uppdrag**.

   ![tilldelningar_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Klicka på **Lägg till tilldelad** för att lägga till en ny tilldelad till malluppgiften. Du kan tilldela användare, roller eller team till en uppgift. Du kan ha flera tilldelningar för en uppgift. De framtida aktiviteterna tilldelas samma resurser när de skapas från den här malluppgiften.
1. (Valfritt) Om du har flera tilldelningar markerar du alternativknappen **Ägare** för att ange vilken användare eller roll som betraktas som aktivitetsägare eller primär tilldelad. Workfront markerar den första användaren eller jobbrollen som du tilldelar en malluppgift som ägare eller primär tilldelad.
1. (Villkorligt och valfritt) Om **Varaktighetstypen** är **Beräknat arbete** eller **Ansträngningsstyrt** anger du **Allokering %** (allokeringsprocent) för varje tilldelad. Det här är den tid från schemat för den tilldelande personen som de kan lägga på den här aktiviteten. Om du ändrar allokeringsprocenten för en tilldelad ändrar du planerad tid för en uppgift.
1. (Villkorligt och valfritt) Om **Varaktighetstypen** är **Enkel** anger du **Timmar** för varje tilldelad

   eller

   Ange det totala antalet **Planerade timmar** för mallaktiviteten. Detta fördelar de totala timmarna jämnt mellan alla tilldelningar.

1. (Villkorligt och valfritt) Om **Varaktighetstypen** är Enkel anger du **Varaktighet** för mallaktiviteten i dagar. Detta blir varaktigheten för den uppgift som skapas från den här mallen.
1. (Valfritt) Välj en roll i listrutan **Tilldelningens roll**. Det är den roll som den som tilldelas kan utföra den här framtida uppgiften. Endast de jobbroller som är kopplade till varje tilldelad i deras profil visas i listrutan.
1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

##### Anpassad Forms {#custom-forms}

Du kan definiera anpassade formulär som ska bifogas automatiskt som standard till uppgifter när uppgifterna läggs till i ett projekt. Mer information om hur du konfigurerar projektet så att det innehåller anpassade formulär för standarduppgifter finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Du kan också lägga till anpassade formulär till de framtida uppgifterna i ett projekt när projektet skapas från en mall genom att lägga till anpassade formulär till malluppgifterna.

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Anpassad Forms**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Markera det eller de anpassade formulär som du vill koppla till malluppgiften.

   Du måste skapa anpassade formulär innan de kan väljas i det här fältet.
Endast aktiva anpassade formulär visas i listan.
Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Du kan lägga till upp till tio anpassade formulär i en mallåtgärd.
Formulären läggs automatiskt till i de uppgifter som skapas från mallen.
1. (Villkorligt och valfritt) Om du har kopplat ett anpassat formulär till malluppgiften kan du redigera alla fält i formuläret. Du måste ange alla obligatoriska fält innan du kan spara malluppgiften.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör anger behörigheter för avsnitten i ditt anpassade formulär kan inte alla visa eller redigera samma fält i ett visst anpassat formulär. Behörigheterna att redigera fält i ett avsnitt i ett anpassat formulär beror på vilka behörigheter du har för malluppgiften eller den framtida uppgiften.\
   >Mer information om att ange behörigheter för avsnitt i ett anpassat formulär finns i [Dela ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Mer information om hur du anger aktivitetsbehörigheter finns i [Dela en uppgift](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Mer information om hur du ställer in mallbehörigheter finns i [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

##### Kommentar {#comment}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Kommentar**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Ange en kommentar som du vill visa i uppdateringsströmmen för malluppgiften i det tillgängliga fältet. Den här kommentaren är synlig för alla som har åtkomst till mallen och malluppgiften och tillgång till vyn Anteckningar.
1. Klicka på **Spara ändringar**.

   När du eller någon annan användare skapar ett projekt från den här mallen används alla inställningar som du har tillämpat på malluppgifter som inställningar för projektuppgifterna.

#### Redigera en malluppgift med den nya funktionen

När du har öppnat rutan **Redigera malluppgift** i den nya versionen bör du överväga att ange information i något av följande avsnitt:

* [Malluppgiftsnamn](#template-task-name)
* [Översikt](#overview-1)
* [Uppdrag](#assignments-1)
* [Ekonomi](#finance-1)
* [Anpassad Forms](#custom-forms-1)
* [Inställningar](#settings-1)
* [Kommentar](#comment-1)

##### Malluppgiftsnamn

>[!TIP]
>
>Avsnittet Malluppgiftsnamn är inte tillgängligt när du redigerar malluppgifter samtidigt.


1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan Redigera mallaktivitet klickar du på **Malluppgiftsnamn** och lägger till ett namn för mallaktiviteten.

   Den här vyn är inte tillgänglig när du redigerar flera malluppgifter samtidigt.

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Översikt {#overview-1}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Översikt** i den vänstra panelen i rutan **Redigera mallaktivitet**.

   ![Översikt över redigering av malluppgift](assets/template-task-edit-overview.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Lägg till ytterligare information om mallaktiviteten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet</strong> </td> 
      <td> <p>Det här är en visuell flagga som gör att du kan prioritera mallåtgärder. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ingen</strong> </p> </li> 
        <li> <p><strong>Låg</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>Hög</b> </p> </li> 
        <li> <p><b>Brådskande</b> </p> </li> 
       </ul> <p>Beroende på vilka projektinställningar du har valt av Workfront-administratören kan prioritetsnamnen vara olika för dig. Mer information om redigeringsprioriteringar finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Skapa och anpassa prioriteringar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktivitetsbegränsning</strong> </td> 
      <td> <p>Aktiviteten i projektet som skapas från den här mallen har den här begränsningen. Uppgiftsbegränsningar identifierar när en uppgift måste slutföras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li><strong>Fasta datum</strong>. Ange en <strong>planerad start</strong> och ett <strong>planerat slutförandedatum.</strong></li> 
        <li><strong>måste börja </strong>. Ange ett <strong>planerat startdatum.</strong></li> 
        <li><strong>Måste avslutas </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Så snart som möjligt</strong> </li> 
        <li><strong>Så sent som möjligt</strong> </li> 
        <li style="font-weight: bold;"><strong>Tidigaste tillgängliga tid</strong> </li> 
        <li style="font-weight: bold;"><strong>Senaste tillgängliga tid</strong> </li> 
        <li>Börja inte senare än. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Starta inte tidigare än </strong>. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Slutför inte senare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Slutför inte tidigare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
       </ul> <p>Mer information om uppgiftsbegränsning finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Startdag</span><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange startdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul> 
        <li>Måste börja på</li> 
        <li>Starta tidigast</li> 
        <li>Starta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar det datum inom tidslinjen för det framtida projektet då aktiviteten startar. För alla andra begränsningar beräknas startdagen i Workfront baserat på föregående beroende mellan uppgifterna. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Slutförandedag</strong><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange slutdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Måste avslutas</li> 
        <li>Avsluta tidigast</li> 
        <li>Avsluta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar datumet inom tidslinjen för det framtida projektet när aktiviteten ska slutföras. För alla andra begränsningar beräknar Workfront Slutförandedagen baserat på Varaktighet och föregående beroende. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Ange en webblänk som relaterar till informationen om mallaktiviteten.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Arbetsinsats</strong> </td> 
      <td>Välj bland följande alternativ:
      <ul><li>Liten</li>
      <li>Medium</li>
      <li>Stor</li></ul>

   <p><b>VIKTIGT</b></p>
      <p>Fältet Arbetsinsats visas endast när du redigerar en malluppgift när du väljer inställningen <b>Använd arbetsinsats för att automatiskt beräkna aktivitetsplanerade timmar</b> när du redigerar mallen.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Uppdrag {#assignments-1}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Uppdrag** i den vänstra panelen i rutan **Redigera malluppgift**.

   ![Redigera tilldelningar för malluppgift](assets/template-task-edit-assignments.png)

1. I fältet **Sök efter personer, roller eller team** börjar du skriva namnet på en tilldelad och markerar den när den visas i listan

   eller

   Klicka på **Tilldela mig** för att tilldela mallaktiviteten till dig själv.
1. Överväg att uppdatera följande information:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody>

   <tr> 
         <td role="rowheader"><strong>Varaktighetstyp</strong> </td> 
         <td> <p>Den framtida uppgift som skapas från den här mallen kommer att ha den här varaktighetstypen. <br>Varaktighetstypen identifierar relationen mellan följande:</p> 
         <ul>
         <li><p>Antal resurser som tilldelats en aktivitet</p> </li>
         <li><p>Den totala arbetsinsats som krävs för att slutföra uppgiften</p></li> 
         <li><p>Aktivitetens totala varaktighet </p></li></ul> <p>Med Varaktighetstyper kan du ange konsekventa resurstilldelningar baserat på uppgiftens behov. Mer information om varaktighetstypen för en aktivitet finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>.</p> <p>Välj bland följande alternativ:</p> 
         <ul> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Beräknad tilldelning</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Beräknat arbete</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Ansträngningsstyrd</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Enkel</span> <br> </p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Varaktighet</strong> </td> 
         <td> <p>Ange varaktigheten för framtida uppgifter i minuter, timmar, dagar, veckor eller månader. Den framtida uppgift som skapas från den här mallen har den varaktighet som anges här.</p> <p>Som standard mäter Workfront Varaktighet i dagar. Det här är den tid som du tillåter att aktiviteten förblir ofullständig innan den måste slutföras. Du kan inte ange varaktigheten för en aktivitet när aktivitetens <strong>Varaktighetstyp</strong> är <strong>Enkel</strong> eller när <strong>Aktivitetsbegränsning</strong> är <strong>Fasta datum</strong>.</p> <p><b>VIKTIGT</b></p> <p>Varaktighet är vanligtvis den tid som förflyter mellan planerad start och planerad slutförandetid för en mallaktivitet, och av den anledningen påverkar den mallens tidslinje. Detta avgör tidslinjen för det framtida projekt som skapas från mallen. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Planerade timmar</strong> </td> 
         <td> <p>Ange antalet planerade timmar för den framtida aktiviteten i det projekt som skapas med den här mallen. Detta är den faktiska tid det skulle ta för uppgiftens tilldelare att slutföra den. Du kan bara ange antalet planerade timmar för en aktivitet när varaktighetstypen <strong>är inställd på </strong>Beräknat uppdrag<strong>.</strong> </p> </td> 
      </tr> 
   </tbody> 
      </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Ekonomi {#finance-1}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan **Redigera mallaktivitet** klickar du på **Ekonomi** i den vänstra panelen.

   ![Malluppgift Redigera finansavsnitt](assets/template-task-edit-finance.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Kostnadstyp</strong> </td> 
      <td> <p>Ange kostnadstyp för den framtida aktiviteten. Detta avgör hur Kostnaden för aktiviteten beräknas, baserat på antalet timmar för aktiviteterna. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Ingen kostnad</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Korrigerad timme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Användartimme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Roll varje timme</span> </p> </li> 
       </ul> <p>Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Intäktstyp</strong> </td> 
      <td> <p>Ange intäktstyp för den framtida aktiviteten. Det här avgör hur Intäkten för uppgiften beräknas, baserat på antalet timmar för uppgifterna.</p> <p style="font-weight: normal;">Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Ej fakturerbar</p> </li> 
        <li> <p style="font-weight: normal;">Användare per timme</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis</p> </li> 
        <li> <p style="font-weight: normal;">Fast en timme</p> </li> 
        <li> <p style="font-weight: normal;">Användartimme med versaler</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis med ändpunkt</p> </li> 
        <li> <p style="font-weight: normal;">Användarens timma plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Fast intäkt</p> </li> 
       </ul> <p>Mer information om att spåra intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Anpassad Forms {#custom-forms-1}

Du kan definiera anpassade formulär som ska bifogas automatiskt som standard till uppgifter när uppgifterna läggs till i ett projekt. Mer information om hur du konfigurerar projektet så att det innehåller anpassade formulär för standarduppgifter finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Du kan också lägga till anpassade formulär till de framtida uppgifterna i ett projekt när projektet skapas från en mall genom att lägga till anpassade formulär till malluppgifterna.

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan **Redigera malluppgift** klickar du på **Egen Forms** i den vänstra panelen.

   ![Malluppgift Redigera eget formuläravsnitt](assets/template-task-edit-custom-forms.png)

1. Markera det eller de anpassade formulär som du vill koppla till malluppgiften.

   Du måste skapa anpassade formulär innan de kan väljas i det här fältet.
Endast aktiva anpassade formulär visas i listan.

   Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Du kan lägga till upp till tio anpassade formulär i en mallåtgärd.
Formulären läggs automatiskt till i de uppgifter som skapas från mallen.
1. (Villkorligt och valfritt) Om du har kopplat ett anpassat formulär till malluppgiften kan du redigera alla fält i formuläret. Du måste ange alla obligatoriska fält innan du kan spara malluppgiften.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör anger behörigheter för avsnitten i ditt anpassade formulär kan inte alla visa eller redigera samma fält i ett visst anpassat formulär. Behörigheterna att redigera fält i ett avsnitt i ett anpassat formulär beror på vilka behörigheter du har för malluppgiften eller den framtida uppgiften.\
   >Mer information om att ange behörigheter för avsnitt i ett anpassat formulär finns i [Dela ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Mer information om hur du anger aktivitetsbehörigheter finns i [Dela en uppgift](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Mer information om hur du ställer in mallbehörigheter finns i [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Inställningar {#settings-1}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Inställningar** i den vänstra panelen i **åtgärdsrutan Redigera mall**.

   ![Inställningsavsnitt för redigering av malluppgift](assets/template-task-edit-settings.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milstolpe</b></p></strong> </td> 
      <td> <p>Välj en milstolpe som ska associeras med den valda malluppgiften.</p>

   <p><b>VIKTIGT</b></p>
   <p>Du måste associera en milstolpe-sökväg med en mall för att det här fältet ska kunna visas. Mer information finns i <a href="../create-and-manage-templates/edit-templates.md">Redigera projektmallar</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Spårningsläge</strong> </td> 
      <td> <p>Ange hur förloppsstatusen för den framtida aktiviteten ska spåras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Användaren måste uppdatera</strong> </p> </li> 
        <li> <p><strong>Anta i tid</strong> </p> </li> 
        <li> <p><strong>Ignorera sena varningar</strong> </p> </li> 
        <li> <p><strong>Komplettera automatiskt</strong> </p> </li> 
        <li> <p><strong>Föregående</strong> </p> </li> 
       </ul> <p>Mer information om spårningsläget för uppgifter finns i <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Översikt över spårningsläget för aktiviteter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Påminnelsemeddelanden</strong> </td> 
      <td> <p>Välj vilka påminnelsemeddelanden som du vill bifoga till malluppgiften. De kommer att bifogas till de framtida aktiviteterna i projektet som skapas från den här mallen. Systemadministratören måste konfigurera påminnelsemeddelanden innan du kan välja dem för en uppgift. Mer information om hur du konfigurerar påminnelsemeddelanden finns i <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Konfigurera påminnelsemeddelanden</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Godkännandeprocess</strong> </td> 
      <td> <p>Välj den godkännandeprocess som du vill associera med malluppgiften. Workfront-administratören måste definiera processer för godkännande av uppgifter på systemnivå innan du kan koppla dem till malluppgifter. <span>En användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.</span> Mer information om hur du skapar godkännandeprocesser finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Skapa en godkännandeprocess för arbetsobjekt</a>.</p> <p>Tänk på följande när du lägger till godkännandeprocesser: </p> 
       <ul> 
       <li>Endast aktiva godkännandeprocesser visas i listan. </li> 
       <li> <p>Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. Godkännandeprocesser som är kopplade till en annan grupp än mallens visas inte i listan.</p> <p>Viktigt: Om gruppen som är kopplad till mallen ändras blir den gruppspecifika godkännandeprocessen en godkännandeprocess för enstaka användning. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>. </p> </li> 
       <li> <p>Om du har lagt till en godkännandeprocess för en enstaka användning visas den som &lt;Anpassad&gt; i det här fältet. Mer information finns i <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associera en ny eller befintlig godkännandeprocess med arbete</a>. </p>  </li> 
       <li> <p>När malluppgifter gruppredigeras finns följande scenarier:</p> 
       <ul> 
       <li> <p>När du väljer malluppgifter från samma mallgrupp visas både godkännandeprocesser på system- och gruppnivå i det här fältet.</p> </li> 
       <li> <p>När du väljer malluppgifter från olika mallgrupper visas endast godkännandeprocesser på systemnivå i det här fältet.</p> </li> 
       <li> <p>När någon av malluppgifterna har en enda godkännandeprocess, ersätts den av den process på systemnivå <span>eller på gruppnivå</span> som du väljer. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

##### Kommentar {#comment-1}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Kommentar** i den vänstra panelen i rutan **Redigera malluppgift**.

   ![Malluppgift Redigera kommentarsavsnittet](assets/template-task-edit-comment.png)

1. I området **Lägg till en uppdatering för mallaktiviteten** anger du en kommentar som du vill visa i uppdateringsströmmen för mallaktiviteten i det tillgängliga fältet. Den här kommentaren är synlig för alla som har åtkomst till mallen och malluppgiften och tillgång till vyn Anteckningar.
1. Klicka på **Spara**.

   När du eller någon annan användare skapar ett projekt från den här mallen används alla inställningar som du har tillämpat på malluppgifter som inställningar för projektuppgifterna.


<div class="preview">

### Redigera malluppgifter i förhandsgranskningsmiljön

Du kan redigera en malluppgift med området Redigera malluppgift eller Malluppgiftsinformation.

{{step1-to-templates}}

1. Klicka på namnet på en mall för att öppna den.
1. Klicka på **Malluppgifter** i den vänstra panelen.
1. Klicka på namnet på en malluppgift i listan för att öppna malluppgiften.
1. Så här redigerar du begränsad information om mallaktiviteten:
   1. (Valfritt) Klicka på **Uppdateringar** i den vänstra panelen för att lägga till uppdateringar i mallaktiviteten. Uppdateringar av malluppgifter överförs inte till projektaktiviteter när mallen används för att skapa ett projekt.
   1. (Valfritt) Klicka på **Dokument** i den vänstra panelen för att lägga till dokument i mallåtgärden. Dokumenten överförs till projektuppgifterna när du använder mallen för att skapa projektet.
   1. (Villkorligt) Om du vill redigera begränsad information om en malluppgift klickar du på **Information om malluppgift** i den vänstra panelen. Gå sedan till områdena i detaljavsnittet för att redigera information för varje område.
   1. (Valfritt) Gör något av följande:
      * Klicka på ikonen **Komprimera alla** ![Komprimera alla ](assets/collapse-all-icon.png) om du vill komprimera alla områden.
      * Klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) och välj sedan något av områdena nedan. Du kan också klicka på **Redigera alla** om du vill redigera information i alla områden:

         * Översikt
         * Anpassad Forms
Namnen på tullformulär visas bara om det finns anpassade formulär kopplade till malluppgiften.
         * Ekonomi

        >[!TIP]
        >
        >Om du vill ha information om alla fält som visas i området Detaljer kan du fortsätta redigera alla fält med rutan Redigera malluppgift, som beskrivs nedan.

   1. (Valfritt) Klicka på avsnittet **Underaktiviteter** i den vänstra panelen för att lägga till underordnade för malluppgiften. Att lägga till underaktiviteter för malluppgifter liknar att lägga till underaktiviteter för projektaktiviteter. Mer information finns i avsnittet Skapa underaktiviteter från avsnittet Underaktiviteter för aktiviteter i artikeln [Skapa underaktiviteter](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Valfritt) Klicka på **Utgifter** i den vänstra panelen och lägg till utgifter i malluppgifterna. Malluppgiftsutgifter överförs till framtida projektaktiviteter när mallen används för att skapa ett projekt.
   1. (Valfritt) Klicka på **Godkännanden** i den vänstra panelen för att skapa godkännanden eller koppla globala godkännanden eller godkännanden på gruppnivå till mallåtgärderna. Godkännandena överförs till framtida projektaktiviteter.
   1. (Valfritt) Klicka på avsnittet **Föregående** i den vänstra panelen för att lägga till föregående för malluppgifterna. Att lägga till malluppgiftsföregångare liknar att lägga till föregångare för projektaktiviteter. Mer information finns i [Skapa en föregående relation med området Föregående användare](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Villkorligt) Om du vill redigera all information om en malluppgift eller om flera uppgifter samtidigt klickar du för att markera dem i en lista och sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) längst upp i listan.

   Rutan **Redigera mallaktivitet** visas.

   ![Ny upplevelse för aktiviteten Redigera mall](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Du kan också välja en malluppgift i en lista och sedan klicka på **Redigera** till höger om malluppgiftens namn i sidhuvudet för att öppna rutan **Redigera malluppgift** .

1. Det kan vara bra att ange information i följande avsnitt:

* [Malluppgiftsnamn](#template-task-name)
* [Översikt](#overview-2)
* [Uppdrag](#assignments-2)
* [Ekonomi](#finance-2)
* [Anpassad Forms](#custom-forms-2)
* [Inställningar](#settings-2)
* [Kommentar](#comment-2)

1. Fortsätt redigera malluppgifterna enligt beskrivningen i avsnitten nedan.

#### Malluppgiftsnamn

>[!TIP]
>
>Avsnittet Malluppgiftsnamn är inte tillgängligt när du redigerar malluppgifter samtidigt.


1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan Redigera mallaktivitet klickar du på **Malluppgiftsnamn** och lägger till ett namn för mallaktiviteten.

   Den här vyn är inte tillgänglig när du redigerar flera malluppgifter samtidigt.

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

#### Översikt {#overview-2}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Översikt** i den vänstra panelen i rutan **Redigera mallaktivitet**.

   ![Översikt över redigering av malluppgift](assets/template-task-edit-overview.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Lägg till ytterligare information om mallaktiviteten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioritet</strong> </td> 
      <td> <p>Det här är en visuell flagga som gör att du kan prioritera mallåtgärder. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Ingen</strong> </p> </li> 
        <li> <p><strong>Låg</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>Hög</b> </p> </li> 
        <li> <p><b>Brådskande</b> </p> </li> 
       </ul> <p>Beroende på vilka projektinställningar du har valt av Workfront-administratören kan prioritetsnamnen vara olika för dig. Mer information om redigeringsprioriteringar finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Skapa och anpassa prioriteringar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktivitetsbegränsning</strong> </td> 
      <td> <p>Aktiviteten i projektet som skapas från den här mallen har den här begränsningen. Uppgiftsbegränsningar identifierar när en uppgift måste slutföras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li><strong>Fasta datum</strong>. Ange en <strong>planerad start</strong> och ett <strong>planerat slutförandedatum.</strong></li> 
        <li><strong>måste börja </strong>. Ange ett <strong>planerat startdatum.</strong></li> 
        <li><strong>Måste avslutas </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Så snart som möjligt</strong> </li> 
        <li><strong>Så sent som möjligt</strong> </li> 
        <li style="font-weight: bold;"><strong>Tidigaste tillgängliga tid</strong> </li> 
        <li style="font-weight: bold;"><strong>Senaste tillgängliga tid</strong> </li> 
        <li>Börja inte senare än. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Starta inte tidigare än </strong>. Ange ett <strong>planerat startdatum</strong>.</li> 
        <li><strong>Slutför inte senare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
        <li><strong>Slutför inte tidigare än </strong>. Ange ett <strong>planerat slutförandedatum</strong>.</li> 
       </ul> <p>Mer information om uppgiftsbegränsning finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Startdag</span><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange startdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul> 
        <li>Måste börja på</li> 
        <li>Starta tidigast</li> 
        <li>Starta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar det datum inom tidslinjen för det framtida projektet då aktiviteten startar. För alla andra begränsningar beräknas startdagen i Workfront baserat på föregående beroende mellan uppgifterna. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Slutförandedag</strong><span style="font-weight: normal;"> (valfritt och villkorligt)</span> </td> 
      <td> <p> Du kan bara ange slutdagen för en malluppgift när aktivitetsbegränsningen är något av följande:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Måste avslutas</li> 
        <li>Avsluta tidigast</li> 
        <li>Avsluta senast</li> 
        <li>Fasta datum</li> 
       </ul> <p>Detta motsvarar datumet inom tidslinjen för det framtida projektet när aktiviteten ska slutföras. För alla andra begränsningar beräknar Workfront Slutförandedagen baserat på Varaktighet och föregående beroende. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Ange en webblänk som relaterar till informationen om mallaktiviteten.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Arbetsinsats</strong> </td> 
      <td>Välj bland följande alternativ:
      <ul><li>Liten</li>
      <li>Medium</li>
      <li>Stor</li></ul>

   <p><b>VIKTIGT</b></p>
      <p>Fältet Arbetsinsats visas endast när du redigerar en malluppgift när du väljer inställningen <b>Använd arbetsinsats för att automatiskt beräkna aktivitetsplanerade timmar</b> när du redigerar mallen.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

#### Uppdrag {#assignments-2}

1. Börja redigera din malluppgift enligt beskrivningen ovan.
1. Klicka på **Uppdrag** i den vänstra panelen.

   Området **Uppdrag** öppnas.

   ![Uppdrag i malluppgifter](assets/assignments-edit-template-tasks-box.png)

1. Börja skriva namnet på en användare, en jobbroll eller ett team i fältet **Sök efter personer, en roll eller ett team** och markera dem sedan när de visas i listan.

1. Uppdatera följande information:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Varaktighetstyp</td> 
   <td> <p>Detta identifierar relationen mellan följande: </p> 
   <ul> 
   <li> <p>Antalet resurser som tilldelats en aktivitet </p> </li> 
   <li> <p>Den totala arbetsinsats som krävs för att slutföra uppgiften </p> </li> 
   <li> <p> Aktivitetens totala varaktighet. </p> </li> 
   </ul> <p>Workfront-administratören eller en gruppadministratör väljer standardinställningen för varaktighetstyp för uppgifterna i ditt system eller din grupp. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Konfigurera systemomfattande uppgifter och inställningar för problem</a>. </p> <p>Med varaktighetstyper kan du ange konsekventa resurstilldelningar baserat på uppgiftens behov. Mer information om varaktighetstypen för en aktivitet finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>. </p> <p>Välj bland följande alternativ: </p> 
   <ul> 
   <li> <p>Beräknad tilldelning </p> </li> 
   <li> <p> Beräknat arbete </p> </li> 
   <li> <p>Ansträngningsstyrd </p> </li> 
   <li> <p>Enkel</p> </li> 
   </ul> </td> 
   </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Varaktighet per förekomst</td> 
   <td> <p>Detta visas endast på den överordnade för återkommande uppgifter. Den visar varaktigheten för varje återkommande uppgift, enligt definition när uppgiften skapades. Mer information om hur du skapar återkommande aktiviteter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande aktiviteter</a>. </p> <p> <b>OBS!</b>

   Varaktigheter som ändras i enskilda återkommande aktiviteter visar inte det värde som anges i det här fältet. </p> </td>
   </tr> 
   <tr> 
   <td role="rowheader">Varaktighet</td> 
   <td> 
   <div> 
   <div> 
   <p>Det här är den tid som du tillåter att en uppgift förblir öppen innan den är slutförd. </p> 
   <p><b>VIKTIGT</b></p>
   <p>Eftersom aktivitetens varaktighet vanligtvis är tiden mellan planerad start och planerad slutförandetid, påverkar det tidslinjen för projektet.</p> 
   <p>Så här anger du aktivitetens varaktighet och tidsenhet:</p> 
   <ul> 
   <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Skriv in tidslängden och välj en tidsenhet i listrutan.</p> <p><b>TIPS</b></p>
   När du uppdaterar varaktigheten för uppgifter i en uppgiftslista kan du använda förkortningen för tidsenheten. </p> </li> 
   </ul> 
   <p> Du kan välja mellan alternativen för normal tid eller förfluten tid i följande tabell: </p> 
   <table style="table-layout:auto"> 
   <col> 
   <col data-mc-conditions=""> 
   <tbody> 
   <tr> 
   <td>Tidsenhet</td> 
   <td>Förkortning</td> 
   </tr> 
   <tr> 
   <td>Minuter</td> 
   <td>M</td> 
   </tr> 
   <tr> 
   <td>Timmar</td> 
   <td>H</td> 
   </tr> 
   <tr> 
   <td>Dagar. Det här är standardinställningen. </td> 
   <td>D</td> 
   </tr> 
   <tr> 
   <td>Veckor</td> 
   <td>B</td> 
   </tr> 
   <tr> 
   <td>Månader</td> 
   <td>T</td> 
   </tr> 
   <tr> 
   <td>Förflutna minuter</td> 
   <td>EM</td> 
   </tr> 
   <tr> 
   <td>Förflutna timmar</td> 
   <td>EH</td> 
   </tr> 
   <tr> 
   <td>Förflutna dagar</td> 
   <td>ED</td> 
   </tr> 
   <tr> 
   <td>Förflutna veckor</td> 
   <td>FV</td> 
   </tr> 
   <tr> 
   <td>Förflutna månader</td> 
   <td>ET</td> 
   </tr> 
   </tbody> 
   </table>

   <p><b>ANMÄRKNING</b>

   <p>Förfluten tid är en tidsenhet för en uppgifts varaktighet. Det är tiden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna.

   Med normal tid räknas helger, helger och ledig tid som undantag från uppgiftens varaktighet. Mer information om aktivitetens varaktighet finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Planerade timmar</td> 
   <td> <p>Ange antalet planerade timmar för aktiviteten, i timmar. Detta är den faktiska tid det skulle ta för de som tilldelats uppgiften att slutföra den. Du kan bara ange antalet planerade timmar för en aktivitet när varaktighetstypen är inställd på Beräknad tilldelning. Mer information om varaktighetstyper finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>.</p> 
   <b>OBS!</b>
   <p>
   När du skapar återkommande uppgifter är de planerade timmarna för varje förekomst. De planerade timmarna för de överordnade uppgifterna är det totala antalet planerade timmar från alla förekomster. Mer information om hur du skapar återkommande aktiviteter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande aktiviteter</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allokering</td> 
   <td> <p>Om aktivitetsbegränsningen är Beräknad arbets- eller insatsstyrd anger du <strong>Allokering %</strong> (allokeringsprocent) för varje tilldelad. Det här är den tid från schemat för den tilldelande personen som de kan lägga på den här aktiviteten. Om du ändrar allokeringsprocenten för en tilldelad ändrar du planerad tid för en uppgift. </p> <p>När aktivitetsbegränsningen är enkel kan du ange följande:</p> 
   <ul> 
   <li> <p>Allokeringstimmar för varje tilldelad.</p> </li> 
   <li> <p>Planerade timmar för uppgiften</p> </li> 
   <li> <p>Uppgiftens varaktighet</p> </li> 
   </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Uppdragarens roll</td> 
   <td> <p>Välj en roll i listrutan <strong>Tilldelarens roll</strong> när du har valt en person som tilldelad. Detta är den roll som den som tilldelas kan utföra den här uppgiften. </p> <p><b>TIPS</b>

   Endast de jobbroller som är kopplade till varje tilldelad i deras profil visas i listrutan.</p> </td>
   </tr> 
   </tbody> 
   </table>

1. Klicka på **Spara** eller fortsätt med följande avsnitt.

#### Ekonomi {#finance-2}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan **Redigera mallaktivitet** klickar du på **Ekonomi** i den vänstra panelen.

   ![Malluppgift Redigera finansavsnitt](assets/template-task-edit-finance.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Kostnadstyp</strong> </td> 
      <td> <p>Ange kostnadstyp för den framtida aktiviteten. Detta avgör hur Kostnaden för aktiviteten beräknas, baserat på antalet timmar för aktiviteterna. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Ingen kostnad</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Korrigerad timme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Användartimme</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Roll varje timme</span> </p> </li> 
       </ul> <p>Mer information om spårningskostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Intäktstyp</strong> </td> 
      <td> <p>Ange intäktstyp för den framtida aktiviteten. Det här avgör hur Intäkten för uppgiften beräknas, baserat på antalet timmar för uppgifterna.</p> <p style="font-weight: normal;">Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Ej fakturerbar</p> </li> 
        <li> <p style="font-weight: normal;">Användare per timme</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis</p> </li> 
        <li> <p style="font-weight: normal;">Fast en timme</p> </li> 
        <li> <p style="font-weight: normal;">Användartimme med versaler</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis med ändpunkt</p> </li> 
        <li> <p style="font-weight: normal;">Användarens timma plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Roll timvis plus fast</p> </li> 
        <li> <p style="font-weight: normal;">Fast intäkt</p> </li> 
       </ul> <p>Mer information om att spåra intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

#### Anpassad Forms {#custom-forms-2}

Du kan definiera anpassade formulär som ska bifogas automatiskt som standard till uppgifter när uppgifterna läggs till i ett projekt. Mer information om hur du konfigurerar projektet så att det innehåller anpassade formulär för standarduppgifter finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Du kan också lägga till anpassade formulär till de framtida uppgifterna i ett projekt när projektet skapas från en mall genom att lägga till anpassade formulär till malluppgifterna.

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. I rutan **Redigera malluppgift** klickar du på **Egen Forms** i den vänstra panelen.

   ![Malluppgift Redigera eget formuläravsnitt](assets/template-task-edit-custom-forms.png)

1. Markera det eller de anpassade formulär som du vill koppla till malluppgiften.

   Du måste skapa anpassade formulär innan de kan väljas i det här fältet.
Endast aktiva anpassade formulär visas i listan.

   Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Du kan lägga till upp till tio anpassade formulär i en mallåtgärd.
Formulären läggs automatiskt till i de uppgifter som skapas från mallen.
1. (Villkorligt och valfritt) Om du har kopplat ett anpassat formulär till malluppgiften kan du redigera alla fält i formuläret. Du måste ange alla obligatoriska fält innan du kan spara malluppgiften.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör anger behörigheter för avsnitten i ditt anpassade formulär kan inte alla visa eller redigera samma fält i ett visst anpassat formulär. Behörigheterna att redigera fält i ett avsnitt i ett anpassat formulär beror på vilka behörigheter du har för malluppgiften eller den framtida uppgiften.\
   >Mer information om att ange behörigheter för avsnitt i ett anpassat formulär finns i [Dela ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Mer information om hur du anger aktivitetsbehörigheter finns i [Dela en uppgift](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Mer information om hur du ställer in mallbehörigheter finns i [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

#### Inställningar {#settings-2}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Inställningar** i den vänstra panelen i **åtgärdsrutan Redigera mall**.

   ![Inställningsavsnitt för redigering av malluppgift](assets/template-task-edit-settings.png)

1. Uppdatera något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milstolpe</b></p></strong> </td> 
      <td> <p>Välj en milstolpe som ska associeras med den valda malluppgiften.</p>

   <p><b>VIKTIGT</b></p>
   <p>Du måste associera en milstolpe-sökväg med en mall för att det här fältet ska kunna visas. Mer information finns i <a href="../create-and-manage-templates/edit-templates.md">Redigera projektmallar</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Spårningsläge</strong> </td> 
      <td> <p>Ange hur förloppsstatusen för den framtida aktiviteten ska spåras. </p> <p>Välj bland följande alternativ:</p> 
       <ul> 
        <li> <p><strong>Användaren måste uppdatera</strong> </p> </li> 
        <li> <p><strong>Anta i tid</strong> </p> </li> 
        <li> <p><strong>Ignorera sena varningar</strong> </p> </li> 
        <li> <p><strong>Komplettera automatiskt</strong> </p> </li> 
        <li> <p><strong>Föregående</strong> </p> </li> 
       </ul> <p>Mer information om spårningsläget för uppgifter finns i <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Översikt över spårningsläget för aktiviteter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Påminnelsemeddelanden</strong> </td> 
      <td> <p>Välj vilka påminnelsemeddelanden som du vill bifoga till malluppgiften. De kommer att bifogas till de framtida aktiviteterna i projektet som skapas från den här mallen. Systemadministratören måste konfigurera påminnelsemeddelanden innan du kan välja dem för en uppgift. Mer information om hur du konfigurerar påminnelsemeddelanden finns i <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Konfigurera påminnelsemeddelanden</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Godkännandeprocess</strong> </td> 
      <td> <p>Välj den godkännandeprocess som du vill associera med malluppgiften. Workfront-administratören måste definiera processer för godkännande av uppgifter på systemnivå innan du kan koppla dem till malluppgifter. <span>En användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.</span> Mer information om hur du skapar godkännandeprocesser finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Skapa en godkännandeprocess för arbetsobjekt</a>.</p> <p>Tänk på följande när du lägger till godkännandeprocesser: </p> 
       <ul> 
       <li>Endast aktiva godkännandeprocesser visas i listan. </li> 
       <li> <p>Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. Godkännandeprocesser som är kopplade till en annan grupp än mallens visas inte i listan.</p> <p>Viktigt: Om gruppen som är kopplad till mallen ändras blir den gruppspecifika godkännandeprocessen en godkännandeprocess för enstaka användning. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>. </p> </li> 
       <li> <p>Om du har lagt till en godkännandeprocess för en enstaka användning visas den som &lt;Anpassad&gt; i det här fältet. Mer information finns i <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associera en ny eller befintlig godkännandeprocess med arbete</a>. </p>  </li> 
       <li> <p>När malluppgifter gruppredigeras finns följande scenarier:</p> 
       <ul> 
       <li> <p>När du väljer malluppgifter från samma mallgrupp visas både godkännandeprocesser på system- och gruppnivå i det här fältet.</p> </li> 
       <li> <p>När du väljer malluppgifter från olika mallgrupper visas endast godkännandeprocesser på systemnivå i det här fältet.</p> </li> 
       <li> <p>När någon av malluppgifterna har en enda godkännandeprocess, ersätts den av den process på systemnivå <span>eller på gruppnivå</span> som du väljer. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara**.

#### Kommentar {#comment-2}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Kommentar** i den vänstra panelen i rutan **Redigera malluppgift**.

   ![Malluppgift Redigera kommentarsavsnittet](assets/template-task-edit-comment.png)

1. I området **Lägg till en uppdatering för mallaktiviteten** anger du en kommentar som du vill visa i uppdateringsströmmen för mallaktiviteten i det tillgängliga fältet. Den här kommentaren är synlig för alla som har åtkomst till mallen och malluppgiften och tillgång till vyn Anteckningar.
1. Klicka på **Spara**.

   När du eller någon annan användare skapar ett projekt från den här mallen används alla inställningar som du har tillämpat på malluppgifter som inställningar för projektuppgifterna.

</div>


