---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Konfigurera inställningar för resurshantering
description: Som  [!DNL Adobe Workfront] administratör kan du konfigurera inställningarna för resurshantering för ditt system. De här resurshanteringsinställningarna avgör hur användartillgänglighet eller -kapacitet och FTE beräknas för  [!DNL Workfront] resursplanerings- och planeringsverktygen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Konfigurera inställningar för [!UICONTROL Resource Management]

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Som [!DNL Adobe Workfront]-administratör kan du konfigurera [!UICONTROL Resource Management] -inställningarna för systemet. De här inställningarna bestämmer hur användarens timma eller FTE-tillgänglighet eller kapacitet beräknas för resursplanerings- och planeringsverktygen i [!DNL Workfront].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Information som beaktas vid beräkning av en användares kapacitet

Vid beräkning av en användares kapacitet tar Workfront hänsyn till följande information:

* Antalet schemalagda timmar, enligt definition i antingen användarens schema eller Workfront-systemets standardschema.
* Schemalägg undantag (beroende på vilket schema som används kan det vara undantagen i användarens schema eller undantagen som är kopplade till Workfront standardschema).
* Användaren är ledig.
* Värdet för heltidsmotsvarigheten ([!UICONTROL FTE]) för användaren eller för systemet [!DNL Workfront]. [!UICONTROL FTE] är lika med 1 när användaren arbetar heltid, enligt schemats definition.
* Värdet [!UICONTROL Work Time] för användaren, som refererar till den tid som användaren lägger på projektrelaterat arbete. Detta inkluderar inte overheadtid, som möten och utbildning. [!UICONTROL Work Time] är lika med 1 när användaren är tillgänglig för arbete under hela den tid som anges av [!UICONTROL FTE] eller schemat, vilket innebär att användaren inte spenderar någon tid på icke-projektrelaterade arbeten som möten eller utbildningar.


Mer information om planering och planering av resurser i [!DNL Workfront] finns i [Kom igång med resurshantering](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Konfigurera inställningar för [!UICONTROL Resource Management]

>[!NOTE]
>
>Eftersom det här är en global inställning påverkar det här valet alla beräkningar för hela systemet, för alla användare, i alla resurshanteringsverktyg.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Resource Management]**.
1. Välj en av följande metoder för att beräkna tillgängligheten för användare i [!DNL Workfront]:

   * **Standardschemat**: [!DNL Workfront] använder systemets standardschema och användarens enskilda FTE för att beräkna användarens tillgängliga timmar i resurshanteringsverktygen.

     Mer information finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) och [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     När det här alternativet är markerat beräknas användarens tillgängliga timmar enligt följande formel:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Om till exempel standardschemat är 40 timmar per vecka är FTE i användarens profil 0,5, användaren har en timmes tid på en dag och [!UICONTROL Work Time] i användarens profil är 0,5 och användaren är tillgänglig för faktiskt projektarbete i 9,5 timmar per vecka.
     >
     >Om användaren har en timmes tid på en dag beräknas deras tillgängliga timmar enligt följande:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--
      This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
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

   * **Användarens schema**: [!DNL Workfront] använder användarens schema samt [!UICONTROL Default Schedule] i systemet för att beräkna det tillgängliga [!UICONTROL FTE]-värdet för användaren i verktygen för resurshantering.   Tillgängliga timmar beräknas endast enligt användarens schema, och värdet för [!UICONTROL FTE] för användaren ignoreras. Det här är standardinställningen.

     Mer information finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) och [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Om användaren inte är associerad med ett schema beräknas användarens tillgängliga timmar endast med [!UICONTROL Default Schedule].

     Tillgängliga timmar för användaren beräknas enligt följande formel:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Tillgängliga [!UICONTROL FTE] för användaren beräknas med följande formel:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Om till exempel [!UICONTROL Default Schedule] är 40 timmar i veckan är användarens schema 30 timmar i veckan, användarens [!UICONTROL Work Time] är 0,5 och användarens [!UICONTROL FTE] är 0,35.
     >
     >Om användaren har två timmars tid på en dag, beräknas deras [!UICONTROL FTE] som tillgängligt varje vecka enligt följande:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

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
