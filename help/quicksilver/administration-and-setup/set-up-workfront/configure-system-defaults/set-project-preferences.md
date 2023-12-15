---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Konfigurera systemomfattande projektinställningar
description: Som en [!DNL Adobe Workfront] kan du konfigurera standardinställningar för alla projekt som skapas i systemet. Inställningarna påverkar projekt, uppgifter och problembeteende.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 0%

---

# Konfigurera systemomfattande projektinställningar

Som en [!DNL Adobe Workfront] kan du konfigurera standardinställningar för alla projekt som skapas i systemet. Inställningarna påverkar projekt, uppgifter och problembeteende.

>[!NOTE]
>
>Som standard är de här inställningarna låsta och gruppadministratörer kan inte ändra dem på gruppnivå om du inte låser upp dem för alla grupper i hela systemet. Mer information finns i [Låsa eller låsa upp projektinställningar för alla grupper i systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera projektinställningar för hela organisationen

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects]**.

1. På den sida som visas fortsätter du med något av de fyra avsnitten nedan för att konfigurera inställningar för [!UICONTROL Project Status], [!UICONTROL Timelines], [!UICONTROL Business Cases]och [!UICONTROL Life after Death].
1. Om du vill att alla grupper i hela organisationen ska använda samma projektinställningar måste du se till att alla inställningar är låsta ![](assets/lock-toggle-button.png) (det här är standardvärdet).

   >[!IMPORTANT]
   >
   >När en projektinställning är låst ärvs alla ändringar du gör i den inställningen av alla grupper i systemet. Det är viktigt att kommunicera med användare och grupper i hela organisationen för att säkerställa att alla behov beaktas när du konfigurerar projektinställningar.

   Mer information om hur du låser upp en inställning så att alla grupper kan konfigurera och hantera den på egen hand finns i [Låsa eller låsa upp projektinställningar för alla grupper i systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Klicka på **[!UICONTROL Save]**.

* [[!UICONTROL Project Status]](#project-status)
* [[!UICONTROL Timelines]](#timelines)
* [[!UICONTROL Business Cases]](#business-cases)
* [[!UICONTROL Life After Death]](#life-after-death)

### Projektstatus {#project-status}

Konfigurera någon av följande inställningar för nyligen skapade projekt i hela systemet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>Med den här inställningen kan användare skapa projekt utan att använda en mall när de skapar ett projekt från följande områden: </p>
      <ul>
        <li>
        <p>Använd [!UICONTROL New Project] i en lista med projekt</p>
        </li>
          <li>
          <p>Konvertera ett problem till ett projekt från problemsidan</p>
          </li>
         </ul>
        <p>Den här inställningen är aktiverad som standard. </p> 
        <p><b>ANMÄRKNING</b></p>
        <p> En gruppadministratör kan ändra den här inställningen för en grupp. När en användare tillhör flera grupper med olika inställningar, får användaren skapa ett projekt utan en mall om den här inställningen är aktiverad för hemgruppen.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Bestäm status för nya projekt.</p>  <p><b>ANMÄRKNING</b>  
     <ul> 
      <li>Om du eller någon annan [!DNL Workfront] administratören döljer statusen som valts här, standardstatusen ändras till den första statusen i statuslistan.</li> 
     </ul> 
     <ul> 
      <li> <p>Om ett låst system eller en grupp är inställd som standardstatus och någon senare låser upp den försöker systemet ersätta den med en låst status av samma statustyp.</p> <p>Om det inte går att hitta någon söker programmet efter en obligatorisk status:</p> 
       <ul> 
        <li>Om det finns en obligatorisk status som motsvarar den olåsta standardstatusen blir den obligatoriska statusen standardstatus, även om den är olåst.</li> 
        <li>Om ingen av de obligatoriska statusvärdena motsvarar den olåsta standardstatusen blir den första obligatoriska statusen i statuslistan standardstatus.</li> 
       </ul> <p>Mer information om obligatoriska statusvärden finns i artiklarna <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Öppna listan över status för systemprojekt</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemaktivitet</a>och <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemproblem</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Procent färdigt för ett projekt eller en överordnad uppgift baseras på aktiviteternas allmänna förlopp. Den här informationen kan beräknas utifrån varaktigheten eller den planerade timmen för aktiviteterna i ett projekt.</p> <p>Om du väljer [!UICONTROL Duration], bestämmer varaktigheten för varje aktivitet i ett projekt den totala procentandelen färdigt för projektet, och varaktigheten för varje underuppgift avgör den totala procentandelen färdigt för den överordnade aktiviteten.</p> <p>Om du väljer [!UICONTROL Duration]måste du ange [!UICONTROL Typical hours per work day] och [!UICONTROL Typical work days per week] i [!UICONTROL Timelines] -avsnitt. [!DNL Workfront] använder den här informationen när en uppgifts procentandel slutförd beräknas baserat på Varaktighet. </p> <p>Om du väljer [!UICONTROL Planned Hours]ska du se till att alla uppgifter i varje projekt har samma antal [!UICONTROL Planned Hours] och att beloppet inte är noll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>Med den här inställningen kan användare ange [!UICONTROL Condition] av ett projekt manuellt ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) eller har [!DNL Workfront] ange [!UICONTROL Condition] (Status) automatiskt baserat på projektets förlopp på tidslinjen. Mer information om villkor för projekt finns i <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Översikt över projektvillkor och villkorstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>Den här inställningen skapar automatiskt en baslinje (ögonblicksbild) av uppgifter och projektinformation när projektets status ändras till [!UICONTROL Current]. Mer information om hur du skapar baslinjer finns i <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Skapa projektbaslinjer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>Prestandaindexmetoden (PIM) för projektet styr metoden [!DNL Workfront] använder för att beräkna värden för upparbetat värde, t.ex. [!UICONTROL Cost Performance Index] (CPI) och [!UICONTROL Estimate At Completion] (EAC) Mer information finns i <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Beräkna [!UICONTROL Cost Performance Index] (CPI)</a> och <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] använder [!UICONTROL Planned Hours] för att beräkna prestandamått som EAC och CPI. När PIM beräknas baserat på timmar visas EAC som ett antal timmar. Se till att du har ett värde för [!UICONTROL Planned Hours], förutom noll.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] använder [!UICONTROL Planned Labor Cost] för att beräkna prestandamått som EAC och CPI. Se till att dina jobbroller eller -användare är kopplade till kostnaden per timme. När PIM beräknas baserat på kostnader visas EAC som ett valutavärde.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med [!UICONTROL Finance] område i [!UICONTROL Project Details]. Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektet [!UICONTROL Finance] area</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Bestäm vilka data [!DNL Workfront] används för att beräkna [!UICONTROL Estimate at Completion] (EAC) som representerar den beräknade totala kostnaden för ett projekt.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong>:EAC för den överordnade aktiviteten och projektet bestäms genom att ange [!UICONTROL Actual Hours] eller [!UICONTROL Actual Labor Cost] i EAC-formlerna. Denna beräkning innehåller [!UICONTROL Actual Hours] eller [!UICONTROL Costs and Expenses] läggs till direkt i den överordnade uppgiften eller det överordnade projektet.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: EAC för den överordnade uppgiften och projektet bestäms genom att EAC summeras för varje underordnad uppgift. Denna beräkning exkluderar [!UICONTROL Actual Hours] eller [!UICONTROL Actual Costs and Expenses] läggs till direkt i den överordnade uppgiften eller det överordnade projektet.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med [!UICONTROL Finance] område i [!UICONTROL Project Details].Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektet [!UICONTROL Finance] area</a>.</p> </li> 
    </ul> <p>Mer information om hur EAC beräknar finns i <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Beräkna [!UICONTROL Estimate At Completion] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Tidslinjer {#timelines}

Konfigurera någon av följande inställningar för nyligen skapade projekt i hela systemet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>Ange om nya projekt ska schemaläggas från Startdatum eller från Slutförandedatum när de skapas.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong>: Nya uppgifter används som standard i [!UICONTROL As Soon As Possible] Uppgiftsbegränsning och projektledare uppmanas att ange en [!UICONTROL Planned Start Date] för projektet.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>: Nya uppgifter används som standard i [!UICONTROL As Late As Possible] Uppgiftsbegränsning och projektledare uppmanas att ange en [!UICONTROL Planned Completion Date] för projektet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Avgör om tiden för den primära tilldelaren för en uppgift justerar de planerade datumen för den uppgiften i ett projekt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>: När en tidpunkt är schemalagd för en uppgifts primära tilldelare justeras aktivitetens planerade datum om tidpunkten för avbrottet inträffar under aktivitetens varaktighet. Det här är standardinställningen. </p> <p>Om en uppgift med en begränsning för [!UICONTROL As Soon As Possible] är planerad att börja den 1 juni och slutföras den 3 juni, och den primära tilldelaren har markerat 2 juni som"Time-off", aktivitetens planerade datum justeras till 1 juni till 4 juni.</p> <p><b>VIKTIGT</b>: Aktivitetens varaktighet ändras inte när du väljer den här inställningen. Endast planerade datum ändras beroende på aktivitetsbegränsning.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>: De planerade datumen för varje uppgift i ett projekt förblir som de ursprungligen var planerade, även om den primära tilldelaren för en uppgift har en ledig tid under varaktigheten.</li> 
    </ul> <p>Tänk på följande när du väljer alternativ för den här inställningen:</p> 
    <ul> 
     <li>När du ändrar den här inställningen ärver endast projekt och mallar som skapats efter ändringen den uppdaterade inställningen. </li> 
     <li> <p>Aktivitetsbegränsningsvärdet för aktiviteten avgör vilka planerade aktivitetsdatum som ska justeras: </p> 
      <ul> 
       <li>Planerat startdatum</li> 
       <li>Planerat slutförandedatum</li> 
       <li>Båda datumen</li> 
       <li>Ingendera datum. </li> 
      </ul> <p>Om en aktivitet till exempel har en begränsning för [!UICONTROL Fixed Dates]justerar inte datumen när den primära tilldelade har en ledig tid, även om alternativet [!UICONTROL Consider user time off in task duration] är markerat. Mer information om uppgiftsbegränsningar finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över uppgiftsbegränsning</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines will be automatically re-calculated]</p> </td> 
   <td> <p>Avgör när tidslinjen för ett projekt beräknas om. Mer information om hur du beräknar om projekttidslinjen finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> <p>Följande alternativ är aktiverade som standard. Du kan välja en eller flera av följande inställningar:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: Välj det här om du vill beräkna om projekttidslinjer varje kväll. Ändringar som du gör i projektet som kan påverka tidslinjen visas inte direkt. [!DNL Workfront​​​] Beräknar om tidslinjer på natten endast för projekt där båda följande villkor är uppfyllda:</p> <p> 
       <ul> 
        <li>Har statusen [!UICONTROL Current]</li> 
        <li>Har haft en uppdatering de senaste tre månaderna</li> 
        <li>Har haft en uppdateringstyp av något av följande:</li>
        <ul>
        <li>Automatiskt och vid ändring</li>
        <li>Ändra endast</li>
        <li>Endast automatiskt</li> 
      </ul>       
    <b>TIPS</b>
    <p>Projekt som har uppdateringstypen Endast manuell påverkas inte av den här inställningen.</p>
    <li> <p><strong>När ett projekts omfång ändras</strong>: Välj det här om du vill beräkna om projekttidslinjer omedelbart när en ändring av projektomfånget sker. Mer information om vad som utgör en ändring av projektets omfång finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>Om ett projekt inte har tilldelats ett schema eller om användarna som är tilldelade till dess uppgifter inte har tilldelats ett schema, [!DNL Workfront] använder systemets standardschema för att beräkna tidslinjen för aktiviteterna.</p> <p>Om du tilldelar flera användare till samma uppgift i ett projekt har ett tilldelat schema - och användarna som tilldelats till aktiviteterna har också ett schema -[!UICONTROL Workfront] använder följande scheman:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>: [!DNL Workfront] använder schemat för den primära tilldelningen för aktiviteten för att beräkna tidslinjer.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] använder schemat för projektet för att beräkna tidslinjen för varje uppgift.</li> 
    </ul> <p>Mer information om scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Skapa ett schema</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>: Ange antalet timmar på en vanlig arbetsdag för användare som ska arbeta med projekt. Standardvärdet är 8 timmar.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong>: Ange standardarbetsveckan för de användare som ska arbeta med projekt. Standardvärdet är 5 dagar.</li> 
    </ul> <p>Dessa två alternativ konverterar dagar till timmar, eller veckor till dagar.</p> <p>Om du till exempel har en aktivitet med 8 planerade timmar och varaktigheten beräknas baserat på planerade timmar, [!DNL Workfront] konverterar timmarna till dagar för att visa Varaktighet som dagar.</p> <p>Från Normal [!UICONTROL work days per week] fält, [!DNL Workfront] beräknar heltidsmotsvarigheten (FTE) för datorn. Det här är vad [!DNL Workfront] används vid beräkning av allokeringar för användare.</p> <p>Dessa värden används när du planerar projekttidslinjer, budgeterar för resurser eller loggar tid mot projekt. </p> <p>De används inte när du skapar tidrapporter för användare i systemet, vilket beskrivs i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] tidrapport och timinställningar</a>.</p> <p><b>ANMÄRKNING</b>: [!DNL Workfront] administratörer kan inte låsa upp [!UICONTROL Timeline Calculations] inställningar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Konfigurera anpassade årliga kvartal för användare som ska arbeta med projekt. Kvartal är vanligtvis kvartal som inte motsvarar den traditionella fördelningen av kvartal under ett kalenderår. Du kan lägga till flera anpassade kvartal. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Aktivera anpassade kvartal för projekt</a>.</p>  <p><b>ANMÄRKNING</b>: [!DNL Workfront] administratörer kan inte låsa upp [!UICONTROL Custom Quarters] inställningar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

