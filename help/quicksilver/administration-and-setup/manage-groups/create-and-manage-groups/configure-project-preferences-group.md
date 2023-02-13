---
title: Konfigurera projektinställningar för en grupp
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Om du är gruppadministratör och en Adobe Workfront-administratör låser upp en projektinställning för alla grupper i systemet kan du konfigurera den inställningen så att den påverkar alla efterföljande projekt som gruppen skapar.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 0%

---

# Konfigurera projektinställningar för en grupp

Om du är gruppadministratör och en Adobe Workfront-administratör låser upp en projektinställning för alla grupper i systemet kan du konfigurera den inställningen så att den påverkar alla efterföljande projekt som gruppen skapar.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>* Normalt förblir en olåst inställning olåst i oändlighet. Om Workfront-administratören låser om den aktiveras systeminställningen igen och inställningarna som gjorts av gruppadministratörerna går förlorade.
>* Inställningarna för gruppen som är kopplad till ett projekt har företräde framför inställningarna för hemgruppen för användaren som skapar projektet.
>* Vissa gruppnivåinställningar påverkar projektmallar som du skapar för gruppen. Mer information finns i avsnittet [Visa, arbeta med och skapa mallar för din grupp i området Grupper](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* När en Workfront-administratör har låst upp en inställning på systemnivå kan du konfigurera den och sedan låsa den så att alla i gruppen och dess undergrupper använder samma konfiguration. Detta är parallellt med möjligheten för en Workfront-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Låsa eller låsa upp ett projekt, en uppgift eller en utleverans för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


Konfiguration på gruppnivå är också möjligt för uppgifter och utgåvor samt för tidrapport- och timinställningar. Mer information finns i [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) och [Konfigurera tidrapport och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Information om hur en Workfront-administratör låser upp en projektinställning finns i [Låsa eller låsa upp projektinställningar för alla grupper i systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Konfigurera en olåst projektinställning för en grupp

>[!TIP]
>
>Om du är Workfront-administratör kan du kringgå steg 1-4 genom att gå till Inställningar > Projektinställningar > Projekt och sedan söka efter gruppens namn i rutan längst upp på sidan.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på namnet på gruppen vars projektinställningar du vill konfigurera.
1. Klicka på i den vänstra panelen **Projektinställningar**.
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
   <td> <p>Fastställ status för nya projekt.</p> <p><b>ANMÄRKNING</b>   
     <ul> 
      <li>Om du eller någon annan Workfront-administratör döljer den status som valts här ändras standardstatusen till den första statusen i statuslistan.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">För gruppprojektinställningar kan du välja enbart en låst status eller en obligatorisk status som standardstatus.</li> 
      <li> <p>Om ett låst system eller en grupp är inställd som standardstatus och någon senare låser upp den försöker systemet ersätta den med en låst status av samma statustyp.</p> <p>Om det inte går att hitta någon söker programmet efter en obligatorisk status:</p> 
       <ul> 
        <li>Om det finns en obligatorisk status som motsvarar den olåsta standardstatusen blir den obligatoriska statusen standardstatus, även om den är olåst.</li> 
        <li>Om ingen av de obligatoriska statusvärdena motsvarar den olåsta standardstatusen blir den första obligatoriska statusen i statuslistan standardstatus.</li> 
       </ul> <p>Mer information om obligatoriska statusvärden finns i artiklarna <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Öppna listan över status för systemprojekt</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemaktivitet</a>och <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Åtkomst till listan över status för systemproblem</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Beräkna procent färdigt baserat på</td> 
   <td> <p>Procent färdigt för ett projekt eller en överordnad uppgift baseras på aktiviteternas allmänna förlopp. Den här informationen kan beräknas utifrån varaktigheten eller den planerade timmen för aktiviteterna i ett projekt.</p> <p>Om du väljer Varaktighet bestämmer varaktigheten för varje aktivitet i ett projekt den totala procentandelen färdigt för projektet, och varaktigheten för varje underaktivitet bestämmer den totala procentandelen färdigt för den överordnade aktiviteten.</p> <p>Om du väljer Varaktighet måste du ange Normal tid per arbetsdag och Normal arbetsdag per vecka i avsnittet Tidslinjer. Workfront använder den här informationen vid beräkning av en uppgifts procentandel slutförd baserat på Varaktighet. </p> <p>Om du väljer Planerade timmar kontrollerar du att antalet planerade timmar har definierats för alla aktiviteter i varje projekt, och att beloppet inte är noll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ange automatiskt projektets villkor baserat på förloppsstatusen</td> 
   <td> <p>Med den här inställningen kan användare ställa in villkoret för ett projekt manuellt (på mål, risk, i problem) eller låta Workfront ställa in villkoret (förloppsstatus) automatiskt baserat på projektets förlopp på tidslinjen. Mer information om villkor för projekt finns i <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Översikt över projektvillkor och villkorstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Skapa baslinjer automatiskt</p> </td> 
   <td> <p>Den här inställningen skapar automatiskt en baslinje (ögonblicksbild) av uppgifter och projektinformation när projektets status ändras till Aktuell. Mer information om hur du skapar baslinjer finns i <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Skapa projektbaslinjer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Resultatindexmetod </p> </td> 
   <td> <p>Performance Index Method (PIM) for the project controls the method Workfront uses to calculate Earned Value metrics such as Cost Performance Index (CPI) and Estimate At Completion (EAC). Mer information finns i <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Beräkna index för kostnadsprestanda (CPI)</a>och <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Beräkna uppskattning vid slutförande</a></p> 
    <ul> 
     <li><strong>Timbaserad</strong>: Workfront använder Planerade timmar för att beräkna prestandamått som EAC och CPI. När PIM beräknas baserat på timmar visas EAC som ett antal timmar. Kontrollera att du har ett annat värde än noll för Planerade timmar.</li> 
     <li> <p><strong>Kostnadsbaserad</strong>: Workfront använder Planerad arbetskostnad för att beräkna prestandamått som EAC och CPI. Se till att dina jobbroller eller -användare är kopplade till kostnaden per timme. När PIM beräknas baserat på kostnader visas EAC som ett valutavärde.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med hjälp av området Ekonomi i Projektinformation. Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektfinansieringsdelen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Uppskattning vid slutförande </p> </td> 
   <td> <p>Bestäm vilka data Workfront använder för att beräkna uppskattningen vid slutförande (EAC) som representerar den beräknade totala kostnaden för ett projekt.</p> 
    <ul> 
     <li><strong>Beräkna på projektnivå</strong>:EAC för den överordnade uppgiften och projektet bestäms genom att Faktiska timmar eller Faktisk arbetskostnad anges i EAC-formlerna. Beräkningen omfattar faktiska timmar eller kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.</li> 
     <li> <p><strong>Samla in uppgifter/underuppgifter</strong>: EAC för den överordnade uppgiften och projektet bestäms genom att sammanfatta EAC för varje underordnad uppgift. Den här beräkningen exkluderar faktiska timmar eller faktiska kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.</p> <p>Projektledaren kan ändra den här inställningen på projektnivå med hjälp av området Ekonomi i Projektinformation. Mer information finns i <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Hantera information i projektfinansieringsdelen</a>.</p> </li> 
    </ul> <p>Mer information om hur EAC beräknas finns i <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Beräkna uppskattning vid slutförande</a>.</p> </td> 
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
     <li><strong>Startdatum</strong>: Som standard för nya uppgifter anges ett planerat startdatum för projektet av aktivitetsbegränsningen Så snart som möjligt och projektansvariga.</li> 
     <li><strong>Slutförandedatum</strong>: Som standard för nya uppgifter anges ett planerat slutförandedatum för projektet av aktivitetsbegränsningen Så sent som möjligt och projektansvariga.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Användningstid av</td> 
   <td> <p>Avgör om tiden för den primära tilldelaren för en uppgift justerar planerade datum för den uppgiften i ett projekt.</p> 
    <ul> 
     <li> <p><strong>Överväg användarens ledig tid i aktivitetsvaraktigheter</strong>: När en tid är schemalagd för en uppgifts primära tilldelare justeras aktivitetens planerade datum om tidpunkten för avbrottet inträffar under aktivitetens varaktighet. Det här är standardinställningen. </p> <p>Om en uppgift med ett villkor som är lika med så snart som möjligt är schemalagd att påbörjas den 1 juni och slutföras den 3 juni, och den primära uppdragen har markerat till 2 juni som"Time-off", justeras aktivitetens planerade datum till 1 juni till 4 juni.</p> <p><b>VIKTIGT</b>: Aktivitetens varaktighet ändras inte när du väljer den här inställningen. Endast planerade datum ändras beroende på aktivitetsbegränsning.</p> </li> 
     <li><strong>Ignorera användartid för aktivitetsvaraktighet</strong>: De planerade datumen för varje uppgift i ett projekt förblir som de ursprungligen planerade, även om den primära tilldelaren för en uppgift har en ledig tid under varaktigheten.</li> 
    </ul> <p>Tänk på följande när du väljer alternativ för den här inställningen:</p> 
    <ul> 
     <li>När du ändrar den här inställningen ärver endast projekt och mallar som skapats efter ändringen den uppdaterade inställningen. </li> 
     <li> <p>Aktivitetsbegränsningsvärdet för aktiviteten avgör vilka planerade aktivitetsdatum som ska justeras: </p> 
      <ul> 
       <li>Planerat startdatum</li> 
       <li>Planerat slutförandedatum</li> 
       <li>Båda datumen</li> 
       <li>Inget datum. </li> 
      </ul> <p>Om en aktivitet till exempel har en begränsning med fasta datum, justeras inte datumen när den primära tilldelaren har en ledig tid, även om alternativet Beakta användarens tid för en uppgift är markerat. Mer information om uppgiftsbegränsningar finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Översikt över uppgiftsbegränsning</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Projektets tidslinjer beräknas om automatiskt</strong> </p> </td> 
   <td> <p>Avgör när tidslinjen för ett projekt beräknas om. Mer information om hur du beräknar om projekttidslinjen finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> <p>Följande alternativ är aktiverade som standard. Du kan välja en eller flera av följande inställningar:</p> 
    <ul> 
     <li> <p><strong>Varje kväll</strong>: Välj det här om du vill beräkna om projekttidslinjer varje kväll. Ändringar som du gör i projektet som kan påverka tidslinjen visas inte direkt. Workfront ​ ​ beräknar om tidslinjer på natten endast för projekt där båda följande villkor är uppfyllda:</p> <p> 
       <ul> 
        <li>Har statusen Aktuell</li> 
        <li>Har haft en uppdatering de senaste tre månaderna</li> 
       </ul> </p> </li> 
     <li> <p><strong>När ett projekts omfång ändras</strong>: Välj det här om du vill beräkna om projekttidslinjer omedelbart när en ändring av projektomfånget sker. Mer information om vad som utgör en ändring av projektets omfång finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Beräkna om projekttidslinjer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>När flera användare tilldelas till en uppgift använder du schemat för</strong> </p> </td> 
   <td> <p>Om ett projekt inte har tilldelats ett schema eller om användarna som är tilldelade till dess uppgifter inte har tilldelats ett schema, använder Workfront systemets standardschema för att beräkna tidslinjen för aktiviteterna.</p> <p>Om du tilldelar flera användare till samma uppgift i ett projekt har ett tilldelat schema - och användarna som tilldelats till uppgifterna har också ett schema - använder Workfront följande scheman:</p> 
    <ul> 
     <li><strong>Primär tilldelning</strong>: Workfront använder schemat för den primära tilldelningen för aktiviteten för att beräkna tidslinjer.</li> 
     <li><strong>Projekt</strong>: Workfront använder schemat för projektet för att beräkna tidslinjen för varje uppgift.</li> 
    </ul> <p>Mer information om scheman finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Skapa ett schema</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Beräkningar av tidslinje </p> </td> 
   <td> 
    <ul> 
     <li><strong>Vanliga timmar per arbetsdag</strong>: Ange antalet timmar på en vanlig arbetsdag för de användare som ska arbeta med projekt. Standardvärdet är 8 timmar.</li> 
    </ul> 
    <ul> 
     <li><strong>Vanliga arbetsdagar per vecka</strong>: Ange standardarbetsveckan för de användare som ska arbeta med projekt. Standardvärdet är 5 dagar.</li> 
    </ul> <p>Dessa två alternativ konverterar dagar till timmar, eller veckor till dagar.</p> <p>Om du till exempel har en aktivitet med 8 planerade timmar och varaktigheten beräknas baserat på Planerade timmar, konverterar Workfront dessa timmar till dagar för att visa Varaktighet som dagar.</p> <p>I fältet Normal arbetsdagar per vecka beräknas heltidsmotsvarigheten (FTE) för datorn. Detta är vad Workfront använder vid beräkning av allokeringar för användare.</p> <p>Dessa värden används när du planerar projekttidslinjer, budgeterar för resurser eller loggar tid mot projekt. </p> <p>De används inte när du skapar tidrapporter för användare i systemet, vilket beskrivs i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Konfigurera tidrapport och timinställningar</a>.</p> <p><b>ANMÄRKNING</b>: Workfront-administratörer kan inte låsa upp inställningarna för tidslinjeberäkningar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Anpassade kvartal</strong> </p> </td> 
   <td> <p>Konfigurera anpassade årliga kvartal för användare som ska arbeta med projekt. Kvartal är vanligtvis kvartal som inte motsvarar den traditionella fördelningen av kvartal under ett kalenderår. Du kan lägga till flera anpassade kvartal. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Aktivera anpassade kvartal för projekt</a>.</p> <p><b>ANMÄRKNING</b>: Workfront-administratörer kan inte låsa upp anpassade kvartal.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Affärsärenden {#business-cases}

Du kan skapa ett affärsärende för nyligen skapade projekt som är kopplade till gruppen för att skicka projektbegäranden. Du kan ange inställningar för vilka områden som ska visas på **Affärsärende** formulär. Vi rekommenderar att du aktiverar de här alternativen så att andra verktyg, som Portfolio-optimering, uppdateras korrekt. Mer information om vad varje fält visar finns i [Definiera ett affärsärende](../../../manage-work/projects/define-a-business-case/define-business-case.md).

När Workfront-administratören har aktiverat avsnitten i affärsärendet kan en projektägare sedan skapa ett affärsärende på projektnivå. Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Liv efter dödsfall  {#life-after-death}

Konfigurera någon av följande inställningar för nyligen skapade projekt som är kopplade till gruppen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>När ett projekt har markerats som fullständigt kan man fortfarande</strong> </p> </td> 
   <td> <p>Bestäm reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) för om en uppgift eller ett problem kan tas bort efter att projektstatusen har markerats som Slutförd.</p> 
    <ul> 
     <li><strong>Ta bort aktiviteter</strong>: Tillåter användare att ta bort uppgifter från ett projekt efter att projektet har markerats som Slutfört.<br></li> 
     <li><strong>Ta bort problem</strong>: Tillåter användare att ta bort utgåvor från ett projekt efter att projektet har markerats som Slutfört.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>När ett projekt har markerats som slutfört, inaktivt eller väntar på godkännande kan man fortfarande</strong> </p> </td> 
   <td> <p>Bestäm reglerna för din organisation (eller grupp, om du konfigurerar projektinställningar för en grupp) för vad som händer med uppgifter, ärenden, dokument och andra objekt i ett projekt när projektstatusen har markerats <strong>Slutförd</strong>, <strong>Död</strong>, eller är <strong>Väntar på godkännande</strong>.</p> 
    <ul> 
     <li><strong>Lägga till och redigera uppgifter</strong> Tillåter användare att: 
      <ul> 
       <li>Redigera uppgifter i ett projekt när projektet har markerats som slutfört, inaktivt eller väntar på godkännande. Detta inkluderar att lägga till timmar och ändra utgiftsposter för en aktivitet.</li> 
       <li>Lägg till uppgifter i ett projekt.</li> 
      </ul></li> 
     <li><strong>Lägga till och redigera problem</strong>: Tillåter användare att: 
      <ul> 
       <li>Redigera problem i ett projekt efter att projektet har markerats som slutfört, inaktuellt eller väntande godkännande.</li> 
       <li>Lägg till problem i ett projekt när projektet har markerats som slutfört eller inaktivt. (Du kan inte lägga till utgåvor i ett projekt som väntar på godkännande.)</li> 
      </ul></li> 
     <li> <p><strong>Lägga till dokument i projektet och i dess uppgifter och ärenden</strong>: Tillåter användare att lägga till dokument i ett projekt (eller att lägga till dokument till aktiviteter och ärenden i projektet) efter att projektet har markerats som Fullständigt eller Dölj.</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
     <li> <p><strong>Bifoga mallar</strong>: Tillåter användare att bifoga mallar till ett projekt efter att projektet har markerats som Fullständigt eller Dölj.</p> <p>Det här alternativet gäller inte projekt som väntar på godkännande.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
