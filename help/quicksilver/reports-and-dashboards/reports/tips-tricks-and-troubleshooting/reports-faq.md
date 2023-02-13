---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Vanliga frågor och svar om rapporter
description: Vanliga frågor och svar om rapporter
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Vanliga frågor och svar om rapporter

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Här följer vanliga frågor om rapporter.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera, arbeta</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Varför visas inte det korrekta resultatet i en kolumn i min anpassade beräkning för en timskillnad?

I en projektrapport har jag en beräkning som subtraherar faktiska timmar (2) från Planerade timmar (4). Resultatet jag får är 120 när det borde vara 2.\
Min beräkning är:
<pre>valueExpression=SUB(workRequired,actualWorkRequired)</pre>

### Svar

Fält som använder timmar i Workfront lagras på några minuter. När du använder fältet i en beräkning blir resultatet i minuter. För att få fram resultatet i timmar måste du dividera resultatet av beräkningen med 60.

Den korrekta beräkningen är:

<pre>valueExpression=SUB(workRequired,actualWorkRequired)/60</pre>

## Varför visas inte värdet för alla mina diagramelement i en rapport i diagrammet?

### Svar

Om du har fler än 50 diagramelement i ett rapportdiagram visas inte värdet för varje element i diagrammet.

När du har färre än 50 element i ett diagram visas värdet för varje element i diagrammet. Du kan lägga till ett filter eller ändra grupperingarna i rapporten för att begränsa hur många objekt som visas i varje element i diagrammet.

## Varför returnerar min rapport för många resultat för att visa diagrammet?

När jag kör en rapport som har ett diagram visas felmeddelandet &quot;Wow där... Den här rapporten returnerade EN MÄNGD data, vilket gör diagrammet oläsligt. Överväg att begränsa resultatet genom att lägga till ett filter eller ändra grupperingarna i diagrammet.&quot;

### Svar

Det här felet innebär att diagrammet innehåller upp till 618 distinkta resultat, till exempel mer än 618 staplar i ett stapeldiagram. För att lösa visningsproblemet måste du förfina resultatet genom att ändra det aktuella filtret och gruppera markeringar.

