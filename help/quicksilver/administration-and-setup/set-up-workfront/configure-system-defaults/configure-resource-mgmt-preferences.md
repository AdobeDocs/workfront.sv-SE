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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Resource Management] inställningar

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Som en [!DNL Adobe Workfront] administratör du kan konfigurera [!UICONTROL Resource Management] Inställningar för systemet. De här inställningarna bestämmer hur användartillgänglighet eller -kapacitet och FTE beräknas för [!DNL Workfront] planerings- och planeringsverktyg för resurser.

Mer information om planering och planering av resurser finns i [!DNL Workfront], se [Kom igång med resurshantering](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Åtkomstkrav

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
   <td> <p>Åtkomstnivå för systemadministratör</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera [!UICONTROL Resource Management] inställningar

>[!NOTE]
>
>Eftersom det här är en global inställning påverkar det här valet alla beräkningar för hela systemet, för alla användare, i alla resurshanteringsverktyg och för alla resurspooler.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på **[!UICONTROL Resource Management]**.
1. Välj en av följande metoder för att beräkna tillgängligheten för användare i [!DNL Workfront]:

   * **Standardschema**: [!DNL Workfront] använder systemets standardschema och användarens enskilda FTE för att beräkna användarens tillgängliga timmar i resurshanteringsverktygen.\

      Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Mer information om värdet för användarens FTE finns i  [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront beräknar tillgängliga timmar för en användare med följande formel när Workfront-administratören väljer Standardschema:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Exempel:**\
      Om till exempel standardschemat är 40 timmar i veckan och FTE i användarens profil är 0,5, kan användaren arbeta 20 timmar i veckan.

      Om användaren har en timmes tid på en dag beräknas deras tillgängliga timmar enligt följande:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **Användarens schema**: [!DNL Workfront] använder användarens schema samt systemets standardschema för att beräkna användarens tillgängliga FTE-värde i resurshanteringsverktygen. Tillgängliga timmar beräknas endast enligt användarens schema. Värdet för användarens FTE ignoreras. Det här är standardinställningen.

      >[!NOTE]
      >
      >Om användaren inte är associerad med ett schema beräknas användarens tillgängliga timmar med hjälp av standardschemat.

      Tillgänglig heltidsanställd för användaren beräknas enligt följande formel:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Exempel:** Om till exempel standardschemat är 40 timmar i veckan och användarens schema är 30 timmar i veckan, är FTE för användaren 0,75.

      Om användaren har två timmars Tid på en dag beräknas deras Veckovisa tillgängliga heltid enligt följande:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Klicka på **[!UICONTROL Save]**.
