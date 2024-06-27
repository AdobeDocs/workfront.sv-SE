---
title: Adobe Workfront Planning best practices
description: Som marknadsledare kan ni använda Adobe Workfront Planning för att organisera arbetet under hela marknadsföringscykeln för alla era team. Det här är några tips som vi rekommenderar när vi börjar med Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Adobe Workfront Planning - bästa praxis

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Som marknadsledare kan ni använda Adobe Workfront Planning för att organisera arbetet under hela marknadsföringscykeln för alla era team.

I den här artikeln beskrivs några metodtips som vi rekommenderar när vi börjar med Workfront Planning.

## Vad är Workfront Planning?

Workfront Planning-modulen är en av tre distinkta, men sammankopplade, Workfront-funktioner som tillsammans skapar ett väl fungerande marknadsföringssystem. De tre funktionerna är:

* **Planering**: De nya avancerade funktionerna i Workfront Planning.

* **Arbetsflöde**: De samarbetsfunktioner du använder idag i Workfront (projektledning, resurshantering etc.)

* **Automatisering och integrering**: De omfattande integrerings- och automatiseringsfunktionerna i Workfront Fusion.

Workfront Planning är mycket anpassningsbart. Mer information om Workfront Planning - terminologi och nyckelbegrepp finns i [Adobe Workfront Planning - översikt](/help/quicksilver/planning/general/planning-overview.md).

## Frågor att ställa innan du konfigurerar Workfront Planning

När du har lärt dig Workfront Planning-terminologi och -arkitektur kan du börja skapa en ny miljö.

Några frågor du kan ställa själv när du konfigurerar Planning är:

* **Vill jag använda arbetsytor för större organisationsgrupper? Eller borde jag uppmuntra folk att skapa egna?**

  Du kanske tycker att det finns en bra användning för båda. Vi rekommenderar att du inte har för många arbetsytor eftersom de kan bli svåra att hantera och arbetsflödena kan vara för fragmenterade.

  >[!TIP]
  >
  >    Du kan ha 1 000 arbetsytor i en Workfront-instans.

* **Vilka anpassade posttyper ska jag skapa på varje arbetsyta?**

  Posttyper fungerar som Workfront objekttyper. Fundera på arbetsflödena och bestäm vilka posttyper (arbetsobjekt, personobjekt, taxonomier osv.) som ska användas varje arbetsflöde kan behöva.

  Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md)

* **Hur ska jag skapa mina register? Finns det en extern lista eller ett kalkylblad som redan innehåller de poster jag behöver lägga till i Planning som jag kan använda? Kommer poster att läggas till gradvis beroende på behov? Eller kommer de att importeras med Fusion eller anpassad API-integrering?**

  Mer information finns i:

   * [Skapa poster](/help/quicksilver/planning/records/create-records.md)
   * [Adobe Workfront Planning-moduler](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **Vilka fält behöver jag skapa för mina register?**

  Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

* **Vilka Workfront- eller AEM Assets-objekttyper behöver jag ansluta till Workfront Planning-posttyper för att kunna visa beroenden och skapa ett smidigt arbetsflöde för min organisation?**

  Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md)

* **Vilka marknadsföringskalendrar och vyer behöver jag berätta om mina kampanjer? Och vilka intressenter kan jag göra dessa vyer tillgängliga för smidigt samarbete?**

  Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).


## Workfront Planning - bästa praxis

I det här avsnittet visas flera riktlinjer för åtgärder och tips för lämpliga metoder när du konfigurerar Workfront Planning.

Riktlinjerna är ordnade beroende på vilket objekt eller område du ställer in.

### Arbetsytor

#### The do&#39;s and don of workspaces

* Designa för den lägsta volymen av arbetsytor på organisationsnivå

  Försök till exempel att skapa en enda Workspace för all marknadsföring

* Utför regelbundet kurser i arbetsytorna. Du kanske kan ändra en befintlig i stället för att skapa en ny från början.

* Skapa en ny Workspace för ett team som har en helt annan operativ rörelse.

  En arbetsyta för produktutveckling ska skilja sig från en arbetsyta för marknadsföring

* Skapa inte en unik arbetsyta för varje liten grej. Se arbetsytorna mer som ett arkivsystem som kan vara till nytta för en hel organisation och göra det möjligt för alla att mappa arbetsflöden och samarbeta i stället för att använda en privat arbetsyta för att hålla reda på personliga förfrågningar.

