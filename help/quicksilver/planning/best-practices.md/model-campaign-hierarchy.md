---
title: 'Framgångsramverket: Modellera er kampanjhierarki'
description: Lär dig hur ni översätter komplexa affärsprocesser till en skalbar, styrd kampanjhierarki med"Centers of Gravity" och en arkitektur för flera arbetsytor.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# Framgångsramverket: utforma kampanjhierarkin

<!--see the file again for additional comments from Seth and others-->

## Mål

Lär dig hur ni översätter komplexa affärsprocesser till en skalbar, styrd kampanjhierarki med&quot;Centers of Gravity&quot; och en arkitektur för flera arbetsytor.



## Översikt

I takt med att era marknadsföringsaktiviteter skalas upp gör även komplexiteten hos era data. Utan en tydlig plan kan ert Marketing System of Record (MSOR) snabbt bli en&quot;skräplåda&quot; med icke-sammankopplade poster, motstridig terminologi och rapportisoleringar.



&quot;Blueprint of Success&quot; är ett ramverk för att utforma kampanjhierarkin i Workfront Planning. Det går från&quot;kaos i kalkylblad&quot; till en styrd, objektorienterad modell som ser till att alla i teamet talar samma språk och samtidigt behåller den flexibilitet de behöver för att kunna genomföra.



## Hierarki: Hitta dina återgivningsnivåer

För att behålla tydlighet och skalbarhet rekommenderar vi att du börjar med en beprövad **kärnsökväg**. Organisationer kan utöka hierarkin allt eftersom deras operativa behov utvecklas, men med dessa tre nivåer blir det en stark bro mellan strategi och utförande.



### Kärnvägen: Strategi till handling

De mest framgångsrika implementeringarna har en tydlig modell i tre nivåer som omfattar både planering och arbetsflöde:



1. **Nivå 1: Kampanjer (planeringsmodul)**

   * **Fokus:** Långsiktiga strategiska pelare och årsinitiativ (t.ex.&quot;Global Brand Awareness&quot;).

   * **Persona:** Marknadschef, VP of Marketing, Strategic Leads.

2. **Nivå 2: Kanaltaktik (planeringsmodul)**

   * **Fokus:** Operativa genomgångar som definierar vad för specifika kanaler (t.ex. Q1 Social Media Blitz). Det här är det sista lagret med strategisk avsikt innan arbetet börjar.

   * **Persona:** Marknadsföringsobjekt, kanalleads, kampanjansvariga.

3. **Nivå 3: Arbetsflödesprojekt (arbetsflödesmodul)**

   * **Fokus:** Den faktiska körningen av &quot;upplevelser&quot; eller &quot;aktiviteter&quot; (t.ex. specifika sociala inlägg, e-post, webbsidor).

   * **Implementering:** Tactik i Planering länkar direkt till **Projekt** i arbetsflödesmodulen, där individuella leveranser hanteras som aktiviteter och ärenden.

   * **Persona:** Kreatörer, enskilda medarbetare.



### Strategisk expansion: lägga till fler nivåer

När affärsvägen är etablerad kan man välja att lägga till ytterligare lager efter att man noga övervägt deras specifika komplexitet:



* **Kanalplaner:** Ett lager mellan *Kampanjer* och *Taktik* som grupperar korsfunktionella strategier (t.ex.&quot;Digital strategi&quot;).

* **Workfront planeringsaktiviteter:** I miljöer med mindre volymer (vanligen &lt;5 000 slutprodukter/år) föredrar vissa team att spåra enskilda&quot;upplevelser&quot; som Workfront Planning-poster innan de blir projekt.


>[!TIP]
>
>**Betydande tips: Tröskelvärdet 5 000 för slutprodukt**
>
>Om din organisation producerar mer än 5 000 aktiviteter per år bör du **alltid** avlasta enskild slutproduktsspårning till **arbetsflödesmodulen**. Hantering av stora volymer av&quot;upplevelseposter&quot; i Planning kan leda till datainsamling som döljer er er strategiska synlighet. Använd Planering för&quot;Varför&quot; och&quot;Vad&quot; och arbetsflödesmodulen för den stora volymen&quot;Hur&quot;.



## Arkitektur: Gravitets centrum

En MSOR på enterprisenivå är inte inbyggd i en enda arbetsyta. Den använder en&quot;Hub-and-Spoke&quot;-arkitektur där posttyper hanteras i sina naturliga **Centrers of Gravity**.



### &#x200B;1. Taxonomihubben (klassificeringar)

Upprätta en central arbetsyta för dina&quot;Global Classifications&quot; (t.ex. varumärken, regioner, produkter, personas).

* **Primär plats:** Den här arbetsytan är sann Source för dessa objekt.

