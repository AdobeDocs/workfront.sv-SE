---
title: 'Playbook: Managed Scaling, After the First Win'
description: Lär dig lansera Adobe Workfront Planning efter den första implementeringen
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 28913661935d5a030cb33dd204fcb3c08daf0b26
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---


# Playbook: hanterad skalning, efter första win

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