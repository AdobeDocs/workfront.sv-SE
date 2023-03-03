---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Konfigurera inställningar för resurshantering
description: Som en [!DNL Adobe Workfront] kan du konfigurera inställningarna för resurshantering för ditt system. De här resurshanteringsinställningarna avgör hur användartillgänglighet eller -kapacitet och FTE beräknas för [!DNL Workfront] planerings- och planeringsverktyg för resurser.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Resource Management] inställningar

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Som en [!DNL Adobe Workfront] administratör du kan konfigurera [!UICONTROL Resource Management] Inställningar för systemet. Dessa inställningar avgör hur tillgängligheten eller kapaciteten för användartimmar eller FTE beräknas för [!DNL Workfront] planerings- och planeringsverktyg för resurser.

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Åtkomstnivå för systemadministratör</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>:

Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Information som beaktas vid beräkning av en användares kapacitet

Vid beräkning av en användares kapacitet tar Workfront hänsyn till följande information:

* Antalet schemalagda timmar, enligt definition i antingen användarens schema eller Workfront-systemets [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (beroende på vilken [!UICONTROL Schedule] används, det kan vara undantagen i användarens schema eller de som är kopplade till [!DNL Workfront] [!UICONTROL Default Schedule])
* Användarens lediga tid
* Värdet för heltidsmotsvarigheten ([!UICONTROL FTE]) för användaren eller [!DNL Workfront] system. The [!UICONTROL FTE] är lika med 1 när användaren arbetar heltid, enligt schemat.
* Värdet för [!UICONTROL Work Time] för användaren som refererar till den tid som användaren lägger på projektrelaterat arbete. Detta inkluderar inte overheadtid, som möten och utbildning. The [!UICONTROL Work Time] är lika med 1 när användaren är tillgänglig för arbete under hela den tid som anges av [!UICONTROL FTE] eller schemat, vilket innebär att de inte spenderar någon tid på icke-projektrelaterade arbeten som möten eller utbildningar.


Mer information om planering och planering av resurser finns i [!DNL Workfront], se [Kom igång med resurshantering](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Konfigurera [!UICONTROL Resource Management] inställningar

>[!NOTE]
>
>Eftersom det här är en global inställning påverkar det här valet alla beräkningar för hela systemet, för alla användare, i alla resurshanteringsverktyg.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på **[!UICONTROL Resource Management]**.
1. Välj en av följande metoder för att beräkna tillgängligheten för användare i [!DNL Workfront]:

   * **Standardschema**: [!DNL Workfront] använder systemets standardschema och användarens enskilda FTE för att beräkna användarens tillgängliga timmar i resurshanteringsverktygen.

      Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Mer information om hur du hittar värdet för användarens [!UICONTROL FTE], se  [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront beräknar tillgängliga timmar för en användare med följande formel när Workfront-administratören väljer [!UICONTROL Default Schedule]:

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]
      ```

      >[!INFO]
      >
      >Om till exempel standardschemat är 40 timmar per vecka är FTE i användarens profil 0,5, användaren har en timmes tid på en dag och [!UICONTROL Work Time] i användarens profil är 0,5, användaren är tillgänglig för faktiskt projektarbete i 9,5 timmar i veckan.
      >
      >Om användaren har en timmes tid på en dag beräknas deras tillgängliga timmar enligt följande:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



      <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **Användarens schema**: [!DNL Workfront] använder användarens schema samt [!UICONTROL Default Schedule] för systemet för att beräkna tillgängliga [!UICONTROL FTE] värdet för användaren i resurshanteringsverktygen. Tillgängliga timmar beräknas endast enligt användarens schema. Värdet för [!UICONTROL FTE] av användaren ignoreras. Det här är standardinställningen.

      Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Mer information om en användares [!UICONTROL Schedule], se  [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Om användaren inte är associerad med ett schema beräknas användarens tillgängliga timmar endast med [!UICONTROL Default Schedule].

      Tillgängliga timmar för användaren beräknas enligt följande formel:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      Tillgängliga [!UICONTROL FTE] för användaren beräknas med följande formel:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Om [!UICONTROL Default Schedule] är 40 timmar per vecka, användarens schema är 30 timmar per vecka och användarens [!UICONTROL Work Time] är 0,5 [!UICONTROL FTE] för användaren är 0,35.
      >
      >Om användaren har två timmars tid ledig från en dag, är hans/hennes Vecka tillgänglig [!UICONTROL FTE] beräknas enligt följande:
      >
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35
      >```

      <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Klicka på **[!UICONTROL Save]**.