Du kan skapa ett affärsärende för nyskapade projekt i hela systemet för att skicka projektförfrågningar. Du kan ange inställningar för vilka områden som ska visas på **[!UICONTROL Business Case]** formulär. Vi rekommenderar att du aktiverar dessa alternativ så att andra verktyg, som [!UICONTROL Portfolio Optimizer], uppdateras korrekt. Mer information om vad varje fält visar finns i [Definiera ett affärsärende: artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Efter [!DNL Workfront] administratören aktiverar avsnitten i [!UICONTROL Business Case]kan en projektägare sedan skapa ett affärsärende på projektnivå. Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Life After Death] {#life-after-death}

Konfigurera någon av följande inställningar för nyligen skapade projekt i hela systemet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Ange reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) för om en uppgift eller ett problem kan tas bort efter att projektstatusen har markerats [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>: Tillåter användare att ta bort uppgifter från ett projekt efter att projektet har markerats [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>: Tillåter användare att ta bort utgåvor från ett projekt efter att projektet har markerats [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Bestäm reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) vad som ska hända med uppgifter, ärenden, dokument och andra objekt i ett projekt när projektstatusen har markerats <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, eller är <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks]</strong> Tillåter användare att:
      <ul>
       <li>Redigera aktiviteter i ett projekt när projektet har markerats [!UICONTROL Complete], [!UICONTROL Dead], eller är [!UICONTROL Pending Approval]. Detta inkluderar att lägga till timmar och ändra utgiftsposter för en aktivitet.</li>
       <li>Lägg till uppgifter i ett projekt.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Add and edit issues]</strong>: Tillåter användare att:
      <ul>
       <li>Redigera problem i ett projekt efter att projektet har markerats [!UICONTROL Complete], [!UICONTROL Dead], eller [!UICONTROL Pending Approval].</li>
       <li>Lägg till utgåvor i ett projekt efter att projektet har markerats [!UICONTROL Complete] eller [!UICONTROL Dead]. (Du kan inte lägga till problem i ett projekt som [!UICONTROL Pending Approval].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>: Tillåter användare att lägga till dokument i ett projekt (eller att lägga till dokument i aktiviteter och ärenden i projektet) efter att projektet har markerats [!UICONTROL Complete] eller [!UICONTROL Dead].</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: Tillåter användare att bifoga mallar till ett projekt efter att projektet har markerats [!UICONTROL Complete] eller [!UICONTROL Dead].</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
