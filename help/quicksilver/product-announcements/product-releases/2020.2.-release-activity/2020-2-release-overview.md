---
content-type: release-notes
navigation-topic: product-releases
title: Översikt över version 2020.2
description: Version 2020.2 gjordes tillgänglig i produktionsmiljön den 11 maj 2020. Den senaste informationen om status för releasen finns på Workfront statuswebbplats. Den här sidan innehåller information om de funktioner som ingår i version 2020.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88a97b1e-4052-485e-8566-963c6ba640b9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2544'
ht-degree: 0%

---

# Översikt över version 2020.2

Version 2020.2 gjordes tillgänglig i produktionsmiljön den 11 maj 2020.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For the most up-to-date information regarding the release status, see the
<a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This page provides information about the functionality included in the 2020.2 release.
</MadCap:conditionalText>
-->

Den här sidan innehåller information om funktioner för både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen som ingår i version 2020.2.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 2020.2 release nears its planned Production release, this page will be updated with all functionality included with 2020.2.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of May 11, 2020. For specific release dates and times for each cluster, see the <a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <MadCap:conditionalText data-mc-conditions="OnlineOrPDF.OnlineOnly">
To download this page in PDF&nbsp;format, go
<a href="https://documentation.my.workfront.com/library/a/9f5c9e44-c9a9-4f33-beec-9e5dc2e0fdc2" target="_blank">here</a>.
</MadCap:conditionalText> </p>
-->

## Förbättringar för administratörer

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-other-enhancements.md#for" class="MCXref xref" xrefformat="{para}">För Workfront-administratörer: Nyare layoutmallar som skapats i Workfront Classic finns nu tillgängliga i den nya Workfront-upplevelsen</a> </p> <p>Layoutmallar som skapats i Workfront Classic efter hösten 2019 finns nu i den nya Workfront-upplevelsen. Det är en bra idé att uppdatera dessa layoutmallar i den nya Workfront-upplevelsen för att utnyttja de nya funktionerna och göra dem så användbara som möjligt för användare i den miljön. </p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsrelease: 6 april 2020</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-project-enhancements.md#for2" class="MCXref xref" xrefformat="{para}">För Workfront-administratörer: Förbättrad design i projektinställningarna</a> </p> <p>Upplevelsen av att ange projektinställningar är nu mer intuitiv och lättanvänd.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 13 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-project-enhancements.md#for" class="MCXref xref" xrefformat="{para}">För Workfront-administratörer: Nytt felsäkert när projektstatusen för nya projekt är dold eller olåst</a> </p> <p>För att säkerställa att nya projekt alltid har en status, även om en administratör döljer eller låser upp statusen som konfigurerats för nya projekt, tilldelar systemet nu den första statusen i statuslistan till alla nya projekt tills du konfigurerar den nya statusen för nya projekt igen.</p> <p>Mer information om hur du anger inställningar för status för alla nya projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref" xrefformat="{para}">Konfigurera systemomfattande projektinställningar</a>.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 13 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## Förbättringar för alla användare

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Some functionality was released prior to the 2020.1 release. To see what was released prior to the 2020.1 release, see <a href="../../../product-announcements/product-releases/2020.1-release-activity/prior-to-2020-1.md" class="MCXref xref" xrefformat="{para}">Other Workfront Classic features released to Production prior to the 2020.1 release</a>.</p>
-->

Version 2020.2 innehåller följande förbättringar för alla användare:

