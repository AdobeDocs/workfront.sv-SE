---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Skapa och hantera jobbroller
description: Som  [!DNL Adobe Workfront] administratör eller en användare med administrativ åtkomst till jobbroller kan du skapa jobbroller som kan tilldelas användare och ta bort standardjobbroller som inte är relevanta för din organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 0%

---

# Skapa och hantera jobbroller

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Som administratör för [!DNL Adobe Workfront] eller användare med administrativ åtkomst till jobbroller kan du skapa jobbroller som kan tilldelas användare och ta bort standardjobbroller som inte är relevanta för din organisation. Mer information om administrativ åtkomst i [!DNL Workfront] finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>
   <p>Nytt: [!UICONTROL Standard]</p>
   <p>eller</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till jobbroller</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en jobbroll

Så här skapar du en jobbroll:

{{step-1-to-setup}}

1. Klicka på &#x200B; **[!UICONTROL Job Roles]i den vänstra panelen.**
1. Klicka på **[!UICONTROL New Job Role].**
1. Konfigurera följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Ange ett namn för jobbrollen. Det här namnet visas överallt i [!DNL Workfront] där fältet [!UICONTROL Job Role] visas. </p> <p>Tips! Namnet på en jobbroll kan innehålla upp till 255 tecken. Längre namn kan dock trunkeras i vissa områden i [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ange en beskrivning för rollen som anger vad som är unikt med den. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Välj <b>[!UICONTROL Yes]</b> om du vill att rollen ska vara aktiv och tillgänglig överallt i [!DNL Workfront] för att associeras med användare, arbetsobjekt osv. </p> </li> 
        <li> <p>Välj <b>[!UICONTROL No]</b> om du vill att rollen ska inaktiveras och inte vara tillgänglig för tilldelning till användare, arbetsobjekt osv. </p> </li> 
       </ul> <p><span>Mer information om hur du inaktiverar jobbroller finns i </span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Inaktivera jobbroller</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>Detta är [!UICONTROL Base Currency], enligt inställningen i området [!UICONTROL Setup] av Workfront-administratören. Mer information finns i </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Konfigurera valutakurser</a> .</p> <p>Tips: <span>Du kan inte redigera [!UICONTROL Base Currency] på jobbrollnivå. Det här fältet är nedtonat och fungerar som en påminnelse om vad basvalutan är för ditt system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Detta är kostnaden per timme för jobbrollen. Detta värde beräknar de planerade och faktiska kostnaderna för aktiviteter och ärenden som är kopplade till rollen samt slutligen de planerade och faktiska kostnaderna för projekten. Ange frekvensen med hjälp av [!UICONTROL Base Currency].</p> 
      <p>Klicka på <strong>[!UICONTROL Add Rate]</strong> om du vill veta vilka datumkostnader som gäller. Ange värdet för kostnad/timme för tidsperioden och tilldela [!UICONTROL Start Date] och [!UICONTROL End Date] efter behov. Den första kostnadstariffen har inget startdatum och den sista kostnadstariffen har inget slutdatum.</p> <p>Vissa datum läggs till automatiskt. Om till exempel den första kostnadstariffen inte har ett slutdatum och du lägger till en andra kostnadstariff med startdatumet 1 maj 2023, läggs ett slutdatum, 30 april 2023, till den första kostnadstariffen så att inga luckor finns.</p> <p>Tips! När du redigerar en befintlig jobbroll kan du välja <strong>Sortera efter startdatum</strong> för att se det senaste startdatumet högst upp i hastighetslistan.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>Det här är faktureringen per timma för jobbrollen. Detta värde beräknar de planerade och faktiska intäkterna för uppgifter och ärenden som är kopplade till rollen och slutligen projektens planerade och faktiska intäkter. Ange frekvensen med hjälp av [!UICONTROL Base Currency].</p> <p>Klicka på <strong>[!UICONTROL Add Rate]</strong> om du vill se gällande faktureringstariffer för datum. Ange värdet för fakturering/timme för tidsperioden och tilldela [!UICONTROL Start Date] och [!UICONTROL End Date] efter behov. Den första faktureringstakten har inget startdatum och den sista faktureringstakten har inget slutdatum.</p> <p>Vissa datum läggs till automatiskt. Om till exempel den första faktureringssatsen inte har ett slutdatum och du lägger till en andra med startdatumet 1 maj 2023, läggs slutdatumet 30 april 2023 till den första faktureringsavgiften så att inga luckor uppstår.</p> <p>Tips! När du redigerar en befintlig jobbroll kan du välja <strong>Sortera efter startdatum</strong> för att se det senaste startdatumet högst upp i hastighetslistan.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Välj en valuta som är associerad med den här jobbrollen. Det här är valutan som [!DNL Workfront] använder för att beräkna kostnader och intäkter som är associerade med den här jobbrollen. </p> 
        <p><span>Detta skiljer sig från [!UICONTROL Base Currency] som har konfigurerats av [!DNL Workfront]-administratören i området [!UICONTROL Setup] och kan skilja sig från valutan som är associerad med ett projekt.</span> </p> 
        <p>Tips! Endast tillgängliga valutor i området [!UICONTROL Exchange Rates] i systemet är tillgängliga i det här fältet. Om du bara har ställt in en valuta visas inte det här fältet.</p> 
       <p><span>Mer information om hur du konfigurerar [!UICONTROL Base Currency] i [!DNL Workfront] finns i </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Konfigurera valutakurser</a>.</p> <p><span>Mer information om hur du ändrar valuta för ett projekt finns i </span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Ändra projektvaluta</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>Detta är kostnaden per timme för jobbrollen som använder den valda [!UICONTROL Override Currency]. [!DNL Workfront] använder det här värdet för att beräkna planerade och faktiska kostnader för aktiviteter och ärenden som är associerade med jobbrollen. </p> 
        <p><span>Ange hastigheten i [!UICONTROL Override Currency] som anges ovan. Detta uppdaterar också kostnadstakten för den här jobbrollen när [!UICONTROL Base Currency] används.</span> </p> 
        <p>Mer information om hur [!DNL Workfront] beräknar kostnader finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> 
       <p>Tips! Vid uppdatering av en befintlig jobbroll som redan har en associerad kostnadstariff, beräknar [!DNL Workfront] hastigheten [!UICONTROL Override Currency] baserat på konverteringsgraden i systemet. Om du uppdaterar [!UICONTROL Override Currency Cost Rate] uppdateras även kostnadstakten för jobbrollen automatiskt.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>Det här är faktureringen per timma för jobbrollen som använder den valda [!UICONTROL Override Currency]. [!DNL Workfront] använder det här värdet för att beräkna planerad och faktisk intäkt för aktiviteter och ärenden som är associerade med jobbrollen. </p>
        <p><span>Ange hastigheten i [!UICONTROL Override Currency] som anges ovan. Detta uppdaterar även faktureringssatsen för den här jobbrollen när [!UICONTROL Base Currency] används.</span> </p>
        <p>Mer information om hur [!DNL Workfront] beräknar intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>.</p>
        <p>Tips! Vid uppdatering av en befintlig jobbroll som redan har en associerad faktureringshastighet, beräknar [!DNL Workfront] åsidosättandevalutakursen baserat på konverteringsgraden i systemet. Om du uppdaterar faktureringshastigheten för åsidosättning av valuta, uppdateras även faktureringshastigheten för jobbrollen automatiskt. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Jobbroller är en viktig del i hanteringen av resurser. Om du vill använda verktygen för resursplanering behöver jobbrollerna en kostnad och faktureringsfrekvens som är kopplad till dem. Mer information finns i [Kom igång med resurshantering](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Klicka på **[!UICONTROL Create Job Role]**. Jobbrollen är nu tillgänglig för att tilldelas aktiviteter, utgåvor, godkännanden eller så kan du dela layoutmallar eller andra objekt med den. Mer information om all användning av jobbroller i [!DNL Workfront] finns i [Översikt över jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Mer information om hur du tar bort en jobbroll finns i [Ta bort jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
