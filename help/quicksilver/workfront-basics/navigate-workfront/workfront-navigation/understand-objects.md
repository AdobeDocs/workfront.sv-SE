---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Förstå objekt i [!DNL Adobe Workfront]
description: Förstå objekt i [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2017'
ht-degree: 0%

---

# Förstå objekt i [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

Den information du visar i [!DNL Adobe Workfront] representeras av objekt som lagras i [!DNL Workfront] databas. Objekten är vad som driver informationen i [!DNL Workfront].

Förstå hur objekt definieras i [!DNL Workfront] är viktigt så att du kan använda rätt objekt för de behov som finns i organisationen.

Om du till exempel planerar en stor mängd arbete måste du använda [!UICONTROL Project] -objekt för att definiera det arbetet. Om du vill dela upp arbetet i mindre planerade steg kan du använda [!UICONTROL Task] -objekt. För en mindre mängd arbete som inte är planerat och som kan utföras oväntat kan du använda objektet Utgåva. Om du vill följa förloppet och hur budgeten och tidslinjen följs för en grupp projekt kan du ordna dem i [!UICONTROL Portfolios] och [!UICONTROL Programs]. Om du vill definiera andra element som kan hjälpa dig att lösa ditt arbete, vill du använda andra objekt som lagras under [!UICONTROL Projects], [!UICONTROL Tasks], [!UICONTROL Issues], eller [!UICONTROL Portfolios], gilla [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users], eller [!UICONTROL Job Roles].

[!UICONTROL Reports] och [!UICONTROL Dashboards] är ett annat exempel på objekt som kan hjälpa dig att ordna mängden data du har i [!DNL Workfront] visuellt för att göra det enkelt för alla användare.

För en fullständig lista över objekt i [!DNL Workfront], se [API Explorer](../../../wf-api/general/api-explorer.md).

## Objektens inbördes beroende och hierarki

Objekt länkas till varandra i [!UICONTROL Workfront]. En aktivitet eller ett problem kan till exempel aldrig finnas oberoende utanför ett projekt. [!UICONTROL Tasks] och [!UICONTROL issues] är exempel på objekt som lagras i [!UICONTROL project] -objekt. [!UICONTROL Tasks] och [!UICONTROL issues] betraktas som underordnade objekt till projekt.

Nedan följer några av de vanligaste objekten i [!DNL Workfront] och deras respektive överordnade och underordnade objekt:

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

För en fullständig lista över objekt i [!DNL Workfront], se [API Explorer](../../../wf-api/general/api-explorer.md).

*Planerna är objekten i [!DNL Workfront Scenario Planner]. Mer information om [!DNL Scenario Planner], se [The [!UICONTROL Scenario Planner] översikt](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Goals] är objekten i [!DNL Workfront Goals]. Mer information om [!DNL Workfront Goals], se [[!DNL Adobe Workfront Goals] översikt](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Anpassa objektnamn

Som [!DNL Workfront] kan du anpassa objektnamn i [!DNL Workfront] genom att använda  [!UICONTROL Layout Template].

Mer information om hur du anpassar objektnamn med en  [!UICONTROL Layout Template], se [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

När du har anpassat en layoutmall och tilldelat den till användare, ser dessa användare de anpassade namnen för objekten. De användare som har tilldelats layoutmallen ser inte längre standardnamnen för objekten någonstans i webbprogrammet.

>[!NOTE]
>
>För att de nya namnen på objekten ska vara synliga för användarna måste de logga ut och logga in igen på [!DNL Workfront] när du har sparat  [!UICONTROL Layout Template].

>[!IMPORTANT]
>
>The [!DNL Workfront] dokumentation refererar alltid till objektens standardnamn. Som [!DNL Workfront] måste du informera användarna om ändringarna i objektnamnen så att de kan förstå hur de använder [!DNL Workfront] dokumentation, samt de områden i programmen som inte återspeglar ändringarna i objektens namn.

* [Objektnamn som kan anpassas med en  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template)
* [Områden i [!DNL Workfront] som återspeglar de anpassade objektnamnen](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Områden i [!DNL Workfront] som inte återspeglar de anpassade objektnamnen](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Objektnamn som kan anpassas med en [!UICONTROL Layout Template]

Som [!DNL Workfront] kan du anpassa namnen på följande objekt så att de matchar terminologin i organisationen:

* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Issue]
* [!UICONTROL Goal]*
* [!UICONTROL Result]*
* [!UICONTROL Activity]*

   *[!UICONTROL Goals], [!UICONTROL results]och [!UICONTROL activities] är endast tillgängliga om ditt företag har köpt [!DNL Workfront Goals]. Mer information om [!DNL Workfront Goals], se [[!DNL Adobe Workfront Goals] översikt](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scenario]**
* [!UICONTROL Plan]**

   **[!UICONTROL Initiatives], [!UICONTROL scenarios]och [!UICONTROL plans] är bara tillgängliga om ditt företag har köpt [!DNL Workfront Scenario Planner]. Mer information om [!DNL Scenario Planner], se [Kom igång med [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


Om den större mängden arbete i organisationen till exempel kallas för engagemang kan du ersätta namnet[!UICONTROL Project]&#39; med &#39;Engagement&#39;. Dina [!DNL Workfront] gränssnittet visar&quot;Engagement&quot; i stället för[!UICONTROL Project]&#39; överallt där namnet &#39;[!UICONTROL Project]visas.

Mer information om hur du kan anpassa objektnamn med  [!UICONTROL Layout Templates], se [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Du kan inte anpassa namnen på andra objekt i Workfront. För en fullständig lista över objekt i [!DNL Workfront], se [API Explorer](../../../wf-api/general/api-explorer.md).

När du anpassar namnet på ett objekt visas det nya namnet för det objektet i de flesta områden i [!DNL Workfront] program där objektnamnet skulle visas.

### Områden i [!DNL Workfront] som återspeglar de anpassade objektnamnen

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

### Områden i [!DNL Workfront] som inte återspeglar de anpassade objektnamnen

I följande områden visas inte objektens uppdaterade namn:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Tillägg

## Konsekvenser av anpassning av objektnamn

Du bör vara medveten om följande när du anpassar objektnamn i [!DNL Workfront]:

* Du kan stöta på stilistiska eller grammatiska fel på systemskärmar. Om du till exempel byter namn på &#39;[!UICONTROL Issue]till &#39;Begäran&#39; och du ser var som helst i systemet frasen &#39;En begäran&#39;, som fungerar som det ska och som inte ska betraktas som ett fel.
* Dina anpassade namn för objekten är inte översättningsbara. Endast [!DNL Workfront] standardnamn kan översättas på de språk som stöds. Mer information om språk som stöds i [!DNL Workfront], se [Språk som stöds på [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). De anpassade objektnamnsfälten har stöd för främmande tecken så att du kan ange terminologi på vilket språk som helst.
* När du anpassar objektnamn med en  [!UICONTROL Layout Template]rekommenderar vi att du tilldelar  [!UICONTROL Layout Templates] runt era affärsenheter (team eller grupper).\
   Vi rekommenderar att du använder namn som är tydliga för användarna av dessa affärsenheter för att undvika förvirring.
* E-postmeddelanden och levererade rapporter innehåller alltid objektnamn som definieras av  [!UICONTROL Layout Template] för den användare som genererar e-postmeddelandet. Dina användare bör vara förberedda på att se objektnamn i sina e-postmeddelanden som inte är relaterade till deras grupp eller team, om de får e-postmeddelanden från användare i andra team och grupper.\
   Som [!DNL Workfront] -administratör, rekommenderar användare att lägga märke till de ikoner som är associerade med varje objekt. Ikonerna är desamma för olika objektnamn och överensstämmer med standardobjektet så som det visas i databasen. För en lista med alla [!DNL Workfront] ikoner som är kopplade till objekt, se [Objektikoner](#object-icons).

   >[!TIP]
   >
   >För vanliga uppgifter i organisationen bör du överväga att skapa anpassad dokumentation som återspeglar din terminologi.

## Objektikoner

The [!DNL Workfront] dokumentation refererar alltid till objektens standardnamn. Om objektens namn har anpassats kan du förlita dig på den ikon som är associerad med dem för att förstå vilket anpassat objekt som motsvarar det [!DNL Workfront] standardobjekt.

Mer information om vilka objekt som kan ha anpassade namn i [!DNL Workfront], se [Objektnamn som kan anpassas med en  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).

Här följer en lista med objekt och motsvarande ikoner för dem i Workfront.

| **Objekt** | **Ikon** | **Anpassningsbart objektnamn** |
|---|---|---|
| [!UICONTROL Company] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Goal] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Group] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Issue] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Job Role] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Program] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Project] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Report] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Task] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Template] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Referensnummer för objekt

