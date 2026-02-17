---
title: 'Bygg Bridge: Koppla strategisk återgivning till projekt'
description: Lär dig hur du skapar en"strategisk koppling" mellan dina högnivåplaner i Adobe Workfront Planning och det dagliga genomförandet av arbetsflöden i Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# Bygg en bro: koppla ihop strategisk avsikt med projekt

{{planning-important-intro}}

Lär dig hur du skapar en strategisk koppling mellan dina högnivåplaner i Adobe Workfront Planning och ditt dagliga utförande i Workfront. Du kan bygga en bro mellan strategi och körning med hjälp av anslutningar.

Den här guiden är avsedd för Workfront-administratörer och arbetsytehanterare som implementerar Workfront Planning.

## Översikt över att anpassa strategi till körning

Att koppla er strategi till ert dagliga arbete omvandlar visionen till verklighet. När högnivåplaner är synkroniserade med körning skapar ni en strategisk tråd som ser till att alla projekt och uppgifter flyttar verksamheten framåt.

För att uppnå den här anpassningen krävs en uppsättning tekniska länkar och processskydd som kopplar samman insatser i Workfront med strategiska register i Workfront Planning.

Genom att överbrygga klyftan mellan planering och handling ser du till att teamets energi alltid är inriktad på de mål som har högst prioritet.

## Skapa grunden genom att skapa en anslutning

Innan du kan brygga planering och körning måste du som arbetsytehanterare definiera vilka posttyper som är berättigade för en anslutning.

### Översikt över anslutningsfältet

Bron börjar med att skapa ett anslutningsfält.

Ett anslutningsfält fungerar som en teknisk handskakning mellan posttyper.

Den här fälttypen är motorn bakom alla relationer i Workfront Planning. Det är ett uttryck för avsikt, i det att det fastställer att en viss posttyp (som en kanaltaktik) kan länkas till andra objekttyper, oavsett om de bor i Planning eller Workfront.

