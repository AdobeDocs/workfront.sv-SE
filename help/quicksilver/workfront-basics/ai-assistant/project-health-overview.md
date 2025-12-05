---
title: Project Health - översikt
content-type: reference
description: Funktionen Project Health utnyttjar funktionerna i AI Assistant för att omedelbart ge dig en bild av hur dina projekt fungerar.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: b95be2e0917b53195ac327880a2ea7399c1485de
workflow-type: tm+mt
source-wordcount: '2060'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Markera eller högre </p> 
<p>Välj eller högre arbetsflöde</p>
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
   <td><p>Du måste vara systemadministratör för att kunna hantera Project Health-konfigurationer </p>
   <p>Redigera åtkomst till projekt för att använda Project Health-konfigurationer </p>
     <p>Visa åtkomst till projekt för att visa Project Health-konfigurationer </p>
     <p>Visa åtkomst till Program för att använda vyn Projekthälsa för alla projekt i ett program</p>
  </td> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td><p>Hantera behörigheter för projekt för att tillämpa Project Health-konfigurationer </p>
     <p>Visa behörigheter till projekt för att visa Project Health-konfigurationer </p>
  </td> 
  </tr> 
  </tr>  
    </tr>  
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Delta i betaversionen av Project Health

Din organisation måste ha AI Assistant aktiverat för att kunna använda Project Health.

Om du vill aktivera AI Assistant och Projekthälsa för din organisation måste du göra något av följande:

* Din organisation måste ha migrerat till Adobe Identity Management System (IMS).
* Din organisation måste ha ett Workfront- eller Workflow Select-, Prime- eller Ultimate-paket.
* Adobe Unified Experience måste aktiveras.
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands.
* Workfront-administratören måste aktivera AI-assistenten för användare i din organisation. AI Assistant aktiveras via åtkomstnivåer.
* Du måste markera alternativen Aktivera AI och Projekthälsa under AI-inställningar under Systeminställningar under Konfigurera.

  ![Avsnittet AI-inställningar](assets/ai-preferences.png)

