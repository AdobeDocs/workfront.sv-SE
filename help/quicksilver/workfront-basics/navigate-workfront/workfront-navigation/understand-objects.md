---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Översikt över [!DNL Adobe Workfront] objekt
description: Den information du visar i  [!DNL Adobe Workfront]  representeras av objekt som lagras i  [!DNL Workfront] databasen. Objekten är vad som driver informationen i  [!DNL Workfront]. Läs mer om dessa objekt i den här artikeln.
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '2133'
ht-degree: 0%

---

# Översikt över [!DNL Adobe Workfront] objekt

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Den information du visar i [!DNL Adobe Workfront] representeras av objekt som lagras i databasen [!DNL Workfront]. Objekten är de som driver informationen i [!DNL Workfront].

Det är viktigt att du förstår hur objekten definieras i [!DNL Workfront] så att du kan använda rätt objekt för de behov som finns i organisationen.

Om du till exempel planerar en stor mängd arbete måste du använda objektet [!UICONTROL Project] för att definiera det arbetet. Om du vill dela upp arbetet i mindre planerade steg kan du använda objektet [!UICONTROL Task]. För en mindre mängd arbete som inte är planerat och som kan utföras oväntat kan du använda objektet Utgåva. Om du vill spåra förloppet och anslutningen till budgeten och tidslinjen för en grupp projekt kan du ordna dem i [!UICONTROL Portfolios] och [!UICONTROL Programs]. Om du vill definiera andra element som kan hjälpa dig att lösa ditt arbete, vill du använda andra objekt som lagras under [!UICONTROL Projects], [!UICONTROL Tasks], [!UICONTROL Issues] eller [!UICONTROL Portfolios], som [!UICONTROL Documents], [!UICONTROL Updates], [!UICONTROL Hours], [!UICONTROL Users] eller [!UICONTROL Job Roles].

[!UICONTROL Reports] och [!UICONTROL Dashboards] är ett annat exempel på objekt som kan hjälpa dig att ordna den datamängd du har i [!DNL Workfront] visuellt, så att den blir lättillgänglig för alla användare.

En fullständig lista över objekt i [!DNL Workfront] finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

## Objektens inbördes beroende och hierarki

Objekt är länkade till varandra i [!UICONTROL Workfront]. En aktivitet eller ett problem kan till exempel aldrig finnas oberoende utanför ett projekt. [!UICONTROL Tasks] och [!UICONTROL issues] är exempel på objekt som lagras i objektet [!UICONTROL project]. [!UICONTROL Tasks] och [!UICONTROL issues] betraktas som underordnade objekt till projekt.

Följande är några av de vanligaste objekten i [!DNL Workfront] och deras respektive överordnade och underordnade objekt:

| **Objekt** | **Överordnade objekt** | **Underordnade objekt** |
|---|---|---|
| [!UICONTROL Portfolios] |  | [!UICONTROL Programs], [!UICONTROL Projects], [!UICONTROL Documents], [!DNL Notes], [!UICONTROL Users] |
| [!UICONTROL Programs] | [!UICONTROL Portfolios] | [!UICONTROL Projects], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Users] |
| [!UICONTROL Projects] | [!UICONTROL Portfolios], [!UICONTROL Programs] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Tasks] | [!UICONTROL Projects] | [!UICONTROL Issues], [!UICONTROL Children Tasks], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Issues] | [!UICONTROL Tasks], [!UICONTROL Projects] | [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Dashboards] |  | [!UICONTROL Reports], externa sidor |
| [!UICONTROL Reports] | [!UICONTROL Dashboards] |  |
| [!UICONTROL Groups] |  | [!UICONTROL Users] |
| [!UICONTROL Teams] |  | [!UICONTROL Users] |
| [!UICONTROL Users] | [!UICONTROL Groups], [!UICONTROL Teams], [!UICONTROL Companies] | [!UICONTROL Job Roles] |
| [!UICONTROL Companies] |  | [!UICONTROL Users] |
| [!UICONTROL Documents] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Projects], [!UICONTROL Portfolios], [!UICONTROL Programs], [!UICONTROL Users] |  |
| [!UICONTROL Plans]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Results], [!UICONTROL Activities] |

En fullständig lista över objekt i [!DNL Workfront] finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

