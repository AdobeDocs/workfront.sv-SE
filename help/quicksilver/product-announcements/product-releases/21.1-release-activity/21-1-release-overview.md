---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatera
navigation-topic: product-releases
title: 21.1 - versionsöversikt
description: 21.1-utgåvan gjordes tillgänglig i produktionsmiljön samma vecka som .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3658'
ht-degree: 0%

---

# 21.1 - versionsöversikt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Den här sidan innehåller information om funktionaliteten för både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen som ingår i version 21.1.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

I den här versionen har vi släppt nya funktioner och förbättringar som hjälper dig att leda återkomsten under 2021 med anpassningsbara strategier, automatiserade arbetsprocesser och en sammankopplad digital infrastruktur som möjliggör framgång i hela företaget.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Dessa förbättringar är för närvarande tillgängliga

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

i produktionsmiljön.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

De släpptes veckan 15 februari 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättrad resurshantering](#resource-management-enhancements)
* [Förbättrad projekthantering](#project-management-enhancements)
* [Förbättrade analysfunktioner](#enhanced-analytics-improvements)
* [Integration enhancements](#integration-enhancements)
* [Mobilförbättringar](#mobile-enhancements)
* [Andra förbättringar](#other-enhancements)

### Administratörsförbättringar {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Ny åtkomstnivåinställning för kopiering av projekt</a> </p> <p>För att du som systemadministratör ska få större kontroll över vad planerare kan göra med ett projekt har vi gjort redigeringsåtkomsten till projekt på åtkomstnivån mer detaljerad genom att införa en ny inställning som gör att du kan aktivera eller inaktivera möjligheten att kopiera projekt. När du aktiverade användarnas åtkomst till redigeringsprojekt hade de automatiskt åtkomst till att kopiera dem före den här ändringen. Med den nya funktionen kan du ge någon åtkomst till redigeringsprojekt utan att nödvändigtvis ha tillgång till kopiera dem genom att inaktivera den nya inställningen Kopiera.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">I ett anpassat formulär på ett objekt markerar du alla objekt i ett flervalsfält</a> </p> <p>När du fyller i ett flervalsfält i ett anpassat formulär på informationssidan för ett objekt kan du klicka på Markera alla om du behöver markera alla tillgängliga alternativ.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Inte tillgängligt för tillfället när du skickar en ny begäran.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Beräkna om alla anpassade formulärfält för ett objekt</a> </p> <p>Nu är det enklare att se till att alla data i beräknade anpassade fält är aktuella för ett objekt. Med det nya menyalternativet Beräkna om uttryck kan du snabbt beräkna om alla data i dessa fält.</p> <p>Detta är särskilt användbart när någon har redigerat data i ett annat objekt som refereras av ett beräknat anpassat fält i objektet.</p> <p>Tidigare var användarna tvungna att använda tillfälliga lösningar för att säkerställa att alla data i beräknade anpassade fält var aktuella. De redigerade till exempel objektet tillsammans med andra objekt för att använda det omberäkningsalternativ som är tillgängligt för massredigering.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 10 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Lås upp uppgifter och utgivningsinställningar för gruppadministratörer</a> </p> <p>Workfront-administratörer kan nu ge gruppadministratörer mer självbestämmande genom att låsa upp enskilda uppgifter och utgåvor. När en inställning är olåst kan gruppadministratörer konfigurera den för sina grupper så att den passar varje grupps unika behov och interna processer.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Före den 24 juni 2021 var detta endast tillgängligt som en del av en fasad utrullning för kunder i kluster 4 och 6 samt några andra kunder. Nu finns det i Production för alla kunder.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Konfigurera åtkomstnivåinställningar för portföljer och program separat</a> </p> <p>Nu är det enklare att hantera användaråtkomst till portföljer och program eftersom du kan konfigurera deras åtkomstnivåinställningar separat.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Markera alla kryssrutor i en serie när du redigerar information i ett anpassat formulär</a> </p> <p>När du fyller i ett fält för anpassat formulär som innehåller kryssrutor på informationssidan för ett objekt kan du klicka på Markera alla om du behöver markera alla kryssrutor som är tillgängliga.</p> <p>Det här alternativet visas bara om fältet innehåller fler än två kryssrutor.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Inte tillgängligt för tillfället när du skickar en begäran.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Konfigurera din Workfront-e-postadress tillåtelselista</a> </p> <p>För att skydda dina data bättre kan du nu använda en e-postdomän som tillåtslista till:</p> 
    <ul> 
     <li> <p>Styr var Workfront e-postmeddelanden kan skickas om de innehåller rapporter eller dokument som lagras i Workfront</p> </li> 
     <li> <p>Kontrollera e-postdomäner i den e-postadress som användarna kan ange i sina användarprofiler</p> </li> 
    </ul> <p>Om du t.ex. vill skydda känsliga data, t.ex. en rapport med en lista över dina riskkunder, kan du bara inkludera din interna e-postdomän eller domäner i e-postmeddelandet som tillåtslista. På så sätt kan användare inte skicka den rapporten (eller någon annan Workfront-rapport) till en extern e-postadress.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: Med version 21.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Tilldela en gruppadministratör för en undergrupp</a> </p> <p>För att göra det enklare för olika nivåer i organisationen att arbeta oberoende har vi lagt till möjligheten att tilldela en gruppadministratör till en undergrupp. Nu kan du se till att du delegerar hantering av undergrupper till rätt personer.</p> <p>Tidigare var det bara en grupp på den översta nivån som kunde ha gruppadministratörer och dessa administratörer hanterade alla undergrupper under den översta gruppen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Arbeta med gruppprojekt och godkännandeprocesser i området Grupper</a> </p> <p>Om du är gruppadministratör är det enkelt att visa och arbeta med gruppens projekt och godkännandeprocesser nu när de listas i gruppområdet. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Konfigurera händelsemeddelanden för grupper</a> <span style="color: #dc143c; font-weight: bold;">Nyheter i förhandsvisning!</span></p> <p>Workfront-administratörer kan nu ge gruppadministratörer större självständighet genom att tillåta dem att konfigurera händelsemeddelanden för sina toppnivågrupper. Undergrupper ärver händelseaviseringskonfigurationer från den översta överordnade gruppen.</p> <p>Tidigare var händelsemeddelanden bara konfigurerbara av en Workfront-administratör på systemnivå, vilket innebär att alla grupper måste använda samma uppsättning händelsemeddelanden.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 22 januari 2021</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Inledningsvis endast tillgängligt i produktion för kunder i kluster 4 som en del av en fasad utrullning; tillgängligt för andra kluster kort därefter)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Visa antalet licenser som används och tilldelas i en grupp</a> </p> <p>För att avgöra hur bra licenserna distribueras kan du nu visa antalet licenser som används i en grupp och eventuella undergrupper under den.</p> <p>Om du hanterar en grupp på den översta nivån kan du visa både antalet licenser som används i en grupp (och dess undergrupper) och det maximala antalet licenser som tilldelas för gruppen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrad resurshantering {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Utjämning av arbetsbelastning för projekt</a> </p> <p>Utjämningen av arbetsbelastning är nu tillgänglig i ett projekt. Nu har du ett alternativ för att välja mellan att använda arbetsbelastningsutjämnaren eller schemaläggningsverktyget för att hantera dina projektresurser.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 17 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront Balancer för ett team</a> </p> <p>Utjämningen av arbetsbelastning är nu tillgänglig i ett team. Nu har du ett alternativ för att välja mellan att använda belastningsutjämnaren eller schemaläggningsverktyget för att hantera dina teamresurser. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrad projekthantering {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Export finns nu i avsnittet Metrics i ett projekt</a> </p> <p>Om du enklare vill dela status och förlopp för ett projekt kan du nu exportera hela kontrollpanelen i avsnittet Metrisk i ett projekt till en PNG-fil.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 15 januari 2021</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Uppdatera utleveransprocent slutfört när projektet eller aktiviteten konverterades från utleveransuppdateringen</a> </p> <p>Vi har uppdaterat hur procentandelen slutförda problem fungerar för problem som har konverterats till projekt eller uppgifter. När ett problem konverteras till en aktivitet eller ett projekt uppdateras procentandelen slutfört av problemet synkroniserat med procentandelen slutfört för den åtgärd eller det projekt som åtgärdas när inställningen"Uppdatera lösningsstatus automatiskt när statusen för det objekt som löses ändras" aktiveras från konfigurationen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Fält som tagits bort från sidan Ny begäran</a> </p> <p>Som en del av omdesignen av sidan Ny begäran har vi uppdaterat de nya fält för problem som har konfigurerats i avsnittet Köinställningar i ett projekt.</p> <p>Olika fält för nya problem visas bara när du skapar ett problem i projektets problemavsnitt. De visas inte när du skickar ett problem med hjälp av en frågekö i området Begäranden.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Borttagen från version)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny upplevelse när begäranden skickas i området Förfrågningar</a> </p> <p>För att skapa enhetlighet med den nya Workfront-upplevelsen och för att effektivisera när du skickar in begäranden har vi gjort om rutan Ny begäran i området Begäranden.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Borttagen från version; kommer att finnas kvar i förhandsgranskning och i Production med version 21.2)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Dela en länk till en begärandekö när du skickar en begäran</a> </p> <p>Vi har nu gjort det möjligt att dela en länk till en begärandekö, en ämnesgrupp eller ett köämne medan du skapar en begäran.</p> <p>Innan du skickar en ny begäran kan du kopiera en länk till begärandekön, ämnesgruppen eller köämnet för begäran och dela den med andra användare, eller bädda in den i en instrumentpanel.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 13 januari 2021</p> <p>Produktionsrelease: Med version 21.1 <span style="color: #dc143c; font-weight: bold;">(Borttagen från version; kommer att finnas kvar i förhandsgranskning och i Production med version 21.2)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Lista över nya skickade begäranden</a> </p> <p>För att du ska kunna hantera dina skickade begäranden på ett enklare och mer konsekvent sätt har vi tagit bort avsnitten Begäranden som jag har skickat och Alla begäranden i området Begäranden och ersatt dem med en ny skickad lista. Listan har en välbekant utseende som matchar alla andra listor i systemet, vilket gör att du kan filtrera efter olika kategorier av skickade begäranden och snabbt söka efter en begäran som kan vara svår att hitta.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Söka efter en grupp som du vill tilldela ett projekt och visa information om den</a> </p> <p>Nu är det enklare att se till att du identifierar rätt grupp när du tilldelar en grupp till ett projekt. Håll muspekaren över namnet på en grupp som du hittar i grupprutan och klicka sedan på infoikonen som visas bredvid namnet för att visa verktygstipset Gruppinformation.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 17 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Ny delegeringsrapport för användare</a> </p> <p>Tidigare kunde information för delegering av uppgifter, utgåvor och projektgodkännande endast visas av delegaten i hemområdet. Om du vill att andra användare ska kunna se den här informationen kan plananvändarna nu skapa rapporten för användardelegering, som innehåller följande information:</p> 
    <ul> 
     <li> <p>Vem har delegerat godkännandena till en annan användare</p> </li> 
     <li> <p>Vilken användare har delegerats dessa godkännanden</p> </li> 
     <li> <p>Start- och slutdatum för dessa delegationer</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 17 december 2020</p> <p>Produktionsrelease: 21 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrade analysfunktioner {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">Personsidan är nu tillgänglig för alla kluster</a> </p> <p>Sidan Personer är nu tillgänglig på Workfront Classic för kluster 4. Den här sidan innehåller diagram för aktivitet per team, resurskapacitet och teamkapacitet.</p> <p>Den här sidan var tidigare tillgänglig med version 20.3 i både Workfront Classic och den nya Workfront-upplevelsen för alla andra kluster.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 28 januari 2021</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Den nya Adobe Workfront-upplevelsen (tidigare)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Förbättrade analysfunktioner visas nu som standard</a> </p> <p>Obs! Den här ändringen gäller endast användare som nyligen har lagts till i layoutmallar. Användare som har tilldelats en anpassad layoutmall påverkas inte heller av den här ändringen.</p> <p>I standardlayoutmallen är Analytics-området nu aktiverat som standard, vilket innebär att användare som är tilldelade den här layoutmallen nu kan se Analytics-området i det globala navigeringsfältet i Workfront Classic och huvudmenyn i den nya Workfront-upplevelsen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 6 november 2020</p> <p>Produktionsrelease: 3 december 2020</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Förbättrad analys tillgänglig för alla kluster</a> </p> <p>Förbättrad analys finns för alla Workfront-kluster, inklusive kunder med kluster 6.</p> <p>Tidigare fanns det ingen förbättrad analys tillgänglig med Google Cloud Platform, vilket förhindrar att kunder i kluster 6 får tillgång till Analytics-området. Nu har Business- och Enterprise-kunder i kluster 6 tillgång till Analytics-området.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 20 november 2020</p> <p>Produktionsrelease: 3 december 2020</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Integration enhancements {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Förbättringar av Adobe Workfront-meddelanden i Microsoft Teams</a> </p> <p>För att göra det enklare för dig att använda Workfront via Microsoft Teams har vi lagt till olika förbättringar i Microsoft Teams-meddelanden som skickas från Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: Ej tillämpligt</p> <p>Produktionsrelease: 12 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mobilförbättringar {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya navigeringsskyltar i Adobe Workfront-appen</a> </p> <p>Vi har lagt till brödtextnavigering i Workfront mobilapp. Nu kan du använda den här funktionen för att navigera till överordnade arbetsobjekt i ett projekt.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: Ej tillämpligt</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">RTF i anpassade formulär i Workfront-appen</a> </p> <p>Nu kan du använda RTF-formatering i anpassade formulärtextfält i Workfront mobilapp.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: Ej tillämpligt</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO-användare kan nu logga in på nytt i Workfront-appen med ansikts-ID eller fingeravtrycksteknik</a> </p> <p>Om din organisation använder enkel inloggning (SSO) kan du nu använda ditt ansikts-ID eller fingeravtryck för att logga in på Workfront-mobilappen efter att sessionen har avslutats. Du måste dock logga in med dina SSO-inloggningsuppgifter från början.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: Ej tillämpligt</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
—&gt;

### Andra förbättringar {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Uppdateringar av kraven för misslyckade händelseprenumerationer</a> </p> <p>Vi uppdaterar kraven för mjuk inaktivering vid fel med händelseprenumeration. Förutom de befintliga kraven inaktiveras nu även Event-prenumerationer om de inte lyckas leverera inom 2 000 försök. Detta är för att stärka den befintliga 70-procentiga felregeln, som under vissa omständigheter kan leda till alltför många fel.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: Ej tillämpligt</p> <p>Produktionsrelease: 11 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya Team-fält tillgängliga för Daily Digest</a> </p> <p>Vi har lagt till fälten för teamgodkännande och tilldelningar i e-postmeddelandet Åtgärd krävs varje dag.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 17 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">Ersätta POP-e-postalternativ i begärandeköer</a> </p> <p>Vi ersätter POP-e-postalternativet för begärandeköer med ett nytt system som hanteras av Workfront. Du kan fortfarande skicka begäranden via e-post, men du måste konfigurera en ny e-postadress som hanteras av Workfront i området Begärandekö i stället. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 17 december 2020</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Begränsa timredigering för tidrapporter</a> </p> <p>För att få bättre kontroll över tidrapporter och timredigering har vi lagt till en inställning som tillåter dig att begränsa timredigering till tidrapportsägare och systemadministratörer.</p> <p>Tidigare kunde användare med alternativet Tidrapporter och timmar aktiverat på åtkomstnivån redigera timmar på alla tidrapporter.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 21 januari 2021</p> <p>Produktionsrelease: Med version 21.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Förbättrade filter och vyer i området Tidrapporter</a> </p> <p>Vi har lagt till filter för projekt och problem samt lagt till alternativen Visa och Gruppera på söksidan.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: 21 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Dölja övertidsrutan i tidrapporter</a> </p> <p>Du kan nu dölja övertidsrutan för att förenkla för användaren om du inte spårar övertid i Workfront. Du kan dölja övertidsrutan för en enskild tidrapport eller i tidrapportprofilen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 2 december 2020</p> <p>Produktionsrelease: 16 december 2020</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Expandera eller komprimera objekt i navigeringen i vägbeskrivningar</a> </p> <p>För att det ska bli enklare att visa hela sökvägen har vi lagt till funktionerna för att expandera och komprimera.</p> <p>Nu grupperas alla trunkerade objekt före projektet med texten "mer". "3 till" betyder t.ex. att det finns 3 objekt som inte visas.</p> <p>Tidigare var du tvungen att klicka på ellipsen för att visa trunkerade objekt i en nedrullningsbar meny.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 7 januari 2020</p> <p>Produktionsrelease: 21 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt utseende och ny känsla för banbrytande navigering</a> </p> <p>För att hjälpa användare att bättre identifiera var de befinner sig i Workfront och enklare navigera mellan objekt har vi förbättrat breadcrumb-navigeringen flera gånger.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Betaversion: 10 december 2020</p> <p>Produktionsrelease: 21 januari 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

## Förbättringar av Workfront-mål

De flesta nya funktionerna som kommer till Workfront Goals-versionen i version 21.1. Mer information om de här nya funktionerna som nu finns i Förhandsgranska finns i [Adobe Workfront Goals with the 21.1 release](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Förbättringar av Workfront Scenario Planner

Nya funktioner i Workfront Scenario Planner i version 21.1. Mer information om de här nya funktionerna som nu finns i Förhandsgranska finns i [Adobe Workfront Scenario Planner med version 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än 21.1-versionen. Mer information om de senaste funktionerna finns i [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API-förbättringar

API-version 12 är nu tillgänglig med version 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Information om nyheter och uppdateringar finns på [Nyheter i API-version 12](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i version 21.1 finns i [Workfront Maintenance Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Meddelanden

* [Nya IP-adresser för Workfront e-post med version 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Tillåtelselista på ytterligare IP-adresser för händelseprenumerationer](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Tillåtelselista av ytterligare domäner som krävs för åtkomst till Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Borttagning av Flash](#flash-deprecation)
* [21.1 Release Webinar](#21-1-release-webinar)
* [Ändringar i förhandsgranskningsversionsstatus](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Nya IP-adresser för Workfront e-post med version 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

I ett försök att öka e-postleveransen lägger vi till nya IP-adresser med 21.1-produktionsutgåvan för kluster 1, 2, 3, 4 och 5.

Mer information om vilka IP-adresser du måste lägga till för ditt kluster finns i [Nya IP-adresser för Adobe Workfront e-post med version 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

Om du vill ta reda på vilket kluster du är ansluten till går du till Inställningar > System > Kundinformation.

### Tillåtelselista på ytterligare IP-adresser för händelseprenumerationer {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

I ett försök att öka den lyckade leveransen av händelseprenumerationer lägger vi till fyra nya IP-adresser med 21.1-produktionsutgåvan under första kvartalet 2021. Du måste lägga till de här IP-adresserna i tillåtelselista före februari 2021 för att se till att dina användare fortfarande får händelseprenumerationer.

Kontakta din interna IT- och/eller säkerhetsavdelning om du behöver hjälp med att lägga till de nya IP-adresserna som finns i artikeln, [API för händelseprenumeration](../../../wf-api/general/event-subs-api.md).

### Tillåtelselista av ytterligare domäner som krävs för åtkomst till Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Om din organisation använder en brandvägg måste du lägga till följande ytterligare domäner i tillåtelselista för att säkerställa oavbruten åtkomst till Workfront:

* event.split.io
* sdk.split.io

Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Borttagning av Flash {#flash-deprecation}

Alla verktyg för Flash togs bort från alla produkter den 19 november 2020.

Läs mer om ersättningslösningar för respektive verktyg i följande Flash: [Ersättning av verktyg baserade på Flash i Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### 21.1 Release Webinar {#21-1-release-webinar}

Workfront 21.1 Release Webinar presenteras den 3 februari kl. 11.00 EDT / kl. 17.00 BST. Registrera dig för webbinariet [här](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Ändringar i förhandsgranskningsversionsstatus {#change-in-preview-release-cadence}

Från och med den 20 maj 2020 började Workfront att tillgängliggöra funktioner i förhandsvisningsmiljön varje vecka. Före den här ändringen släpptes funktionen vanligtvis till förhandsvisningsmiljön varannan vecka.

Mer information finns i [Ändringar i Workfront förhandsgranskningsversion, vanliga frågor och svar](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Med Workfront One hittar du det viktigaste innehållet, resurserna och nyheterna från Workfront - allt på ett och samma ställe, med en enda inloggning. Vi har samlat webbplatserna för upplevelser, community och utbildning, vilket gör det enklare att hitta det du söker.

[Läs mer om Workfront One](https://www.workfront.com/campaigns/workfront-one).