Mer information finns i [Översikt över AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) och [Konfigurera systeminställningar](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Hur Project Health beräknas

AI Assistant ger dig en snabb bedömning av ett projekts övergripande tillstånd genom att tilldela det ett av de tillgängliga Project Health-lägena:

* På mål
* Risk
* I problem

Det här läget beräknas med projektkomponenter, som projektförlopp, underskattat arbete och mycket annat. En fullständig lista över de komponenter som används för att mäta Project Health finns i avsnittet [Lista över projekt- och programtillstånd](#project-and-program-states-list).

Varje projektkomponent tilldelas en numerisk riskpoäng som sträcker sig från (0-100), som sedan beräknas som ett genomsnitt för att skapa det övergripande Project Health-tillståndet:

* I mål (75 eller senare): Projektets prestanda ligger inom förväntat tröskelvärde.
* Risk (50-74): Nya fel som kan påverka projektets prestanda upptäcks.
* I problem (49 eller färre): Projektets prestanda ligger under godtagbara tröskelvärden och kräver omedelbar åtgärd.

>[!NOTE]
>
>* AI Assistant utvärderar för närvarande bara det valda projektets data.
>* Projekt- eller historikanalyser ingår ännu inte i beräkningen av projekthälsotillstånd.

### Exempel på beräkning av projekthälsotillstånd för ett projekt

I det första exemplet utvärderas fyra projektkomponenter och deras individuella riskpoäng beräknas enligt följande:

* 2 På mål (90 riskpoäng)
* 1 Vid risk (45 riskpoäng)
* 1 I Problem (20 riskpoäng)

När du räknar ut dessa poäng blir resultatet 61. Med hjälp av de ovan angivna kriterierna för Projekthälsa hamnar projektet i riskläge.

I nästa exempel har en schemaändring på 1 dag inträffat tidigt i projektets tidslinje. I det här scenariot utvärderar AI Assistant både tidpunkten för och effekten av ändringen i förhållande till projektets totala längd:

* En 1-dagars schemaläggning tidigt på en 60-dagars projekttidslinje är liten och räknas vanligtvis som På mål.
* En 1-dagars schemaläggning nära projektets slutförandedatum är mer störande och kan poängteras som Risk eller I Problem.

Eftersom ändringen var mindre och inträffade tidigt på projekttidslinjen placeras projektet i läget Vid mål.

Om flera schemaändringar inträffar inom ett projekts tidslinje, räknas dessa ändringar och beräknas sedan som medelvärden innan de tillämpas på beräkningen av projekthälsan.

## Förstå skillnaden mellan projektvillkor och projekthälsa

Projektvillkor och Projekthälsa är liknande begrepp i Workfront och har samma standardnamn som beskriver projektvillkoret eller projekttillståndet (Vid mål, Vid risk och I problem), men de har olika syften.

Projektvillkor ger en grundläggande ögonblicksbild av hur ett projekt för närvarande fungerar baserat enbart på planerade, planerade och beräknade datum. Den kan ställas in manuellt av projektägaren eller automatiskt av Workfront utifrån projektets uppgifter. Alternativt är Project Health mer omfattande och utvärderar ytterligare faktorer, vilket ger dig en bättre förståelse för hur det fungerar.

Mer information om projektvillkor finns i följande artiklar:

* [Uppdatera villkor för ett projekt](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-condition-on-project.md)
* [Anpassade villkor](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

## Project and program Project Health state list

Tabellen nedan innehåller en beskrivning av de tillgängliga lägena AI Assistant tilldelar ditt projekt eller program när du genererar en Project Health-utvärdering.

<table>
    <tr>
        <td><b>Projekttillstånd</b></td>
        <td><b>Definition</b></td>
        <td><b>Faktorer</b></td>
    </tr>
    <tr>
        <td>På mål</td>
        <td>Detta tilldelas när den genomsnittliga risknivån för följande faktorer ligger inom det friska tröskelvärdet.
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
        <td>Detta tilldelas när den genomsnittliga risknivån för följande faktorer ligger precis under det friska tröskelvärdet.</td>
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
        <td>Detta tilldelas när den genomsnittliga risknivån för följande faktorer ligger under det friska tröskelvärdet.</td>
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

## AI Assistant-frågelista

Nedan visas en lista med frågor som du kan använda för att be AI-assistenten att generera en Project Health-bedömning för ett projekt, ett program eller alla projekt som du har tillgång till att visa.

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

## Hantera Project Health-konfigurationer

Du måste vara systemadministratör för att kunna hantera Project Health-konfigurationer.

En projekthälsokonfiguration innehåller specifika kriterier som avgör hur projektets hälsotillstånd beräknas. När Workfront-administratören har skapat en konfiguration kan du sedan använda den i ett projekt.

Du kan ha flera Project Health-konfigurationer i systemet.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** i den vänstra panelen och välj sedan **Projekthälsa**.

1. Klicka på **Ny konfiguration** i det övre högra hörnet på sidan.

   Sidan **AI-inställningar** öppnas.

1. (Valfritt) Klicka i rubriken **Namnlös konfiguration** för att byta namn på konfigurationen.

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

1. I **Vilka vill du söka efter obligatoriska fält?**-avsnitt, markera ett eller flera fält som måste innehålla ett värde för projektet.

   ![Obligatoriska projektfält för projekthälsa](assets/project-completeness-fields.png)

1. Klicka på **Lägg till** i fler inbyggda eller anpassade projekt- eller aktivitetsfält.

1. Klicka på **Spara** längst upp till höger.

## Använd konfigurationer för projekthälsa

När Workfront-administratören har skapat en projekthälsokonfiguration kan du använda den i ett projekt om du har behörigheten Hantera i ett projekt.

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Klicka på ikonen **Mer** ![Mer &#x200B;](assets/more-icon.png) till höger om projektnamnet och välj sedan **Redigera**. Rutan **Redigera projekt** öppnas.

1. Klicka på **Projektinställningar** i den vänstra panelen.

1. I fältet **Projekthälsokonfiguration** väljer du den konfiguration som du vill använda för det här projektet.

   ![Konfigurationsfält för projekthälsa](assets/project-health-configurations.png)

1. Klicka på **Spara** längst ned till vänster på sidan.

## Generera en Project Health-utvärdering för ett projekt eller program

Du kan generera en Project Health-utvärdering från AI-assistenten inom följande områden:

* För ett projekt kan du generera utvärderingen antingen från projektsidan eller genom att referera till projektnamnet när du frågar assistenten hur ett visst projekt fungerar.

* För ett program kan du generera utvärderingen av programmets informationssida.

>[!NOTE]
>
>* Du behöver behörigheten Visa för projektet eller programmet för att kunna generera en utvärdering.
>* Det går inte att generera en Project Health-utvärdering för ett projekt förrän projektet har startats. Du kan konfigurera vilka händelser som utlöser ett projekt till att börja med i projektinställningarna

Mer information finns i avsnittet [Hantera projekthälsokonfigurationer](#manage-project-health-configurations) i den här artikeln.

Så här genererar du en Project Health-utvärdering för ett projekt eller program:

1. Navigera till det projekt eller program som du vill generera en Project Health-utvärdering för.

1. Klicka på ikonen **AI Assistant** ![AI Assistant](assets/ai-assistant-icon.png) i skärmens övre högra hörn på sidan med projekt-/programinformation. AI-assistenten öppnas.

1. Skriv följande i fältet **Fråga mig om Workfront**: *Vad är tillståndet för det här projektet?*

   eller

   Skriv följande i fältet **Fråga mig om Workfront**: *Vad är tillståndet för det här programmet?*

   >[!NOTE]
   >
   >Om du använder AI Assistant från en annan sida i Workfront kan du skriva *Vad är tillståndet för projektet [PROJEKTNAMN]?* eller *Vad är tillståndet för programmet [PROGRAM NAME]?* <br>
   >En fullständig lista över de aktuella uppmaningar du kan ange finns i avsnittet [AI Assistant-frågelista](#ai-assistant-prompts-list) i den här artikeln.

1. Klicka på ikonen **Skicka** ![Skicka](assets/send-icon.png). Utvärderingen av projektets hälsotillstånd genereras och visas på panelen. Ett emblem visas högst upp i varje Project Health-bedömning, som avspeglar projektets aktuella tillstånd.

   ![Project Health Assessment](assets/health-assessment.png)

   Om du gör en utvärdering för ett program visas flera märken som visar villkoret för varje projekt i programmet. Mer information om märkordsetiketter finns i avsnittet [Project and program states list](#project-and-program-states-list) i den här artikeln.

1. (Valfritt) Klicka på en av utvärderingspunkterna för att utöka detaljerna.

1. (Valfritt) Klicka på projektlänken i det utökade informationsläget för att öppna projektinformationen.

   ![Utökad information](assets/expanded-details.png)

1. När du har granskat projekthälsoinformationen klickar du på ikonen **Stäng** ![Stäng &#x200B;](assets/close-icon.png) i det övre högra hörnet av AI Assistant.

## Generera en Project Health-utvärdering för flera projekt

Du kan generera en kombinerad Project Health-utvärdering för alla projekt som du har vybehörighet för eller högre.

Ett projekt inkluderas bara i den kombinerade Project Health-bedömningen om projektet har startats. Du kan konfigurera vilka händelser som utlöser ett projekt så att det börjar i projektinställningarna. Mer information finns i avsnittet [Hantera projekthälsokonfigurationer](#manage-project-health-configurations) i den här artikeln.

1. Klicka på ikonen **AI-assistenten** ![AI-assistenten](assets/ai-assistant-icon.png) i skärmens övre högra hörn. AI-assistenten öppnas.

1. Skriv följande i **Fråga mig om Workfront-fältet**: *Vad är tillståndet för mina projekt?*

   En fullständig lista över de aktuella uppmaningar du kan ange finns i följande avsnitt i den här artikeln: [AI Assistant-frågelistan](#ai-assistant-prompts-list).

1. Klicka på ikonen **Skicka** ![Skicka](assets/send-icon.png). Utvärderingen av projektets hälsotillstånd genereras och visas på panelen.

   ![Utvärdering av flera projekt](assets/multiple-projects-assessment.png)

   När du genererar en utvärdering för flera projekt grupperar AI Assistant resultaten baserat på hur projekten för närvarande fungerar.

1. (Valfritt) Klicka på ett av projektets hälsovillkorsemblem för att expandera projektlistan och välj sedan en länk för ett visst projekt för att gå till informationssidan för det projektet.

1. När du har granskat projektens hälsoinformation klickar du på ikonen **Stäng** ![Stäng &#x200B;](assets/close-icon.png) i det övre högra hörnet av AI Assistant för att stänga den.

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