*Planer är objekt för [!DNL Adobe Workfront Scenario Planner]. Mer information om [!DNL Scenario Planner] finns i [Översikt [!UICONTROL Scenario Planner]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Goals] är objekten i [!DNL Adobe Workfront Goals]. Mer information om [!DNL Workfront Goals] finns i [[!DNL Adobe Workfront Goals] översikt](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Anpassa objektnamn

Som [!DNL Workfront]-administratör kan du anpassa objektnamn i [!DNL Workfront] genom att använda en [!UICONTROL Layout Template] .

Mer information om hur du anpassar objektnamn med en [!UICONTROL Layout Template] finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

När du har anpassat en layoutmall och tilldelat den till användare, ser dessa användare de anpassade namnen för objekten. De användare som har tilldelats layoutmallen ser inte längre standardnamnen för objekten någonstans i webbprogrammet.

Om den större mängden arbete i organisationen till exempel kallas för engagemang kan du ersätta namnet [!UICONTROL Project] med Engagement. Gränssnittet [!DNL Workfront] visar&quot;Engagement&quot; i stället för [!UICONTROL Project] överallt där namnet [!UICONTROL Project] skulle visas.

>[!NOTE]
>
>För att de nya namnen på objekten ska vara synliga för dina användare måste de logga ut och logga in på [!DNL Workfront] igen när du har sparat [!UICONTROL Layout Template].

>[!IMPORTANT]
>
>[!DNL Workfront]-dokumentationen refererar alltid till objektens standardnamn. Som [!DNL Workfront]-administratör måste du informera användarna om ändringarna i objektnamnen, så att de kan förstå hur [!DNL Workfront] -dokumentationen ska användas, samt vilka områden i programmen som inte återspeglar ändringarna i objektnamnen.

* [Objektnamn som kan anpassas med en [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template)
* [Områden av  [!DNL Workfront] som återspeglar de anpassade objektnamnen](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Områden av  [!DNL Workfront] som inte återspeglar de anpassade objektnamnen](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Objektnamn som kan anpassas med en [!UICONTROL Layout Template]

Som [!DNL Workfront]-administratör kan du anpassa namnen på följande objekt så att de matchar terminologin i din organisation:

* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Issue]
* [!UICONTROL Goal]*
* [!UICONTROL Result]*
* [!UICONTROL Activity]*

  *[!UICONTROL Goals], [!UICONTROL results] och [!UICONTROL activities] är bara tillgängliga om ditt företag har köpt [!DNL Workfront Goals]. Mer information om [!DNL Workfront Goals] finns i [[!DNL Adobe Workfront Goals] översikt](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scenario]**
* [!UICONTROL Plan]**

  **[!UICONTROL Initiatives], [!UICONTROL scenarios] och [!UICONTROL plans] är bara tillgängliga om ditt företag har köpt [!DNL Workfront Scenario Planner]. Mer information om [!DNL Scenario Planner] finns i [Kom igång med  [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Mer information om hur du kan anpassa objektnamn med [!UICONTROL Layout Templates] finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Du kan inte anpassa namnen på andra objekt i Workfront. En fullständig lista över objekt i [!DNL Workfront] finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

När du anpassar namnet på ett objekt visas det nya namnet för det objektet i de flesta områden i [!DNL Workfront]-programmet där objektnamnet skulle visas.

### Områden av [!DNL Workfront] som återspeglar de anpassade objektnamnen

I följande områden visas det uppdaterade namnet på objekten:

* Övre navigering
* Alla avsnitt i den vänstra panelens navigering
* Alla menyer
* Meddelanden i appen
* Report builder och rapportelement (vyer, filter och grupperingar)
* [!UICONTROL Save] knappar
* Exporterade filer
* E-post
* Mobilappar

### Områden av [!DNL Workfront] som inte återspeglar de anpassade objektnamnen

I följande områden visas inte objektens uppdaterade namn:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook]-tillägg

### Konsekvenser av anpassning av objektnamn

Du bör vara medveten om följande när du anpassar objektnamn i [!DNL Workfront]:

* Du kan stöta på stilistiska eller grammatiska fel på systemskärmar. Om du t.ex. byter namn på [!UICONTROL Issue] till Request och du någonstans i systemet ser frasen An request, fungerar detta som det ska och bör inte betraktas som ett fel.
* Dina anpassade namn för objekten är inte översättningsbara. Endast standardnamnen [!DNL Workfront] kan översättas på de språk som stöds. Mer information om språk som stöds i [!DNL Workfront] finns i [Språk som stöds i [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). De anpassade objektnamnsfälten har stöd för främmande tecken så att du kan ange terminologi på vilket språk som helst.
* När du anpassar objektnamn med en [!UICONTROL Layout Template] rekommenderar vi att du tilldelar din [!UICONTROL Layout Templates] baserat på dina affärsenheter (team eller grupper).\
   Vi rekommenderar att du använder namn som är tydligt begripliga för användarna av dessa affärsenheter för att undvika förvirring.
* E-postmeddelanden och levererade rapporter innehåller alltid objektnamn som definieras av [!UICONTROL Layout Template] för den användare som genererar e-postmeddelandet. Dina användare bör vara förberedda på att se objektnamn i sina e-postmeddelanden som inte är relaterade till deras grupp eller team, om de får e-postmeddelanden från användare i andra team och grupper.\
   Som [!DNL Workfront]-administratör bör du råda användarna att lägga märke till de ikoner som är associerade med varje objekt. Ikonerna är desamma för olika objektnamn och överensstämmer med standardobjektet så som det visas i databasen. En lista med alla [!DNL Workfront] ikoner som är associerade med objekt finns i [Objektikoner](#object-icons).

  >[!TIP]
  >
  >För vanliga uppgifter i organisationen bör du överväga att skapa anpassad dokumentation som återspeglar din terminologi.

## Objektikoner

[!DNL Workfront]-dokumentationen refererar alltid till objektens standardnamn. Om objektens namn har anpassats kan du förlita dig på den ikon som är associerad med dem för att förstå vilket anpassat objekt som motsvarar [!DNL Workfront] standardobjekt.

Mer information om vilka objekt som kan ha anpassade namn i [!DNL Workfront] finns i [Objektnamn som kan anpassas med en [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).

Här följer en lista med objekt och motsvarande ikoner för dem i Workfront.

| **Objekt** | **Ikon** | **Anpassningsbart objektnamn** |
|---|---|---|
| [!UICONTROL Company] | ![](assets/company-icon-nwe.png), ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png), ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Goal] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Group] | ![](assets/groups-icon-nwe.png), ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Issue] | ![](assets/issue-icon-nwe.png), ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Job Role] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png), ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Program] | ![](assets/program-icon-nwe.png), ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Project] | ![](assets/project-icon-nwe.png), ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Report] | ![](assets/report-icon-nwe.png), ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Task] | ![](assets/task-icon-new.png), ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png), ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Template] | ![](assets/template-icon-nwe.png), ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL User] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## Referensnummer för objekt

