---
content-type: overview
product-area: projects
navigation-topic: financials
title: Översikt över fakturering och intäkt
description: Som projektledare kan du använda faktureringstariffer för att få intäkter från dina projekt.
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# Översikt över fakturering och intäkt

Som projektledare kan du använda faktureringstariffer för att få intäkter från dina projekt.

I den här artikeln beskrivs hur du spårar intäkter för projekt. Intäkterna beräknas på olika sätt i utnyttjanderapporten. Information om intäktsberäkningar i användningsrapporten finns i [Visa information om resursutnyttjande](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Översikt över faktureringspriser

Tänk på följande när du arbetar med faktureringstaxor:

* Du behöver en avtalslicens med Redigera åtkomst till finansiella data för att kunna hantera faktureringstaxor.\
   Mer information om att bevilja åtkomst till finansiella data finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Faktureringstariffer är intäkter per arbetsenhet som är kopplad till jobbroller eller användare.

   Om du multiplicerar hastigheten med timmarna du lagt ned på arbetet genereras intäkter för dina projekt.

* När du har fastställt dina faktureringstariffer kan du sedan spåra intäkterna genom att skapa faktureringsposter som registrerar vad som har och inte har fakturerats.

   >[!TIP]
   >
   >När du markerar en faktureringspost som Fakturerad kan den aldrig redigeras. Detta är viktigt när priset varierar och du vill låsa intäkt- och utgiftsinformationen för projektet. Om du lägger till den i en faktureringspost och markerar den som Fakturerad uppdateras den inte när tarifferna uppdateras i ditt system.

   Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

* Du kan skapa faktureringstaxor för användare, jobbroller eller så kan du ha en engångsavgift för ett projekt eller en uppgift.

>[!IMPORTANT]
>
>Kurserna som beräknar intäkten tillhör användaren som loggar tiden eller deras jobbroller.

* [Faktureringstaxor för användare](#user-billing-rates)
* [Faktureringshastigheter för jobbroll](#job-role-billing-rates)
* [Fasta faktureringspriser för projekt eller uppgifter](#fixed-billing-rates-for-projects-or-tasks)
* [Åsidosätt faktureringstariffer](#override-billing-rates)

### Faktureringstaxor för användare {#user-billing-rates}

När du skapar en användare som användaradministratör kan du associera dem med en faktureringstakt genom att ange ett värde för fältet Fakturering per timme i profilen.\
Mer information om hur du skapar användare finns i artikeln [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### Faktureringshastigheter för jobbroll {#job-role-billing-rates}

När du skapar en jobbroll som Adobe Workfront-administratör kan du associera den med en faktureringstakt genom att ange ett värde för fältet Fakturering/Timme.

Du kan definiera värdet för faktureringssatsen för en jobbroll med hjälp av basvalutan i ditt Workfront-system eller med en annan anpassad valuta.

Mer information om hur du skapar jobbroller och åsidosätter deras valutor finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### Fasta faktureringspriser för projekt eller uppgifter {#fixed-billing-rates-for-projects-or-tasks}

Utöver timtaxor för användare och jobbroller kan du även ha följande fasta faktureringstariffer:

* Fast belopp för fast timintäktstyp
* Fast belopp för intäktstyp med fast intäkt

Mer information om hur de fasta faktureringstarifferna används för att beräkna intäkter finns i [Översikt över intäktstyper för uppgifter](#overview-of-task-revenue-types).

### Åsidosätt faktureringstariffer {#override-billing-rates}

>[!IMPORTANT]
>
>Du kan åsidosätta faktureringstariffer som är kopplade till jobbroller. Du kan inte åsidosätta användarfaktureringstaxor eller fasta taxor.

Du kan åsidosätta faktureringstaxor för jobbroller för:

* Ett specifikt företag

   Mer information om hur du skapar faktureringstaxor för jobbroller för ett företag finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Ett specifikt projekt

   Mer information om hur du skapar faktureringstariffer för jobbroller för ett projekt finns i artikeln [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Spåra intäktsbelopp

Workfront kan automatiskt spåra planerade intäkter när uppgifter skapas baserat på aktiviteternas planerade timmar.

Den kan också automatiskt spåra faktiska intäkter när faktiska timmar är inloggade på uppgifter, ärenden och projektet.

I följande tabell visas vilka typer av intäkter som är associerade med uppgifter, utgåvor och projekt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planerad intäkt</td> 
   <td> <p>För uppgifter är detta den intäkt som är kopplad till de planerade timmarna för uppgifter. Planerade timmar från alla uppgifter räknas upp till planerade timmar för projektet för att bidra till beräkningen av projektets planerade timmar. </p> <p>Mer information om planerade timmar i Workfront finns i <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Översikt över planerade timmar</a>. </p> <p>Workfront beräknar planerade intäkter för uppgifter och projekt med hjälp av följande formler:</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>ANMÄRKNING</b>

<p>Projektets planerade inkomster som visas i området Projektinformation och i projektrapporter skiljer sig från den planerade intäkten som visas i användningsrapporten. </p> <p>Den planerade intäkten i området Projektinformation återspeglar uppgiftsintäkten som är kopplad till aktiviteten Planerade timmar samt projektets fasta intäkt. Planerad intäkt i användningsrapporten visar planerad intäkt som bara är associerad med de planerade timmarna från aktivitetstilldelningarna i projektet. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Om projektet har 1 uppgift med 10 timmar, som tilldelats en konsult med en timtaxa på 20 USD och projektet har en fast intäkt på 100 USD, visar användningsrapporten 200 USD för planerad intäkt (den planerade intäkten som är associerad med timmarna för uppgiften). I avsnittet Projektinformation visas $300 (den planerade intäkten från aktiviteten och den fasta intäkten för projektet). </p> 
     </div> </p> <p>Uppgiftsplanerad intäkt beräknas med hjälp av timtaxan för fakturering för användare eller jobbroller som är tilldelade till aktiviteterna. Inkomsttypen för aktiviteterna påverkar vilken tariff (användare eller roll) som används för att beräkna planerad intäkt. Mer information finns i följande avsnitt i den här artikeln:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Översikt över intäktstyper för uppgifter</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Intäktsberäkningar för uppgifter som baseras på användar- och rolltilldelningar</a> </p> </li> 
    </ul> <p>Information om beräkningar av planerade intäkter i användningsrapporten finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visa information om resursutnyttjande </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Faktisk intäkt*</td> 
   <td> <p>Associerat med de faktiska timmarna för uppgifter, utgåvor och projekt. </p> <p>I allmänhet beräknas Faktiska intäkter i Workfront enligt följande formel:</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>Information om faktiska intäktsberäkningar i användningsrapporten finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visa information om resursutnyttjande </a>. </p> <p><b>TIPS</b>

Du kan inte visa Faktisk intäkt på utleveransnivå, men intäkterna som är kopplade till Faktiska timmar i problemen bidrar till projektets faktiska intäkt. </p> </td>
</tr> 
 </tbody> 
</table>

*För faktiska timmar avser användarens priser alltid den användare som loggar timmarna eller antalet jobbroller. Information om när Workfront använder användarsiffrorna och när de använder sina jobbroller finns i [Intäktsberäkningar](#revenue-calculations) i den här artikeln.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Om en uppgift med Inkomsttyp för användartimme till exempel planeras ta 2 timmar och användaren som är tilldelad till den har en timkostnad på 30 USD per timme, är aktivitetens planerade intäkt 60 USD. När uppgiften är slutförd och användaren bara loggar 1,5 timmar som den faktiska tid som har ägnats åt att slutföra uppgiften, är det faktiska intäktsbeloppet 45 USD. Om en annan användare som inte är tilldelad till uppgiften loggar tiden beräknas den faktiska intäkten utifrån användarens faktureringstariffer.

Du kan registrera intäkter på följande sätt:

* Genom att definiera intäktstypen för dina uppgifter och associera användare eller roller som tilldelats till arbetsobjekt med faktureringstariffer. Detta beräknar intäkten med beloppet för planerade eller faktiska timmar för arbetsposterna. Du kan ange ett tak till det högsta belopp som debiteras för timtaxor, eller inte.\
   Mer information om hur du anger en uppgifts intäktstyp finns i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Genom att fakturera en fast intäktsnivå för aktiviteter eller projekt.\
   Om du har uppgifter med Fast intäkt läggs beloppet för Fast intäkt till som planerad intäkt för en aktivitet eller ett projekt, och den planerade intäkten för en aktivitet blir tillgänglig att läggas till i en faktureringspost som fast intäkt.
* Genom att ställa in en fast faktureringsnivå för fasta intäkter för ett projekt och sedan ställa in timtaxor för aktiviteterna i projektet. Workfront lägger till timtaxorna för uppgifterna i projektets schablonbelopp.\
   En mekaniker som använder Workfront kan till exempel ange en kostnad för delar som fasta intäkter för projektet och sedan fakturera timvis för den tid som går åt till att reparera en bil. Fast intäkt för projekt eller uppgifter realiseras sedan när de har slutförts.

Du kan också markera dina uppgifter som&quot;Inte fakturerbar&quot;, vilket innebär att det inte finns någon planerad eller faktisk intäkt kopplad till dem.

## Översikt över intäktstyper för uppgifter {#overview-of-task-revenue-types}

Som standard anges Intäktstypen för alla nya uppgifter i enlighet med de inställningar för Aktivitet och problem som du har angett av Workfront- eller gruppadministratören.\
Mer information om hur du definierar inställningar för åtgärder och problem för din Workfront-instans finns i artikeln [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Projektägaren kan ändra aktiviteternas intäktstyp och Fast intäkt för projekt.\
Mer information om hur du anger fasta intäkter för ett projekt finns i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).\
Mer information om hur du anger en uppgifts intäktstyp finns i artikeln [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Du kan använda följande intäktstyper för dina uppgifter eller projekt:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Intäktstyp</strong> </p> </th> 
   <th> <p><strong>Beskrivning</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Fast intäkt</p> </td> 
   <td> <p>Den här typen kan användas med projekt och uppgifter. </p> <p>När du kopplar en mall till ett projekt läggs den fasta intäkten från mallen till projektets fasta intäkt. Mer information finns i <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Översikt över att bifoga en mall till ett projekt</a>. </p> <p>För uppgifter beräknas alltid aktivitetens intäkt, oavsett aktivitetstilldelningar, med det fasta belopp som har angetts för uppgiften. </p> <p>Fasta intäkter från underordnade uppgifter summeras till intäkten för den överordnade aktiviteten och sedan till intäkterna för projektet. Om ett fast belopp definieras för den överordnade aktiviteten och/eller projektet läggs beloppet till i den planerade intäkten som samlas in från underordnade aktiviteter.</p> <p>Beloppet för fasta intäkter för uppgifter kan inkluderas i en faktureringspost i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användare per timme</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter. </p> <p>Den faktureringsfrekvens som du anger för en viss användare multiplicerad med antalet planerade timmar för den uppgiften blir uppgiftens planerade intäktsbelopp. Den faktureringsfrekvens som du anger för en viss användare multiplicerad med antalet timmar som användaren loggar mot uppgiften är uppgiftens faktiska intäktsbelopp. <br>Om du till exempel skapar en användare och anger $20 för fältet Fakturering per timme, och användaren skickar 5 timmar för en uppgift på tidrapporten, blir aktivitetens faktiska faktureringsbelopp $100.</p> <p><b>TIPS</b>

Det här är standardintäktstypen när du skapar en uppgift.</p> </td>
</tr> 
  <tr> 
   <td> <p>Roll timvis</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter.</p> <p>Den här typen liknar Användare per timme, men använder jobbrollfrekvenser i stället för användarfrekvenser.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användare per timme med ändpunkt</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter.</p> <p>Aktiviteter faktureras varje timme som användaren anger, men de har ett maxbelopp som du kan ange. <br>Om en användares faktureringsfrekvens till exempel är $25, men aktivitetens beloppsgräns är $20, och användaren loggar en timme, är aktivitetens faktiska intäkt $20. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Roll timvis med ändpunkt</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter.</p> <p>Den här typen liknar Användare per timme med Ände men använder jobbrollfrekvenser i stället för användarfrekvenser. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Användarens timma plus fast</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter. </p> <p>Aktiviteter faktureras varje timme som användaren använder per timme, men har ett fast belopp som du kan lägga till i användarpriset. Det fasta belopp som har angetts för aktiviteten kan inkluderas i faktureringsposter för projektet. Det fasta beloppet multipliceras inte med timmarna för aktiviteten. Endast användarens faktureringstaxa gör det. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Roll timvis plus fast</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter. </p> <p>Aktiviteter faktureras timvis som i rolltimmen, men har ett ytterligare fast belopp som du kan lägga till i rollfrekvensen. Det fasta belopp som har angetts för aktiviteten kan inkluderas i faktureringsposter för projektet. Det fasta beloppet multipliceras inte med timmarna för aktiviteten. Endast faktureringssatsen för jobbrollen gör det. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fast en timme</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter.</p> <p>Det tak eller fasta belopp som du anger för uppgiften multiplicerat med antalet timmar som anges för uppgiften (oavsett användare eller deras jobbroller) är faktureringsbeloppet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ej fakturerbar</p> </td> 
   <td> <p>Den här typen kan bara användas för uppgifter.</p> <p>Denna intäktstyp påverkar inte intäkterna. </p> <p>Om ett överordnat objekt har den här inställningen kommer underordnade uppgifter med en faktureringstyp fortfarande att gälla som vanligt.</p> <p>När en användare utan åtkomst till ekonomiska data eller en användare utan ekonomisk behörighet för en mall skapar ett projekt från den mallen, är det här standardintäktstypen för aktiviteterna i projektet.</p> <p>Mer information om åtkomst till finansiella data finns i artikeln <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till finansiella uppgifter</a>.<br>Mer information om objektbehörigheter finns i artikeln <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.<br>Mer information om hur du skapar projekt från mallar finns i artikeln <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Skapa ett projekt med en mall</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Översikt över intäkt för överordnade uppgifter

Om du ändrar en fristående uppgift med faktureringsinformation för den till en överordnad aktivitet, behåller den nya överordnade aktiviteten all faktureringsinformation som tidigare använts, tillsammans med de timmar som tidigare använts. Faktureringsinformation som kommer från timmar som loggats till de underordnade uppgifterna kommer att samlas in som Faktisk intäkt till den nya överordnade uppgiften.

Den planerade intäkten från de underordnade aktiviteterna sammanställs också med den överordnade aktiviteten.

## Översikt över intäkt för utleveranser

Ärenden har inga belopp för Planerad eller Faktisk intäkt, men de kan ha Faktisk kostnad.

Om du loggar timmar för en utgåva och använder en timtyp som är markerad som &quot;Räkna som intäkt&quot;, beräknar Workfront ett verkligt kostnadsbelopp enligt hastigheten för den användare som loggar in på tiden. Det här numret läggs till projektets faktiska kostnad. Timmarna kan också inkluderas i en faktureringspost.

Mer information om att hålla reda på kostnaderna finns i artikeln [Spåra kostnader](../../../manage-work/projects/project-finances/track-costs.md).

Mer information om timtyper finns i artikeln [Hantera timtyper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Intäktsberäkningar

* [Intäktsberäkningar för uppgifter som baseras på användar- och rolltilldelningar](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Intäktsberäkningar för uppgifter som baseras på användar- och rolltilldelningar {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Tänk på följande när du beräknar intäkter för en aktivitet:

* Om en användare eller en jobbroll visar ett belopp på $0,00, läser Workfront det som ett giltigt belopp och multiplicerar beloppet med antalet timmar i aktiviteten för att beräkna intäkten. Om du inte vill visa någon intäkt för dina aktiviteter kontrollerar du att fältet för faktureringssatsen för användaren eller jobbrollen är tomt.
* När faktureringstariffer för jobbroller gäller, använder Workfront åsidosättningsfrekvensen på projektnivå i stället för faktureringstakten för den rollen som definieras på systemnivå varje gång det finns en åsidosättningsfrekvens för projektet.
* Om det finns flera tilldelningar för uppgifterna gäller scenarierna nedan för varje tilldelad.

Det finns en hierarki som du använder för intäktsberäkningar baserat på uppgiftstilldelningar.

Om Workfront-administratören har aktiverat **Tilldela jobbroller till timposter manuellt** inställning i området Inställningar för tidrapporter och timmar, och användarens loggningstid i projektet väljer en annan roll att associera med den här tiden, beräknar alltid aktivitetens eller projektets faktiska intäkt baserat på rollen som är associerad med timposten. Mer information om hur du aktiverar loggningstid för en viss jobbroll finns i artikeln [Inställningar för tidrapport och timme](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Följande scenarier används för att beräkna aktivitetsinkomster baserat på intäktstyp och aktivitetstilldelningens typ:

* **Uppgiftens intäktstyp är Användd timme**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Fakturering per timtariff</td> 
     <td>Ingen tilldelning</td> 
     <td>Användartilldelning</td> 
     <td>Tilldelning av jobbroll</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fakturering per timma för planerad intäkt</td> 
     <td>$0.00</td> 
     <td> Om en användare har en faktureringstaxa i sin profil används den taxan för att beräkna planerad intäkt. I annat fall används systemets faktureringsfrekvens för den primära jobbrollen. <br><p><b>ANMÄRKNING</b>  Användaren kan tilldelas till uppgiften med en av de sekundära jobbrollerna, men i stället används den primära jobbrollens hastighet här.</p></td> 
     <td>Systemfaktureringssatsen för den jobbroll som tilldelats uppgiften används för att beräkna planerad intäkt. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fakturering per timtariff för faktisk intäkt</td> 
     <td>Om användaren som loggar timmarna har en faktureringsfrekvens i sin profil används den taxan. <br>I annat fall används faktureringsfrekvensen för deras primära jobbroll. Om det inte finns någon faktureringstaxa som är associerad med användaren eller dennes primära roll är den faktiska intäkten 0,00 USD. <br><p><b>ANMÄRKNING</b>

   Endast de frekvenser som är associerade med användaren som loggar tiden tas med i beräkningen, även när en annan användare tilldelas till uppgiften.</p></td>
   <td>Om användaren som loggar timmarna har en faktureringsfrekvens i sin profil används den taxan. <br>I annat fall används faktureringsfrekvensen för deras primära jobbroll. Om det inte finns någon faktureringstaxa som är associerad med användaren eller dennes primära roll är den faktiska intäkten 0,00 USD. <br><p><b>ANMÄRKNING</b>

   Endast de frekvenser som är associerade med användaren som loggar tiden tas med i beräkningen, även när en annan användare tilldelas till uppgiften.</p></td>
   <td>Om användaren som loggar timmarna har en faktureringsfrekvens i sin profil används den taxan. I annat fall används faktureringsfrekvensen för deras primära jobbroll.<br><p><b>ANMÄRKNING</b>

   Om användarens loggningstid inte har någon associerad faktureringsfrekvens, och de inte har någon jobbroll eller någon faktureringsfrekvens för sin jobbroll, används avgiften från den jobbroll som är associerad med uppgiften. Om det inte finns någon faktureringstaxa för den här rollen är intäkterna 0,00 USD</p></td>
   </tr> 
   </tbody> 
  </table>

* **Uppgiftens intäktstyp är roll per timme**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Fakturering per timtariff</td> 
     <td>Ingen tilldelning</td> 
     <td>Användartilldelning</td> 
     <td>Tilldelning av jobbroll</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fakturering per timma för planerad intäkt</td> 
     <td>$0.00</td> 
     <td>Workfront tittar på den jobbroll som användaren utför för uppgiften att beräkna den planerade intäkten. <br>Om användaren inte är associerad med någon roll för uppgiften är Intäkterna $0,00. </td> 
     <td>Faktureringsfrekvensen för den jobbroll som tilldelats uppgiften används för att beräkna planerad intäkt.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fakturering per timtariff för faktisk intäkt</td> 
     <td>Workfront använder faktureringsfrekvensen för den primära jobbrollen för användaren som loggar tiden. <br>Om användaren som loggar tiden inte har någon jobbroll associerad med dem, eller om den primära jobbrollen inte har någon faktureringsfrekvens, är den faktiska intäkten 0,00 USD. </td> 
     <td> Om användaren som loggar tiden är tilldelad uppgiften, används faktureringssatsen för den jobbroll som är associerad med användaren för uppgiften för att beräkna den faktiska intäkten. I annat fall används faktureringsfrekvensen för deras primära jobbroll. Om användaren inte har någon primär jobbroll eller om deras primära jobbroll inte har någon faktureringsfrekvens, är Faktisk intäkt $0,00. </td> 
     <td>Om en av jobbrollerna för användaren som loggar tiden är tilldelad uppgiften, används den jobbrollfrekvensen. Om den jobbroll som är tilldelad uppgiften inte är associerad med användaren som loggar tiden, används faktureringssatsen för användarens primära roll för att beräkna den faktiska intäkten. Om användaren inte har någon jobbroll eller om ingen hastighet är associerad med den primära jobbrollen, används den jobbroll som tilldelats uppgiften. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Intäktsberäkningar för projekt

Du kan spåra följande intäktstyper för projekt:

* Planerad intäkt för ett projekt beräknas enligt följande formel:

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   Information om hur planerad intäkt beräknas för aktiviteten finns i [Intäktsberäkningar för uppgifter som baseras på användar- och rolltilldelningar](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) i den här artikeln.

* Faktisk intäkt för ett projekt beräknas med följande formel:

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

Information om hur aktiviteten Faktisk intäkt beräknas finns i [Intäktsberäkningar för uppgifter som baseras på användar- och rolltilldelningar](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) i den här artikeln.

För den faktiska intäkt som är associerad med de timmar som är loggade direkt till projektet eller problemen, använder Workfront faktureringshastigheten för den användare som loggar tiden i projektet. Om användaren inte har någon faktureringstakt kopplad till sin profil använder Workfront faktureringstakten för sin primära roll. Om båda tarifferna är noll är den faktiska intäkt som är associerad med de timmar som är loggade i projektet eller utställningarna noll.
