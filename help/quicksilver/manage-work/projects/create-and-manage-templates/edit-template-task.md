---
product-area: templates
keywords: uppgift,standard,automatisera,skapa
navigation-topic: templates-navigation-topic
title: Redigera en malluppgift
description: När du har skapat en mall kan du redigera information om malluppgifterna. Den information som du uppdaterar för en malluppgift kopplas till projektuppgifter när du har använt mallen för att skapa ett projekt eller bifogat mallen till ett projekt.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: 5bdf1bd285023d29ee6c61f16a4bd6a622d964d8
workflow-type: tm+mt
source-wordcount: '2491'
ht-degree: 0%

---

# Redigera en malluppgift

<!--Audited: 09/2024-->

När du har skapat en mall kan du redigera informationen för malluppgifterna. Den information som du uppdaterar för en malluppgift kopplas till projektuppgifter när du har använt mallen för att skapa ett projekt eller bifogat mallen till ett projekt.

Mer information om hur du skapar en mall finns i [Skapa en projektmall](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Du kan redigera malluppgifter eller redigera malluppgifter samtidigt.

>[!NOTE]
>
>Du kan inte redigera malluppgifter som tillhör olika mallar samtidigt. Du kan bara redigera malluppgifter som tillhör samma mall.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter </td> 
   <td> <p>Hantera behörigheter för en mall. </p> <p>Du kan inte dela en malluppgift. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du

* Skapa en mall.

  Mer information om hur du skapar en mall finns i [Skapa en projektmall](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Redigera malluppgift

Du kan redigera en malluppgift med området Redigera malluppgift eller Malluppgiftsinformation. I följande steg beskrivs hur du redigerar en uppgift i rutan Redigera malluppgift.

{{step1-to-templates}}

1. Klicka på namnet på en mall för att öppna den.
1. Klicka på **Malluppgifter** i den vänstra panelen.
1. Klicka på namnet på en malluppgift i listan för att öppna malluppgiften.
1. (Valfritt) Klicka på avsnittet **Föregående** i den vänstra panelen för att lägga till föregående för malluppgifterna. Att lägga till malluppgiftsföregångare liknar att lägga till föregångare för projektaktiviteter. Mer information finns i [Skapa en föregående relation med området Föregående användare](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
1. (Valfritt) Klicka på avsnittet **Underaktiviteter** i den vänstra panelen för att lägga till underordnade för malluppgiften. Att lägga till underaktiviteter för malluppgifter liknar att lägga till underaktiviteter för projektaktiviteter. Mer information finns i avsnittet Skapa underaktiviteter från avsnittet Underaktiviteter för aktiviteter i artikeln [Skapa underaktiviteter](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

1. (Villkorligt) Om du vill redigera begränsad information om en malluppgift klickar du på **Information om malluppgift** i den vänstra panelen. Gå sedan till områdena i detaljavsnittet för att redigera information för varje område.
1. (Valfritt) Klicka på ikonen **Komprimera alla** ![Komprimera alla ](assets/collapse-all-icon.png) om du vill komprimera alla områden.
1. Om du vill redigera information i detaljavsnittet klickar du på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) , väljer något av områdena nedan eller klickar på **Redigera alla** om du vill redigera information i alla områden:

   * Översikt
   * Anpassad Forms

     Namnen på tullformulär visas bara om det finns anpassade formulär kopplade till objektet.

   * Ekonomi

   >[!TIP]
   >
   >Om du vill ha information om alla fält som visas i området Detaljer kan du fortsätta redigera alla fält med rutan Redigera malluppgift, som beskrivs nedan.
1. (Valfritt) Om du vill redigera flera malluppgifter samtidigt markerar du flera malluppgifter och klickar sedan på **Redigera** överst i malllistan.
1. (Villkorligt) Om du vill redigera all information om mallaktiviteten eller om flera åtgärder samtidigt klickar du för att markera dem i en lista och sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) längst upp i listan.

   Rutan **Redigera mallaktivitet** visas.

   >[!TIP]
   >
   >Du kan också välja en malluppgift i en lista och sedan klicka på Redigera för att öppna rutan Redigera malluppgift.

   ![Redigera malluppgift](assets/edit-template-tasks-box-classic-350x356.png)

1. Det kan vara bra att ange information i följande avsnitt:

   * [Översikt](#overview)
   * [Ekonomi](#finance)
   * [Inställningar](#settings)
   * [Uppdrag](#assignments)
   * [Anpassad Forms](#custom-forms)
   * [Kommentar](#comment)

### Översikt {#overview}

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

### Ekonomi {#finance}

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

### Inställningar {#settings}

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

### Uppdrag {#assignments}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Uppdrag**.

   ![tilldelningar_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Klicka på **Lägg till tilldelad** för att lägga till en ny tilldelad till malluppgiften. Du kan tilldela användare, roller eller team till en uppgift. Du kan ha flera tilldelningar för en uppgift. De framtida aktiviteterna tilldelas samma resurser när de skapas från den här malluppgiften.
1. (Valfritt) Om du har flera tilldelningar markerar du alternativknappen **Ägare** för att ange vilken användare eller roll som betraktas som aktivitetsägare eller primär tilldelad. Workfront markerar den första användaren eller jobbrollen som du tilldelar en malluppgift som ägare eller primär tilldelad.
1. (Villkorligt och valfritt) Om aktivitetsbegränsningen är Beräknad arbets- eller insatsstyrd anger du **Allokering %** (allokeringsprocent) för varje tilldelad. Det här är den tid från schemat för den tilldelande personen som de kan lägga på den här aktiviteten. Om du ändrar allokeringsprocenten för en tilldelad ändrar du planerad tid för en uppgift.
1. (Villkorligt och valfritt) Om uppgiftsbegränsningen är enkel anger du **Timmar** för varje tilldelad

   eller

   Ange det totala antalet **Planerade timmar** för mallaktiviteten. Detta fördelar de totala timmarna jämnt mellan alla tilldelningar.

1. (Villkorligt och valfritt) Om aktivitetsbegränsningen är enkel anger du **Varaktighet** för mallaktiviteten i dagar. Detta blir varaktigheten för den uppgift som skapas från den här mallen.
1. (Valfritt) Välj en roll i listrutan **Tilldelningens roll**. Det är den roll som den som tilldelas kan utföra den här framtida uppgiften. Endast de jobbroller som är kopplade till varje tilldelad i deras profil visas i listrutan.
1. (Valfritt) Fortsätt redigera följande avsnitt, beroende på vilken information du vill ändra.

   eller

   Klicka på **Spara ändringar**.

### Anpassad Forms {#custom-forms}

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

### Kommentar {#comment}

1. Börja redigera en malluppgift enligt beskrivningen ovan.
1. Klicka på **Kommentar**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Ange en kommentar som du vill visa i uppdateringsströmmen för malluppgiften i det tillgängliga fältet. Den här kommentaren är synlig för alla som har åtkomst till mallen och malluppgiften och tillgång till vyn Anteckningar.
1. Klicka på **Spara ändringar**.

   När du eller någon annan användare skapar ett projekt från den här mallen används alla inställningar som du har tillämpat på malluppgifter som inställningar för projektuppgifterna.