Mer information finns i [Översikt över anslutna posttyper](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Definiera när en anslutning ska skapas

I idealfallet måste du bestämma om du behöver skapa anslutningar innan något arbete skapas.

Genom att lägga till ett anslutningsfält skapar du en miljö som stöder en strategisk tråd, oavsett hur de enskilda posterna skapas till slut.

## Ställ in strategi och körning synkroniserat

Vi rekommenderar att du inriktar dig på dina strategiska lager genom att fokusera dina planeringsdokument på hög nivå samtidigt som du använder Workfront för taktisk exekvering.

Den här metoden använder de unika styrkorna för båda modulerna på följande sätt:

* **Workfront Planning (det strategiska lagret):** Står på hög nivå. Det spårar Campaign, Channel Tactic och Budget. Det är bullerfritt och verkställande.

* **Workfront (körningslagret):** Hantera de taktiska detaljerna. Ni kan hantera enskilda upplevelser eller aktiviteter som projekt, uppgifter och ärenden. Du kan tilldela dem för ägarskap och bygga in godkännanden för körning.

## Gå från avsikt till åtgärd genom att aktivera bryggan

När anslutningen har konfigurerats måste du bestämma hur länken mellan en viss strategisk post och ett körningsprojekt ska aktiveras.

### Använda en tabell-ledd bana

Strategister och avancerade användare använder ofta tabellvyn som sin workbench för att förfina planerna över tid.

När du skapar en post i en tabell skapas som standard ingen länk till Workfront.

Anslutningen till ett körningsprojekt upprättas när en användare bestämmer sig för att aktivera länken.

Detta kan göras på följande sätt:

* Skapa manuellt ett projekt som är anslutet längre fram i kedjan direkt från anslutningsfältet i Workfront Planning eller från en valfri Connections-sida i postens detaljvy.

  Manuellt skapande resulterar i ett tomt projekt utan specifika anpassade formulär.

  Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

* Automatiskt, med Workfront Planning Automations, för mer komplexa behov.

  Dessa automatiseringar är tillgängliga som knappar i åtgärdsfältet när du markerar en rad i en tabell.

  Detta gör att man kan lägga in tillsyn eller platshållare, vilket säkerställer att projekten bara genereras i arbetsflödesmiljön när de verkligen behövs.

  Mer information finns i [Skapa objekt med hjälp av postautomatisering för Adobe Workfront Planning ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Skapa automatiska aktiveringar

För organisationer med stora volymer eller avancerade automatiseringsbehov kan bryggan aktiveras automatiskt baserat på specifika händelser eller baserat på fältvärden som konfigurerats i ett begärandeformulär.

Du behöver en licens för Adobe Workfront Fusion för den här metoden.

Mer information finns i [Konfigurera och hantera Workfront Fusion: artikelindex](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **Använd utlösare för överföring:** Eftersom formulär erbjuder en enda, ren inskickningshändelse kan de användas som utlösare för Fusion-automatisering. Ett Fusion-scenario kan identifiera en formulärskickning och omedelbart generera ett länkat projekt i Workfront.

* **Använd fältvärdesutlösare:** Du kan konfigurera Fusion för att övervaka specifika fält. En enkel kryssruta med namnet&quot;Klart för körning&quot; kan fungera som katalysator och automatiskt upprätta bryggan när den är markerad.

## Lägg till sökfält till synlighet för yta

När ett projekt är länkat kan du visa realtidsdata från Workfront direkt i Planning-posten genom att lägga till sökfält från projektet.

Som arbetsytehanterare kan du konfigurera sökfält så att alla system eller anpassade fält hämtas från det länkade projektet (till exempel Verkligt slutförandedatum eller Creative Lead) till posttypen Planering. När dessa data har samlats in kan de samlas in på flera nivåer i er strategiska hierarki, ända upp till kampanjnivån. Detta ger en kraftfull aggregerad rapportering för intressenter under hela marknadsföringscykeln, så att de hålls informerade utan att behöva lämna planeringsmiljön.

## Få synlighet genom att koppla ihop strategi med handling

Det ultimata värdet för bron är synlighet i realtid.

Genom att koppla avsikten till en åtgärd kan ni snabbt besvara viktiga affärsfrågor. Nedan följer några exempel på dessa frågor:

* Levererar vår kampanj&quot;FY26 Brand Awareness&quot; aktivt resultat just nu?

* Var behöver vår strategiska strategi mer kreativ support för att hålla tidsplanen?

* Hur anpassar vi våra resurser till våra högprioriterade strategiska pelare?

## God praxis och tips

### Dos:

* **Använd metaforen &quot;strategisk tråd&quot;:** Påminn team om att alla projekt ska vara en&quot;tråd&quot; i en strategisk sträng.

* **Automatisera överföringen:** Använd automatisering för att starta projektframtagning för att spara tid och arbete samtidigt som du förbättrar dataanslutningen och styrningen.

* **Länk, duplicera inte:** Använd sökfält för att visa körningsdata i realtid (som status eller slutförandedatum) i dina strategiska poster. Detta gör att dina strategiska vyer alltid är korrekta utan att ditt team behöver göra manuella uppdateringar.

### Gör inte:

* **Hantera inte planeringsposter som uppgiftslistor:** Bryggan är utformad för att ansluta strategisk återgivning till körningsprojekt. Håll dina planeringsdokument fokuserade på&quot;vad&quot; och&quot;varför&quot; och låt arbetsflödesmodulen hantera detaljerade&quot;hur&quot;-uppgifter och ärenden.

* **Översynkronisera inte:** Du behöver inte synkronisera alla projektnivådetaljer tillbaka till Planning. Håll det strategiska lagret högt och utan brus.

* **Åsidosätt inte bryggan:** Om arbetet startar i arbetsflödesmodulen utan en länk till Planning har du skapat en&quot;Skuggplan&quot; som inte syns för ledningen.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



