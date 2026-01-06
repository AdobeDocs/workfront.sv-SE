---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Översikt över affärsområdet
description: I den här artikeln beskrivs områdena i affärsärendet för ett projekt.
author: Becky
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 0%

---

# Översikt över ärendeområden

<!-- Audited: 4/2025 -->

I den här artikeln beskrivs områdena i affärsärendet för ett projekt.

Mer information om hur du skapar ett affärsärende för ett projekt finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Din Adobe Workfront-administratör eller gruppadministratör måste aktivera alla avsnitt i affärsärendet innan de visas i projektet, utom avsnittet Projektinformation. Avsnittet Projektinformation är aktiverat som standard.

Mer information om hur du aktiverar områden för affärsärenden finns i avsnittet Affärsfall i artikeln [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Följande är områden i ett projekts affärsmodell:

* Projektinformation
* Mål
* Utgifter
* Resursbudgetering
* Risker
* Styrkort
* Anpassad Forms
* Översikt över affärsärenden

## Projektinformation

Avsnittet Projektinformation i affärsärendet innehåller grundläggande information om ett projekt innan projektet faktiskt har startats.

Alla projekt har ett projektinformationsområde i affärsärendet med förinställda fält, vilket innebär att Workfront-administratörer inte kan konfigurera vilka fält som ska visas i det här området.

Överväg att redigera följande fält:

* **Beskrivning**: Lägg till en beskrivning av projektet.

* **Projektägare**: Som standard är den användare som skapar projektet också projektägare. Redigera det här fältet om du vill välja en annan aktiv användare som projektägare.

* **Projektsponsor**: Välj en aktiv användare som ska vara projektsponsor. Sponsorn får affärsärendets godkännande.

* **Portfolio**: Välj en Portfolio för projektet. Du måste skapa Portfolio-filen och placera den i aktiv status innan den kan väljas i den här listrutan.

  Mer information om portföljer finns i [Översikt över Portfolio i Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Mer information om hur du skapar portföljer finns i [Skapa en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Planerad förmån**: Uppskattar vilken ekonomisk förmån som planeras för din organisation när det här projektet har slutförts. Det kan vara valfritt valutabelopp och det måste vara ett positivt värde (t.ex. 10 000 dollar).

* **Status**: Som standard är status för en projektförfrågan Idea. Om du ändrar status till något annat än Idea eller Planning försvinner knappen Skicka under Affärsärendesammanfattning och du kan inte längre skicka affärsärendet för godkännande.

* **Fast startdatum**: Ange ett datum när du vill att projektet ska starta.

* **Fast slutdatum**: Ange ett datum då du vill att projektet ska avslutas.

  >[!NOTE]
  >
  >Fasta start- och slutdatum i affärsärendet påverkar inte projektets planerade start- och slutdatum. Dessa representerar de datum som den som skapat projektet begär när projektet helst skulle utvecklas. I stället visar projektets planerade start- och slutdatum den planerade tidslinjen för projektet, som baseras på projektets uppgifter.

## Mål

Mål definierar projektets mål. Det här området är aktiverat som standard i affärsärendet, men Workfront-administratören kan välja att inte visa det. I det här fältet visas målen i prioritetsordning.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Du kan skapa strategiska mål för din organisation som inte är kopplade till ett projekts enskilda affärsärende. Du måste ha tillgång till Adobe Workfront-mål för att kunna skapa strategiska mål. Sedan kan du koppla dem till projekt utanför deras affärsärenden. Mer information om hur du skapar mål med hjälp av Workfront-mål finns i [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).

Att definiera målen är valfritt för att projektet ska få en poäng i Portfolio Optimizer. Det här avsnittet är det enda valfria avsnittet i affärsärendet. Alla andra avsnitt i affärsärendet måste slutföras innan projektet kan hanteras i Portfolio Optimizer. Du kan ange en prioritetsnivå för ett mål när du skapar målet.

Mer information finns i [Skapa mål för affärsärenden](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Utgifter

Utgifter är de icke-arbetskostnader som kan uppstå under ett projekts livslängd. Det här området är aktiverat som standard i affärsärendet, men Workfront-administratören kan välja att inte visa det.

Alla utgifter som du anger i affärsärendet anges också som Planerade utgifter på fliken Utgifter i projektet.

Utgifter påverkar följande fält i projektet:

* Budgeterad kostnad
* Nettovärde

Din Workfront-administratör kan konfigurera anpassade utgiftstyper.

Mer information om budgeterade kostnader och nettovärden finns i [Översikt över finansiella fält för affärsärenden](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Mer information om utgifter finns i [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Mer information om hur du skapar anpassade utgiftstyper finns i [Skapa anpassade utgiftstyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

## Resursbudgetering

Du kan utföra följande åtgärder i området Resursbudgetering i affärsärendet:

* Associera resurspooler med projektet.
* Budgetera dina resurser på projektnivå.

De timmar som har budgeterats för projektets resurser visas i området Resursbudgetering i affärsärendet och genererar projektets budgeterade arbetskostnad. Det här området är aktiverat som standard.

Mer information om budgeteringsresurser för projektet i affärsärendet finns i [Budgetresurser i affärsärendet](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

<!--![Business case resource budgeting](assets/business-case-sp-selected-with-choose-button-350x121.png)-->

Tänk på följande när du visar avsnittet Resursbudgetering i affärsärendet:

* Du kan budgetera resursinformation här med följande verktyg:

   * Resursplaneraren

     Mer information finns i [Budgetresurser i affärsärendet med hjälp av resursplaneraren](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Scenarioplanen

     Mer information finns i [Budgetresurser i affärsärendet med scenarioplaneraren](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

* Den information som visas här visas även i resursplaneraren på systemnivå eller i scenarioplaneraren.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in NWE only)<br></p>
  -->

* När du har budgeterat dina resurser visas projektets budgeterade arbetskostnad i området Resursbudgetering om rollerna är kopplade till Kostnad per timme. Budgeterad arbetskostnad visas i projektets valuta.

  >[!IMPORTANT]
  >
  >Budgeterad arbetskostnad är kostnaden som är associerad med rollerna i projektet, inte med användarna. Summan av alla budgeterade arbetskostnader för användarna kan vara lika med eller inte vara lika med den budgeterade arbetskostnaden för den jobbroll som är associerad med användarna.

  Mer information om budgeterad arbetskostnad finns i [Översikt över ekonomiska fält för affärsärenden](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Mer information om hur du skapar jobbroller och associerar Kostnad per timme med dem finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Risker

Risker är faktorer som kan förhindra att ett projekt slutförs i tid eller i budgeten. Det är viktigt att du definierar dessa faktorer för att Portfolio-chefen eller projektsponsorn ska kunna fatta ett väl underbyggt beslut om projektets godkännande. Det här området är aktiverat som standard i affärsärendet, men Workfront-administratören kan välja att inte visa det.

Du kan koppla en potentiell kostnad till de risker du definierar om de skulle inträffa. Riskkostnaderna påverkar projektets nettovärde.

Din Workfront-administratör kan konfigurera anpassade risktyper.

Mer information om projektets nettovärde finns i [Översikt över finansiella fält för affärsärenden](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Mer information om att skapa risker finns i [Skapa och redigera risker i projekt](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Mer information om hur du skapar och redigerar anpassade risktyper finns i [Redigera och skapa risktyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Styrkort

Styrkort mäter justeringen av projektet. Det här området är aktiverat som standard i affärsärendet, men Workfront-administratören kan välja att inte visa det.

Om du vill använda ett styrkort måste Workfront-administratören först skapa ett. Styrkortsområdet i affärsärendet visas bara om ett styrkort har skapats.

Mer information om hur du använder ett styrkort i ett projekt och genererar ett justeringsmoment finns i [Använda ett styrkort i ett projekt och generera ett justeringsmoment](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Mer information om hur du skapar ett styrkort finns i [Skapa ett styrkort](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Anpassad Forms

Du kan koppla anpassade Forms till ett projekt när du definierar ett affärsärende. Det här området är inte aktiverat som standard i Business Case och Workfront-administratören måste aktivera det för att det ska kunna visas i Business Case.

Om du vill använda ett anpassat formulär måste Workfront-administratören först skapa ett.

Du kan använda anpassade formulär för att samla in ytterligare information som inte visas i andra fält i affärsärendet.

Mer information om hur du aktiverar områden i affärsärendet finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Mer information om hur du skapar ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Mer information om hur du använder ett anpassat formulär finns i [Koppla ett anpassat formulär till ett affärsärende](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Översikt över affärsärenden

* [Översikt över affärsärendesammanfattning](#overview-of-the-business-case-summary)
* [Exportera affärsärendet](#export-the-business-case)

### Översikt över ärendesammanfattningen {#overview-of-the-business-case-summary}

Du kan se en sammanfattning av projektets huvudsakliga ekonomi och om ett projekt är justerat eller inte med ett styrkort på panelen Affärsärendesammanfattning, som finns i det övre högra hörnet av affärsärendet.

Översikt över affärsärenden är bara en snabb vy av projektets status i förhållande till finansiella fält och styrkortet, och kan inte redigeras.

Följande fält visas i Översikt över affärsärenden:

* Projektets nettovärde
* Projektbudgeterad kostnad
* Den potentiella riskkostnaden
* Planerad förmån
* Justeringspoäng

Mer information om de här fälten finns i [Översikt över ekonomiska fält för affärsärenden](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exportera affärsärendet {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Du kan exportera affärsärendet till en PDF-fil om du behöver skriva ut den eller bifoga den till ett e-postmeddelande i ett mer komprimerat format.

Mer information finns i [Exportera affärsärendet för ett projekt](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it. </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.  The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>

