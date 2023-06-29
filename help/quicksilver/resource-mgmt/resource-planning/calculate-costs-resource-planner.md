---
product-area: resource-management
navigation-topic: resource-planning
title: Beräkna kostnader i resursplaneraren
description: Du kan budgetera dina resurser i Adobe Workfront Resursplanering genom att använda kostnadsvärden i stället för timvärden eller FTE-värden. Kostnadsvärden är inte tillgängliga för vyn**Visa efter användare** i resursplaneraren.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Beräkna kostnader i resursplaneraren

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Du kan budgetera dina resurser i Adobe Workfront Resursplanering genom att använda kostnadsvärden i stället för timvärden eller FTE-värden. Kostnadsvärden är inte tillgängliga för **Visa efter användare** i resursplaneraren.

>[!IMPORTANT]
>
>Du måste associera användare och jobbroller med kostnad per timme för att visa kostnadsinformation i resursplaneraren.\
>Mer information om hur du associerar självkostnad per timme med jobbroller finns i [Skapa och hantera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Mer information om hur du associerar självkostnad per timme med användare finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Innan du budgeterar dina resurser måste du se till att du har en god förståelse för vad som behöver göras (Planerade timmar, FTE eller Kostnad) och vilken tid användarna är öppna för arbete (Tillgängliga timmar, FTE eller Kostnad).\
Mer information om hur du förstår informationen i resursplaneraren vid budgetering med timmar eller heltidsekvivalenter finns i [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Redigera prioriteringar och budgettimmar i Resursplanering</p> <p>Redigera åtkomst till finansiella data, projekt och användare</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för de projekt som du vill budgetera information för med möjlighet att hantera finanser</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa information i resursplaneraren efter kostnad

Som standard visas tillgänglighets- och allokeringsinformationen i timmar i resursplaneraren.

Så här visar du tillgänglig, planerad och budgeterad information efter kostnad i resursplaneraren:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Resurser**.
1. Gå till Resursplaneraren.
1. (Villkorligt) Välj **Visa efter projekt** eller **Visa efter roll**.\
   Som standard **Visa efter projekt** är markerat.\
   Allokerings- och tillgänglighetsinformationen visas i timmar.

1. Från **Timmar** nedrullningsbar meny, välja **Kostnad**.

   Om du inte har åtkomst till finansiella data på din åtkomstnivå är det här alternativet inte tillgängligt.\
   Om projekt har en annan valuta än systemvalutan visas Kostnad för de här projekten i resursplaneraren, konverterad i systemets valuta. Systemadministratören definierar systemvalutan.\
   Mer information om hur du ställer in systemvalutan i Workfront och konverteringsgrader finns i [Ställ in valutakurser](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Beräkna tillgänglig kostnad i resursplaneraren

Om du vill visa tillgängliga kostnadsvärden i resursplaneraren måste du ha följande:

* Kostnad per timme för användare och roller
* Information om tillgänglighet för användare.

  Hur du får information om användartillgänglighet beror på hur Workfront-administratören konfigurerar inställningarna för resurshantering.\
  Mer information om hur du beräknar användartillgänglighet och anger inställningar för resurshantering finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Följande tabell visar hur den tillgängliga kostnaden beräknas i resursplaneraren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Tillgänglig kostnad</strong> </th> 
   <th><strong>Beräkning</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tillgänglig kostnad för användare</td> 
   <td> <p>Tillgänglig kostnad per användare beräknas med följande formel:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>ANMÄRKNING</b>

Om användaren inte har en kostnad per timme i sin profil används kostnaden per timme för den jobbroll som de är listade under i beräkningen. Om användaren inte har någon associerad roll är den tillgängliga användarkostnaden $0. </p> </td>
</tr> 
  <tr> 
   <td>Tillgänglig kostnad för roll</td> 
   <td> <p>Tillgänglig kostnad per roll beräknas med följande formel:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>ANMÄRKNING</b>

Om rollen inte har någon kostnad per timme är den tillgängliga rollkostnaden $0.</p> </td>
</tr> 
  <tr> 
   <td>Projektets tillgängliga kostnad</td> 
   <td> <p>Tillgänglig kostnad per projekt beräknas med följande formel:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Beräkna planerad kostnad i resursplaneraren

Även om du inte kan visa aktivitetsinformation i resursplaneraren beräknas de planerade kostnaderna för användare, roller och projekt med hänsyn till följande uppgiftsinformation:

* Typen av tilldelning för aktiviteten.\
  Du kan lämna en uppgift utan tilldelning eller tilldela följande entiteter till en uppgift:

   * En användare (med eller utan en jobbroll)
   * En roll
   * Ett team\
     En uppgift som tilldelats ett team betraktas som icke tilldelad, enligt resursplaneraren.

* The **Kostnadstyp** av projektets uppgifter.\
  Mer information om kostnadstypen för en uppgift finns i [Spåra kostnader](../../manage-work/projects/project-finances/track-costs.md).

<div class="preview">

* Giltiga datum för kostnadstarifferna för jobbroller och användare.

  Om rollen eller användaren till exempel har 10 planerade timmar i februari och 10 planerade timmar i mars, men kostnadsnivån har ändrats från 12 till 20 USD i mars, är värdet för den planerade kostnaden i februari 120 USD och i mars är den planerade kostnaden 200 USD.

</div>

>[!NOTE]
>
>Planerade kostnader för användare påverkar inte den planerade kostnaden för projektet. Endast de planerade kostnaderna för rollen påverkar de projektplanerade kostnaderna i resursplaneraren.

Följande scenarier används vid beräkning av planerad kostnad för användare, roller och projektet:

* När **Kostnadstyp** är **Användartimme **och det finns **ingen tilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     De planerade kostnaderna för roll och användare är $0,00.

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad är 0,00 USD.

* När **Kostnadstyp** är **Användare per timme** och det finns en **användartilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     Planerad kostnad för användare beräknas med följande formel:



     ```
     User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
     ```

     Om en användare har en kostnadstariff i sin profil används den taxan för att beräkna planerad kostnad. I annat fall används systemnivåkostnaden per timme för den primära rollen.

     >[!NOTE]
     >
     >Användaren kan tilldelas till uppgiften med en av de sekundära jobbrollerna, men i stället används den primära jobbrollens hastighet här.

     Den planerade kostnaden för roll beräknas med följande formel:

     ```
     Role Planned Cost = SUM(User Planned Cost)
     ```

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad är 0,00 USD.

* När **Kostnadstyp** är **Användare per timme** och det finns en **jobbrolltilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     Den planerade kostnaden för användaren är $0,00.

     Den planerade kostnaden för roll beräknas med följande formel:

     ```
     Role Planned Cost = Role Planned Hours * Role Cost per Hours
     ```

     Systemnivåkostnaden per timkostnad för den jobbroll som är tilldelad till aktiviteten används för att beräkna planerad kostnad.

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad är 0,00 USD.

* När **Kostnadstyp** är **Roll timvis** och det finns **ingen tilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     De planerade kostnaderna för roll och användare är $0,00.

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad är 0,00 USD.

* När **Kostnadstyp** är **Roll timvis** och det finns en **användartilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     Den planerade kostnaden för användaren är $0,00.

     Den planerade kostnaden för roll beräknas enligt följande formel:

     ```
     Role Planned Cost = Role Planned Hours * Role Cost per Hours
     ```

     Workfront tittar på den jobbroll som användaren utför i uppgiften för att beräkna den planerade kostnaden för rollen.

     Om användaren inte är associerad med någon roll i aktiviteten är den planerade kostnaden $0,00.

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad beräknas med följande formel:

     ```
     Project Planned Cost = SUM(Role Planned Costs)
     ```

* När **Kostnadstyp** är **Roll timvis** och det finns en **jobbrolltilldelning** på uppgiften:

   * **Roll och användarplanerad kostnad**:

     Den planerade kostnaden för användaren är $0,00.

     Den planerade kostnaden för roll beräknas enligt följande formel:

     ```
     Role Planned Cost = Role Planned Hours * Role Cost per Hours
     ```

     Workfront tittar på den jobbroll som användaren utför i uppgiften för att beräkna den planerade kostnaden för rollen.

   * **Planerad kostnad för projekt**:

     Projektets planerade kostnad beräknas med följande formel:

     ```
     Project Planned Cost = SUM(Role Planned Costs)
     ```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
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
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Beräkna budgeterad kostnad i resursplaneraren

Om du vill visa budgeterade kostnadsvärden i resursplaneraren måste du ha följande:

* Budgeterade timmar för roller, användare och projekt.
* Kostnad per timme för användare och roller.

>[!NOTE]
>
>De budgeterade timmarna för projekten beräknas utifrån de budgeterade timmarna för rollerna, inte användarnas.

Följande tabell visar hur budgeterad kostnad beräknas i resursplaneraren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Budgeterad kostnad</strong> </th> 
   <th><strong>Beräkning</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Användarbudgeterad kostnad</td> 
   <td> <p>Budgeterad kostnad per användare beräknas med följande formel:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>ANMÄRKNING</b>

Om användaren inte har en kostnad per timme i sin profil är den budgeterade användarkostnaden $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Roll budgeterad kostnad</td> 
   <td> <p>Rollens budgeterade kostnad beräknas med följande formel:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>ANMÄRKNING</b>

Om rollen inte har någon kostnad per timkostnad är den budgeterade rollkostnaden $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Projektbudgeterad kostnad</td> 
   <td> <p>Budgeterad kostnad per projekt beräknas med följande formel:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