* Skapa inte unika arbetsytor för varje team eller process i en organisation.

  Marknadsföringsorganisationen bör sträva efter att behålla endast en arbetsyta för att bibehålla synligheten och tillåta att data samlas på global planeringsnivå.

  Undvik att skapa likartade eller duplicerade arbetsytor för team som följer liknande processer (t.ex. EMEA: s marknadsföring VS APAC-marknadsföring), särskilt där dessa team kan arbeta som sammanfaller med en gemensam strategisk kampanj.

#### Hur ska jag använda arbetsyteavsnitt?

* Skapa och etikettera avsnitt som hjälper användarna att förstå hur ni organiserar er operativa livscykel.

  Du kan till exempel skapa ett avsnitt med namnet&quot;Kärnposter&quot; där du placerar ut kampanjer, taktik och slutprodukter.

* Gruppera posttyper som liknar.

  Du kan skapa ett avsnitt med namnet&quot;Geografiska&quot; som innehåller posttyper som: Region, Land och Ort.

#### Hur hanterar jag behörigheter för arbetsytan?

* Begränsa&quot;Hantera&quot;-åtkomsten till en viss grupp med betrodda personer, som inte av misstag tar bort en posttyp eller på annat sätt skapar onödiga posttyper och fält.

  >[!TIP]
  >
  >Under betaprogrammet har vi fått veta att många kunder känner att de kommer att ge gruppadministratörer&quot;Hantera&quot;-åtkomst.

* Lägg till planeringsområdet i layoutmallen för användare med en standardlicens.

* Tillåt inte användare med en standardlicens att skapa personliga arbetsytor. Det ger dem en säker arbetsyta att lära sig verktyget och bli bekväma med det. Detta kommer inte att röja andras upplevelser och kan förbättra användarens personliga produktivitet.

  >[!TIP]
  >
  >    Rekommendera dem att inte dela sina personliga arbetsytor som en god vana.


### Posttyper

#### Ett enskilt eller flervalsfält jämfört med en länkad posttyp

* Skapa en ny posttyp om objektet ska användas i flera andra posttyper

  En kampanj kan till exempel ha en anslutning till flera målgrupper, och en aktivitet kan ha en koppling till en enda målpublik.

* Bygg en ny posttyp om objektet behöver lagra ytterligare metadatavärden som kan vara användbara i uppslag.

  En kanalposttyp som &quot;E-post&quot; kan t.ex. lagra en lista över slutprodukter som stöds, antingen som inbyggda metadata eller som en anslutning till en fristående &quot;slutprodukt&quot;-posttyp.

* Lägg inte till en ny posttyp om de data du lagrar bara behöver omfång till en enda posttyp. Använd ett urvalsfält i stället.

  En Campaign-posttyp kan t.ex. ha ett envalsfält med namnet Kampanjstorlek som bara är relevant när det är direkt kopplat till en viss kampanj.

#### Hur ska jag märka mina posttyper?

Skapa och etikettera posttyper som representerar en enskild konstruktion eller ett substantiv, till exempel&quot;Campaigns&quot;

:no_entry_sign: Skapa inte en posttyp som bättre representeras som ett visningslager - t.ex. &quot;Kalender&quot; är ett dåligt val för en posttyp, eftersom det inte är själva posttypen utan en vy över poster.

### Hur många lager i hierarkin ska jag skapa?

Vyer

...

Arbetsflöde

...

### Fälthantering

Primärt fält

Använd unika primära fältvärden för att göra det enklare att hitta och&quot;hämta&quot; posterna när du skapar anslutningar.

När du skapar en anslutning söker användarna efter värdena i fältet Primär och om de inte är unika vet användarna inte vilken de ska välja.

Undvik att använda icke-unika värden som primärfält eftersom det kan skapa förvirring för användare som måste söka i det primära fältet när de använder anslutningsväljarmenyn.



Från Chris O&#39;Neal:

Ett annat område att tänka på är användningsområden som är (eller inte är) bäst när det gäller planering. Till exempel den resurshanteringsdiskussion vi hade idag.



Alinas anteckningar:

Exempel på artikeln&quot;Best practices&quot; från ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Ytterligare information från fältberedskap från Lauren S: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346