Varje objekt som skapas i [!DNL Workfront] tilldelas ett unikt referensnummer. Referensnummer är användbara när du ska skilja mellan två i övrigt liknande objekt (till exempel uppgifter med samma namn). Du kan söka efter objekt med hjälp av deras referensnummer och du kan inkludera referensnummer i rapporter.

Mer information om hur du söker efter objekt efter referensnummer finns i [Använda referensnummer för objekt](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Objektspecifika sökningar

Du kan söka bland alla objekt som är sökbara i [!DNL Workfront] eller välja ett specifikt objekt att söka efter i dina grundläggande och avancerade sökningar.

Alla objekt är inte sökbara i [!DNL Workfront]. Du kan köra enkla och avancerade sökningar för följande objekt i [!DNL Workfront]:

| **Objekt** | **Grundläggande sökning** | **Avancerad sökning** |
|---|---|---|
| [!UICONTROL Projects] | ✓ | ✓ |
| [!UICONTROL Tasks] | ✓ | ✓ |
| [!UICONTROL Issues] | ✓ | ✓ |
| [!UICONTROL Reports] | ✓ | ✓ |
| [!UICONTROL Users] | ✓ | ✓ |
| [!UICONTROL Templates] | ✓ | ✓ |
| [!UICONTROL Documents] | ✓ | ✓ |
| [!UICONTROL Portfolios] | ✓ | ✓ |
| [!UICONTROL Programs] | ✓ | ✓ |
| [!UICONTROL Dashboards] | ✓ | ✓ |
| [!UICONTROL Companies] | ✓ | ✓ |
| [!UICONTROL Notes] (eller [!UICONTROL Updates]) | ✓ |  |

Mer information om hur du kör grundläggande och avancerade sökningar i [!DNL Workfront] finns i [Sök [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Begränsad åtkomst till objekt

När en användare inte har åtkomst till ett objekt visas&quot;Ingen åtkomst&quot; var som helst där objektnamnet visas i Workfront.

Åtkomsten till objekt kan begränsas på åtkomstnivån eller i ett specifikt objekts behörigheter.

Detta gäller alla objekt och underordnade objekt som listas i avsnittet [Beroende och hierarki för objekt](#interdependency-and-hierarchy-of-objects) i den här artikeln. Detta gäller inte för Team- och User-objekt.

## Rapport om objekt

Det är mycket viktigt att förstå hierarkin och objektens inbördes beroende innan du börjar skapa rapporter i [!DNL Workfront]. Rapporterna är objektspecifika. Du måste välja rätt objekt för rapporten innan du kan visa de data du vill ha.

>[!IMPORTANT]
>
>Du kan bara rapportera det markerade objektet och de överordnade objekten i samma rapport. Du kan inte ha information om de underordnade objekten i en överordnad objektrapport. Du kan till exempel visa projektinformation i en aktivitetsrapport, men inte i en projektrapport.

Du kan rapportera alla objekt i databasen med vårt öppna API. En fullständig lista över alla objekt i databasen finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Om du har anpassat namnen på objekten med hjälp av en layoutmall har även namnen på objekten i Report Builder anpassats. Se till att du vet vilka objekt som har anpassats och letar efter det anpassade namnet i Report Builder. Mer information om vilka objekt som kan ha anpassade namn i [!DNL Workfront] finns i [Objektnamn som kan anpassas med en [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template) i den här artikeln.
> * När du använder textläge i rapporter är namnen på objekten i textlägesuttryck standardnamnen i [!DNL Workfront], inte de anpassade objektnamnen. Mer information om hur du använder textläge i rapporter finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Mer information om vårt API finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

### Objekt som är tillgängliga för rapporter

Du kan rapportera följande objekt när du använder rapportverktyget i webbprogrammet [!DNL Workfront]. Punkter med indrag ger mer information om objektet och representerar inte ytterligare objekt.

* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Hour]
* [!UICONTROL Issue]
* [!UICONTROL User]
* [!UICONTROL Access]-nivå
* [!UICONTROL Approval]
* [!UICONTROL Approval Process]
* [!UICONTROL Assignment]
* [!UICONTROL Baseline]
* [!UICONTROL Baseline Task]
* [!UICONTROL Billing Record]
* [!UICONTROL Budgeted Hour]
   * Detta är [!UICONTROL Budgeted Hours], så som de visas i de äldre, föråldrade resurshanteringsverktygen.
   * &quot;Bud&quot;. Fältet Timmar i rapporten [!UICONTROL Budgeted Hour] refererar till de timmar som har budgeterats för jobbroller i [!UICONTROL Resource Planner]. Mer information finns i [Förstå [!UICONTROL Budgeted Labor Cost] och [!UICONTROL Budgeted Hours] för projekt](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Calendar Event]
* [!UICONTROL Company]
* [!UICONTROL Custom Form]
* [!UICONTROL Dashboard]
* [!UICONTROL Document]
* [!UICONTROL Document Approval]
* [!UICONTROL Document Version]
   * Du kan visa information om dokumentets version, det dokument som versionen är kopplad till, vem som skapade versionen och den användare som skapade korrekturet i dokumentversionen om det finns ett sådant (korrekturläsare).
* [!UICONTROL Email Template]
* [!UICONTROL Expense]
* [!UICONTROL Expense Type]
* [!UICONTROL External Page]
* [!UICONTROL Favorite]
* [!UICONTROL Filter]
* [!UICONTROL Goal]
   * Du kan skapa en rapport för strategiska mål eller så kan du visa målrelaterad information i en projektrapport när projekt är kopplade till mål som målaktiviteter. Du kan skapa strategiska mål och ansluta projekt till dem endast om din organisation har köpt en [!DNL Workfront Goals]-licens. Mer information om [!DNL Workfront Goals] finns i [[!DNL Workfront Goals] översikt](../../../workfront-goals/goal-management/wf-goals-overview.md). Mer information om hur du ansluter projekt till strategiska mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Du kan inte rapportera projektmål som är associerade med en [!UICONTROL Business Case]. Mer information om projektmål och strategiska mål finns i [Ordlista för  [!DNL Adobe Workfront] terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Group]
* [!UICONTROL Grouping]
* [!UICONTROL Hour Type]
* [!UICONTROL Initiative]
   * Du kan bara skapa en rapport för initiativ som är underordnade objekt för en plan om ditt företag har köpt en [!DNL Workfront Scenario Planner]-licens. Mer information om initiativ finns i [Översikt över initiativ i  [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Initiera jobbroll
   * Du kan bara skapa en rapport för de jobbroller som är associerade med initiativen i en plan om ditt företag har köpt en [!DNL Workfront Scenario Planner]-licens. Mer information om hur du skapar initiativ och associerar dem med jobbroller finns i [Skapa och redigera initiativ i  [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteration]
* [!UICONTROL Job Role]
* [!UICONTROL Journal Entry]
   * Du kan rapportera om spårade systemuppdateringar i [!UICONTROL Updates]-området med objekt som uppgifter, projekt, problem osv. Mer information finns i [Rapport om uppdateringsområdet med en journalpostrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout Template]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone Path]
* [!UICONTROL Note] eller [!UICONTROL Updates]
   * Du kan rapportera kommentarer som lagts till av enskilda användare.

* [!UICONTROL Parameter] (eller [!UICONTROL Custom Field])
* [!UICONTROL Parameter Group] (eller [!UICONTROL Section Break])
* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project (Financial Data)]
   * Den ekonomiska informationen fylls i i [!UICONTROL Project (Financial Data)] rapporter endast när de data som är associerade med den är mindre än 5 år gamla. Om en jobbroll till exempel allokerades till en aktivitet i januari 2015 och idag är september 2021, fylls inte ett ekonomiskt fält som [!UICONTROL Allocation Date] för jobbrollen i rapporten [!UICONTROL Project (Financial Data)].

  >[!CAUTION]
  >
  >När du kör en projektrapport (ekonomiska data) utförs en omberäkning av dina finansiella data, vilket kan skriva över tidigare ekonomiska data och kan ta lång tid. Mer information om konsekvenserna av omberäkning av ekonomiska data finns i [Beräkna om projektekonomi](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Proof Approval]
   * Gör det möjligt för dig att visa olika information om bevisgodkännandet, inklusive: det bevis som skickades för godkännande, information om [!UICONTROL Approver], information om den begärande parten (om den begärande parten är en licensierad [!DNL Workfront]-användare), versionsinformation, korrektur-ID och datumet när beviset skapades.\
      [!UICONTROL Proof Approval] rapporter innehåller endast korrektur som är tillgängliga i användarnas Mina arbetsområden där beslut ännu inte har fattats.\
   * Korrekturgodkännanden tilldelas i [!DNL Workfront] enligt beskrivningen [Lägg till användare i ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) i [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Queue]
* [!UICONTROL Queue Topic]
* [!UICONTROL Rate] (här visas information om jobbrollen [!UICONTROL Billing Rate])
* [!UICONTROL Reminder Notification]
* [!UICONTROL Report]
* [!UICONTROL Resource Pool]
* [!UICONTROL Risk]
* [!UICONTROL Risk Type]
* [!UICONTROL Schedule]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Template]
* [!UICONTROL Template Task]
* [!UICONTROL Time Off]
   * Du kan rapportera användarens ledig tid enligt vad användaren anger i sin profil.

* [!UICONTROL Timesheet]
* [!UICONTROL Timesheet Profile]
* [!UICONTROL Topic Group]
* [!UICONTROL User Approval]
* [!UICONTROL User Delegation]

   * Du kan rapportera om användare som har delegerats att utföra andra uppgifter och problem medan de inte är på kontoret. Den här rapporten visar den användare som inte är på kontoret samt den användare som fullgör sina uppgifter medan de är ute.

* [!UICONTROL Users Decisions]

   * Du kan rapportera hur många beslut användare har fattat om korrektur och dokument under den aktuella månaden.

* [!UICONTROL View]
* [!UICONTROL Work Item] (detta skapar en rapport för uppgifter och ärenden)
