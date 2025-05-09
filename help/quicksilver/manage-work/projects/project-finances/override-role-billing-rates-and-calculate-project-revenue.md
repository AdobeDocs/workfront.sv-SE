---
product-area: projects
navigation-topic: financials
title: Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt
description: Du kan använda faktureringstariffer för att beräkna intäkterna från dina projekt när du multiplicerar dem med timmarna som har ägnats åt projektet. Mer information om faktureringstariffer och intäkter finns i artikeln Översikt över fakturering och intäkter.
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '3860'
ht-degree: 0%

---

# Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt

{{highlighted-preview}}

Du kan använda faktureringstariffer för att beräkna intäkterna från dina projekt när du multiplicerar dem med timmarna som har ägnats åt projektet. Mer information om faktureringstariffer och intäkter finns i artikeln [Översikt över fakturering och intäkter](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Översikt över faktureringstariffer för jobbroller och intäktstyper för roller per timme

Som Adobe Workfront-administratör kan du associera faktureringstaxor med både användare och jobbroller.\
Mer information om hur du skapar användare och associerar dem med faktureringstariffer finns i artikeln [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Mer information om hur du skapar jobbroller och associerar dem med faktureringsfrekvenser finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Faktureringstariffer som är associerade med användare kan inte åsidosättas.

Faktureringstariffer som är associerade med jobbroller kan åsidosättas på företags- eller projektnivå.

Om du vill beräkna intäkter för projekt baserat på faktureringsfrekvenser för jobbroller måste **intäktstypen** för aktiviteterna i projekten vara något av följande:

* Roll timvis
* Roll timvis med ändpunkt
* Roll timvis plus fast

Mer information om **intäktstyp** och faktureringstariffer finns i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hierarki för faktureringshastighet åsidosätter vid beräkning av intäkt

En jobbroll kan ha en associerad faktureringsfrekvens på följande sätt:

* Som Workfront-administratör kan du definiera den faktureringsfrekvens på systemnivå som är kopplad till en jobbroll när du skapar den jobbrollen.\
  Mer information om hur du skapar jobbroller finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Som Workfront-administratör kan du definiera faktureringsnivån på företagsnivå för samma jobbroll när du skapar ett företag.\
  När Workfront beräknar intäkter för de projekt som är kopplade till det här företaget används företagsfaktureringssatsen när rollen tilldelas aktiviteter, i stället för faktureringssatsen på systemnivå för den här jobbrollen.\
  Jobbrollstarifferna som ändras på företagsnivå kommer att påverka alla projekt som är kopplade till det företaget.

  >[!NOTE]
  >
  >Om du behöver uppdatera företagsfaktureringstariffen kommer projektavgiften inte att uppdateras automatiskt. Du måste ta bort företaget från projektet, uppdatera priset för företaget och sedan koppla företaget till projektet igen innan den nya företagsavgiften börjar gälla för projektet. Instruktioner om hur du bifogar ett företag till ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

  Mer information om hur du skapar faktureringstariffer för jobbroller för ett företag finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Som Workfront-administratör kan du aktivera ett alternativ när du redigerar ett projekt för att tillämpa ändringar av faktureringstariffer på företagsnivå på projektet när användare manuellt beräknar om projektekonomin.\
  Mer information finns i [Åsidosätt faktureringstariffer på projektnivå med faktureringstariffer på företagsnivå](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Som Workfront-administratör kan du definiera tariffkort med flera faktureringspriser per roll, baserat på plats och datum. När ett betalningskort kopplas till ett projekt läggs alla roller (per plats, om platser används) och deras associerade faktureringstariffer till i projektets faktureringstaxsektion. Om du bifogar ett betalkort åsidosätts alla befintliga faktureringspriser för projektet.

  Mer information finns i [Hantera tariffkort](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) och [Koppla ett tariffkort till ett projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Som projektledare kan du definiera faktureringssatsen för samma jobbroll på projektnivå.\
  De ändrade rollsatserna i projektet kommer endast att påverka det projektet.

  Mer information om att åsidosätta rollfrekvenser för projektet finns i [Åsidosätt faktureringshastigheter för jobbroller på projektnivå](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Om en jobbroll är associerad med en faktureringsfrekvens på systemnivå, företagsnivå och projektnivå, beräknar Workfront intäkterna för aktiviteterna med hjälp av faktureringssatsen för jobbrollen på projektnivå, när jobbrollsnivåerna används. Inkomsterna från alla uppgifter räknas upp till projektets intäkter.

## Åsidosätt faktureringshastigheter för jobbroller på projektnivå

Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.

<span class="preview">Du kan även koppla ett betalkort till projektet, som importerar faktureringstaxorna för jobbrollen från tariffkortet till projektet.</span>

Mer information om hur du åsidosätter faktureringshastigheter för jobbroller på projektnivå finns i [Åsidosätt faktureringshastigheter för jobbroller på projektnivå](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Mer information om vilken jobbroll som används för att beräkna intäkter för projektet finns i avsnittet Inkomstberäkningar för aktiviteter baserade på användar- och rolltilldelningar i [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Mer information om hur du kopplar ett tariffkort till ett projekt finns i [Koppla ett tariffkort till ett projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>När det gäller Faktisk intäkt bör de faktureringstariffer som tillämpas på timmar som läggs till i en faktureringspost som är markerad som Fakturerad inte påverkas av åsidosättningar av faktureringstaxor som inträffar efter att faktureringsposten har fakturerats.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Översikt över avsnittet Faktureringssatser i ett projekt

När du har angett åsidosättningsfaktureringssatserna för de jobbroller som är associerade med projektet kan du se alla jobbroller och deras åsidosättningar på fliken **Faktureringssatser** i projektet.

Observera följande information i listan över **faktureringstariffer**:

* [Gruppering av jobbroller](#job-role-grouping)
* [Faktureringsvärde för projekt](#project-billing-rate-value)
* [Standardvärde för faktureringshastighet](#default-billing-rate-value)
* [Företagets faktureringsvärde](#company-billing-rate-value)
* [Flera faktureringsvärden och tidsramar](#multiple-billing-rate-values-and-timeframes)

### Gruppering av jobbroller {#job-role-grouping}

Faktureringstariffer grupperas i området **Faktureringstariffer** efter deras respektive jobbroller. <span class="preview">Om ett tariffkort är kopplat till projektet grupperas även jobbrollerna efter tariffkort. Om platser används för jobbroller inkluderas platsnamnet som en del av jobbrollens namn. Du kan ha samma jobbroll listad för flera platser.</span>

### Faktureringsvärde för projekt {#project-billing-rate-value}

I grupperingsraden som motsvarar en jobbroll lägger du märke till faktureringsnivån för den jobbrollen på projektnivå i kolumnen **Projektfaktureringsgrad**. Om jobbrollen har flera åsidosättningsfrekvenser visas den åsidosättningsfrekvens som motsvarar det aktuella datumet i grupperingsraden i kolumnen **Projektfaktureringsgrad**.

### Standardvärde för faktureringsfrekvens {#default-billing-rate-value}

Observera faktureringsfrekvensen för den jobbrollen på systemnivå i kolumnen **Standardfaktureringsfrekvens** i grupperingsraden för en jobbroll.

>[!NOTE]
>
>Om det finns projektfaktureringstariffer för en jobbroll används **standardfaktureringstakten** aldrig för att beräkna projektets inkomster. Endast de **projektfaktureringstarifferna** används för att beräkna intäkt.

### Faktureringsvärde för företag {#company-billing-rate-value}

Observera faktureringssatsen för den jobbrollen på företagsnivå i kolumnen **Företagets faktureringsfrekvens** i grupperingsraden för en jobbroll. Det innebär att det finns ett företag som är associerat med det här projektet och att den här jobbrollen har en annan faktureringsfrekvens för det företaget. Faktureringsräntan för företaget visas, även om den är samma som projekträntan.

>[!NOTE]
>
><span class="preview">När ett kurskort är kopplat till projektet importeras inte **Företagets faktureringstariffer** i faktureringstarifferna. Beräkningarna baseras antingen på tariffkort eller företagstaxor för jobbrollerna.</span>
>
>Om det finns projektfaktureringstariffer för en jobbroll används aldrig **Företagets faktureringstariff** för att beräkna projektets intäkter. Endast faktureringstarifferna **för projekt** används för att beräkna intäkten.

### Flera faktureringsvärden och tidsramar {#multiple-billing-rate-values-and-timeframes}

Om du har flera åsidosatta faktureringssatser för en viss jobbroll visas de under grupperingen för den jobbrollen. Med hjälp av intern redigering kan du ändra åsidosättningsfrekvenserna och **Start** **Date** och **End Date** för åsidosättningsdebiteringarna på den här fliken.

>[!NOTE]
>
>Du kan inte ange ett **startdatum** för den första åsidosättningsfrekvensen och du kan inte ange ett **slutdatum** för den senaste åsidosättningsfrekvensen. Workfront antar att den första åsidosättningsfrekvensen används för alla timmar med ett datum som är äldre än **Slutdatum** för den första åsidosättningen och att den senaste åsidosättningsfrekvensen används för alla timmar med ett datum som är senare än **Startdatum** för den senaste åsidosättningen.\
>Om en timme loggas före projektets planerade startdatum används den första faktureringstakten.\
>Om en timme loggas efter projektets planerade slutförandedatum används den senaste faktureringstakten.

## Beräkna planerade intäkter

* [Beräkna planerad intäkt baserat på en engångsåsidosättning av faktureringsgrad](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Beräkna planerad intäkt baserat på flera åsidosättningar av faktureringsfrekvens](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Fördelning av planerade timmar under en uppgifts varaktighet](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Beräkna planerad intäkt baserat på en engångsfaktureringsåsidosättning {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Tänk på följande när du beräknar planerad intäkt baserat på åsidosättning av en engångsavgift:

* När **intäktstypen** för en aktivitet är **Roll timme** multiplicerar Workfront antalet planerade timmar för en aktivitet med faktureringsfrekvensen för den jobbroll som är associerad med aktiviteten för att beräkna planerad intäkt för aktiviteten.

* När faktureringsgraden för jobbrollen har åsidosatts på projektnivå använder Workfront åsidosättningsfrekvensen från projektet för att beräkna planerad intäkt.
* När en uppgift har flera tilldelningar beräknas den planerade intäkten genom att multiplicera faktureringsfrekvensen för varje tilldelnings jobbroll och deras respektive allokering av planerad timma.

>[!NOTE]
>
>De planerade timmarna per tilldelning är inte samma som de planerade timmarna för aktiviteten, när det gäller flera tilldelningar.

Mer information om vilken jobbroll som används för att beräkna planerad intäkt finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Beräkna planerad intäkt baserat på flera åsidosättningar av faktureringssats {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Tänk på följande när du beräknar planerad intäkt baserat på åsidosättningar av flera faktureringsgrader:

* När **intäktstypen** för en aktivitet är **Roll timme** multiplicerar Workfront antalet planerade timmar för en aktivitet med faktureringsfrekvensen för den jobbroll som är associerad med aktiviteten för att beräkna planerad intäkt för aktiviteten.

  Mer information om vilken jobbroll som används för att beräkna planerad intäkt finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Om flera faktureringstariffer åsidosätts, den frekvens med vilken de planerade timmarna multipliceras med ändringar under en uppgifts varaktighet. Som standard distribuerar Workfront de planerade timmarna jämnt över en uppgifts varaktighet och tilldelar ett jämnt antal timmar för varje dag. När du beräknar **Planerad intäkt** för en aktivitet multiplicerar Workfront den planerade timmen per dag med faktureringsfrekvensen för den dagen. Vid flera faktureringspriser kan priset vara olika varje dag.

  Du har till exempel en aktivitet med en roll som är **Inkomsttyp** per timme. Aktiviteten har en varaktighet på 5 dagar och ett värde på 40 timmar för planerade timmar. Planerade timmar per dag är 8 timmar. Tilldela en projekthanterarjobbroll till aktiviteten och åsidosätt faktureringsfrekvensen för den här jobbrollen för de tre sista dagarna i aktiviteten, så att du har en faktureringsgrad på 1 för de två första dagarna och en faktureringsfrekvens på 2 för de tre återstående dagarna av aktiviteten för den här jobbrollen.

  Formeln som beräknar de **planerade intäkterna** för den här aktiviteten är:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Mer information om hur du hittar beloppet för planerade timmar per dag i Workfront finns i avsnittet [Distribution av planerade timmar under en uppgifts varaktighet](#distribution-of-planned-hours-across-the-duration-of-a-task) i den här artikeln.

>[!NOTE]
>
>Om du har flera tilldelningar för aktiviteten fördelas antalet planerade timmar först till varje tilldelad och sedan till varje dag under aktivitetens varaktighet. I det här fallet kommer den planerade intäkten att beräknas med hänsyn till antalet timmar per dag för varje tilldelad och faktureringsfrekvensen för varje arbetsroll som kan ändras under uppgiftens varaktighet, om det finns flera faktureringstariffer.

### Fördelning av planerade timmar under en uppgifts varaktighet {#distribution-of-planned-hours-across-the-duration-of-a-task}

Tänk på följande när du är införstådd med hur planerade timmar är fördelade över en uppgifts varaktighet:

* Som standard distribuerar Workfront de planerade timmarna jämnt över varaktigheten för en aktivitet och tilldelar samma antal planerade timmar för varje dag av aktiviteten, baserat på tillgängligheten för projektschemat.

  Mer information om hur du förstår fördelningen av planerade timmar under en uppgifts varaktighet finns i avsnittet Förstå distributionen av planerade timmar över en uppgifts varaktighet i artikeln [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Planerade timmar per dag är fördelningen av planerade timmar för varje dag under uppgiftens varaktighet. Om aktiviteten har ett uppdrag representerar det här numret även antalet planerade timmar per dag och tilldelning. Om aktiviteten har flera tilldelningar skiljer sig Planerade timmar per dag och tilldelning från planerade timmar per dag för aktiviteten. Det finns ingen visuell representation i Workfront av antalet planerade timmar per dag per uppdrag för uppgifter med flera uppdrag.
  >
  >
  >Planerade timmar per dag multipliceras med faktureringssatsen för den jobbroll som tilldelats uppgiften för den dagen för att beräkna den planerade intäkten per dag för den uppgiften. Summan av alla planerade intäkter per dag som beräknas på det här sättet motsvarar de planerade intäkterna för den uppgiften.

## Beräkna faktisk intäkt

* [Beräkna faktisk intäkt baserat på en engångsåsidosättning av faktureringsgrad](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Beräkna faktisk intäkt baserat på flera åsidosättningar av faktureringssats](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Beräkna faktisk intäkt baserat på en engångsåsidosättning av faktureringssats {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Tänk på följande när du beräknar faktisk intäkt baserat på en engångsfaktureringsränta:

* När **intäktstypen** för en aktivitet är **Roll per timme** multiplicerar Workfront **Faktiska timmar** för en aktivitet med faktureringsfrekvensen för den jobbroll som är associerad med aktiviteten för att beräkna **Faktisk intäkt** för aktiviteten. Faktiska timmar är timmar som loggas direkt till uppgiften.

  Mer information om vilken jobbroll som används för att beräkna **Faktisk intäkt** finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Om faktureringssatsen för jobbrollen har åsidosatts på projektnivå använder Workfront åsidosättningsfrekvensen från projektet för att beräkna faktisk intäkt. När du åsidosätter faktureringssatsen för jobbrollen i projektet beräknas projektets **faktiska inkomster** automatiskt om med den nya justerade tariffen.

  Mer information om att åsidosätta rollfrekvenser för projektet finns i [Åsidosätt faktureringshastigheter för jobbroller på projektnivå](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Om du vill behålla de timmar som du redan har loggat in på projektet innan du åsidosätter den ursprungliga faktureringstakten som fakturerades med den ursprungliga avgiften måste du inkludera dem i en **faktureringspost**, och du måste markera **faktureringsposten** som **Fakturerad**. I annat fall beräknas den **faktiska inkomsten** från de timmar som loggades innan faktureringstakten åsidosattes för projektet på nytt med den nya avgiften när projektens ekonomi beräknas om.\
>Mer information om hur du inkluderar timmar i en faktureringspost och markerar den som **Fakturerad** finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

### Beräkna faktisk intäkt baserat på flera åsidosättningar av faktureringssats {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Tänk på följande när du beräknar faktisk intäkt baserat på flera åsidosättningar av faktureringsgrad:

* När **intäktstypen** för en aktivitet är **Roll per timme** multiplicerar Workfront aktivitetens **faktiska timmar** med faktureringsfrekvensen för de jobbroller som tilldelats för aktiviteten för att beräkna **Faktisk intäkt** för aktiviteten. Faktiska timmar är timmar som loggas direkt till uppgiften.

* Om det finns flera åsidosättningar av faktureringssatsen kan den frekvens med vilken **faktiska timmar** multipliceras för att beräkna **faktisk intäkt** ändras under en uppgifts varaktighet. Workfront använder faktureringsfrekvensen för den jobbroll vars tidsram matchar **anmälningsdatumet** för de timmar som loggats för uppgiften för att beräkna **Faktisk intäkt.**

  En aktivitet har till exempel **intäktstypen** för **rollen varje timme** och har tilldelats jobbrollen för Project Manager. Åsidosätt faktureringssatsen för den här jobbrollen med tariff 1 för datumen mellan 19 juni och 25 juni. Från och med 26 juni åsidosätter du faktureringssatsen med ränta 2. Logga 2 timmar för 20 juni och 3 timmar för 28 juni.

  Workfront beräknar den **faktiska intäkten** för den här aktiviteten med följande formel:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Mer information om vilken jobbroll som används för att beräkna **Faktisk intäkt** finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Effekten av tidszoner vid beräkning av intäkter baserat på flera faktureringstariffer

Användare kan se olika planerade timmar per dag jämfört med andra användare, om tidszonsskillnader inträffar mellan dem och andra enheter i Workfront. Följande scenarier kan skeva informationen om planerade timmar per dag för en användare utifrån vad en annan användare ser:

* De två användarna kan ha sina datorer inställda för två olika tidszoner
* De två användarprofilerna i Workfront kan ha två olika tidszoner
* Tidszonen som är associerad med användarprofilen kan vara en annan än systemtidszonen i Workfront
* Tidszonen som är associerad med användarprofilen kan vara en annan än tidszonen i schemat för projektet.

I dessa fall kan antalet planerade timmar per dag vara olika för två användare som inte delar samma inställningar för tidszoner. De ser också olika planerade intäktsnummer när de använder flera åsidosättningar av faktureringsfrekvensen för ett projekt.

* [Beräkna planerad intäkt för användare i olika tidszoner](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Beräkna faktisk intäkt för användare i olika tidszoner](#calculate-actual-revenue-for-users-in-different-time-zones)

### Beräkna planerad intäkt för användare i olika tidszoner {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Om du har användare i olika tidszoner som arbetar med samma projekt rekommenderar vi att du inte ändrar åsidosättningarna av faktureringsfrekvensen för dina projekt under veckan. Om du gör det kan en felaktig mängd av Planerad intäkt för ditt projekt visas som ett resultat av timskillnader mellan tidszonerna i schemat för användare och Workfront systemtidszon. De flesta scheman tillåter att helger exkluderas från beräkningarna för Planerade timmar. Om en ändring inträffar i åsidosättningen av faktureringsfrekvensen för en jobbroll är det bättre att den inträffar under en helg än i mitten av en vecka när den kan sammanfalla med mitten av varaktigheten för en uppgift.

Tänk på följande när du beräknar planerad intäkt för användare i olika tidszoner:

* För aktiviteter som har **intäktstypen** av **Roll per timme** och som har tilldelats till jobbroller, beräknas **Planerad intäkt** genom att multiplicera **Planerade timmar** för en aktivitet med faktureringsfrekvensen för jobbrollen.

* **Planerade timmar** fördelas jämnt över aktivitetens **Varaktighet**.

* **Varaktighet** är tidsperioden mellan aktivitetens **planerade start** **datum** och **planerade slutförandedatum**. Eftersom aktiviteternas planerade startdatum **och** Planerade slutförandedatum **kan variera beroende på tidszonerna för de användare som visar aktiviteten, kan antalet planerade timmar per dag vara olika för två användare i två olika tidszoner.**

* Det planerade antalet timmar per dag ändrar inte den planerade intäkten för ett projekt om faktureringsnivån för jobbrollen inte ändras, eller om det bara finns en åsidosättning av faktureringssatsen. Även om två användare från två olika tidszoner ser olika planerade timmar per dag är projektets totala planerade inkomster densamma för de två användarna.

  Om flera debiteringstariffer åsidosätts kan dock projektets totala **planerade inkomster** se annorlunda ut för två användare i två olika tidszoner, eftersom den baseras på antalet planerade timmar per dag (som kan vara olika för de två användarna) och åsidosättningen av faktureringssatsen (som kan vara olika för samma dag, när varje användare tittar på uppgiften i sin egen tidszon).

* Det korrekta beloppet för **Planerad intäkt** är det som visas av användaren som har samma tidszon som tidszonen för din Workfront-instans. Din Workfront-administratör definierar Workfront tidszon i området Systemkundinformation.\
  Mer information om hur du definierar tidszonen för ditt system finns i artikeln [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Beräkna faktisk intäkt för användare i olika tidszoner {#calculate-actual-revenue-for-users-in-different-time-zones}

Tänk på följande när du beräknar faktisk intäkt för användare i olika tidszoner:

* När **intäktstypen** för en aktivitet är **Roll per timme** multiplicerar Workfront aktivitetens **faktiska timmar** med faktureringsfrekvensen för de jobbroller som tilldelats för aktiviteten för att beräkna den **faktiska intäkten**. Faktiska timmar är timmar som loggas direkt till uppgiften.

* Om det finns flera åsidosättningar av faktureringsfrekvensen använder Workfront faktureringsfrekvensen för den jobbroll vars tidsram matchar **anmälningsdatumet** för de timmar som loggats för uppgiften för att beräkna **Faktisk intäkt**.

* Eftersom det inte finns någon tidsstämpel på **bokföringsdatumet** för loggade timmar och det inte finns någon tidsstämpel på datumintervallen för flera åsidosättningar av faktureringsfrekvensen, påverkas inte beräkningarna för **Faktisk intäkt** av tidszonen som är associerad med användare.

Mer information om vilken jobbroll som används för att beräkna **Faktisk intäkt** finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Beräkna om projektfinansiering

Ekonomer beräknas för ett projekt när ändringar sker i de timmar som är loggade för projektet.

Om räntor ändras under ett projekts löptid kan du beräkna om kostnader och intäkter för projektet manuellt med hjälp av alternativet Beräkna om finansiering för ett projekt. Dessutom utlöser vissa åtgärder en automatisk omberäkning.

Mer information om hur du beräknar om projektekonomi finns i artikeln [Beräkna om projektekonomi](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Lägg till en ny faktureringstakt med API

Om du vill lägga till en ny faktureringsfrekvens för en jobbroll med API:t utför du en *setRatesForRole*-åtgärd för **Rate**-objektet med *PUT-metoden*.
Åtgärds- och datumfälten i objektet **Rate** är tillgängliga i API-version 8.0.
Om du redan har definierat flera faktureringstariffer för en jobbroll i ett projekt och du vill lägga till en ny faktureringstakt för det med ett nytt datumintervall, måste du inkludera både den befintliga avgiften och den avgift som ska läggas till i samma API-anrop. Det liknar hur du uppdaterar samlingar på objekt.

Följande API-anrop är ett exempel där **attachableID** är **Project ID** för projektet där du lägger till hastigheten och **RoleID** är det **Job Role ID** som du lägger till den nya faktureringstakten för.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f0150000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;frekvenser&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startdatum&quot;:null,&quot;slutdatum&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;}</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Mer information om hur du använder Workfront API finns i artikeln [API Basics](https://experience.workfront.com/s/article/API-Basics-638808549).
