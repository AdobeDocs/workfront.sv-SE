---
title: 'Playbook: Managed Scaling, After the First Win'
description: Lär dig lansera Adobe Workfront Planning efter den första implementeringen
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# Playbook: hanterad skalning, efter första win

{{planning-important-intro}}

**Version**: 1.0

**Kontext**:&quot;Vi har landat vårt första användningsfall, och nu vill alla in.&quot;



## 1. The &quot;Success Trap&quot;

Ibland kan det kännas som att den farligaste fasen av WFP-implementering är direkt efter det första framgångsrika användningsexemplet eller POC. Engagemanget är stort, men rädsla för&quot;teknisk skuld&quot; och&quot;administrativ spraktik&quot; kan leda till två lika skadliga reaktioner:

1. **Styrning överstyrt**: Systemet låses så hårt att nya team återgår till kalkylblad.

2. **Ingen styrning**: Alla team kan skapa egna fält och posttyper och återskapa den fragmenterade metadatautbredningen som finns i äldre miljöer.



## &#x200B;2. Kärnfilosofin: WFP som&quot;avstämningsmotor&quot;

I stället för att försöka hindra team från att vara olika, placerar vi WFP som den plats där skillnaderna **görs synliga så att de kan avstämas**.



* **Hantera Adobes hastighet**: Det är naturligt att vara försiktig med att utöka till ett nytt verktyg innan du&quot;rensar&quot; befintliga miljöer. Om du väljer att **förenkla första** får du en välstyrd grund, men det kan fördröja time-to-value för team som är redo att justera. Vi anser att det effektivaste sättet att gå igenom den här ändringen är att känna igen att **synlighet är steg 1**. Det som i slutänden sätter fart på de långsiktiga målen är att gå mot ett delat, företagsfärdigt verktyg (och gå från mängden PPT och kalkylblad).



  **Rekommendation**: Istället för ett&quot;Rensa först&quot;-mandat rekommenderar vi att du allokerar en mindre del resurser till pågående underhåll och en betydligt större del till att lösa akuta affärsbehov. Om du till exempel lägger ett år på att enbart rensa upp taxonomier får du ett litet stegvis värde. Om du levererar **synlighet mellan team** (t.ex. via en enhetlig Enterprise-kalender eller en konsoliderad GTM-färdplan) får du det omvandlingsvärde som dina intressenter behöver, samtidigt som du får den enhetliga datastruktur som du behöver för att styra miljön över tiden.

* **Bekräfta verkligheten**: Oberoende team utvecklar sina egna processer på ett naturligt sätt, som ofta döljs i isolerade kalkylblad. Att gå över till WFP skapar inte en enda röra; det lyser upp den som redan finns. Genom att göra dessa processer synliga i en delad miljö placerar ni dem på ett ställe där de äntligen kan hanteras och förbättras.

* **Förloppssignalen**: När ett team frågar efter sina egna fält är det inte&quot;sprawl&quot;, utan **Adobe**. Det innebär att de ser WFP som sin arbetsyta.

* **Hantera skuld, Dölj inte**: Det är naturligt att bekymra sig om den ansträngning som krävs för att rensa bort avvikande taxonomier senare. Alternativet - som tvingar strikta standarder för tidigt - leder ofta tillbaka team till kalkylblad där deras processer (och deras skulder) förblir dolda. Genom att låta teamen börja i WFP med sina nuvarande klassificeringar, flyttar ni den skulden till en synlig, styrd miljö. Detta gör den slutliga avstämningen till en iterativ uppgift snarare än ett enda överväldigande migreringsprojekt.



## &#x200B;3. &quot;Lanes on a Road&quot; Governance Model

Skala utan skuld genom att definiera&quot;Global Lanes&quot; och&quot;Local Playgrounds&quot;.



### A. The Global Lanes