* **Fördelen:** Genom att syndikera dessa definitioner till resten av verksamheten löser du&quot;Semantic Drift&quot;, vilket säkerställer att&quot;Region: EMEA&quot; betyder samma sak för alla team.



### &#x200B;2. Strategic Planning Workspace (Executive Centre)

Det är här som **kampanjer** på hög nivå (och alla **kanalplaner**) finns.

* **Primär plats:** Detta är tyngdpunkten i ledningen och ger en brusfri miljö för strategiskt beslutsfattande.

* **Fördelen:** Ledarskap kan hantera portföljen utan att behöva se den dagliga taktiska röran.



### &#x200B;3. Funktionella penseldrag (arbetsytor för team)

Funktionsenheter (Social, Creative, Email) har egna arbetsytor för att hantera sina **taktik**.

* **Primär plats:** De här arbetsytorna är tyngdpunkten för lokal gruppkörning.

* **Fördelen:** Team&quot;konsumerar&quot; globala kampanjer och klassificeringar från navet, samtidigt som de behåller sina egna lokala objekt (som *Mediekanaler* eller *användningsrättigheter*).



## Icke-baserad styrning: Tala ett språk

Följ principen för **ICKE-baserad styrning** för att se till att din plan hålls under tryck.



* **Använd antal, inte verb:** Namnge dina posttyper efter de &quot;saker&quot; som du spårar (`Campaign`, `Tactic`), inte efter &quot;åtgärder&quot; (`Campaigning`, `Planning`).

* **Standardiseringsnomenklatur:** Använd samma namn på alla arbetsytor. På så sätt kan ni samla in data i hela portföljen för företagsintern rapportering.



## Vad gäller för befintliga portfolior och program?

En vanlig fråga för mogna organisationer är hur de ska hantera de portföljer och program som de redan har skapat i **arbetsflödesmodulen**. Tidigare användes dessa objekt ofta för att efterlikna strategisk planering.



### &#x200B;1. Portföljer &amp; program → Posttyper

I många organisationer används **Portföljer** för att representera varumärken eller affärsenheter på hög nivå (BU), medan **Program** representerar strategiska teman.

* **Skift:** De här modellerna är bäst som **Posttyper** i din **taxonomihubb**. Genom att behandla&quot;Varumärke&quot; eller&quot;Affärsenhet&quot; som en posttyp kan du länka dem till valfri kampanj eller taktik i hela företaget, vilket ger en mycket mer flexibel rapportering än en statisk Portfolio/Program-struktur.



### &#x200B;2. The Reporting Bridge Strategy

Även om Workfront Planning är framtiden för strategiska avsikter kommer den interna rapporteringen via **Canvas Dashboards** fortfarande att fungera. Många organisationer förlitar sig fortfarande på de kraftfulla rapporteringsfunktionerna som är knutna till deras tidigare Portfolio- och programstrukturer i arbetsflödesmodulen.

* **Rekommendationen:** Ta inte bort dina portföljer och program än. Använd i stället **Fusion Automations** för att skapa en brygga.

* **Så här fungerar det:** När en aktivitet eller kampanj skapas i Workfront Planning kan Fusion automatiskt spegla posten till en motsvarande Portfolio eller ett program i arbetsflödesmodulen. På så sätt kan du:

   1. Använd Workfront Plannings **överlägsna strategiska visualisering** (tidslinjer/kalendrar).

   2. Underhåll din **gamla**-rapportering i arbetsflödesmodulen för intressenter som ännu inte är redo att gå över till arbetsytan.

## Bästa praxis och tips

### Gör:

* **Håll dig till kärnsökvägen först.** Upprätta ditt arbetsflöde från kampanj till interaktion till projekt innan du lägger till mer komplexitet.

* **Ange primära arbetsytor.** Kontrollera att varje posttyp har en hemarbetsyta (tyngdpunkten) som fungerar som aggregator för rapportering.

* **Prioritera Forms för intag.** Använd postformulär för grupper med mindre finess i Workfront Planning för att säkerställa metadataintegriteten. Power Users kan ha nytta av direkt datainmatning i tabellvyer, men detta bör hanteras med försiktighet - större förändringar i en tabell kan enkelt skapa datarubriker för andra intressenter.


### Gör inte:

* **Säg inte &quot;Core&quot;.** Referera specifikt till **arbetsflödesmodulen** och **Project** -objekten när du pratar om körning.

* **Överdriv inte kompliceringen.** Varje ytterligare hierarkinivå lägger till en&quot;hanteringsskatt&quot;. Lägg bara till nivåer som besvarar en affärsfråga som du inte kan svara på just nu.

* **Skapa inte isoleringar.** Kontrollera att posttyperna delas mellan arbetsytorna så att team inte skriver om samma data.




