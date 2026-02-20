---
title: 'Skapa en lyckad arbetsmiljö: skapa en ny kampanjhierarki'
description: Lär dig hur ni översätter komplexa affärsprocesser till en skalbar, styrd kampanjhierarki med"Centers of Gravity" och en arkitektur för flera arbetsytor.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# Skapa din framgång: skapa en modell för kampanjhierarkin

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, en extrafunktion från Adobe Workfront.
>
>Din organisation måste ha ett Workfront Planning Prime-paket eller ett högre paket för att kunna stödja de funktioner som rekommenderas i den här artikeln.
>
>En lista över krav för åtkomst till Workfront Planning finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Allmän information om Workfront Planning finns i [Kom igång med Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Lär dig hur du översätter komplexa affärsprocesser till en skalbar, styrd kampanjhierarki med tyngdpunktsarkitektur och en flerarbetsytearkitektur i Adobe Workfront Planning.

Den här guiden är avsedd för Workfront-administratörer och Power Users som implementerar och designar din miljös arkitektur i Workfront Planning.

## Översikt över framgångens arkitektur

I takt med att era marknadsföringsaktiviteter utvecklas, gör även komplexiteten hos era data. Utan en tydlig plan kan ert Marketing System of Record snabbt bli ett skräpfack för icke sammankopplade poster, motstridig terminologi och rapportluckor.

När ni bygger upp en framgångsrik arkitektur kan ni skapa ett ramverk för att modellera er kampanjhierarki i Workfront Planning. Det går från kalkylbladskaos till en styrd, objektorienterad modell som ser till att alla i teamet talar samma språk samtidigt som de behåller den flexibilitet de behöver för att kunna genomföra.

## Bygg en hierarki för att definiera dina avsiktsnivåer

För att behålla tydlighet och skalbarhet rekommenderar vi att du börjar med en beprövad grundväg när du utformar arbetsflödet i Workfront Planning.

Därifrån kan ni utöka er strategi genom att lägga till fler nivåer i er arkitektur.

### Kärnvägen: hur man går från strategi till handling

Organisationer kan utöka hierarkin allt eftersom deras operativa behov utvecklas, men med början från de tre nivåer som beskrivs i avsnitten nedan ser vi en stark bro mellan strategi och utförande.

Utifrån våra resultat har vi märkt att de mest framgångsrika implementeringarna av Workfront Planning har en ren, treskiktsmodell som omfattar både Planning och Workfront.

Nedan följer en nivå av en lyckad planeringsimplementering och de artefakter som du kan tänka dig att skapa som stöd för processen:

* **Nivå 1: Kampanjer (Workfront Planning)**

   * **Fokus:** Definiera de långsiktiga strategiska pelarna och årsinitiativen. Du kan till exempel definiera ett initiativ för din organisation som heter&quot;Global Brand Awareness&quot; (FY26 Global Brand Awareness). Detta är ditt fokus för en given tidsram. Skapa kampanjer som stöder det här initiativet.

   * **Personas:** Intressenterna för den här nivån kan vara marknadsföringsansvariga, en VP för marknadsföring eller andra strategiska leads.

  Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

* **Nivå 2: Kanaltaktik (Workfront Planning)**

   * **Fokus:** Definiera de operativa informationsdokumenten som anger vad som ska användas för specifika kanaler. Det här är det sista lagret med strategisk avsikt innan arbetet börjar. Skapa till exempel en&quot;Q1 Social Media Blitz&quot;-taktik. Sedan kan ni kombinera det med era kampanjer.

   * **Personas:** Huvudintressenter är en marknadsledare, kanalledare eller kampanjledare.

* **Nivå 3: Projekt (Planering och Workfront)**

   * **Fokus:** Utför exakt de upplevelser eller aktiviteter som till slut kommer att slutföra ditt initiativ. Vissa produkter är specifika, som sociala inlägg, e-post och webbsidor.

   * **Implementering:** Du kan skapa taktik i planeringen och länka dem direkt till **Projekt** i Workfront, där individuella slutprodukter hanteras som aktiviteter och ärenden.

   * **Persona:** Här är de viktigaste aktörerna kreatörer, enskilda medarbetare och alla som ansvarar för att stödja initiativet.

### Strategisk expansion: lägga till fler nivåer

När du väl har fastställt grundvägen kan du välja att lägga till ytterligare lager efter att ha noggrant övervägt deras specifika affärskomplexitet.

Du kan skapa följande ytterligare objekt:

* **Kanalplaner:** Ett lager mellan kampanjer och taktik för att gruppera korsfunktionella strategier. Exempel: en plan som kallas&quot;digital strategi&quot;.

* **Aktiviteter:** Om du arbetar i en miljö med mindre volymer (du kanske har 5 000 eller färre produkter per år) kan det vara bättre att spåra enskilda upplevelser som Workfront Planning-poster innan de blir Workfront-projekt.

>[!IMPORTANT]
>
>Om din organisation producerar mer än 5 000 aktiviteter per år bör du flytta individuell leveransspårning till Workfront.
>
>Hantering av kundupplevelseposter i stora volymer i Planning kan leda till datainsamling som döljer er er strategiska synlighet.
>Vi rekommenderar den här breda riktlinjen för maximal effektivitet:
>
>* Använd Planning för&quot;varför&quot; och&quot;vad&quot;
>* Använd Workfront för storvolyminformationer.

## Förstå tyngdpunkterna för att bygga din arkitektur

Ett marknadssystem av högsta kvalitet är inte byggt i en enda arbetsyta. Den använder en&quot;nav-och-skräddarsydd&quot; arkitektur där posttyper hanteras i sina naturliga gravitationscentrum.

Mer information finns i [Ta fram ditt strategiska hem: en 30-dagars startplatta](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Om du vill skapa en arkitektur med hjälp av navet och skräddarsydda lösningar måste du skapa följande:

* Ett taxonominav
* En strategisk planeringsyta
* Funktionspolar

### Bygg upp taxonominavet som dina klassificeringar

Du måste först skapa en central arbetsyta för dina globala klassificeringar för att definiera de huvudbegrepp som alla i organisationen måste förstå. Du kan till exempel skapa följande posttyper på en central arbetsyta: Varumärken, Områden, Produkter, Personas.

Mer information finns i:

* [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)

* [Posttypöversikt för arbetsytan över flera arbetsytor](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

Ange följande när du skapar klassificeringar:

* **Primär plats:** Välj en primär arbetsyta. Den här arbetsytan bör vara källan till sanning för de posttyper som du skapar.

* **Fördelen:** Genom att syndikera dessa definitioner till resten av verksamheten kan du klargöra att begrepp som &quot;Region: EMEA&quot; betyder samma sak för alla team.

### Skapa en strategisk planeringarbetsyta som ditt ledningscenter

Ledningscentralen är den plats där högnivåkampanjer (och alla kanalplaner) finns.

* **Primär plats:** Detta är tyngdpunkten i ledningen och ger en brusfri miljö för strategiskt beslutsfattande.

* **Fördelen:** Ledarskap kan hantera kampanjportföljen utan att lyssna på det dagliga taktiska ljudet.

### Definiera funktionspolarna som arbetsytor för dina team

Funktionsenheter (Social, Creative, Email) har egna arbetsytor för att hantera sina taktiker.

* **Primär plats:** De här arbetsytorna är de enskilda tyngdpunkterna för lokal gruppkörning.

* **Fördelen:** Team använder globala kampanjer och klassificeringar från navet, samtidigt som de behåller sina egna lokala objekt.

  Teamet kan till exempel lägga till posttypen Campaign från den centrala arbetsytan i teamets arbetsyta, men skapa kampanjer som bara är relevanta för deras arbetsyta. Exempel på kampanjer är &quot;Medieutsändningar&quot; eller &quot;Användningsrättigheter&quot;.

## Använd en icke-baserad styrningsmetod

Följ principen om icke-baserad styrning för att vara säker på att din arkitektur håller press.

Vi rekommenderar följande när du skapar dina enheter i Workfront Planning:

* **Använd substantiv, inte verb:** Namnge dina posttyper efter det du håller på att spåra (kalla dem&quot;Campaign&quot; eller&quot;Tactic&quot;), inte de åtgärder som ska utföras (namnge dem inte&quot;Campaigning&quot; eller&quot;Planning&quot;).

* **Standardisera nomenklatur:** Använd samma namn på alla arbetsytor. På så sätt kan ni samla in data i hela portföljen för företagsintern rapportering.

## Hur är det med befintliga portfolior och program?

En vanlig fråga för mogna organisationer är hur man hanterar de portfolior och program man redan har byggt in i Workfront. Tidigare användes dessa objekt ofta för att efterlikna strategisk planering.

Nu rekommenderar vi att ni övergår till Workfront Planning, som naturligtvis passar in i den strategiska planeringen.

### Ersätt portföljer och program med posttyper

I många organisationer används portföljer för att representera varumärken eller affärsenheter på hög nivå, medan program representerar strategiska teman.

I Workfront Planning är de här modellerna bäst som Posttyper i ditt taxonominav.

Genom att behandla ett varumärke eller en affärsenhet som en posttyp kan ni länka dem till en kampanj eller taktik i hela företaget, vilket ger en mycket mer flexibel rapportering än en statisk Portfolio - programstruktur.

### Använda en strategi för rapportbrygga

Även om Workfront Planning är framtiden för strategiska avsikter kommer den inbyggda rapporteringen via Canvas Dashboard fortfarande att fungera.

Många organisationer förlitar sig fortfarande på de kraftfulla rapporteringsfunktionerna som är knutna till deras tidigare Portfolio- och programstrukturer i Workfront.

Vi rekommenderar följande:

* Ta inte bort dina portföljer och program.
* Använd automatiserade planeringsprocesser för att skapa en bro mellan olika posttyper, portfolior och program.

  När en aktivitet eller kampanj skapas i Workfront Planning kan den posten generera en motsvarande Portfolio eller Program i Workfront.

  Mer information finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

På så sätt kan du:

* Använd Workfront Plannings överlägsna strategiska visualisering med tidslinjer och kalendrar.

* Hantera era gamla rapporter i Workfront för intressenter som ännu inte är redo att gå över till Canvas.

## God praxis och tips

### Dos

* **Håll dig till det centrala arbetsflödet för att hitta den bästa vägen:** Upprätta ditt arbetsflöde för Campaign-to-Tactic-to-Project innan du lägger till mer komplexitet.

* **Ange primära arbetsytor:** Kontrollera att varje posttyp har en hemarbetsyta (tänk på att dess tyngdpunkt) som fungerar som aggregator för rapportering.

* **Prioritera begärandeformulär för inmatningsprocessen:** Använd postformulär för grupper med mindre avancerad i Workfront Planning för att säkerställa metadataintegriteten.

  >[!CAUTION]
  >
  >Power Users kan ha nytta av direkt datainmatning i tabellvyer, men detta bör göras med försiktighet.
  >Om du gör stora ändringar i en tabell blir det enkelt att skapa datarubriker för andra intressenter.

### Gör inte

* **Använd inte generaliseringar:** I stället för att tala om en huvudmiljö ska du referera specifikt till Workfront och Project-objektet när du talar om körning.

* **Överdriv inte kompliceringen:** Varje ytterligare nivå i hierarkin lägger till en hanteringsskatt. Lägg bara till nivåer som besvarar en affärsfråga som du för närvarande inte kan besvara.

* **Skapa inte isolerade objekt:** Kontrollera att posttyperna delas mellan arbetsytorna så att team inte skriver om samma data.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->