* **Kontrollerade objekt**: Objekt som alla team måste använda för företagsrapportering (t.ex. `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Hanteras av**: Den centrala COE/Marketing Ops-administratören.

* **Regel**: Dessa fält är&quot;delade&quot; och obligatoriska.



### B. Lokala spelgrunder (Spokes)

* **Experimentella objekt**: Fält eller posttyper som är specifika för ett teams taktiska behov (t.ex. det sociala teamets `Influencer Handle` eller ett webbgrupps `URL Slug`).

* **Hanteras av**: Gruppledaren (med ljusvägledning).

* **Regel**: Team kan förnya sig här. Om ett&quot;lokalt&quot; fält används av >3 team är det&quot;Befordrad&quot; till ett globalt plan.



## &#x200B;4. Styrningsparadox: Teams First, Standards follow

En vanlig utmaning vid skalning av WFP är att bestämma vilket som kommer först: **Företagsstyrning** eller **Teamanpassning**.



Vi anser att det effektivaste sättet att navigera på detta är att inse att företagsvärdet bygger på en dubbelriktad gata:

1. **Team behöver relevans**: Företaget realiserar bara värdet när dess team aktivt körs. Därför måste styrning **betjäna team** genom att tillhandahålla en struktur som stöder deras kända operativa behov.

2. **Enterprise behöver synlighet**: Ledarskap kan bara fatta välgrundade beslut när data är tillräckligt rena för att aggregera. Teamen måste därför **betjäna företaget** genom att tillhandahålla de metadata som krävs för portföljens synlighet.



Målet med&quot;Managed Scaling&quot; är att hitta skärningspunkten mellan dessa två behov - tillräckligt att standardisera för att ge synlighet, men inte så mycket att teamkörningen avbryts.



### A. Justeringsprioriteter: Data kontra visualisering

När du skalförändrar måste du känna igen att definitionen av&quot;Värde&quot; skiljer sig mellan olika personligheter:

* **Admin-/produktägaren**: Värden **enhetliga taxonomier och klassificeringar**. Målet är en ren dataarkitektur som stöder långsiktig skalbarhet.

* **Intressenten/ledaren**: Värden **visualisering och insikt** (t.ex. en global kalender eller en Portfolio-tidslinje). Deras mål är&quot;Lightning Moment&quot; som gör att data kan användas.



**Strategin**: Använd intressentens behov av visualisering som *incitament* för teamets efterlevnad av administratörens behov av datastandarder. Ni får den enhetliga taxonomin genom att leverera den superkalender som ledningen kräver.



### B. Den serviceinriktade observationsfasen

Under den tidiga uppgraderingen är administratörens roll att underlätta utbytet mellan team och företaget.

* **Prioritera åtgärd framför standardisering**: Det är bättre att ha team som aktivt planerar i isolerade arbetsytor än att ha dem installerade på grund av brist på globala definitioner. Denna aktivitet är den&quot;rådata&quot; som krävs för att skapa sunda, verkliga standarder.

* **Identifiera &quot;Synlighetsminimum&quot;**: Arbeta med ledarskap för att identifiera de 3-5 fält som *måste* vara rena för företagsrapportering (t.ex. `Strategic Alignment`, `Start Date`, `Budget`). Fokusera ENDAST på er exekveringsenergi här.



### B. Retroaktiv harmonisering (företagsstyrning som tjänst)

När ett mönster med&quot;kända behov&quot; uppstår mellan olika team kan företaget gå över för att konsolidera dessa mönster till en global tjänst.

1. **Observera lyckade mönster**: Identifiera de &quot;vinnande&quot; taxonomier som team redan har skapat och antagit.

2. **Handskakningen för samarbete**: Samla ihop grupper för att förfina deras lokala framgångar i en delad företagsstandard.

3. **Distribuera som en tjänst**: Rulla ut de nya globala språken inte som en &quot;begränsning&quot;, utan som ett sätt att förenkla rapportering och gruppöverskridande anpassning för de personer som utför arbetet.



**Nyckelhanterare**: Styrning ska vara ett svar på om operationen lyckas, inte en förutsättning för det.



## &#x200B;5. Skalningsmekanism: Den mönsterbaserade tillväxtmodellen

För att tillämpa denna filosofi krävs en genomtänkt strategi för datastrukturen. För att undvika&quot;Styrningsspill&quot; måste man motstå behovet av att skapa globala fält för varje enskild begäran. Använd i stället **Sökväg för fältmognad** för att låta verkliga användningsmetoder vägleda dina företagsstandarder:



1. **Nivå 1: Lokal experiment**: Team A skapar ett anpassat fält på sin arbetsyta.

2. **Nivå 2: Mönsterigenkänning**: Admin notices Teams B and C använder eller frågar efter ett liknande fält.

3. **Nivå 3: Företagsstandardisering**: Admin skapar en enda standardiserad version av det fältet som en posttyp i **Global Taxonomy Workspace** och syndikerar det till team.



### Mekaniken för&quot;mjuk minskning&quot;

Eftersom WFP för närvarande inte har någon inbyggd arkivfunktion för fält, måste en avsiktlig&quot;mjuk pensionering&quot;-process för att bevara historiska data utan att användargränssnittet behöver renderas för att ett lokalt fält ska kunna tas bort:



1. **Datamigrering**: Använd en tabellvy (eller Fusion) om du vill kopiera värden från det lokala skuggfältet till det nya fältet Global Lane. Se till att data valideras och rensas under flyttningen.

2. **Byt namn på borttagning**: Byt namn på det lokala fältet med ett prefix som `[DEPRECATED]` eller `z_` (t.ex. `z_Language (Old)`). Detta gör att fältet hamnar längst ned i fältväljare och signalerar till användarna att det inte längre är&quot;Source of Truth&quot;.

3. **Borttagning av formulär**: **Detta är det mest kritiska steget.** Ta bort det inaktuella fältet från alla **Spela in Forms**. Detta förhindrar att nya data matas in samtidigt som gamla data förblir synliga i befintliga tabellvyer eller rapporter vid behov.

4. **Solnedgångsperioden**: Behåll det inaktuella fältet (prefix och off-form) i 30-60 dagar för att säkerställa att inga data missades under migreringen. Efter den här perioden kan det lokala fältet tas bort från arbetsytan om data är helt avstämda i det globala lagret.



## &#x200B;6. Undvika&quot;kärndrivrutin&quot; (abstraktionsregeln).

För att förhindra att planering blir så rörig som kärnan:

* **Abstraktionslagret**: Varje fält i WFP ska svara på en **strategisk fråga**. Om ett fält bara används för taktisk spårning (t.ex. &quot;Godkänd av detta bevis?&quot;) ska du behålla det i kärnan.

* **Konsolidering först**: Om ett team vill ha ett nytt metadatafält bjuder du in dem att kontrollera Global Taxonomy först. Detta kräver att teamet beviljar **skrivskyddad åtkomst** till arbetsytan Global Taxonomy (se avsnitt 7). Genom att mappa deras taktiska behov till ett befintligt strategiskt fält kan du förhindra onödiga dubbletter och bevara rapportens integritet.



## &#x200B;7. Synlighetsmodellen Skrivskyddad åtkomst

Lös &quot;Siloed&quot;-känslan utan oljud från &quot;Siloed&quot;-arbetet.

* **Problem**: Team i skämt känns isolerade eftersom de bara ser sina egna poster.

* **Korrigera**: Bevilja team **skrivskyddad åtkomst till arbetsytorna som har angetts som primära för de delade posttyperna**.

* **Resultatet**: De kan se den bredare företagssammanhanget för inspiration och anpassning, men deras lokala arbetsyta är fortfarande ren och fokuserad på sina specifika uppgifter.



## &#x200B;8. Hantera tillväxt via Workshops

Att bygga ut WFP är lika mycket en kulturell utmaning som en teknisk utmaning. Använd målinriktade workshops för att överbrygga&quot;Governance Gap&quot;.



### A. The &quot;Necessary Mess&quot; Discovery Workshop

* **Målgrupp**: Regional Marketing Leads and Ops Champions.

* **Mål**: Dokumentera den aktuella &quot;Siloed Reality&quot; (de fragmenterade användningsdata).

* **Meddelandet**:&quot;Vi är inte här för att ta bort dina fält. Vi är här för att förstå hur de länkar till den globala strategin.&quot;

* **Resultat**: Ett utkast till mappning av lokala taktiska fält till globala strategiska banor.



### B. Justeringssessionen&quot;Strategisk synlighet&quot;

* **Målgrupp**: Marknadsförare på hög nivå (ledarskap).

* **Mål**: Rama in ångest om Förenkla första.

* **Meddelandet**:&quot;Vi behöver ingen perfekt taxonomi för att starta. Vi använder WFP som miljö för att *bygga* den perfekta taxonomin.&quot;

* **Resultat**: Godkännande att gå vidare med WFP som avstämningsmotor medan Core fortfarande är i det aktuella tillståndet.



### C. The &quot;Spoke-to-Global&quot; Showcase

* **Målgrupp**: Nya team utforskar WFP.

* **Mål**: Minska känslan av isolering.

* **Meddelandet**: &quot;Se hur Team A:s lokala arbete automatiskt matar den primära Workspace-datorn? Det kan du också göra för ditt material.&quot;

* **Resultat**: Välj från nya avdelningar som ser fördelarna med att vara anslutna utan att förlora sitt lokala oberoende.



### D. Kontorstiderna för&quot;pågående support&quot;

* **Målgrupp**: Alla WFP-användare (aktuella och potentiella).

* **Mål**: Tillhandahåll en återkommande lågprismiljö för felsökning och taktisk vägledning.

* **Meddelandet**:&quot;Det finns inga fel frågor. Vi är här för att hjälpa er att lösa era specifika planeringsutmaningar i realtid.&quot;

* **Resultat**: Ökat användarförtroende, snabbare upplösning av teknisk friktion och identifiering av nya mönster som kan göra global standardisering berättigad.



## &#x200B;9. Anställda för skalning: roller och ansvarsområden

Om du lyckas med en hanterad skalningsmodell krävs mer än bara verktygskonfiguration. Det krävs en tydlig fördelning av roller mellan globala team och Spoke-team.



### A. Enterprise Architect (Central COE/Marketing Ops)

* **Fokus**: Företagsintegritet, systemprestanda och **enhetlig datataxonomi**.

* **Ansvarsområden**:

   * Hanterar **Global Taxonomy Workspace**.

   * Underlättar sökvägen **Fältmognad** (befordrar lokala framgångar till globala standarder).

   * Upprätthåller de **primära Workspace**-vyerna för chefsrapportering.

   * Leder till den månatliga **semantiska granskningen** över arbetsytor.



### B. The Spoke Champion (teamprocessens ägare)

* **Fokus**: Teamrelevans och acceptans snabbt.

* **Ansvarsområden**:

   * Fungerar som en enda kontaktpunkt för det funktionella teamet.

   * Äger den lokala arbetsytestrukturen och anpassade fältförsök.

   * Ser till att teamet använder **Styrd gateway** (Forms) för datainmatning.

   * Deltar i **Samverkande handskakning** under harmoniseringen.



### C. Den verkställande sponsorn (marknadsledande)

* **Fokus**: Strategisk justering, OKR-synlighet och **portföljvisualisering (t.ex. global kalender)**.

* **Ansvarsområden**:

   * Definierar företagets **OKR för marknadsföring** på arbetsytan Global taxonomi.

   * Fördelar värdet för &quot;Synlighetsteg 1&quot; med andra ledare.

   * Förstärker resursallokeringen 80/20 (värde över rensning).



### D. Aktiveringsansvarig (ändringshantering)

* **Fokus**: Kulturförskjutning och kompetensutveckling.

* **Ansvarsområden**:

   * Värdar återkommande **kontorstimmar** och **identifieringsworkshops**.

   * Underhåller den interna &quot;Success Story&quot;-showcase.

   * Identifierar tekniska friktionspunkter som företagsarkitekten kan lösa.



## &#x200B;10. Checklista för skalning av nästa team

* [ ] **Identifiera Champion**: Vem är den nya gruppens processägare eller mästare?

* [ ] **Definiera lokal ändring**: Vilka 2-3 fält behöver det här teamet som den globala standarden inte tillhandahåller för närvarande?

* [ ] **Mappa till globala band**: Vilka befintliga globala fält kan tillgodose 80 % av deras behov?

* [ ] **Bevilja global synlighet**: Ge dem skrivskyddad åtkomst till de relevanta primära arbetsytorna och den globala taxonomiarbetsytan dag 1.

* [ ] **Upprätta porten**: Hur matar deras arbete in de relevanta primära arbetsytorna? (t.ex. via en global posttyp eller en specifik sökning).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->