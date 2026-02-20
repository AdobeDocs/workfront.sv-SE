---
title: Adobe Workfront planeringsrekommendationer för implementering
description: Som marknadsledare kan ni använda Adobe Workfront Planning för att organisera arbetet under hela marknadsföringscykeln för alla era team. Det här är några tips som vi rekommenderar när vi börjar med Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '3405'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Implementeringsrekommendationer för Adobe Workfront Planning

<!-- this used to be called Adobe WFP best practices, but the best practice piece was replaced by this folder of articles: [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) -->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, en extrafunktion från Adobe Workfront.
>
>En lista över krav för åtkomst till Workfront Planning finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Allmän information om Workfront Planning finns i [Kom igång med Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>
>För mer information rekommenderar vi även att du konsulterar artiklarna i [Adobe Workfront Planning best practices: artikelindex](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

Som marknadsledare kan ni använda Adobe Workfront Planning för att organisera arbetet under hela marknadsföringscykeln för alla era team.

I den här artikeln beskrivs några vanliga frågor och metodtips som vi rekommenderar när vi börjar med Workfront Planning.


## Bästa praxis för konfiguration

### Arbetsytor

Arbetsytorna är centraliserade platser där team kan planera arbetet. En arbetsyta är en samling posttyper som används av ett team och representerar teamets arbetslivscykel.

Nedan följer några vanliga frågor om hur du konfigurerar Workfront Planning.

#### Hur ska jag börja?

* ✅ När du loggar in på Planning för första gången följer du vår introduktionsprocess i appen som tydligt anger Planning värde och vägleder dig om hur du navigerar och använder produkten effektivt. Detta gör att du enkelt kan förstå dess funktioner och hur du enkelt kan börja arbeta.
* ✅ Börja med att utforska våra fördefinierade arbetsytemallar för idéer om befintliga liknande användningsfall. Du kan använda de fördefinierade posttyperna och fälten som finns i en mall eller lägga till egna.
* ✅ Identifiera de huvudsakliga användningsfall du vill lösa med Workfront Planning. De flesta organisationer vill till exempel förbättra synligheten i strategiska aktiviteter, som kan inkludera att skapa en bättre&quot;kampanjkalender&quot;. I det fallet vill du börja med att svara på några frågor:

   * Vem ber om det?
   * Vad kallas de saker de vill ha i kalendern?
Kampanjer? Tactik? Initiativ? Verksamheter? Händelser?
   * Vilka typer av frågor vill de svara på med den här kalendern?
   * Har de några överlappande kampanjer för samma målgrupp?
   * Vad är budgeten för den kampanjen, taktiken, aktiviteten eller händelsen?

  Svaren på dessa frågor styr vad du behöver bygga inuti Workfront Planning.

  Tänk också på att det kan finnas andra planerare som för närvarande inte använder Workfront. Dessa planerare kan arbeta med Excel-kalkylblad, Word-dokument, PowerPoint-presentationer osv. Tänk på hur de kan komma åt dina data i Workfront Planning.

* ✅ Om du vill utnyttja Workfront Planning till fullo bör du ersätta användningen av portföljer och program i Workfront med någon annan överordnad struktur i Workfront Planning.

  Idag representerar Workfront kunder sitt strategiska arbete genom portfolior och program, i vissa fall som projekt av olika slag. I och med lanseringen av Planning bör allt sådant strategiskt arbete hanteras med anpassade posttyper i Workfront Planning, medan Workfront kommer att centreras kring den körningsfas som utgörs av projekt och uppgifter.

#### När ska jag skapa en ny arbetsyta istället för att ändra en befintlig?

* ✅ Designa för den lägsta volymen av arbetsytor på organisationsnivå. Du kan skapa arbetsytor för specifika enheter för operativ organisation, så att de matchar det unika sätt som varje enhet fungerar på.

  Att ha informationen i en enda Workspace säkerställer att relationen mellan alla data enkelt kan hanteras.

  Försök till exempel att skapa en enda arbetsyta för all marknadsföring.

  Det är ok att skapa en ny arbetsyta för ett team som har en helt annan operativ struktur:

  En **produktutvecklingsyta** bör till exempel skilja sig från en **marknadsyta**.

* ⛔ Skapa inte unika arbetsytor för varje team eller process i en organisation.

  Marknadsföringsorganisationen bör sträva efter att behålla endast en arbetsyta för att bibehålla synligheten och tillåta data att samlas på global planeringsnivå.

  Undvik att skapa liknande eller dubblerade arbetsytor för team som följer liknande processer (t.ex. EMEA Marketing jämfört med APAC Marketing), särskilt där dessa team kan arbeta som leder upp till vanliga strategiska kampanjer.

#### Hur ska jag använda Workspace Sections?

* ✅ Skapa och etikettera avsnitt som hjälper dina användare att förstå hur du organiserar din operativa livscykel.

  Du kan till exempel skapa ett avsnitt med namnet **Core records** där du placerar dina kampanjer, taktik och slutprodukter på din arbetsyta.
* ✅ Gruppera posttyper som liknar.

  Du kan till exempel skapa ett avsnitt med namnet **Geografier** som innehåller posttyper som: Region, Land och Ort.

### Posttyper

Posttyper är byggstenarna i en Workfront Planning Workspace. Du kan definiera hur posttyper ska kopplas samman.

#### Hur definierar jag posttyper på arbetsytan?

* ✅ Ta dig tid att identifiera vilken information du behöver spåra (vilka posttyper jag behöver) och hur den här informationen behöver kopplas. Tala med de intressenter som ska använda arbetsytan för att ta hänsyn till alla deras behov. Du kan också skapa anpassade avsnitt med olika posttyper för att presentera informationen på ett mycket användbart sätt.

* ⛔ Duplicera inte posttyper för en annan period (skapa till exempel inte separata posttyper för **Campaigns 2024** och **Campaigns 2025**).

  När du skapar olika posttyper bryts dataflödet när du vill jämföra data över flera år. Vyerna i dag är per posttyp, så så när året avslutas kommer vyn av den posttypen inte längre att visa framtida artiklar. Det bästa sättet är att ha en posttyp för arbetstypen och segmentera data med filter som baseras på olika fält eller vid behov arkivera dem.

#### När ska jag använda ett enskilt eller flervalsfält jämfört med en länkad posttyp?

* ✅ Lägg till en ny posttyp om objektet kommer att användas i anslutning till flera andra posttyper

  En kampanj kan till exempel ha en anslutning till flera målgrupper, och en aktivitet kan ha en anslutning till en enda målpublik. Därför bör Campaign, Tactic och Audience vara posttyper i stället för flervalsfält.

* ✅ Lägg till en ny posttyp om objektet behöver lagra ytterligare metadatavärden som kan vara användbara i uppslag

  En kanalposttyp, till exempel **E-post**, kan exempelvis lagra en lista över vilka slutprodukter som stöds, antingen som interna metadata eller som en anslutning till en fristående **slutprodukter** -posttyp.
* ⛔ Lägg inte till en ny posttyp om de data du lagrar bara är relevanta för en enskild posttyp.

  En **Campaign**-posttyp kan till exempel ha ett envalsfält med namnet **Kampanjstorlek** som bara är relevant när det är direkt kopplat till en viss kampanj. Skapa ett fält i stället om du vill hämta informationen.

#### Hur ska jag märka mina posttyper?

* ✅ Skapa och etikettera posttyper som representerar en enda konstruktion eller ett enda substantiv, till exempel **Kampanjer**.
* ⛔ Skapa inte en posttyp som bättre representeras som en vy.

  **Kalender** är till exempel ett dåligt val för en posttyp eftersom det inte är själva posttypen, utan en vy med poster.

### Fälthantering

Fält är attribut för posttyper och visas som kolumner i tabellvyn. Du kan skapa anpassade fält för posttyper och sedan associera fälten med Workfront Planning-poster för att förbättra postinformationen.

#### Vilket fält rekommenderas för att definieras som primärt fält?

* ✅ Använd unika primära fältvärden för att göra det enklare att hitta och&quot;hämta&quot; dessa poster när du skapar anslutningar. 

  När du skapar en anslutning söker användarna efter värdena i fältet Primär och om de inte är unika vet användarna inte vilken de ska välja. 
* ⛔ Undvik att använda icke-unika värden som primärt fält eftersom det kan skapa förvirring för användare som måste söka i det primära fältet när de använder anslutningsväljarmenyn. 

#### Hur ska jag använda formler?

* ✅ Använd formelfälttyper för att minska manuell inmatning. När du anger information baserat på data som redan finns i tabellvyn kan du spara en del arbete genom att beräkna informationen automatiskt med hjälp av formler.

#### Hur ska jag börja ansluta data på min arbetsyta?

* ✅ Att skapa anslutningar är en av de mest kraftfulla funktionerna i Workfront Planning. Du kan ansluta posttyper till varandra eller posttyper med objekttyper från andra program, som Adobe Workfront (anslutning till projekt, portföljer, program, företag och grupper), Adobe Experience Manager Assets (anslutning till resurser och mappar) och Adobe GenStudio for Performance Marketing.

  Genom att koppla objekt och posttyper får du en fullständig översikt över hur allt i företaget är sammankopplat.

  Du har till exempel posttypen **Campaign** och posttypen **Tactics**, och du kan skapa en anslutning mellan de här två posttyperna för att se vilka **Tactics** som är kopplade till en viss **Campaign**.

  När du har definierat anslutningen kan alla personer på arbetsytan börja lägga till värden för **kampanjer** genom att dubbelklicka i anslutningsfältet där de ser en lista över alla **taktik** som är tillgängliga. På så sätt kan ni snabbt hitta vilken taktik som behöver kopplas till era kampanjer.

#### Hur ska jag använda uppslagsfält?

* ✅ När du har upprättat anslutningen mellan poster eller objekttyper kan du ansluta enskilda poster till varandra och visa fält från den länkade posten eller objekttyperna på en Workfront Planning-post. Du minskar antalet platser där du måste uppdatera samma information och se till att de matchar perfekt.

  När du till exempel har en anslutning mellan posttypen **Campaign** och posttypen **Tactics**, ser du den primära fältinformationen, men när du lägger till uppslagsfält kan du hämta ytterligare information från den posttypen, till exempel **Startdatumet** för en **aktivitet** . Data för dessa sökfält fylls i automatiskt efter att posterna har lagts till.

#### Vilken fälttyp rekommenderas för URL:er? 

* ✅ Använd ett textfält med en rad för att lägga till URL-data till en post.

### Vyer

#### Hur avgör jag vad som ska vara en vy eller en posttyp?

* ✅Skapa en posttyp för objekt som representerar en enskild konstruktion eller ett substantiv (till exempel **Kampanjer**). 

* ⛔ Skapa inte en posttyp som bättre representeras som en vy.

  **Kalender** är till exempel ett dåligt val för en posttyp eftersom det inte är själva posttypen, utan en vy med poster. 

#### Ska jag dölja eller ta bort fält som inte är relevanta för mig?

* ✅ Dölj kolumnen i stället för att ta bort den när den här informationen kan vara relevant för en annan person som använder samma posttyp. Om du tar bort fältet i en viss tabellvy tas även det här fältet bort i resten av vyerna för den här posten, liksom i alla andra delar som den här posttypen är länkad från.

#### Hur ska jag använda filter och grupperingar i tabell- och tidslinjevyerna?

* ✅ Använd vyer med filter och grupperingar för att visa en ögonblicksbild av det du behöver se. Du kan filtrera och gruppera data så att de blir mer användbara för att förstå vad som planeras. Du kan gruppera posterna efter metadatafält.

  Du kan till exempel ha en tidslinjevy för posttypen **Campaign** som du kan gruppera efter **målgrupper** och filtrera den efter **Datum** så att endast det aktuella året visas.

#### Varför ser jag inte alla poster i min tidslinjevy?

* ✅ Kom ihåg att definiera 2 datumfält för dina poster. Du kan bara skapa en tidslinjevy om du har minst två datumfält kopplade till en posttyp. Vissa poster kanske inte visas i tidslinjevyn när start- eller slutdatumet eller båda inte har några värden eller när startdatumet är efter slutdatumet.

#### Hur använder jag tidslinjevisningsinställningarna?

* ✅ Definiera inställningarna för tidslinjevyn, till exempel **Stapelstil** och **Färg**, för att få en mer visuellt föränderlig vy. Du kan anpassa **stapelformatet** genom att definiera om du vill se en miniatyrbild med en meningsfull bild och lägga till fler fält som ska visas i fältet (till exempel **Ägare** eller **Status**).

  Som standard visas bara det primära fältet. Du kan också definiera färgen på stapeln efter fältvärden (du kan till exempel anpassa färgerna på staplarna genom att matcha den med statusfältet) eller efter den gruppering du har använt. Som standard matchar färgen färgen färgen för posttypen.

  Endast posttypsfärger eller fält med alternativ som är kopplade till färger kan påverka färgerna för postfälten på tidslinjen.

### Behörigheter och delning

Använd delningsfunktionen för att ge lämplig behörighet till andra för vyer och arbetsytor.

#### Hur hanterar jag behörigheter till arbetsytor?

* ✅ När du skapar en **arbetsyta** är den bara tillgänglig för dig. Alla andra som inte är systemadministratörer kan inte hitta den. När arbetsytan har definierats och du är redo att ta med teamet för att starta samarbetet, måste du dela den med dem och definiera deras behörighetsnivå.

  Du kan välja mellan följande behörighetsnivåer:

   * **Hantera**: Personer kan redigera, ta bort och dela arbetsytan, posttyper samt redigera, ta bort och skapa poster.
   * **Contribute**: Personer kan skapa, redigera och ta bort poster.
   * **Visa**: Personer kan visa poster.

* ✅ Även om många kunder känner att de skulle ge **Hantera** behörigheter till arbetsytor till de flesta, bör du begränsa **Hantera**-behörigheterna till en viss grupp med betrodda personer som inte av misstag tar bort en posttyp eller på annat sätt skapar onödiga posttyper och fält. De kan redigera, dela och till och med ta bort arbetsytan. Den här behörighetsnivån ger dem fullständig administrativ åtkomst till Workspace.

  En standardanvändarlicens krävs för att någon ska ha behörigheten Hantera på en arbetsyta.

* ✅ Ge användarna **Contribute** behörighet om du vill att de bara ska kunna skapa, redigera och ta bort poster, men du vill inte att de ska ändra arbetsytans struktur. Med **Contribute**-behörigheter kan de inte skapa posttyper eller ändra fälten på befintliga posttyper.

  En standardanvändarlicens krävs för att någon ska ha **Contribute**-behörighet till en arbetsyta.

* ✅ Ge användarna **Visa** behörigheter om du bara vill att de ska kunna visa poster.

#### Hur hanterar jag behörigheter för att spela in typer?

* ✅ Kom ihåg att användare med behörigheten Hantera på arbetsytor inte kan ha sina behörigheter nedsänkta för posttypen. De ärver även behörigheterna Hantera till posttypen. Du kan inte ge en användare behörigheten Hantera på arbetsytan, men Contribute eller Visa behörigheter för posttypen.
* ✅ Om du vill att användarna ska ha en lägre behörighetsnivå (till exempel Visa behörigheter) för posttypen än de har för arbetsytan, rekommenderar vi att de får Contribute-behörigheter till arbetsytan. Du kan sedan ge dem behörigheten Visa till posttypen.
* Om du tar bort en användare från posttypens behörigheter får användaren ändå minst behörigheten Visa på arbetsytan.

#### Hur hanterar jag behörigheter till vyer?

* ✅ Bevara behörigheterna **Hantera** för personer som du vill kunna redigera, ta bort och dela vyn. Det innebär att de kan ändra filter, grupperingsfält eller någon konfiguration av vyn. Ändringarna påverkar vyns huvudkonfiguration för alla andra som också använder vyn.

  En standardanvändarlicens krävs för att någon ska ha behörigheten Hantera för en vy.

* ✅ Ge användarna **Visa** behörighet att använda vyn. De kommer att kunna ändra vissa av filtren, grupperingarna och sorteringen, men dessa ändringar är bara tillfälliga. Ändringarna sparas inte för alla andra användare som kommer åt vyn. Ändringarna påverkar inte vyns huvudkonfiguration för alla andra som också använder vyn.  Ändringarna är bara synliga för den användare som använder de ändrade inställningarna. När skärmen har uppdaterats återställs ändringarna till standardvärdet.

* ✅ Ge **alla på arbetsytan behörighet att visa** när du vill att alla som kan visa arbetsytan ska kunna se posterna och fälten i den specifika vyn. På så sätt behöver du inte lägga till någon manuellt i delningsbehörighetsrutan för vyn.

  >[!NOTE]
  >
  >Om en vy inte har delats och du delar en länk till den med andra personer, kan de se posterna i **standardtabellvyn**. Om de har en Standard Workfront-licens kan de själva skapa en egen vy.

#### Hur skiljer sig **Workspace-delning** från **Visa delning**?

* **Workspace-delning** definierar andras åtkomst till arbetsytan, dess posttyper, poster och deras fält.

* **Visningsdelning** definierar om användaren kan se den vy som du har skapat och om han eller hon kan ändra filtret, grupperingsfälten eller någon annan konfiguration av vyn. Synligheten för posterna som visas i vyn styrs av delning med Workspace och inte av Visa delning.

#### Hur Workfront licenstyper påverkar behörigheterna för Workfront Planning?

* För **Workspace-delning**: Ljus- och Contribute-licensanvändare kan bara få åtkomst till en arbetsyta via Visa. Om du vill ge någon Contribute- eller Hantera-behörighet till en arbetsyta måste du ha en standardlicens.

* **Vydelning**: Standardlicensanvändare som har behörigheten Hantera på en arbetsyta kan skapa en vy. Ljus- och Contribute-licensanvändare kan bara använda de vyer som standardanvändare har skapat och delat med sig av. Om inget har delats kan användarna annars se **standardtabellvyn**.

#### Vad ska jag göra när en Workspace-ägare ändras?

* Workfront anger att arbetsytan ska skapas som ägare, men ägaren har samma behörigheter som alla användare med behörigheten Hantera.
* Om ägaren är inaktiverad kan andra medlemmar fortsätta arbeta på arbetsytan utan avbrott.
* Systemadministratörer har åtkomst till alla arbetsytor, så om ägaren var den enda personen med behörigheten Hantera kan administratörer lägga till en annan person och ge dem behörigheten Hantera för att hantera arbetsytan.

### Skicka begäranden i Workfront Planning

Du kan skapa ett begärandeformulär för varje posttyp om du vill att användare ska lägga till poster utanför en posttyps sida. När du skickar formuläret läggs en ny post till i posttypen.

#### När ska jag börja skapa ett begärandeformulär för en posttyp?

* ✅ Du bör kontrollera att posttypstrukturen har konfigurerats först genom att lägga till de nödvändiga fälten i tabellen. Dessa fält beskriver dina poster och kan nås i formulärbyggaren.

  Det bästa är om du bygger formuläret för begäran eller inmatning när posttypens struktur är klar, så att inga nyckelfält saknas.

#### Vem kan skapa frågeformulär?

* ✅ Alla användare med behörigheten Hantera på arbetsytan kan skapa eller redigera ett begärandeformulär för en posttyp. Kontrollera att användarens behörigheter är korrekt tilldelade för att tillåta den här funktionen.

#### Hur skapar eller redigerar jag ett begärandeformulär för en posttyp?

* ✅ Alla användare med behörigheten Hantera på arbetsytan kan följa stegen som beskrivs i artikeln [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### Vem kan skicka in nya poster med hjälp av frågeformuläret?

* ✅ Sändningsbehörigheter beror på inställningarna som du konfigurerar för varje formulär.

  När du har publicerat formuläret i formulärbyggaren kan du hantera behörigheter för att styra vem som kan skicka begäranden.

  Du kan välja mellan följande delningsalternativ:

   * För intern delning med människor i Workfront:

      * **Alla som visar eller har högre åtkomst till arbetsytan:** Tillåter alla användare med behörighet att visa eller högre på arbetsytan att skicka en begäran som skapar en post.
      * **Alla som har Contribute eller senare åtkomst till arbetsytan**: Begränsar överföringar till användare med Contribute eller högre behörighet till arbetsytan.
      * **Endast inbjudna personer kan komma åt**: Lägg till personer, team, roller, grupper eller företag som kan skicka begäranden till formuläret.
   * För extern delning med personer som inte har ett Workfront-konto:
      * **Skapa en offentlig länk**, kopiera och dela den sedan med vem som helst, även med personer som saknar ett Workfront-konto: Gör det möjligt för alla som har formulärlänken att skicka en begäran.
      * **Länkens förfallodatum:** Kontrollera att du har angett ett förfallodatum för den offentliga länken för att förbättra säkerheten.

### Metodtips för att hantera förfrågningsformulär

Nedan följer några rekommendationer för hur du hanterar förfrågningsformulär:

* Planera i förväg: Definiera tydligt vilken information som behövs eller som krävs från den som gjorde begäran innan formuläret skapas för att undvika överdrivet många ändringar senare.
* Använd tydliga etiketter: Se till att fältetiketter och beskrivningar är tydliga och begripliga för alla användare.
* Testa formulär: Innan du distribuerar nya formulär till en större publik bör du testa dem med hjälp av formulärlänken och förhandsgranskningsalternativet för formulär för att säkerställa att alla fält och logik fungerar som förväntat.
* Håll formulären uppdaterade: Granska formulär regelbundet och uppdatera dem för att matcha ändringar i posttypsstrukturen eller operativa processer.

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/sv/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/sv/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/sv/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->