Mer information om hur du ändrar filter och grupperingar finns i artiklarna [Översikt över filter i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) och [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Varför ser jag mina uppgifter (eller problem) när jag öppnar samma rapport (eller kalender) som min medarbetare och de ser sina uppgifter istället?

### Svar

Rapporten eller kalendern kan ha en jokerteckensfiltervariabel som pekar på användaren som är inloggad. I det här fallet visar rapporten information baserat på den användare som är inloggad. Justera filtret för att ta bort jokertecknet som pekar på den inloggade användaren.\
![](assets/qs--user.id-filter-variable-350x79.png)

En fullständig lista över användarbaserade jokertecken-filtervariabler finns i [Variabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Varför verkar uppgifterna i min rapport ofullständiga?

### Svar

Detta kan inträffa i de flesta fall om du har begränsad åtkomst som förhindrar att objekt visas i systemet. Objekten som du vill visa delas inte heller med dig.

Rapportens skapare kan redigera rapporten och köra den med åtkomsträttigheterna för en systemadministratör eller en plananvändare som har åtkomst till informationen.

Mer information finns i [Kör och leverera en rapport med åtkomsträttigheter för en annan användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Hur rapporterar jag uppgifter (eller problem) som jag har tilldelats, oavsett om jag är ägare av dem eller inte?

### Svar

Om du vill visa alla uppgifter eller ärenden som du har tilldelats, oavsett om du är ägare (eller primär tilldelad) eller inte, använder du följande filter i en aktivitets- eller problemrapport:

1. Öppna en aktivitets- eller problemrapport.
1. På **Filter** flik, klicka **Lägg till en filterregel**.

1. I **Börja skriva fältnamn..** fält, börja skriva **Namn på uppdragsanvändare** markerar du den när den visas i listan.

   >[!NOTE]
   >
   >Använd inte **Tilldelad till namn** som det här filtret endast för de uppgifter och utgåvor som du är primär tilldelad eller ägare för.

1. Välj **Jämn** modifierare.
1. Börja skriva *$$USER.ID* i textrutan och välj den i listrutan som visas.\
   På så sätt ser du alla uppgifter och problem som har tilldelats den inloggade användaren. Du kan ersätta jokertecknet med ett specifikt användarnamn.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Klicka **Spara + Stäng**.

## Varför visas inte länkarna Lägg till problem/Lägg till uppgifter längst ned i listan med ärenden och uppgifter i ett projekt?

### Svar

Kontrollera först att du har rätt behörighet och behörighet för att lägga till problem och uppgifter i ett projekt. I det här fallet bör du se **Lägg till problem** och **Lägg till aktiviteter** länkar längst ned i **Problem** och **Uppgifter** listor.

Det finns dock några saker som kan förhindra att länkarna visas:

* Om du har använt snabbfiltret på de här listorna visas inte länkarna. Ta bort snabbfiltret och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
   Information om snabbfiltret finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Om du har en **Gruppering** länkarna visas inte i de här listorna. Ta bort **Gruppering** och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
   Mer information om hur du skapar grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Om du har en **Visa** länkarna visas inte i listor som har en annan valuta än projektets standardvaluta. Ändra **Visa** till **Projektets ursprungliga valuta** och länkarna ska visas så att du kan lägga till problem och uppgifter i dina projekt.\
   Mer information om hur du ändrar valuta i vyn finns i [Skapa rapporter om finansiella data med unika valutakurser](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## Uppdateras informationen i min rapport eller instrumentpanel automatiskt?

### Svar

Informationen i rapporter eller kontrollpaneler uppdateras inte automatiskt.

Informationen kan uppdateras manuellt i en cachelagrad rapport.\
Mer information om hur du uppdaterar en cachelagrad rapport finns i [Köra en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Informationen kan uppdateras manuellt i en cachelagrad kontrollpanel.\
Mer information om hur du uppdaterar en cachelagrad kontrollpanel finns i avsnittet [Visa instrumentpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) i artikeln [Kom igång med instrumentpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Kan jag ändra rapportens ägare?

### Svar

Du kan inte ändra rapportens ägare. Den användare som skapade rapporten kan dock tillåta andra användare att redigera rapporten. Hur du kan tillåta användare att redigera en rapport beror på vilken typ av användare du är.

* Systemadministratörer kan tillåta användare med en planlicens att redigera rapporter genom att konfigurera alternativet Redigera i rapportraden så att de får tillgång till Skapa en rapport.\
   Mer information finns i [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Alla slutanvändare som har tillgång till att skapa och dela rapporter kan låta andra redigera enskilda rapporter genom att dela dem och ge andra användare behörigheten Hantera.\
   Mer information finns i [Dela en rapport i Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Om du har behörighet att visa eller hantera en rapport kan du också göra en kopia av rapporten, som du sedan blir ägare till som standard. Mer information om hur du kopierar en rapport finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Varför kan jag inte komma åt en rapport som ägs av en inaktiverad användare?

### Svar

Ibland är rapportens ägare även den användare som anges i **Kör den här rapporten med åtkomsträttigheterna för:** i rapporten. Om **Kör den här rapporten med åtkomsträttigheterna för:** om användaren är inaktiverad visas rapporten inte längre för användare som har delat rapporten med sig. När det händer kan du göra rapporten tillgänglig igen genom att lämna **Kör den här rapporten med åtkomsträttigheter för:** tomt eller ange en aktiv användare i fältet.

Läs mer om **Kör den här rapporten med åtkomsträttigheter för:** fält, se [Kör och leverera en rapport med åtkomsträttigheter för en annan användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Information om hur du identifierar alla rapporter som ägs av inaktiverade användare finns i [Skapa en rapport om rapporteringsaktiviteter](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Hur får jag åtkomst till en instrumentpanel som innehåller en rapport som ägs av en borttagen användare?

### Svar

När du tar bort en användare kan du fortfarande få åtkomst till alla rapporter som de har skapat, men alla instrumentpaneler som innehåller rapporten tas också bort. Det innebär att du inte längre kan komma åt följande:

* En instrumentpanel som innehåller rapporten
* Ett anpassat avsnitt som innehåller en kontrollpanel för rapporten

Mer information om hur du tar bort en användare finns i [Ta bort användare](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Om du har åtkomst till rapporten via Visa kan du göra följande:

1. Skapa en kopia av rapporten.\
   Mer information om hur du skapar en kopia av en rapport finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Uppdatera instrumentpanelen så att den kopierade rapporten inkluderas.\
   Mer information om hur du redigerar en kontrollpanel finns i [Redigera en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
