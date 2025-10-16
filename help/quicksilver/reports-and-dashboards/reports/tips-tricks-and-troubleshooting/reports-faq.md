---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Vanliga frågor och svar om rapporter
description: Vanliga frågor och svar om rapporter
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# Vanliga frågor och svar om rapporter

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Här följer vanliga frågor om rapporter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Varför visas inte det korrekta resultatet i en kolumn i min anpassade beräkning för en timskillnad?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

I en projektrapport har jag en beräkning som subtraherar faktiska timmar från planerade timmar.

Resultatet jag får är felaktigt.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

Min beräkning är:

`valueexpression=SUB(workRequired,actualWorkRequired)`

### Svar

De flesta fält som använder timmar i Workfront lagras på några minuter. När du använder dessa fält i en beräkning blir resultatet oftast i minuter. För att få fram resultatet i timmar måste du dividera resultatet av beräkningen eller fältet som du refererar till med 60.

Planerade timmar sparas i minuter.

Beroende på vilket fält för Faktiska timmar du vill använda för beräkningen är de korrekta formlerna:

* För befintliga faktiska timmar som lagras i minuter:

  `valueexpression=SUB(workRequired,actualWorkRequired)/60`

* För faktiska timmar som lagras i timmar:

  `valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

Mer information finns i [Visa faktiska timmar](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Varför visas inte värdet för alla mina diagramelement i en rapport i diagrammet?

### Svar

Om du har fler än 50 diagramelement i ett rapportdiagram visas inte värdet för varje element i diagrammet.

När du har färre än 50 element i ett diagram visas värdet för varje element i diagrammet. Du kan lägga till ett filter eller ändra grupperingarna i rapporten för att begränsa hur många objekt som visas i varje element i diagrammet.

## Varför returnerar min rapport för många resultat för att visa diagrammet?

När jag kör en rapport som har ett diagram visas felmeddelandet &quot;Wow där... Den här rapporten returnerade EN MÄNGD data, vilket gör diagrammet oläsligt. Överväg att begränsa resultatet genom att lägga till ett filter eller ändra grupperingarna i diagrammet.&quot;

### Svar

Det här felet innebär att diagrammet innehåller upp till 618 distinkta resultat, till exempel mer än 618 staplar i ett stapeldiagram. För att lösa visningsproblemet måste du förfina resultatet genom att ändra det aktuella filtret och gruppera markeringar.

Mer information om hur du ändrar filter och grupperingar finns i artiklarna [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) och [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Varför ser jag mina uppgifter (eller problem) när jag öppnar samma rapport (eller kalender) som min medarbetare och de ser sina uppgifter istället?

### Svar

Rapporten eller kalendern kan ha en jokerteckensfiltervariabel som pekar på användaren som är inloggad. I det här fallet visar rapporten information baserat på den användare som är inloggad. Justera filtret för att ta bort jokertecknet som pekar på den inloggade användaren.\
![Filter-variabel för användar-ID](assets/qs--user.id-filter-variable-350x79.png)

En fullständig lista med användarbaserade översikt över jokerteckenfiltervariabler finns i [Översikt över jokerteckensfiltervariabler](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Varför verkar uppgifterna i min rapport ofullständiga?

### Svar

Detta kan inträffa i de flesta fall om du har begränsad åtkomst som förhindrar att objekt visas i systemet. Objekten som du vill visa delas inte heller med dig.

Rapportens skapare kan redigera rapporten och köra den med åtkomsträttigheterna för en systemadministratör eller en plananvändare som har åtkomst till informationen.

Mer information finns i [Kör och leverera en rapport med åtkomsträttigheter för en annan användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Hur rapporterar jag uppgifter (eller problem) som jag har tilldelats, oavsett om jag är ägare av dem eller inte?

### Svar

Om du vill visa alla uppgifter eller ärenden som du har tilldelats, oavsett om du är ägare (eller primär tilldelad) eller inte, använder du följande filter i en aktivitets- eller problemrapport:

1. Få åtkomst till en aktivitet eller en problemrapport.
1. Klicka på **Lägg till en filterregel** på fliken **Filter**.

1. I fältet **Börja skriva fältnamn ...** börjar du skriva **Tilldelningsanvändarnamn** och markerar det när det visas i listan.

   >[!NOTE]
   >
   >Använd inte fältet **Tilldelad till namn** eftersom det här filtret endast gäller de uppgifter och utgåvor som du är primär tilldelad eller ägare för.

1. Välj modifieraren **Lika med**.
1. Börja skriva *$$USER.ID* i textrutan och välj den i listrutan som visas.\
   På så sätt ser du alla uppgifter och problem som har tilldelats den inloggade användaren. Du kan ersätta jokertecknet med ett specifikt användarnamn.\
   ![Uppgifter tilldelade mig](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Klicka på **Spara + Stäng**.

## Varför visas inte länkarna Lägg till problem/Lägg till uppgifter längst ned i listan med ärenden och uppgifter i ett projekt?

### Svar

Kontrollera först att du har rätt behörighet och behörighet för att lägga till problem och uppgifter i ett projekt. I det här fallet bör du se länkarna **Lägg till problem** och **Lägg till uppgifter** längst ned i listorna **Problem** och **Åtgärder** .

Det finns dock några saker som kan förhindra att länkarna visas:

* Om du har använt snabbfiltret på dessa listor visas inte länkarna. Ta bort snabbfiltret och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
  Mer information om snabbfiltret finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Om du har använt en **gruppering** på de här listorna visas inte länkarna. Ta bort **grupperingen** och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
  Mer information om hur du skapar grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Om du har använt en **Visa** på de här listorna som har en annan valuta än projektets standardvaluta, visas inte länkarna. Ändra **Visa** till **Projektets ursprungliga valuta** och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
  Mer information om hur du ändrar valutan i din vy finns i [Skapa ekonomiska datarapporter med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Projektvaluta](assets/nwe-project-original-currency-350x229.png)

## Uppdateras informationen i min rapport eller instrumentpanel automatiskt?

### Svar

Informationen i rapporter eller kontrollpaneler uppdateras inte automatiskt.

Informationen kan uppdateras manuellt i en cachelagrad rapport.\
Mer information om hur du uppdaterar en cachelagrad rapport finns i [Kör en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Informationen kan uppdateras manuellt i en cachelagrad kontrollpanel.\
Mer information om hur du uppdaterar en cachelagrad kontrollpanel finns i avsnittet [Visa kontrollpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) i artikeln [Kom igång med kontrollpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Kan jag ändra rapportens ägare?

### Svar

Du kan inte ändra rapportens ägare. Den användare som skapade rapporten kan dock tillåta andra användare att redigera rapporten. Hur du kan tillåta användare att redigera en rapport beror på vilken typ av användare du är.

* Systemadministratörer kan tillåta användare med en planlicens att redigera rapporter genom att konfigurera alternativet Redigera i rapportraden så att de får tillgång till Skapa en rapport.\
  Mer information finns i [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Alla slutanvändare som har tillgång till att skapa och dela rapporter kan låta andra redigera enskilda rapporter genom att dela dem och ge andra användare behörigheten Hantera.\
  Mer information finns i [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Om du har behörighet att visa eller hantera en rapport kan du också göra en kopia av rapporten, som du sedan blir ägare till som standard. Mer information om hur du kopierar en rapport finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Varför kan jag inte komma åt en rapport som ägs av en inaktiverad användare?

### Svar

Ibland är rapportens ägare också den användare som anges i **Kör den här rapporten med åtkomsträttigheten** i rapportfältet. Om **Kör den här rapporten med åtkomsträttigheterna för**-användaren inaktiveras visas inte längre rapporten för användare som har den delade rapporten. När det inträffar kan du göra rapporten tillgänglig igen genom att lämna **Kör den här rapporten med åtkomstbehörigheten** tom eller genom att ange en aktiv användare i fältet.

Om du vill veta mer om fältet **Kör den här rapporten med åtkomsträttigheter för:** kan du läsa [Kör och leverera en rapport med åtkomsträttigheter för en annan användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Information om hur du identifierar alla rapporter som ägs av inaktiverade användare finns i [Skapa en rapport om rapporteringsaktiviteter](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Hur får jag åtkomst till en instrumentpanel som innehåller en rapport som ägs av en borttagen användare?

### Svar

När du tar bort en användare kan du fortfarande få åtkomst till alla rapporter som de har skapat, men alla instrumentpaneler som innehåller rapporten tas också bort. Det innebär att du inte längre kan komma åt följande:

* En kontrollpanel som innehåller rapporten, inklusive kontrollpaneler i den vänstra panelen av ett objekt

Mer information om konsekvenserna av att ta bort en användare finns i [Ta bort användare](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Om du har åtkomst till rapporten via Visa kan du göra följande:

1. Skapa en kopia av rapporten.\
   Mer information om hur du skapar en kopia av en rapport finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Uppdatera instrumentpanelen så att den kopierade rapporten inkluderas.\
   Mer information om hur du redigerar en kontrollpanel finns i [Redigera en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
