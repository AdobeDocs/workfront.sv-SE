---
title: Project Health - översikt
content-type: reference
description: Funktionen Project Health utnyttjar funktionerna i AI Assistant för att omedelbart ge dig en bild av hur dina projekt fungerar.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: d1ded406b8c4da975e2ff4d6825954cabd483ed2
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 0%

---

# Project Health - översikt

>[!IMPORTANT]
>
>Funktionen Project Health är för närvarande bara tillgänglig för användare som deltar i betatestet.

Adobe Workfront Project Health-funktion utnyttjar funktionerna i AI Assistant för att omedelbart ge dig en bild av hur dina projekt fungerar, vilka områden du behöver åtgärda och hur du undviker problem som kan kosta dig tid och pengar.

AI Assistant kan generera en Project Health-utvärdering för följande objekt:

* Ett enda projekt
* Ett enda program
* Flera projekt

Mer information om AI Assistant finns i [Översikt över AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Expandera om du vill visa åtkomstkraven. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Select, Prime eller Ultimate </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Administratör för att hantera Project Health-konfigurationer </p>
   <p>Redigera för att tillämpa Project Health-konfigurationer </p>
     <p>Visa för att visa Project Health-konfigurationer </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Delta i betaversionen av Project Health

Om du vill använda Project Health måste AI Assistant vara aktiverat i organisationen.

Om du vill aktivera AI Assistant och Projekthälsa för din organisation måste du göra något av följande:

* Din organisation måste ha migrerat till Adobe IMS (Identity Management System).
* Din organisation måste ha en Select-, Prime- eller Ultimate Workfront-plan
* Adobe Unified Experience måste aktiveras.
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands.
* Workfront-administratören måste aktivera AI-assistenten för användare i din organisation. AI Assistant aktiveras via åtkomstnivåer.
* Du måste markera alternativen Aktivera AI och Projekthälsa i AI-inställningarna under Inställningar > System > Inställningar.

  ![Avsnittet AI-inställningar](assets/ai-preferences.png)

Mer information finns i [Översikt över AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) och [Konfigurera systeminställningar](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## AI Assistant-frågelista

Nedan visas en lista med frågor som du kan använda för att be AI-utvärdering att generera en Project Health-bedömning för ett projekt, ett program eller alla projekt på ditt konto.

<table>
    <tr>
        <td><b>Plats</b></td>
        <td><b>Fråga</b></td>
    </tr>
    <tr>
        <td>En specifik projektinformationssida</td>
        <td><em>Hur är tillståndet?</em></td>
    </tr>
    <tr>
        <td>Alla sidor i Workfront </td>
        <td><em>Vad är tillståndet för projektet [PROJEKTNAMN]?</em></td>
    </tr>
    <tr>
        <td>Alla sidor i Workfront </td>
        <td><em>Vad är hälsan i mina projekt?</em></td>
    </tr>
       <tr>
        <td>En specifik programinformationssida</td>
        <td><em>Vad är programmets hälsa?</em></td>
    </tr>
       <tr>
        <td>Alla sidor i Workfront </td>
        <td><em>Hur är programmets [PROGRAM NAME] hälsa?</em></td>
    </tr>
   </table>


## Lista över projekt- och programvillkor

Nedan beskrivs de tillgängliga villkoren för att AI Assistant ska tilldela ditt projekt eller program när en Project Health-utvärdering genereras.

<table>
    <tr>
        <td><b>Projektvillkor</b></td>
        <td><b>Status för projektförlopp</b></td>
        <td><b>Projektvillkorsfaktorer</b></td>
    </tr>
    <tr>
        <td>På mål</td>
        <td>Denna analys tilldelas när den genomsnittliga risknivån för följande faktorer ligger inom det friska tröskelvärdet.
        </td>
        <td> 
        <ul><li>Krypning av omfång</li>
        <li>Saknade fält</li>
        <li>Schemalägg ändringar</li>
        <li>Underskattat arbete</li>
        <li>Projektförlopp</li>
        <li>Försenade uppgifter</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>Risk</td>
        <td>Denna analys tilldelas när den genomsnittliga risknivån för följande faktorer ligger precis under det friska tröskelvärdet.</td>
        <td>
        <ul><li>Krypning av omfång</li>
        <li>Saknade fält</li>
        <li>Schemalägg ändringar</li>
        <li>Underskattat arbete</li>
        <li>Projektförlopp</li>
        <li>Försenade uppgifter</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>I problem</td>
        <td>Denna analys tilldelas när den genomsnittliga risknivån för följande faktorer ligger under det friska tröskelvärdet.</td>
        <td>
        <ul><li>Krypning av omfång</li>
        <li>Saknade fält</li>
        <li>Schemalägg ändringar</li>
        <li>Underskattat arbete</li>
        <li>Projektförlopp</li>
        <li>Försenade uppgifter</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## Hantera Project Health-konfigurationer

En projekthälsokonfiguration innehåller specifika kriterier som avgör hur projektets hälsotillstånd beräknas. När en konfiguration har skapats kan du sedan använda den i ett projekt.

>[!NOTE]
>
>Du måste vara systemadministratör för att kunna hantera Project Health-konfigurationer.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** i den vänstra panelen och välj sedan **Projekthälsa** i listrutan som visas.

1. Välj **Ny konfiguration** i det övre högra hörnet på sidan.

1. (Valfritt) Ersätt *Namnlös konfiguration* med en ny konfiguration **Namn** på sidan med konfigurationsinformation.

1. I avsnittet **Vilka faktorer du vill ta med i projekthälsotillståndet** avmarkerar du de faktorer du inte vill ta med när du fastställer dina projekthälsovillkor:
   * **Omfångskrypning**: Hur mycket projektomfånget har utökats sedan det startades.

   * **Obligatoriska fält**: Om obligatoriska fält saknas (t.ex. projektbeskrivning). De här obligatoriska fälten avgör om projektet är klart och anges i **Vilka fält vill du kontrollera om det är fullständigt?Konfigurationsavsnittet** nedan.


   * **Schemaändringar**: Hur många schemaändringar som har gjorts sedan projektet startades.

   * **Uppgiftsuppskattning**: Hur exakt uppgiftsarbetet har uppskattats (t.ex. inga försenade aktiviteter för närvarande i projektet).

   * **Aktivitetsfel**: Hur projektarbetet fortskrider jämfört med projekttidslinjen.

   * **Försenade aktiviteter**: Hur många aktiviteter som för närvarande har passerat förfallodatumet.

   * **Kostnad**: Om projektet för närvarande överskrider budgeten.

1. I **När startar ditt projekt officiellt?** väljer du händelsen som signalerar början av projektet i listrutan.

1. I **Hur beräknar du omfattningen av arbetet i ett projekt?**-avsnitt, välj vilken projektfaktor som ska öka när projektomfånget ökar.

1. I **Vilka fält vill du kontrollera om de är fullständiga?**-avsnitt, markera ett eller flera fält som ska kontrolleras för att avgöra om projektet är klart.

   ![Fält för projektfullständighet](assets/project-completeness-fields.png)


1. Klicka på **Spara** längst upp till höger.

## Använd konfigurationer för projekthälsa

När en administratör har skapat en projekthälsokonfiguration kan användare med behörigheten Redigera använda den på ett projekt.


{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Klicka på ikonen **Mer** ![Mer ](assets/more-icon.png) till höger om projektnamnet och välj sedan **Redigera**. Sidpanelen **Redigera projekt** öppnas.

1. Välj **Projektinställningar** i den vänstra panelen.

1. I fältet **Projekthälsokonfiguration** väljer du den konfiguration som du vill använda för det här projektet.

   ![Konfigurationsfält för projekthälsa](assets/project-health-configurations.png)

1. Klicka på **Spara** i panelens nedre vänstra hörn.

## Generera en Project Health-utvärdering för ett projekt eller program

Om du har åtkomst till Visa för ett projekt eller program kan du generera en Project Health-utvärdering med hjälp av AI-assistenten.

Om du genererar en utvärdering för ett projekt kan du göra det antingen från projektsidan eller genom att referera till projektnamnet när du frågar assistenten hur projektet fungerar.

Om du genererar en utvärdering för ett program kan du göra det från sidan med programinformation.

>[!NOTE]
>
>Det går inte att generera en Project Health-utvärdering för ett projekt förrän projektet har startats. Du kan konfigurera vilka händelser som utlöser ett projekt så att det börjar i projektinställningarna.

Mer information finns i följande avsnitt i den här artikeln: [Hantera projekthälsokonfigurationer](#manage-project-health-configurations).

1. Navigera till det projekt eller program som du vill generera en Project Health-utvärdering för.

1. Klicka på ikonen **AI Assistant** ![AI Assistant](assets/ai-assistant-icon.png) i skärmens övre högra hörn på sidan med projekt-/programinformation. AI-assistenten öppnas.

1. Skriv följande i fältet **Fråga mig om Workfront**: *Vad är tillståndet för det här projektet?*

   eller

   Skriv följande i fältet **Fråga mig om Workfront**: *Vad är tillståndet för det här programmet?*

   >[!NOTE]
   >
   >Om du använder AI Assistant från en annan sida i Workfront kan du skriva *Vad är tillståndet för projektet [PROJEKTNAMN]?* eller *Vad är tillståndet för programmet [PROGRAM NAME]?* <br>
   >En fullständig lista över de aktuella uppmaningar du kan ange finns i följande avsnitt i den här artikeln: [AI Assistant-frågelistan](#ai-assistant-prompts-list).

1. Klicka på ikonen **Skicka** ![Skicka](assets/send-icon.png). Utvärderingen av projektets hälsotillstånd genereras och visas på panelen. Ett emblem visas högst upp i varje Project Health-bedömning, som avspeglar projektets aktuella tillstånd.

   ![Project Health Assessment](assets/health-assessment.png)

   Om du genererar en utvärdering för en portfölj visas flera märken som visar villkoret för varje projekt i programmet. Mer information om märkordsetiketter finns i följande avsnitt i den här artikeln: [Project and program conditions list](#project-and-program-conditions-list).

1. (Valfritt) Klicka på en av utvärderingspunkterna för att utöka detaljerna.

1. (Valfritt) I det utökade informationsläget klickar du på uppgiftslänken för att öppna uppgiftsinformationen.

   ![Utökad information](assets/expanded-details.png)

1. När du har granskat projekthälsoinformationen klickar du på ikonen **Stäng** ![Stäng ](assets/close-icon.png) i det övre högra hörnet av AI Assistant.

## Generera en Project Health-utvärdering för flera projekt

Du kan generera en kombinerad Project Health-utvärdering för alla projekt som du för närvarande har View-åtkomst (eller senare) för.

Ett projekt inkluderas bara i den kombinerade Project Health-bedömningen om projektet har startats. Du kan konfigurera vilka händelser som utlöser ett projekt så att det börjar i projektinställningarna. Mer information finns i följande avsnitt i den här artikeln: [Hantera projekthälsokonfigurationer](#manage-project-health-configurations).

1. Klicka på ikonen **AI-assistenten** ![AI-assistenten](assets/ai-assistant-icon.png) i skärmens övre högra hörn. AI-assistenten öppnas.

1. Skriv följande i **Fråga mig om Workfront-fältet**: *Vad är tillståndet för mina projekt?*

   En fullständig lista över de aktuella uppmaningar du kan ange finns i följande avsnitt i den här artikeln: [AI Assistant-frågelistan](#ai-assistant-prompts-list).

1. Klicka på ikonen **Skicka** ![Skicka](assets/send-icon.png). Utvärderingen av projektets hälsotillstånd genereras och visas på panelen.

   ![Utvärdering av flera projekt](assets/multiple-projects-assessment.png)

   När du genererar en utvärdering för flera projekt grupperar AI Assistant resultaten baserat på hur projekten för närvarande fungerar.

1. (Valfritt) Klicka på ett av projektets hälsovillkorsemblem för att expandera projektlistan och välj sedan en länk för ett visst projekt för att gå till informationssidan för det projektet.

1. När du har granskat projektens hälsoinformation klickar du på ikonen **Stäng** ![Stäng ](assets/close-icon.png) i det övre högra hörnet av AI Assistant för att stänga den.

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
