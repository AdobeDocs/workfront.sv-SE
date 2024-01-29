---
title: Konfigurera inställningar för aktiviteter och utgåvor för en grupp
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupp,inställningar,aktivitet,problem,låsa upp
navigation-topic: create-and-manage-groups
description: Om grupper i din organisation måste konfigurera en uppgift eller en utgåva oberoende av hur den är konfigurerad på systemnivå, kan en Adobe Workfront-administratör låsa upp inställningen. Som gruppadministratör kan du sedan konfigurera inställningen för gruppen så att den påverkar alla uppgifter eller problem som är kopplade till gruppen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 0%

---

# Konfigurera inställningar för aktiviteter och utgåvor för en grupp

Om grupper i din organisation måste konfigurera en uppgift eller en utgåva oberoende av hur den är konfigurerad på systemnivå, kan en Adobe Workfront-administratör låsa upp inställningen. Som gruppadministratör kan du sedan konfigurera inställningen för gruppen så att den påverkar alla uppgifter eller problem som är kopplade till gruppen.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om hur Workfront-administratören låser upp inställningarna finns i [Låsa eller låsa upp projektinställningar för alla grupper i systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Konfiguration på gruppnivå är också möjligt för projektinställningar. Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalt förblir en olåst inställning olåst i oändlighet. Om Workfront-administratören låser om den aktiveras systeminställningen igen och inställningarna som gjorts av gruppadministratörerna går förlorade.
>* Inställningarna för gruppen som är kopplad till ett projekt har företräde framför inställningarna för hemgruppen för användaren som skapar projektet.
>* Vissa gruppnivåinställningar påverkar projektmallar som du skapar för gruppen. Mer information finns i avsnittet [Visa, arbeta med och skapa mallar för din grupp i området Grupper](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* När en Workfront-administratör har låst upp en inställning på systemnivå kan du konfigurera den och sedan låsa den så att alla i gruppen och dess undergrupper använder samma konfiguration. Detta är parallellt med möjligheten för en Workfront-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Låsa eller låsa upp ett projekt, en uppgift eller en utleverans för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

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

## Konfigurera olåsta uppgifter och utgivningsinställningar för en grupp på den översta nivån

>[!TIP]
>
>Om du är Workfront-administratör kan du kringgå steg 1-4 genom att gå till Inställningar > Projektinställningar > Åtgärder och problem och sedan söka efter gruppens namn i rutan längst upp på sidan.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på namnet på gruppen som du vill konfigurera olåsta uppgifter och utgivningsinställningar för.
1. På sidan som visas för gruppen klickar du på **Inställningar för aktivitet och problem**.
1. På sidan som visas fortsätter du med ett av de 5 avsnitten som anges nedan för att konfigurera inställningar för områdena Ny åtgärdsstandard, Problem, Borttagning, Faktiska datum och Åtkomst. Klicka sedan på **Spara**.

   Om du hovrar över låsikonen ![](assets/lock-toggle-button-dimmed.png) Om du vill ha en inställning som du måste konfigurera och ett verktygstips visas som anger att den är låst kan du be Workfront-administratören att låsa upp den för alla grupper i organisationen.

   När den är olåst kan du och andra gruppadministratörer konfigurera den separat för dina egna grupper. Du kan även låsa den för gruppen och alla undergrupper under gruppen.

   * [Nya standardinställningar för aktivitet](#new-task-defaults)
   * [Problem](#issues)
   * [Borttagning](#deletion)
   * [Faktiska datum](#actual-dates)

     <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Åtkomst](#access)

### Nya standardinställningar för aktivitet {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Startdatum för nya uppgifter</td> 
      <td> <p>Bestämmer standardstartdatumet för nya uppgifter för projektledare. Startdatumet för nya aktiviteter kan antingen vara det planerade startdatumet för projektet eller den dag då aktiviteten skapas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Varaktighetstyp </p> </td> 
      <td> <p>Bestämmer relationen mellan antalet resurser (och deras allokeringsprocent) och varaktigheten eller den totala ansträngningen för aktiviteten. Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Typer av varaktighet och varaktighet för aktivitet: artikelindex</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intäktstyp</td> 
      <td> <p>Beräknar planerade och faktiska intäktsuppskattningar för en aktivitet. När <strong>Intäktstyp</strong> är inställd på<strong>Ej fakturerbar</strong>, genererar de planerade timmarna och de faktiska registrerade timmarna ingen intäktsuppskattning för uppgiften och arbetet med uppgiften bidrar inte till intäkterna på projektnivå.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostnadstyp</td> 
      <td> <p>Beräknar planerade och faktiska kostnadsuppskattningar för en aktivitet. När inställt på <strong>Ingen kostnad</strong>, planerade timmar och registrerade timmar inte genererar en planerad eller faktisk kostnadsuppskattning för uppgiften, och arbetet med uppgiften bidrar inte till projektnivåkostnaderna.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problem {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Uppdatera automatiskt status för lösta problem när statusen för det lösta objektet ändras</td> 
      <td> <p>När någon konverterar ett problem till ett projekt eller en uppgift blir både det ursprungliga problemet och det konverterade projektet eller den konverterade aktiviteten objekt som löses. Med den här inställningen kan du korrelera upplösningen för det ursprungliga problemet med upplösningen för dess objekt som kan lösas. Mer information om hur du löser objekt finns i <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Översikt över objekt som kan lösas och lösas </a>.</p> <p>För att den här inställningen ska ha någon effekt kan du välja att <strong>Behåll det ursprungliga problemet och knyt lösningen till uppgiften</strong> måste väljas.</p> 
       <ul> 
        <li>När den här inställningen är aktiverad kan du skapa anpassade statusvärden med samma nyckel för både utgåvor, projekt och uppgifter. När projektet eller aktiviteten (som ett upplösningsbart objekt) blir en anpassad status, återspeglas ändringen även i problemets status. Statusnyckeln måste vara densamma för utleverans- och projekt- eller aktivitetsstatus.</li> 
        <li>När den här inställningen är inaktiverad ställs objektstatus automatiskt in på standardstatus i stället för de anpassade. Mer information om standardstatusvärdena finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Åtkomst till listan över status för systemproblem</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När ett problem konverteras till en uppgift</td> 
      <td> <p>Inställningarna i det här avsnittet avgör vad som händer under konverteringsprocessen från problem till uppgift:</p> 
       <ul> 
        <li><strong>Behåll det ursprungliga problemet och knyt lösningen till uppgiften</strong>: När du konverterar ett problem förblir det synligt som ett problem tills det är klart. Status för problemet ändras automatiskt till Stängd när uppgiften har slutförts.</li> 
        <li><strong>Tillåt att den primära kontakten har åtkomst till uppgiften</strong>: Ger den primära kontakten (den som skapat problemet) åtkomst till uppgiften för att granska den, göra uppdateringar och hålla dig informerad om hur den fortlöper</li> 
        <li> <p><strong>Tillåt att de här inställningarna ändras under konverteringen</strong>: Användare som konverterar problemet kan ändra dessa alternativ under konverteringen av ett problem till en aktivitet.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När ett problem konverteras till ett projekt</td> 
      <td> <p>Inställningarna i det här avsnittet avgör vad som händer under konverteringsprocessen från problem till projekt:</p> 
       <ul> 
        <li><strong>Behåll det ursprungliga problemet och knyt dess lösning till projektet</strong>: När du konverterar problemet förblir det synligt som ett problem tills projektet är klart. Status för problemet ändras automatiskt till Stängd när projektet har slutförts.</li> 
        <li><strong>Tillåt att primär kontakt har åtkomst till projektet</strong>: Ger den primära kontaktpersonen (den som skapat problemet) tillgång till projektet för att granska projektet, göra uppdateringar och hålla sig informerad om projektets förlopp.</li> 
        <li><strong>Tillåt att de här inställningarna ändras under konverteringen</strong>: Användare som konverterar problemet kan ändra de listade alternativen under konverteringen av en utgåva till ett projekt.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Borttagning {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tillåt användare att ta bort uppgifter och problem med loggade timmar</td> 
      <td> <p> Här kan du avgöra om du tillåter att uppgifter tas bort eller om frågor där timmar loggas. Det här alternativet är markerat som standard.</p> 
       <div> 
        <p><b>Tips</b>: Den här inställningen gäller även för att ta bort projekt som har uppgifter eller problem med timmar som är inloggade. Den här inställningen gäller inte för att ta bort projekt där tiden loggas direkt för projektet. </p> 
        <p>Tänk på följande:</p> 
        <ul> 
         <li> <p>När det är markerat får du en informativ varning när du tar bort en uppgift eller ett problem. Varningen påminner dig om att om aktiviteten eller problemet har loggat timmar kommer de antingen att flyttas till projektet eller tas bort. Du kan konfigurera om timmarna ska tas bort eller flyttas till projektet under Inställningar för tidrapport och timmar i inställningarna för inställningarna. När du har bekräftat att du har sett varningen tas uppgiften eller problemet bort. Mer information om hur du konfigurerar inställningar för tidrapport och timmar finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Konfigurera tidrapport och timinställningar</a>. </p> <p>Tips: <span>När du tar bort ett projekt med uppgifter och ärenden som har loggade timmar, tas de loggade timmarna bort eller så bevaras de enligt inställningarna i Inställningar för tidrapport och timmar i Inställningar</span>. </p> </li> 
         <li><span>När du avmarkerar det här alternativet får du en varning när du tar bort en uppgift eller ett problem med loggade timmar, eller när du tar bort ett projekt med timmar som loggats för dess uppgifter eller problem</span> <span>.</span> Varningen anger att administratören inte tillåter att uppgifter eller problem med loggade timmar tas bort. Aktiviteter, problem<span>eller projekt som har loggat timmar efter uppgifter och ärenden</span> kan inte tas bort. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Faktiska datum {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">När en uppgift eller ett problem går från"Nytt" till"Pågår" anger du det faktiska startdatumet som</td> 
      <td> <p>Välj ett av följande alternativ för när det faktiska startdatumet registreras i Workfront när en uppgift eller ett problem uppstår <strong>Nytt</strong> till <strong>Pågår</strong>:</p> 
       <ul> 
        <li><strong>Nu:</strong> Faktiskt startdatum anges till aktuellt datum.</li> 
        <li><strong>Planerat startdatum:</strong> Det faktiska startdatumet är inställt på det planerade startdatumet för aktiviteten eller utgåvan.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När en uppgift eller ett problem har slutförts anger du det faktiska slutförandedatumet till</td> 
      <td> <p>Välj något av följande alternativ för när det faktiska slutförandedatumet registreras i Workfront när en uppgift eller ett problem har slutförts:</p> 
       <ul> 
        <li><strong>Nu:</strong> Faktiskt slutförandedatum anges till aktuellt datum.</li> 
        <li> <p><strong>Planerat slutförandedatum:</strong> Faktiskt slutförandedatum anges till planerat slutförandedatum för aktiviteten eller utgåvan.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Åtkomst {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">När någon tilldelas till en uppgift</td> 
      <td> 
       <ul> 
        <li><strong>Ge dem ... åtkomst till en uppgift</strong>: Definierar standardbehörigheten som en användare har för den uppgift han/hon är tilldelad till. Mer information om aktivitetsbehörigheter finns i<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Bevilja åtkomst för användare</a>.</li> 
        <li> <p><strong>Ge även ... tillgång till projektet</strong>: Definierar standardbehörigheten som en användare har för det projekt som han/hon har en uppgift tilldelad till. Mer information om projektbehörigheter finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När någon har tilldelats ett problem</td> 
      <td> 
       <ul> 
        <li><strong>Ge dem ... åtkomst till en uppgift</strong>: Definierar standardbehörigheten som en användare har för den uppgift han/hon är tilldelad till. Mer information om aktivitetsbehörigheter finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</li> 
        <li> <p><strong>Ge även ... tillgång till projektet</strong>: Definierar standardbehörigheten som en användare har för det projekt som han/hon har en uppgift tilldelad till. Mer information om projektbehörigheter finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">När någon skickar en begäran</td> 
      <td> 
       <ul> 
        <li><strong>Ge dem ... åtkomst till problemet</strong>: Definierar standardbehörigheten som en användare har på en begäran som de har skickat. Mer information finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Dela ett ärende</a>.</li> 
        <li> <p><strong>Personer från samma företag ärver samma behörigheter för alla begäranden</strong>: Tillåter användare att se begäranden som andra användare från samma företag skickar. De har samma behörigheter för de begäranden som de själva har skickat.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