* [Förbättringar av resurshantering: Utjämning av arbetsbelastning](#resource-management-enhancements-the-workload-balancer)
* [Projektförbättringar](#project-enhancements)
* [Språkförbättringar](#proofing-enhancements)
* [Mobila förbättringar](#mobile-enhancements)
* [Andra förbättringar](#other-enhancements)

### Förbättrad resurshantering: Utjämning av arbetsbelastning {#resource-management-enhancements-the-workload-balancer}

Personer är en Tier 1-resurs. Med belastningsutjämnaren kan du skydda dem från utbränning och ge dem möjlighet att göra sitt bästa, samtidigt som de anpassas till viktiga företagsstrategier.

Vi presenterar en omdesignad schemaläggningsfunktion som gör att du kan visualisera och hantera människors arbetsbelastning och efterfrågan i samma vy. Användargränssnittet ger tydlig visuell mappning av över- och underanvändning och är transparent för alla intressenter. Personhanterare kan använda den informationen som indata och från samma skärm balansera arbetet genom tidslinjen, som sedan återspeglas i resten av Workfront-plattformen.

>[!NOTE]
>
>Utjämningen av arbetsbelastning började lanseras som en betaversion i version 2019.4. Alla förbättringar av belastningsutjämnaren är i allmänhet tillgängliga i version 2020.2. Följande förbättringar lades till i version 2020.2. En översikt över belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#a" class="MCXref xref" xrefformat="{para}">Ett bekvämare sätt att uppdatera allokeringar i arbetsbelastningsutjämnaren</a> </p> <p>För att göra det enklare att hantera en användares tilldelningar till en arbetsuppgift i Utjämning av arbetsbelastning kan du nu dubbelklicka på arbetsposten. Du kan även använda menyalternativet Redigera allokeringar. Dessutom behöver du inte längre aktivera displaying-allokeringar för att kunna uppdatera dem.</p> </td> 
   <td> <p>Beta Preview-version: 8 maj 2020</p> <p>Produktionsrelease: Med version 2020.2 <span style="color: #ff0000;">(Borttagen från version; kommer att vara tillgänglig i förhandsversion och produktion i en fasad lansering strax efter version 2020.2.)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#update" class="MCXref xref" xrefformat="{para}">Uppdatera aktivitetsplanerade timmar i arbetsbelastningsutjämnaren</a> </p> <p>Ett nytt alternativ i området Resurshantering på åtkomstnivån ger nu användare med den här åtkomsten möjlighet att redigera Planerade timmar från belastningsutjämnaren. När du justerar allokeringar i belastningsutjämnaren behöver den totala dagliga allokeringen inte matcha antalet planerade timmar för aktiviteterna. När du har sparat dina allokeringar blir det totala antalet allokeringstimmar antalet planerade timmar för uppgiften. Detta är bara möjligt för aktiviteter som har en enkel varaktighetstyp.</p> </td> 
   <td> <p>Beta Preview-version: 8 maj 2020</p> <p>Produktionsrelease: Med version 2020.2 <span style="color: #ff0000;">(Borttagen från version; kommer att vara tillgänglig i förhandsversion och produktion i en fasad lansering strax efter version 2020.2.)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#adjust" class="MCXref xref" xrefformat="{para}">Justera daglig- och veckoallokering i Utjämning av arbetsbelastning</a> </p> <p>För att undvika att resurser belastas kan du nu justera användarnas dagliga och veckovisa allokering så att de fungerar med hjälp av Utjämning av arbetsbelastning. </p> <p>Före den här förbättringen var detta bara möjligt med verktygen för resursplanering.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2 <span style="color: #ff0000;">(Borttagen från version; kommer att vara tillgänglig i förhandsversion och produktion i en fasad lansering strax efter version 2020.2.)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#workload" class="MCXref xref" xrefformat="{para}">Utjämningsfilter för arbetsbelastning</a> </p> <p>Om du vill göra informationen i Utjämning av arbetsbelastning relevant för dig kan du nu skapa filter för både Ej tilldelat arbete och Tilldelade arbetsområden i Utjämning av arbetsbelastning och spara dem för framtida bruk. Du kan sedan redigera den sparade versionen för att göra små ändringar i den i stället för att börja från början med ett nytt filter.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#show" class="MCXref xref" xrefformat="{para}">Visa återstående timmar i arbetsbelastningsutjämnaren</a> </p> <p>För att du ska kunna fatta rätt beslut om tilldelning kan du nu med en ny inställning visa skillnaden mellan antalet timmar mellan de timmar som en användare är tillgänglig att arbeta enligt sitt schema och de timmar som han/hon redan har tilldelats till arbetet (återstående timmar). Den nya inställningen är nu tillgänglig i Utjämning av arbetsbelastning.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#show2" class="MCXref xref" xrefformat="{para}">Visa planerade timmar per dag för aktiviteter och projekt i området Ej tilldelat arbete i Utjämning av arbetsbelastning</a> </p> <p>För att du lättare ska förstå hur uppgifter påverkar arbetsbelastningen för dina användare innan du tilldelar dem hanterar inställningen Visa tilldelningar nu vilken information som visas i området Ej tilldelat arbete i Utjämning av arbetsbelastning. När den här inställningen är aktiverad visas Planerade timmar för både uppgifter och projekt i området Ej tilldelat arbete i Utjämning av arbetsbelastning.</p> <p>Före den här ändringen uppdaterades endast information i området Tilldelad arbetsyta i Utjämnaren.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Den nya Adobe Workfront-upplevelsen (tidigare endast för uppgifter)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#new2" class="MCXref xref" xrefformat="{para}">Rutan Nya inställningar för arbetsbelastningsutjämnaren</a> </p> <p>För att effektivisera din upplevelse finns nu en inställningsruta som visar ytterligare verktyg för att uppdatera vyn i belastningsutjämnaren. Den här rutan innehåller följande inställningar:</p> 
    <ul> 
     <li>Gruppera efter projekt</li> 
     <li>Visa antingen Allokerade timmar eller Återstående timmar för dina aktiviteter och projekt.</li> 
    </ul> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#share" class="MCXref xref" xrefformat="{para}">Dela arbetsbelastningsutjämnaren med en länk</a> </p> <p>Nu kan du dela personalens arbetsbörda med chefer så att de kan få en kontext om personalens behov. För detta kan du nu dela arbetsbelastningsutjämnaren genom att dela en unik URL till arbetsbelastningsutjämnaren med någon annan.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#alter" class="MCXref xref" xrefformat="{para}">Ändra datumintervallet i arbetsbelastningsutjämnaren</a> </p> <p>För att ytterligare hjälpa dig att anpassa tidslinjens varaktighet för belastningsutjämnaren så att den passar dina behov kan du nu välja en anpassad period på 2, 4 eller 6 veckor att visa samtidigt. </p> <p>Före den här förbättringen visas alltid information om arbetsbelastningsutjämnaren med början i den aktuella veckan.</p> </td> 
   <td> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Den nya Adobe Workfront-upplevelsen (tidigare)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-resource-management.md#removing" class="MCXref xref" xrefformat="{para}">Tar bort betaetiketten från arbetsbelastningsutjämnaren </a> </p> <p>I version 2020.2 är arbetsbelastningsutjämnaren inte längre i betaversion och du kan använda resursutjämnaren för att granska och hantera resurstilldelningar och allokeringar. Betaetiketten har tagits bort i förhandsvisningsmiljön. Samma ändring kommer att göras i 20.2-utgåvan. Mer information om belastningsutjämnaren för arbetsbelastning finns i <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref" xrefformat="{para}">Översikt över belastningsutjämnaren</a>.</p> </td> 
   <td> <p>Beta Preview-version: 8 maj 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Projektförbättringar {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-project-enhancements.md#moving" class="MCXref xref" xrefformat="{para}">Om du flyttar och kopierar aktiviteter till ett annat projekt behålls aktivitetsbegränsningen när aktiviteter får plats inom projektets tidslinje</a> </p> <p>Vi har förbättrat sättet som Workfront hanterar den datumspecifika uppgiftsbegränsningen för en uppgift när du kopierar uppgiften eller flyttar den till ett annat projekt. Exempel på datumspecifika aktivitetsbegränsningar är Måste starta, Måste sluta på, Fasta datum, Starta inte senare än och så vidare.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-project-enhancements.md#selected" class="MCXref xref" xrefformat="{para}">Markerat filter, vald vy och gruppering behålls i rapportlistor</a> </p> <p>Tidigare, när en användare tillämpade ett filter, en vy eller en gruppering på en rapportlista och sedan navigerade bort från den sidan, visades standardfiltret, vyn eller grupperingen nästa gång användaren navigerade till samma rapport.</p> <p>Nu väljs det senaste filtret, vyn eller grupperingen som tillämpats på en viss rapport, även om användaren loggar ut och in på Workfront igen.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-project-enhancements.md#preventi" class="MCXref xref" xrefformat="{para}">Förhindra dataförlust när du gör ändringar på fliken Information eller i en uppgiftslista</a> </p> <p>För att förhindra dataförlust när du uppdaterar information på detaljsidan för ett objekt eller uppgifter i en uppgiftslista på projektnivå när du sparar ändringar manuellt, visas ett varningsmeddelande som meddelar dig om att du har osparade ändringar innan du navigerar bort. De enda åtgärder som är tillåtna innan du sparar ändringarna är att prenumerera eller lägga till objektet i dina favoriter.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 22 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättringar av korrektur {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p> </p> <p>För att effektivisera samarbetet vid korrektur visas gästkommentarer i uppdateringsområdet.</p> <p>Tidigare fanns endast korrekturkommentarer från gäster tillgängliga i beviset.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 1 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p> </p> <p>Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till följande extra URL i din vitlista för att säkerställa att användare i organisationen kan visa korrektur i Workfront både i webbläsarvisningsprogrammet och i skrivbordsvisningsprogrammet:</p> <p>*.workfront.com</p> <p>*proofhq.com URL krävs fortfarande.</p> </td> 
   <td> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsversion: 9 maj 2020</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-mobile-enhancements.md#help" class="MCXref xref" xrefformat="{para}">Hjälp oss att testa den nya virtuella assistenten för mobila enheter i beta</a> </p> <p>Vi lanserar en ny virtuell assistent till Workfront mobilapp för både betatestare från Android och iOS.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 1 april 2020</p> <p>Produktionsrelease: TBD (kommer att släppas efter version 2020.2, andra halvåret 2020.)</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Endast betaprogram för mobiler. </p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-other-enhancements.md#group-sp" class="MCXref xref" xrefformat="{para}">Gruppspecifika godkännandeprocesser är tillgängliga för alla objekt</a> </p> <p>Om du vill utnyttja gruppspecifika godkännandeprocesser fullt ut kan du nu lägga till dem i uppgifter, ärenden och projekt när du redigerar dessa objekt.</p> <p>Du kan också automatiskt koppla en gruppspecifik godkännandeprocess till en uppgift i området Åtgärder i rutan Redigera projekt, samt till problem, när du konfigurerar begärandeköer eller Köämnen i ett projekt.</p> </td> 
   <td> <p>Beta Preview-version: 8 maj 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-other-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Skapa godkännandeprocesser för grupper med anpassade statusvärden</a> </p> <p>För att göra det enklare för grupper att hantera sina egna unika arbetsflöden kan du nu använda gruppspecifika anpassade statusvärden i godkännandeprocesser.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 10 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya övertäckningssidor för sökning</a> </p> <p>För att användarna enklare ska kunna navigera fram och tillbaka mellan söksidor och tidigare sidor i den nya Workfront-upplevelsen har vi lagt till en sökövertäckningssida som delvis täcker skärmen.</p> <p>När du klickar på Avancerad sökning på menyn Sök eller utför en grundläggande sökning öppnas nu en sida från skärmens högra sida.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 25 april 2020</p> <p>Produktionsrelease: Med version 2020.2</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Uppdateringar av händelseprenumerationer</a> </p> <p>För att göra det lättare för användare att trigga, felsöka och lösa problem har vi ändrat beteendet och lagt till mer data i API:t för händelseprenumerationer. </p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 1 maj 2020</p> <p>Produktionsversion: 8 maj 2020 </p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## API-förbättringar

API version 11 släppt med version 2020.1. Information om nyheter och uppdateringar finns i [Nyheter i API-version 11](../../../wf-api/api/new-api-version-11.md) [Nyheter i API-version 11](https://experience.workfront.com/s/article/What-s-new-in-API-version-11-1760875145).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md) [API-versionens utgåva och supportschema](https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1).

## Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i version 2020.1 finns i [Workfront Maintenance Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Meddelanden

* [Ändringen i förhandsgranskningsversionsstatus](#change-in-preview-release-cadence) Nyhet!

* [Lägger till ytterligare domäner till tillåtelselista som krävs för åtkomst till Workfront](#adding-additional-domains-to-the-allowlist-required-for-accessing-workfront)
* [Workfront One](#workfront-one)
* [2020.1 versionswebbseminarium](#2020-1-release-webinar)
* [Q1 Product Roadmap Webinar](#q1-product-roadmap-webinar)

### Ändringar i förhandsgranskningsversionsstatus {#change-in-preview-release-cadence}

Från och med 20 maj 2020 kommer Workfront att göra funktionerna tillgängliga i förhandsvisningsmiljön varje vecka. Före den här ändringen släpptes funktionen vanligtvis till förhandsvisningsmiljön varannan vecka.

Mer information finns i [Förändringar i Workfront förhandsgranskningsversion - frågor och svar](https://experienceleague.adobe.com/sv/docs/workfront/using/home)

### Lägga till ytterligare domäner till tillåtelselista som krävs för åtkomst till Workfront {#adding-additional-domains-to-the-allowlist-required-for-accessing-workfront}

Om din organisation använder en brandvägg måste du lägga till följande ytterligare domäner i tillåtelselista för att säkerställa oavbruten åtkomst till Workfront:

* event.split.io
* sdk.split.io

Mer information finns i avsnittet [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#urls) i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

Med Workfront One hittar du det viktigaste innehållet, resurserna och nyheterna från Workfront - allt på ett och samma ställe, med en enda inloggning. Vi har samlat webbplatserna för upplevelser, community och utbildning, vilket gör det enklare att hitta det du söker.

[Läs mer om Workfront One](https://business.adobe.com/products/workfront.html).

### 2020.1 Release Webinar {#2020-1-release-webinar}

Visa 2020.1-utgåvan av webbinariet [här](https://webinars.on24.com/workfront/product_roadmap032620?partnerref=blog).

### Q1 Product Roadmap Webinar {#q1-product-roadmap-webinar}

Läs mer om vad som kommer att hända under [Q1 Roadmap-webbinariet](https://webinars.on24.com/workfront/product_roadmap032620?partnerref=announcementcenter). Det här webbinariet hölls den 26 mars 2020. Klicka på länken för att registrera och se inspelningen på begäran.

Testa
