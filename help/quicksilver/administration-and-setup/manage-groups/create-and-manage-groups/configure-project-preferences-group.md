---
title: Konfigurera projektinställningar för en grupp
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Om du är gruppadministratör och en Adobe Workfront-administratör låser upp en projektinställning för alla grupper i systemet kan du konfigurera den inställningen så att den påverkar alla efterföljande projekt som gruppen skapar.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '2736'
ht-degree: 0%

---

# Konfigurera projektinställningar för en grupp


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Om du är gruppadministratör och en Adobe Workfront-administratör låser upp en projektinställning för alla grupper i systemet kan du konfigurera den inställningen så att den påverkar alla efterföljande projekt som gruppen skapar.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>* Normalt förblir en olåst inställning olåst i oändlighet. Om Workfront-administratören låser om den aktiveras systeminställningen igen och inställningarna som gjorts av gruppadministratörerna går förlorade.
>* Inställningarna för gruppen som är kopplad till ett projekt har företräde framför inställningarna för hemgruppen för användaren som skapar projektet.
>* Vissa gruppnivåinställningar påverkar projektmallar som du skapar för gruppen. Mer information finns i avsnittet [Visa, arbeta med och skapa mallar för din grupp från gruppområdet](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* När en Workfront-administratör har låst upp en inställning på systemnivå kan du konfigurera den och sedan låsa den så att alla i gruppen och dess undergrupper använder samma konfiguration. Detta är parallellt med möjligheten för en Workfront-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Lås eller lås upp ett projekt, en uppgift eller en utgåva för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

Konfiguration på gruppnivå är också möjligt för uppgifter och utgåvor samt för tidrapport- och timinställningar. Mer information finns i [Konfigurera aktivitets- och probleminställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) och [Konfigurera tidrapport- och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Mer information om hur en Workfront-administratör låser upp en projektinställning finns i [Lås eller lås upp projektinställningar för alla grupper i systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera en olåst projektinställning för en grupp

>[!TIP]
>
>Om du är Workfront-administratör kan du kringgå steg 1-4 genom att gå till Inställningar > Projektinställningar > Projekt och sedan söka efter gruppens namn i rutan längst upp på sidan.

{{step-1-to-setup}}

1. Klicka på ikonen **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen vars projektinställningar du vill konfigurera.
1. Klicka på **Projektinställningar** i den vänstra panelen.
1. På den sida som visas fortsätter du med ett av de fyra avsnitten nedan för att konfigurera inställningar för Projektstatus, Tidslinjer, Affärsfall och Livstid efter dödsfall.

   >[!TIP]
   >
   >Om du håller muspekaren över en inställning och ett verktygstips visas som talar om att den är låst, kan du be Workfront-administratören att låsa upp den för alla grupper i organisationen.

* [Projektstatus](#project-status)
* [Tidslinjer](#timelines)
* [Affärsärenden](#business-cases)
* [Liv efter dödsfall](#life-after-death)

### Projektstatus {#project-status}

Konfigurera någon av följande inställningar för nyligen skapade projekt som är kopplade till gruppen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Tillåt användare att skapa projekt utan att använda en mall</td>
<td><p>Med den här inställningen kan användare skapa projekt utan att använda en mall när de skapar ett projekt från följande områden:</p>
<ul>
<li><p>Använd alternativet Nytt projekt i en lista med projekt</p></li>

<li><p>Konvertera ett problem till ett projekt från problemsidan</p></li>
</ul>

<p>Den här inställningen är aktiverad som standard på systemnivå.</p>
<p><b>ANMÄRKNING</b></p>
<p>När en användare tillhör flera grupper med olika inställningar kan användaren skapa ett projekt utan en mall om minst en av grupperna har den här inställningen aktiverad.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Ange status för det nya projektet till</td> 
   <td> <p>Bestäm status för nya projekt.</p> <p><b>OBS!</b>   
     <ul> 
      <li>Om du eller någon annan Workfront-administratör döljer den status som valts här, ändras standardstatusen till den första statusen i statuslistan.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">För gruppprojektinställningar kan du välja enbart en låst status eller en obligatorisk status som standardstatus.</li> 
      <li> <p>Om ett låst system eller en grupp är inställd som standardstatus och någon senare låser upp den försöker systemet ersätta den med en låst status av samma statustyp.</p> <p>Om det inte går att hitta någon söker programmet efter en obligatorisk status:</p> 
       <ul> 
        <li>Om det finns en obligatorisk status som motsvarar den olåsta standardstatusen blir den obligatoriska statusen standardstatus, även om den är olåst.</li> 
        <li>Om ingen av de obligatoriska statusvärdena motsvarar den olåsta standardstatusen blir den första obligatoriska statusen i statuslistan standardstatus.</li> 
       </ul> <p>Mer information om obligatoriska statusvärden finns i artiklarna <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemprojekt</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemaktivitet</a> och <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemproblem</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Beräkna procent färdigt baserat på</td> 
   <td> <p>Procent färdigt för ett projekt eller en överordnad uppgift baseras på aktiviteternas allmänna förlopp. Den här informationen kan beräknas utifrån varaktigheten eller den planerade timmen för aktiviteterna i ett projekt.</p> <p>Om du väljer Varaktighet bestämmer varaktigheten för varje aktivitet i ett projekt den totala procentandelen färdigt för projektet, och varaktigheten för varje underaktivitet bestämmer den totala procentandelen färdigt för den överordnade aktiviteten.</p> <p>Om du väljer Varaktighet måste du ange Normal tid per arbetsdag och Normal arbetsdag per vecka i avsnittet Tidslinjer. Workfront använder den här informationen vid beräkning av en uppgifts procentandel slutförd baserat på Varaktighet. </p> <p>Om du väljer Planerade timmar kontrollerar du att antalet planerade timmar har definierats för alla aktiviteter i varje projekt, och att beloppet inte är noll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ställ in projektets villkor automatiskt baserat på förloppsstatusen</td> 
   <td> <p>Med den här inställningen kan användare ställa in villkoret för ett projekt manuellt (på mål, risk, i problem) eller låta Workfront ställa in villkoret (förloppsstatus) automatiskt baserat på projektets förlopp på tidslinjen. Mer information om villkor för projekt finns i <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Översikt över projektvillkor och villkorstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Skapa baslinjer automatiskt</p> </td> 
   <td> <p>Den här inställningen skapar automatiskt en baslinje (ögonblicksbild) av uppgifter och projektinformation när projektets status ändras till Aktuell. Mer information om hur du skapar baslinjer finns i <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Skapa projektbaslinjer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Resultatindexmetod </p> </td> 
   <td> <p>Performance Index Method (PIM) for the project controls the method Workfront uses to calculate Earned Value metrics such as Cost Performance Index (CPI) and Estimate At Completion (EAC). Mer information finns i <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Beräkna kostnadsprestandaindex (CPI)</a> och <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Beräkna uppskattning vid slutförande (EAC)</a></p> 
    <ul> 
     <li><strong>Timbaserad</strong>: Workfront använder planerade timmar för att beräkna prestandamått som EAC och CPI. När PIM beräknas baserat på timmar visas EAC som ett antal timmar. Se till att du har ett annat värde än noll för Planerade timmar.</li> 
     <li> <p><strong>Kostnadsbaserad</strong>: Workfront använder Planerad arbetskostnad för att beräkna prestandamått som EAC och CPI. Se till att dina jobbroller eller -användare är kopplade till kostnaden per timme. När PIM beräknas baserat på kostnader visas EAC som ett valutavärde.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med hjälp av området Ekonomi i Projektinformation. Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektfinansieringsdelen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Uppskattning vid slutförande </p> </td> 
   <td> <p>Bestäm vilka data Workfront använder för att beräkna uppskattningen vid slutförande (EAC) som representerar den beräknade totala kostnaden för ett projekt.</p> 
    <ul> 
     <li><strong>Beräkna på projektnivå</strong>:EAC för den överordnade aktiviteten och projektet bestäms genom att ange Faktiska timmar eller Faktisk arbetskostnad i EAC-formlerna. Beräkningen omfattar faktiska timmar eller kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.</li> 
     <li> <p><strong>Samla in uppgifter/underaktiviteter</strong>: EAC för den överordnade aktiviteten och projektet bestäms genom att summera EAC för varje underordnad aktivitet. Den här beräkningen exkluderar faktiska timmar eller faktiska kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med hjälp av området Ekonomi i Projektinformation. Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektfinansieringsdelen</a>.</p> </li> 
    </ul> <p>Mer information om hur EAC beräknar finns i <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Beräkna beräkning vid slutförande (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Tidslinjer {#timelines}

Konfigurera någon av följande inställningar för nyligen skapade projekt som är kopplade till gruppen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Schemalägg från</td> 
   <td> <p>Ange om nya projekt ska schemaläggas från Startdatum eller från Slutförandedatum när de skapas.</p> 
    <ul> 
     <li><strong>Startdatum</strong>: Nya aktiviteter som standard är som standard aktivitetsbegränsning så snart som möjligt och projektledare uppmanas att ange ett planerat startdatum för projektet.</li> 
     <li><strong>Slutförandedatum</strong>: Nya aktiviteter anges som standard till aktivitetsbegränsningen Så sent som möjligt och projektledare uppmanas att ange ett planerat slutförandedatum för projektet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Användningstid av</td> 
   <td> <p>Avgör om tiden för den primära tilldelaren för en uppgift justerar de planerade datumen för den uppgiften i ett projekt.</p> 
    <ul> 
     <li> <p><strong>Överväg användarens inaktivitet i varaktigheter</strong>: Alla tidsperioder som är schemalagda för en uppgifts primära tilldelningsdatum justerar aktivitetens planerade datum om tiden för inaktivitet inträffar under aktivitetens varaktighet. Det här är standardinställningen. </p> <p>Om en uppgift med ett villkor som är lika med så snart som möjligt är schemalagd att påbörjas den 1 juni och slutföras den 3 juni, och den primära uppdragen har markerat till 2 juni som"Time-off", justeras aktivitetens planerade datum till 1 juni till 4 juni.</p> <p><b>VIKTIGT</b>: Aktivitetens varaktighet ändras inte när du väljer den här inställningen. Endast planerade datum ändras beroende på aktivitetsbegränsning.</p> </li> 
     <li><strong>Ignorera användartid för aktivitetsvaraktigheter</strong>: De planerade datumen för varje aktivitet i ett projekt förblir som de ursprungligen planerade, även om den primära tilldelaren för en aktivitet har en ledig tid under varaktigheten.</li> 
    </ul> <p>Tänk på följande när du väljer alternativ för den här inställningen:</p> 
    <ul> 
     <li>När du ändrar den här inställningen ärver endast projekt och mallar som skapats efter ändringen den uppdaterade inställningen. </li> 
     <li> <p>Aktivitetsbegränsningsvärdet för aktiviteten avgör vilka planerade aktivitetsdatum som ska justeras: </p> 
      <ul> 
       <li>Planerat startdatum</li> 
       <li>Planerat slutförandedatum</li> 
       <li>Båda datumen</li> 
       <li>Ingendera datum. </li> 
      </ul> <p>Om en aktivitet till exempel har en begränsning med fasta datum, justeras inte datumen när den primära tilldelaren har en ledig tid, även om alternativet Beakta användarens tid för en uppgift är markerat. Mer information om uppgiftsbegränsningar finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över uppgiftsbegränsningar</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Projekttidslinjer beräknas om automatiskt</strong> </p> </td> 
   <td> <p>Avgör när tidslinjen för ett projekt beräknas om. Mer information om hur du beräknar om projekttidslinjen finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> <p>Följande alternativ är aktiverade som standard. Du kan välja en eller flera av följande inställningar:</p> 
    <ul> 
     <li> <p><strong>Varje kväll</strong>: Välj det här alternativet om du vill beräkna om projekttidslinjer varje kväll. Ändringar som du gör i projektet som kan påverka tidslinjen visas inte direkt. Workfront ​ ​ beräknar om tidslinjer på natten endast för projekt där båda följande villkor är uppfyllda:</p> <p> 
       <ul> 
        <li>Har statusen Aktuell</li> 
        <li>Har haft en uppdatering de senaste tre månaderna</li> 
       </ul> </p> </li> 
     <li> <p><strong>När ett projekts omfång ändras</strong>: Välj det här om du vill beräkna om projekttidslinjer omedelbart när en ändring av projektomfånget sker. Mer information om vad som utgör en ändring av projektomfattning finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>När flera användare tilldelas till en aktivitet ska du använda schemat för ...</strong> </p> </td> 
   <td> <p>Om ett projekt inte har tilldelats ett schema eller om användarna som är tilldelade till dess uppgifter inte har tilldelats ett schema, använder Workfront systemets standardschema för att beräkna tidslinjen för aktiviteterna.</p> <p>Om du tilldelar flera användare till samma uppgift i ett projekt har ett tilldelat schema - och användarna som tilldelats till uppgifterna har också ett schema - använder Workfront följande scheman:</p> 
    <ul> 
     <li><strong>Primär tilldelning</strong>: Workfront använder schemat för den primära tilldelningen för aktiviteten för att beräkna tidslinjer.</li> 
     <li><strong>Projekt</strong>: Workfront använder projektschemat för att beräkna tidslinjen för varje aktivitet.</li> 
    </ul> <p>Mer information om scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Skapa ett schema</a>.</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><strong>När en användare tilldelas till en aktivitet ska du använda schemat för ...</strong> </p> </td> 
   <td> <p>Om ett projekt inte har tilldelats ett schema, eller om användarna som är tilldelade till dess aktiviteter inte har tilldelats ett schema, använder [!DNL Workfront] systemets standardschema för att beräkna tidslinjen för aktiviteterna.</p>

<p>Om du tilldelar en användare till en aktivitet i ett projekt och både projektet och användaren har ett associerat schema, använder [!UICONTROL Workfront] följande scheman:</p> 
    <ul> 
     <li><strong>[!UICONTROL User]</strong>: Schemat för den tilldelade användaren i aktiviteten för att beräkna tidslinjer.</li> 
     <li><strong>[!UICONTROL Project]</strong>: Schemat för projektet för att beräkna tidslinjen för aktiviteten.</li> 
    </ul> <p>Mer information om scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Skapa ett schema</a>.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Beräkningar av tidslinje </p> </td> 
   <td> 
    <ul> 
     <li><strong>Vanliga timmar per arbetsdag</strong>: Ange antalet timmar på en vanlig arbetsdag för användare som ska arbeta med projekt. Standardvärdet är 8 timmar.</li> 
    </ul> 
    <ul> 
     <li><strong>Vanliga arbetsdagar per vecka</strong>: Ange standardarbetsveckan för de användare som ska arbeta med projekt. Standardvärdet är 5 dagar.</li> 
    </ul> <p>Dessa två alternativ konverterar dagar till timmar, eller veckor till dagar.</p> <p>Om du till exempel har en aktivitet med 8 planerade timmar och varaktigheten beräknas baserat på Planerade timmar, konverterar Workfront dessa timmar till dagar för att visa Varaktighet som dagar.</p> <p>I fältet Normal arbetsdagar per vecka beräknas heltidsmotsvarigheten (FTE) för datorn. Detta är vad Workfront använder vid beräkning av allokeringar för användare.</p> <p>Dessa värden används när du planerar projekttidslinjer, budgeterar för resurser eller loggar tid mot projekt. </p> <p>De används inte när du skapar tidrapporter för användare i systemet, vilket beskrivs i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Konfigurera tidrapport och timinställningar</a>.</p> <p><b>Obs!</b> Workfront-administratörer kan inte låsa upp inställningarna för tidslinjeberäkningar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Egna kvartal</strong> </p> </td> 
   <td> <p>Konfigurera anpassade årliga kvartal för användare som ska arbeta med projekt. Kvartal är vanligtvis kvartal som inte motsvarar den traditionella fördelningen av kvartal under ett kalenderår. Du kan lägga till flera anpassade kvartal. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Aktivera anpassade kvartal</a>.</p> <p><b>Obs!</b> Workfront-administratörer kan inte låsa upp anpassade kvartal.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Affärsärenden {#business-cases}

Du kan skapa ett affärsärende för nyligen skapade projekt som är kopplade till gruppen för att skicka projektbegäranden. Du kan definiera inställningar för att avgöra vilka områden som visas i formuläret **Affärsärende**. Vi rekommenderar att du aktiverar dessa alternativ så att andra verktyg, som Portfolio Optimizer, uppdateras korrekt. Mer information om vad varje fält visar finns i [Definiera ett affärsfall: artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

När Workfront-administratören har aktiverat avsnitten i affärsärendet kan en projektägare sedan skapa ett affärsärende på projektnivå. Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Liv efter dödsfall  {#life-after-death}

Konfigurera någon av följande inställningar för nyligen skapade projekt som är kopplade till gruppen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>När ett projekt har markerats som fullständigt kan andra användare fortfarande</strong> </p> </td> 
   <td> <p>Bestäm reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) för om en uppgift eller ett problem kan tas bort efter att projektstatusen har markerats som Slutförd.</p> 
    <ul> 
     <li><strong>Ta bort aktiviteter</strong>: Tillåter användare att ta bort aktiviteter från ett projekt efter att projektet har markerats som Slutfört.<br></li> 
     <li><strong>Ta bort problem</strong>: Tillåter användare att ta bort problem från ett projekt efter att projektet har markerats som Slutfört.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>När ett projekt har markerats som slutfört, inaktivt eller väntar på godkännande kan andra fortfarande</strong> </p> </td> 
   <td> <p>Bestäm reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) vad som ska hända med aktiviteter, ärenden, dokument och andra objekt i ett projekt när projektstatusen har markerats som <strong>Fullständigt</strong>, <strong>Borttaget</strong> eller är <strong>Väntande godkännande</strong>.</p> 
    <ul> 
     <li><strong>Lägg till och redigera uppgifter</strong> Tillåter användare att: 
      <ul> 
       <li>Redigera uppgifter i ett projekt när projektet har markerats som slutfört, inaktivt eller väntar på godkännande. Detta inkluderar att lägga till timmar och ändra utgiftsposter för en aktivitet.</li> 
       <li>Lägg till uppgifter i ett projekt.</li> 
      </ul></li> 
     <li><strong>Lägg till och redigera problem</strong>: Tillåter användare att: 
      <ul> 
       <li>Redigera problem i ett projekt efter att projektet har markerats som slutfört, inaktuellt eller väntande godkännande.</li> 
       <li>Lägg till problem i ett projekt när projektet har markerats som slutfört eller inaktivt. (Du kan inte lägga till utgåvor i ett projekt som väntar på godkännande.)</li> 
      </ul></li> 
     <li> <p><strong>Lägg till dokument i projektet och i dess aktiviteter och ärenden</strong>: Tillåter användare att lägga till dokument i ett projekt (eller att lägga till dokument i aktiviteter och ärenden i projektet) efter att projektet har markerats som Slutfört eller Dölj.</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
     <li> <p><strong>Bifoga mallar</strong>: Tillåter användare att bifoga mallar till ett projekt efter att projektet har markerats som Fullständigt eller Dölj.</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