Varje objekt som skapas i [!DNL Workfront] tilldelas ett unikt referensnummer. Referensnummer är användbara när du ska skilja mellan två i övrigt liknande objekt (till exempel uppgifter med samma namn). Du kan söka efter objekt med hjälp av deras referensnummer och du kan inkludera referensnummer i rapporter.

Mer information om hur du söker efter objekt efter referensnummer finns i [Använd referensnumret för objekt](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Objektspecifika sökningar

Du kan söka bland alla objekt som är sökbara i [!DNL Workfront]eller du kan markera ett specifikt objekt att söka efter i dina grundläggande och avancerade sökningar.

Alla objekt är inte sökbara i [!DNL Workfront]. Du kan utföra enkla och avancerade sökningar för följande objekt i [!DNL Workfront]:

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
| [!UICONTROL Notes] | ✓ |  |

Mer information om hur du kör enkla och avancerade sökningar i [!DNL Workfront], se [Sök [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Rapport om objekt

Det är mycket viktigt att förstå hierarkin och objektens inbördes beroende innan du börjar skapa rapporter i [!DNL Workfront]. Rapporterna är objektspecifika. Du måste välja rätt objekt för rapporten innan du kan visa de data du vill ha.

Beroende på vilket objekt du har valt för rapporten kan du bara komma åt de objekt som är direkt länkade till rapportens objekt.

>[!IMPORTANT]
>
>Du kan bara rapportera det markerade objektet och de överordnade objekten i samma rapport. Du kan inte ha information om de underordnade objekten i en överordnad objektrapport. Du kan till exempel visa projektinformation i en aktivitetsrapport, men inte i en projektrapport.

Du kan rapportera alla objekt i databasen med vårt öppna API. En fullständig lista över alla objekt i databasen finns i [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Om du har anpassat namnen på objekten med hjälp av en layoutmall har även namnen på objekten i Report Builder anpassats. Se till att du vet vilka objekt som har anpassats och letar efter det anpassade namnet i Report Builder. Mer information om vilka objekt som kan ha anpassade namn i [!DNL Workfront], se *[Objektnamn som kan anpassas med en  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).*
>När du använder textläge i rapporter är namnen på objekten i textlägesuttryck standardnamnen i [!DNL Workfront]och inte de anpassade objektnamnen. Mer information om hur du använder textläge i rapporter finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Mer information om vårt API finns i [API Explorer](../../../wf-api/general/api-explorer.md).

Du kan rapportera följande objekt när du använder rapportverktyget i [!DNL Workfront] webbprogram:

* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Hour]
* [!UICONTROL Issue]
* [!UICONTROL User]
* [!UICONTROL Access] Nivå
* [!UICONTROL Approval]
* [!UICONTROL Approval Process]
* [!UICONTROL Assignment]
* [!UICONTROL Backlog Work Item]\
   Visar aktiviteter eller problem i den flexibla eftersläpningen. Mer information om den flexibla eftersläpningen finns i [Hantera den flexibla eftersläpningen](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL Baseline]
* [!UICONTROL Baseline Task]
* [!UICONTROL Billing Record]
* [!UICONTROL Budgeted Hour]

   Det här är [!UICONTROL Budgeted Hours], som de visas i de äldre, föråldrade resurshanteringsverktygen.

   &quot;Bud. Timmar i fältet [!UICONTROL Budgeted Hour] rapport refererar till de timmar som har budgeterats för jobbroller i [!UICONTROL Resource Planner]. Mer information finns i [Förstå [!UICONTROL Budgeted Labor Cost] och [!UICONTROL Budgeted Hours] för projekt](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Calendar Event]
* [!UICONTROL Category] (eller [!UICONTROL Custom Form])
* [!UICONTROL Company]
* [!UICONTROL Dashboard]
* [!UICONTROL Document]
* [!UICONTROL Document Approval]
* [!UICONTROL Document Version]\
   Här kan du visa olika information om dokumentets version, det dokument som versionen är kopplad till, vem som skapade versionen och den användare som skapade korrekturet i dokumentversionen om det finns ett sådant (korrekturläsare).
* [!UICONTROL Email Template]
* [!UICONTROL Expense]
* [!UICONTROL Expense Type]
* [!UICONTROL External Page]
* [!UICONTROL Favorite]
* [!UICONTROL Filter]
* [!UICONTROL Goal]

   Du kan skapa en rapport för strategiska mål eller så kan du visa målrelaterad information i en projektrapport när projekt är kopplade till mål som målaktiviteter. Du kan skapa strategiska mål och koppla ihop projekt med dem endast om din organisation har köpt en [!DNL Workfront Goals] licens. Mer information om [!DNL Workfront Goals], se [[!DNL Workfront Goals] översikt](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). Mer information om hur du ansluter projekt till strategiska mål finns i [Lägga till projekt i mål i Adobe Workfront-mål](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >Du kan inte rapportera om projektmål som är kopplade till en [!UICONTROL Business Case]. Mer information om projektmål jämfört med strategiska mål finns i [Ordlista för [!DNL Adobe Workfront] terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Group]
* [!UICONTROL Grouping]
* [!UICONTROL Hour Type]
* [!UICONTROL Initiative]

   Du kan bara skapa en rapport för initiativ som är underordnade objekt till en plan om ditt företag har köpt en [!DNL Workfront Scenario Planner] licens. Mer information om initiativ finns i [Översikt över initiativen i [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* Initiera jobbroll

   Du kan bara skapa en rapport för de jobbroller som är kopplade till initiativen i en plan om ditt företag har köpt en [!DNL Workfront Scenario Planner] licens. Mer information om hur du skapar initiativ och associerar dem med jobbroller finns i [Skapa och redigera i [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL Iteration]
* [!UICONTROL Job Role]
* [!UICONTROL Journal Entry]

   Du kan rapportera om spårade systemuppdateringar i [!UICONTROL Updates] områden med objekt som uppgifter, projekt, problem osv. Mer information finns på [Rapport om [!UICONTROL Updates] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout Template]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone Path]
* [!UICONTROL Note]

   >[!NOTE]
   >
   >Du kan rapportera kommentarer som lagts till av enskilda användare.

* [!UICONTROL Parameter] (eller [!UICONTROL Custom Field])
* [!UICONTROL Parameter Group] (eller [!UICONTROL Section Break])
* [!UICONTROL Portal Profile] (här visas information som har tagits bort)
* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project] ([!UICONTROL Financial Data])

   >[!NOTE]
   >
   >Ekonomisk information fylls i i [!UICONTROL Project] ([!UICONTROL Financial Data]) rapporteras endast när de data som hör till den är yngre än 5 år. Om en jobbroll till exempel allokerades till en uppgift i januari 2015 och idag är september 2021, är det ett finansfält som [!UICONTROL Allocation Date] för jobbrollen inte fylls i i [!UICONTROL Project (Financial Data)] rapport.

* [!UICONTROL Proof Approval]\
   Här kan du visa olika information om korrekturgodkännandet, inklusive: Beviset som skickats in för godkännande, information om [!UICONTROL Approver], information om den begärande (om den begärande parten är en licensierad [!DNL Workfront] användare), versionsinformation, korrektur-ID och datum när korrekturet skapades.\
   [!UICONTROL Proof Approval] rapporter innehåller endast korrektur som är tillgängliga i användarnas arbetsytor där beslut ännu inte har fattats.\
   Bevisgodkännanden tilldelas i [!DNL Workfront] enligt beskrivning [Lägga till användare i ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Queue]
* [!UICONTROL Queue Topic]
* [!UICONTROL Rate] (här visas jobbroll [!UICONTROL Billing Rate] information)
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

   Du kan rapportera användarens ledig tid enligt vad användaren anger i sin profil.

* [!UICONTROL Timesheet]
* [!UICONTROL Timesheet Profile]
* [!UICONTROL Topic Group]
* [!UICONTROL User Delegation]

   Du kan rapportera om användare som har delegerats att utföra andra uppgifter och problem medan de inte är på kontoret. Den här rapporten visar den användare som inte är på kontoret samt den användare som fullgör sina uppgifter medan de är ute.

* [!UICONTROL View]
* [!UICONTROL Work Item] (avser uppgifter och ärenden)
