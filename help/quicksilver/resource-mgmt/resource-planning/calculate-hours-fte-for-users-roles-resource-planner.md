---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren
description: Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Översikt över beräkning av timmar och heltidsekvivalent för användare och roller i resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Du kan visa allokeringen och tillgängligheten för dina resurser i resursplaneraren efter timmar, heltid eller kostnad.\
Mer information om hur du beräknar kostnader i resursplaneraren finns i [Beräkna kostnader i resursplaneraren](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; står för&quot;Full Time Equivalent&quot;. Det är ett tidsmått som representerar antalet timmar som är dedikerade till verkligt arbete under en dag eller vecka för en användare eller jobbroll.

Följande uppsättningar med resursinformation beräknas annorlunda i resursplaneraren:

* Tillgängliga timmar eller FTE-värden beräknas utifrån hur systemadministratören konfigurerar inställningarna för resurshantering i systemet.\
  Mer information om hur värdena Tillgängliga timmar och FTE beräknas finns i [Beräkna tillgängliga timmar eller heltidsanställda för användare och jobbroller i resursplaneraren](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Mer information om hur du definierar inställningar för resurshantering i Adobe Workfront-systemet finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Alla andra FTE-värden beräknas baserat på systemets standardschema.\
  Mer information om hur alla andra värden visas i resursplaneraren när du använder FTE finns i avsnittet [Beräkna alla andra timma- och FTE-värden för användare och jobbroller i resursplaneraren](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) i den här artikeln.

Det är viktigt att förstå vad FTE är för var och en av dina användare och deras jobbroller för att hantera dina resurser korrekt när du tilldelar dem till arbetet.

## Beräkna tillgängliga timmar eller heltidsanställda för användare och jobbroller i resursplaneraren {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Beräkna tillgängliga timmar och heltidsanställda för en användare i resursplaneraren](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Beräkna tillgängliga timmar och heltidsanställda för en jobbroll i resursplaneraren](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Beräkna tillgängliga timmar och heltidsanställda för en användare i resursplaneraren (exempel)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Beräkna tillgängliga timmar och heltidsanställda för en användare i resursplaneraren {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront-administratören avgör hur den tillgängliga tiden för en användare beräknas genom att välja att använda något av följande i området Resurshantering i installationsprogrammet:

* Standardschemat för systemet och användarens FTE.
* Användarens schema.

Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### Beräkna tillgängliga timmar och heltidsanställda för en jobbroll i resursplaneraren {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Först måste du beräkna användartillgängligheten och sedan kan du beräkna tillgängligheten för varje jobbroll.

Tillgängligheten av jobbroller i resursplaneraren tar hänsyn till användarens totala tillgänglighet och **Procent tillgängliga heltidsanställda** associeras med användarens roll.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Mer information om hur du associerar en **Procent tillgängliga heltidsanställda** värde med en jobbroll för en användare, se [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Om värdet för Tillgängliga timmar för en användare till exempel är 40 och de kan fylla en primär roll för 75 % av den tiden, och en annan roll för 25 % av den tiden, visar resursplaneraren att **Tillgängliga timmar** värdet för den primära rollen för en vecka är 30 timmar och att **Tillgängliga timmar** Värdet för den andra rollen är 10 timmar. I det här fallet är heltidsanställda för den primära rollen 0,75 och heltidsanställda för den andra rollen 0,25.

>[!NOTE]
>
>Den totala tillgängliga tiden för användaren beräknas med någon av de två metoder som beskrivs i [Beräkna tillgängliga timmar och heltidsanställda för en användare i resursplaneraren](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) i den här artikeln.

När du visar resursplaneraren i rollvyn är tillgängligheten för en jobbroll en total tillgänglighet för alla användare som kan slutföra den jobbrollen.\
Mer information om tillgängliga resurser i resursplaneraren finns i [Översikt över resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Beräkna tillgängliga timmar och heltidsanställda för en användare i resursplaneraren (exempel) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Följande tabell visar hur Tillgängliga timmar och Tillgängliga FTE beräknas för användaren i resursplaneraren, beroende på vilken metod som används av systemadministratören för FTE-beräkningen i Resurshanteringsinställningar.

I det här exemplet använder vi följande tal:

* Ett standardschema för system på 40 timmar
* Ett användarschema på 20 timmar
* En användares FTE på 0,75

| Metod för FTE-beräkning (systeminställning) | **Timmar från användarens schema** | **Timmar från standardschemat** | **FTE-fält för användare** | **Tillgängliga timmar i resursplaneraren** | **Tillgänglig heltidsanställd i resursplaneraren** |
|---|---|---|---|---|---|
| **Standardschema** | Ignorerad | 40 | 0.75 | **30** (beräknat) | **0.75** |
| **Användarens schema** | 20 | 40 | Ignorerad | **20** | **0,5** (beräknat) |

Schemalagda undantag och ledig tid kan påverka antalet planerade timmar eller heltidsanställda. Mer information finns i [Konfigurera inställningar för resurshantering](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Beräkna alla andra timma- och FTE-värden för användare och jobbroller i resursplaneraren {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Förutom Tillgängliga timmar eller FTE visas även följande tidsinformation i resursplaneraren:

* Planerade timmar
* Budgeterade timmar
* Timavvikelse
* Nettotimmar\
  Mer information om dessa värden finns i [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Timskillnad\
  Mer information om vad det här värdet representerar finns i [Översikt över timmar, heltidsekvivalenter och kostnadsinformation i projekt- och rollvyerna i resursplaneraren](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Du kan visa samma information i resursplaneraren som FTE eller som timmar.

Workfront använder följande formel för att visa alla andra värden som FTE i resursplaneraren:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>Användarens schema ignoreras vid beräkning av FTE för alla värden utom för tillgängliga (AVL) FTE-värden i resursplaneraren. Endast standardschemat tas med i beräkningen.

Denna beräkning gäller följande värden:

* Planerad heltidsekvivalent (zloty)
* Budgeterad heltidsanställd personal (BDG)
* FTE-avvikelse (VAR)
* NET FTE
* FTE-differens (DIF)
