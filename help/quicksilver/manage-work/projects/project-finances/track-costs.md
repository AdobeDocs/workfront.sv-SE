---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Spåra kostnader
description: Du kan spåra kostnader för projekt, uppgifter och problem i Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 23a5c90b9321b72a20f21752f957b3be0a9f3a02
workflow-type: tm+mt
source-wordcount: '2499'
ht-degree: 0%

---

# Spåra kostnader

<!-- Audited: 02/2024 -->

Du kan spåra kostnader för projekt, uppgifter och problem i Adobe Workfront.

## Hur Workfront beräknar kostnader

För att hålla reda på kostnaderna måste du koppla användare och jobbroller till timkostnadstariffer.

Kostnadsnivåer per timme är belopp för kostnader per arbetsenhet som är kopplad till jobbroller eller användare. Om du multiplicerar hastigheten med timmarna du lagt ned på arbetet genereras kostnader för dina projekt, uppgifter eller utgåvor.

Följande scenarier finns:

* Om kostnadstypen för dina uppgifter är Användare per timme, beräknar användaren kostnaderna för uppgiften och projektet per timme.

  Mer information om hur du associerar användare med kostnadstariffer finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Om kostnadstypen för dina aktiviteter är Roll-timme, beräknar timpriset för jobbrollen för att beräkna uppgifts- och projektkostnaderna.

  Mer information om hur du associerar jobbroller med kostnadstariffer finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront beräknar endast faktisk kostnad för utleveranser, och utleveranser saknar kostnadstyp. Mer information finns i avsnittet [Hur Workfront spårar kostnader för problem](#how-workfront-tracks-costs-for-issues) i den här artikeln.

>[!TIP]
>
>Du kan inte åsidosätta kostnadstariffer för projekt. När du har fastställt kostnaden per timme för en användare eller en jobbroll, beräknas alla kostnader i systemet med den taxan.

## Workfront kostnadsprestandaindex

Workfront beräknar ett antal kostnadsprestandaindex för projekt så att projekten kan spåras för kostnadseffektivitet.\
Mer information om hur du beräknar kostnadsprestandaindex finns i:

* [Beräkna index för kostnadsprestanda (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Beräkna prestanda för kostnadsschema (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Beräkna SPI (Schedule Performance Index)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Hur Workfront spårar kostnader för uppgifter och projekt

Typerna av kostnader beräknas på olika sätt för aktiviteter och projekt.

### Hur Workfront spårar kostnader {#how-workfront-tracks-costs}

Du kan spåra olika typer av kostnader för uppgifter och projekt i Workfront. De totala kostnaderna beräknas enligt följande formel:

`Costs = Labor Costs + Expense Costs`

* **Arbetskostnaden** är associerad med timarna för aktiviteter och projekt samt timkostnaden för resurser som är associerade med aktiviteter. I allmänhet beräknas följande arbetskostnader av Workfront:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Planerade arbetskostnader</td> 
     <td> <p>De beräknas med följande formel:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Budgeterade arbetskostnader</td> 
     <td> <p>De beräknas med följande formel:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Faktiska arbetskostnader</td> 
     <td> <p>De beräknas med följande formel:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> 
     <p><strong>OBS!</strong>
     <p>Workfront beräknar den faktiska arbetskostnaden med hjälp av de gamla faktiska timmarna. Mer information finns i <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Visa faktiska timmar</a>. </p>

  </td> 
    </tr> 
   </tbody> 
  </table>

  Mer information finns i avsnittet [Hur Workfront beräknar planerade, budgeterade och faktiska kostnader](#how-workfront-calculates-planned-budgeted-and-actual-costs) i den här artikeln.

* **Utgiftskostnader** är associerade med utgifter för projekt och aktiviteter.\
  När du skapar ett projekt kan du ange planerade utgifter för hela projektet. Dessutom kan du associera utgifter med nya eller befintliga uppgifter. Mer information finns i [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Fasta kostnader** definieras som ett fast kostnadsbelopp för ett projekt. Detta är en del av den planerade kostnaden för projektet, som representerar den summa pengar som du behöver för att slutföra projektet.

  >[!TIP]
  >
  >När du kopplar en mall till ett projekt läggs den fasta kostnaden för en mall till projektets fasta kostnad. Mer information finns i [Översikt över hur du bifogar en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Hur Workfront beräknar planerade, budgeterade och faktiska kostnader {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront beräknar den planerade kostnaden och den faktiska kostnaden för varje enskild aktivitet i ett projekt. Workfront använder dessa beräkningar för enskilda uppgifter för att beräkna den planerade kostnaden och den faktiska kostnaden för projektet.

#### Planerad kostnad {#planned-cost}

Den planerade kostnaden för ett projekt är kostnaden som är associerad med det planerade arbetet (Planerade timmar) i projektet.

Den planerade kostnaden för ett projekt beräknas enligt följande formel:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Du har till exempel följande utgifter på fliken Utgifter för en uppgift: en marknadsföringsutgift på 100 USD och en administrativ utgift på 50 USD. På fliken Ekonomi väljer du kostnadstypen Användare per timme. En användare tilldelas uppgiften och användarens timtaxa är 15 USD. Användaren har tilldelats 5 timmar att arbeta med den här uppgiften. På fliken Utgifter i projektet har du en planerad kostnad på 100 USD för en utgift som kallas Konsult. Du har också en fast kostnad på 200 USD för projektet.

Projektets planerade kostnad beräknas enligt följande:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

Timtaxan i formeln tar hänsyn till eventuella faktiska datumändringar av räntesatsen.

#### Budgeterad kostnad {#budgeted-cost}

Budgeterad kostnad för ett projekt är kostnaden som är associerad med det budgeterade arbetet (Budgeterade timmar) för projektet.

Den budgeterade kostnaden för projektet är densamma som den planerade kostnaden för projektet om följande två villkor uppfylls:

* De planerade timmarna för aktiviteterna i projektet matchar de budgeterade timmarna (i resursplaneraren).
* Faktureringstypen för aktiviteterna är Roll timme.

Projektets budgeterade kostnad beräknas med hjälp av formeln nedan om följande villkor uppfylls:

* De planerade timmarna för aktiviteterna i projektet matchar inte de budgeterade timmarna (i resursplaneraren).
* Faktureringstypen för aktiviteterna är Roll timme.

När ovanstående villkor är uppfyllda beräknar Workfront den budgeterade kostnaden för projektet med följande formel:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Faktisk kostnad {#actual-cost}

Den faktiska kostnaden för ett projekt är kostnaden som är associerad med det faktiska arbetet (timmar som är loggade) i projektet.

Faktisk kostnad beräknas med följande formel:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Du har till exempel följande utgifter på fliken Utgifter för en uppgift: en marknadsföringsutgift med en faktisk kostnad på 110 USD och en administrativ utgift med en faktisk kostnad på 40 USD. Du väljer kostnadstypen Roll per timme och tilldelar rollen Konsultjobb till uppgiften. Rollen för konsultjobbet är 15 USD per timme och uppgiften för konsultföretagets jobbroll är 6 timmar inloggad. Det finns en utgift för konsulttjänster som är associerad med projektet (på fliken Utgifter), med en faktisk kostnad på 100 USD och en användare med en kostnad per timme på 20 USD i användarprofilen loggar 10 timmar på projektet. Du har också en fast kostnad på 200 USD för projektet.

Projektets faktiska kostnad beräknas enligt följande:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

Timtaxan i formeln tar hänsyn till eventuella faktiska datumändringar av räntesatsen.

>[!NOTE]
>
>Projektets faktiska utgiftskostnad beräknas enligt följande:
>&#x200B;>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Dessa kostnader dupliceras inte i den faktiska kostnadsberäkningen. Om till exempel en fast kostnad är en del av projektets faktiska utgiftskostnad, läggs den inte till separat i den faktiska kostnaden.

>[!NOTE]
>
>När du loggar tid för ett projekt finns följande scenarier när du beräknar faktisk arbetskostnad för projektet:
>
>* Som standard använder Workfront användarens kostnad per timme för att beräkna den faktiska arbetskostnaden.
>* Om användaren som loggar tiden inte är kopplad till någon kostnad, använder Workfront priset per timme för användarens primära roll.
>* Om din Workfront-administratör har aktiverat inställningen **Tilldela jobbroller till timposter manuellt** i Inställningar för tidrapporter och timmar i installationsprogrammet, och inloggningstiden för projektet väljer en annan roll att associera med den här tiden, beräknas projektets faktiska kostnad baserat på den roll som angavs när timmarna loggades. Mer information om hur du aktiverar loggningstid för en viss jobbroll finns i artikeln [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Hur Workfront beräknar kostnadstyper för uppgifter {#how-workfront-calculates-cost-types-for-tasks}

Den planerade och faktiska kostnaden för aktiviteterna och deras arbetskostnader bestäms av kostnadstypen för varje uppgift.

Du kan konfigurera kostnadstypen för enskilda uppgifter i projektet. Varje kostnadstyp påverkar värdena för Planerad kostnad och Verklig kostnad.

Mer information om hur du ändrar kostnadstypen för en aktivitet finns i [Uppdatera uppgiftens kostnadstyp](../../../manage-work/tasks/task-information/update-task-cost-type.md).

I följande tabell beskrivs de tillgängliga kostnadstyperna för uppgifter i Workfront:

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Aktivitetskostnadstyp</strong> </p> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>Användare per timme</p> </td> 
   <td> <p>Det här är standardkostnadstypen när du skapar en uppgift.</p> <p><strong>Planerad kostnad</strong> beräknas med följande formel: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Om den planerade arbetskostnaden beräknas enligt följande:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Obs! <p>Tänk på följande effekter när du använder användarens timkostnadstyp och beräknar planerad kostnad:</p> 
     <ul> 
      <li>Om du tilldelar flera resurser till en aktivitet, justerar Workfront beräkningarna för Planerad kostnad baserat på procentandelen av uppgiften som tilldelats varje resurs.</li>
      <li>För datumfaktiska kostnadstariffer är den planerade arbetskostnaden summan av de planerade kostnaderna för varje tidsperiod som omfattas av uppgiften.</li>
      <li>Värdet i fältet Planerad kostnad kan variera beroende på om du visar den planerade kostnaden från själva aktiviteten eller från användningsrapporten.<br><strong>När du visar planerad kostnad från själva aktiviteten:</strong> Fältet Planerad kostnad tar hänsyn till fältet Kostnad/tim som angetts på jobbrollnivå (när fältet Kostnad/tim inte har angetts på användarnivå).<br><strong>När du visar planerad kostnad från användningsrapporten för projektet:</strong> Fältet Planerad kostnad tar inte hänsyn till fältet Kostnad/tim som angetts på jobbrollnivå. Om du i stället vill att fältet Kostnad/timme som angetts på jobbrollsnivån ska beaktas i användningsrapporten, måste du ange uppgiftens kostnadstyp till Roll timme. </li> 
     </ul> </p> <p><strong>Faktisk kostnad</strong> beräknas med följande formel: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Om den faktiska arbetskostnaden beräknas med</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>En användare har till exempel en kostnad per timme på $20 i sin profil. När de loggar 5 timmar för en uppgift är den faktiska arbetskostnaden 100 USD för den uppgiften. Om användaren inte har någon kostnad per timme som är kopplad till sig, beräknas den faktiska kostnaden utifrån kostnaden per timme för den primära rollen. Om de inte har någon jobbroll eller om Kostnad per timme inte har definierats för sin jobbroll är den faktiska kostnaden för aktiviteten noll. </p> <p>Obs! Faktiska kostnader beräknas baserat på kostnaden per timme för den användare som loggar tiden, oavsett vem som tilldelats uppgiften. Dessutom tar timtaxan för fakturering i formeln hänsyn till eventuella datumändringar i räntesatsen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Roll timvis</p> </td>
   <td> <p><strong>Planerad kostnad</strong> beräknas med följande formel: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Där den planerade arbetskostnaden beräknas av:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Obs! Om du tilldelar flera resurser till en aktivitet, justerar Workfront beräkningarna för Planerade timmar baserat på procentandelen av uppgiften som tilldelats varje resurs. Dessutom tar timtaxan i formeln hänsyn till eventuella faktiska datumändringar av räntesatsen.</p> <p><strong>Faktisk kostnad</strong> beräknas med följande formel: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Där den faktiska arbetskostnaden för aktiviteten beräknas av:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>En uppgift tilldelas till exempel en jobbroll eller en användare med en jobbroll där kostnaden per timme är 20 USD. När en användare loggar 5 timmar för en uppgift är den faktiska arbetskostnaden 100 USD för den uppgiften. Om användaren som är tilldelad till uppgiften inte har någon jobbroll kopplad till sig för aktiviteten, beräknas den faktiska kostnaden baserat på kostnaden per timme för den primära rollen. Om de inte har någon jobbroll eller om Kostnad per timme inte har definierats för sin jobbroll är den faktiska kostnaden för aktiviteten noll. </p> <p>Obs! De faktiska timmarna för en roll-timtauppgift beräknas baserat på jobbrollerna för de användare som är associerade med uppgiften, inte på rollerna som är kopplade till den användare som loggar tiden. Dessutom tar timtaxan för fakturering i formeln hänsyn till eventuella datumändringar i räntesatsen.</p> <p>Om din Workfront-administratör har aktiverat inställningen <strong>Tilldela jobbroller till timposter manuellt</strong> i Inställningar för tidrapporter och timmar i Inställningar, och inloggningstiden för aktiviteten väljer en annan roll att associera med den här tiden, beräknas den faktiska kostnaden för en roll-timme baserat på den roll som angavs när timmarna loggades. Mer information om hur du aktiverar loggningstid för en viss jobbroll finns i artikeln <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Konfigurera tidrapport och timinställningar</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fast en timme</p> </td> 
   <td> <p><strong>Planerad kostnad</strong> beräknas med följande formel:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Där arbetskostnaden för aktiviteten beräknas av:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Faktisk kostnad</strong> beräknas med följande formel: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Där den faktiska arbetskostnaden för aktiviteten beräknas av:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Den här kostnadstypen tar inte hänsyn till enskilda användare eller jobbroller.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ingen kostnad</p> </td> 
   <td> <p>Kostnadstypen påverkar inte kostnaderna. Om en överordnad aktivitet har den här kostnadstypen, beräknas underaktiviteter med en annan kostnadstyp utifrån deras individuella kostnadstyper, och kostnaden för den överordnade aktiviteten påverkas i enlighet med detta. </p> <p>När en användare utan åtkomst till ekonomiska data eller en användare utan ekonomisk behörighet för en mall skapar ett projekt från den mallen, är det här standardkostnadstypen för aktiviteterna i projektet.</p> <p>Mer information om åtkomst till finansiella data finns i artikeln <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till ekonomiska data</a>.</p> <p>Mer information om objektbehörigheter finns i artikeln <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Dela ekonomiska behörigheter för ett objekt</a>.</p> <p>Mer information om hur du skapar projekt från mallar finns i artikeln <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Skapa ett projekt med en mall</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Hur Workfront håller reda på kostnaderna för olika problem {#how-workfront-tracks-costs-for-issues}

Problem har inte, och påverkar inte, följande typer av kostnader för ett projekt:

* Planerad kostnad
* Budgeterad kostnad

Problem kan dock ha en **faktisk kostnad**, vilket även påverkar projektets faktiska kostnad.

I följande tabell beskrivs hur Faktisk kostnad beräknas för utgåvor, beroende på vilken typ av tilldelning det gäller:

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>Användartilldelning</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Faktisk kostnad</strong> beräknas med följande formel:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Kostnaden per timme för den användare som loggar tiden räknas här, oavsett vem som är tilldelad problemet. </p> <p>Om användaren som loggar tiden inte har en kostnad per timme i sin profil, beräknar kostnaden per timme för den primära rollen för jobbet den faktiska kostnaden för utgåvan.</p> <p>Om användaren som loggar tiden inte har någon roll i sin profil eller inget värde som är kopplat till den, beräknas de faktiska timmarna med hjälp av kostnaden per timme för den primära rollen för jobbet för den primära personen i ärendet. Om den rollen inte har någon definierad tariff är den faktiska kostnaden för utleveransen noll. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rolltilldelning</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Faktisk kostnad</strong> beräknas med följande formel:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Kostnaden per timme för användaren som loggar tiden för ett problem beaktas här, oavsett vilken roll som är tilldelad problemet. </p> <p>Om användaren som loggar tiden inte har någon kostnad per timme som är associerad med dem, beräknar kostnaden per timme för deras primära roll den faktiska kostnaden för utgåvan.</p><p>Om användaren som loggar tiden inte har någon roll i sin profil eller inget värde är associerat med den, är den faktiska kostnaden för problemet noll. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ingen tilldelning</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Faktisk kostnad</strong> beräknas med följande formel:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Om användaren som loggar tiden inte har en kostnad per timme som är associerad med profilen, beräknar kostnaden per timme för den primära rollen för jobbet den faktiska kostnaden för utgåvan. </p> <p>Om användaren som loggar tiden inte har någon jobbroll kopplad till sin profil eller om rollen för primärt jobb inte har en definierad kostnad per timme, är den faktiska kostnaden för problemet noll. </p> </td> 
  </tr> 
 </tbody> 
</table>
