---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatera
navigation-topic: 2021-4-release-activity
title: 21.4 Versionsöversikt
description: Den här sidan innehåller information om funktionaliteten för både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen som ingår i version 21.4. för att hjälpa dig att öka produktiviteten och samarbetet.[Marknadsföring - ett streck för releasen]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '4718'
ht-degree: 0%

---

# 21.4 Versionsöversikt

Den här sidan innehåller information om funktionaliteten för både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen som ingår i version 21.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

Dessa förbättringar har gjorts tillgängliga i produktionsmiljön den 4 oktober 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Flexibla förbättringar](#agile-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättringar av resurshantering](#resource-management-enhancements)
* [Rapporteringsförbättringar](#reporting-enhancements)
* [Förbättringar av förfrågningar](#requests-enhancements)
* [Språkförbättringar](#proofing-enhancements)
* [Integreringsförbättringar](#integration-enhancements)
* [Mobila förbättringar](#mobile-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">För administratörer: Se vilka grupper som är associerade med en godkännandeprocess</a> </p> <p>För att du ska få reda på vilka grupper som är kopplade till godkännandeprocesserna i ditt system har vi lagt till en gruppnamnskolumn i standardvyn på sidan Godkännanden i Inställningar. Nu kan du visa den här informationen utan att behöva skapa en anpassad vy.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Grupper kan konfigurera egna inställningar för tidrapport och timme</a> </p> <p>I en stor organisation kan vissa grupper behöva konfigurera tidrapport- och timinställningar separat för att passa sina unika arbetsflöden, i stället för att ärva inställningarna som konfigurerats av en administratör på systemnivå. Nu kan Workfront-administratörer låsa upp en tidrapport och timinställning för alla grupper i systemet så att de själva kan konfigurera den.</p> <p>Den här funktionen lades också till nyligen för projektinställningar och för inställningar för uppgifter och utgåvor.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4 <span style="color: #ff0000;"> (ursprungligen endast tillgänglig i produktion för kunder i kluster 4)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt för Workfront-administratörer: Konfigurera layoutmallar för automatiskt tilldelade användare i den nya Workfront-upplevelsen</a> </p> <p>Nu kan du konfigurera layoutmallar i den nya Workfront-upplevelsen för användare som etablerats automatiskt. I listrutan Workfront-användarattribut, där du mappar användarattribut (Inställningar &gt; System &gt; Enkel inloggning), finns det nu ett nytt menyalternativ på menyn Ny layoutmall som du kan använda för att göra den här konfigurationen. Tidigare kunde du bara konfigurera layoutmallar för användare med automatisk etablering i Workfront Classic.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nytt fält visar de grupper som användarna tillhör</a> </p> <p>Nu är det enkelt att ta reda på vilka grupper användarna tillhör. I en rapport eller vy som listar användare kan du skapa en kolumn med det nya fältet Andra grupper. I det här fältet visas de grupper där varje användare är medlem.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Sidan med information om utkast visar nu en bild</a> </p> <p>På informationssidan för varje plan visas nu en bild av projektmallen som installeras tillsammans med ritningen. Bilden innehåller en förhandsvisning av det blå innehållet så att du vet vad du håller på att installera. Du kan också förhandsvisa hela bilden i webbläsaren eller hämta bilden.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Inställningar för utkast av nya utgåvor</a> </p> <p>Nya inställningar för utgåvor finns nu för vissa utkast. De installeras som standard, men du kan välja att inte installera inställningarna när du konfigurerar installationsinformationen.</p> <p>Inställningarna omfattar ämnesgrupper i kön, köämnen och routningsregler för att samla in korrekt information när ett problem eller en förfrågan skickas och skicka ärendet eller förfrågan till rätt jobbroll eller team. Inställningarna gör att du kan skapa ett konsekvent sätt att hantera nya utgåvor eller förfrågningar i dina projekt.</p> <p>Observera att när du använder dessa inställningar konverteras inte projekt som skapats från mallen till begärandeköer.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nytt för gruppadministratörer: Visa och hantera en grupps nyligen borttagna och återställda objekt</a> </p> <p>Vi fortsätter att göra det enklare att hantera dina grupper och tillhörande objekt på ett och samma ställe. Nu kan du visa och arbeta med en grupps nyligen borttagna och återställda objekt i området Grupper. Detta gör att du inte behöver gå till området Senast borttaget eller Senast återställt i installationsprogrammet för att hantera dessa objekt. Listan med gruppobjekt som du arbetar med hålls åtskild från andra borttagna och återställda objekt i systemet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 26 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nytt för gruppadministratörer: Gruppinställningar påverkar nu gruppmallar</a> </p> <p>Nu är det enklare att se till att gruppens projektmallar motsvarar gruppens behov. När du tilldelar en ny projektmall till en grupp när du skapar den, ärver mallen olika inställningar från gruppens projekt- och uppgiftsinställningar.</p> <p>När du skapar en ny malluppgift i en projektmall som är kopplad till en grupp, ärver malluppgiften olika inställningar från gruppens uppgiftsinställningar.</p> <p>Tidigare har projektmallar och projektmallsuppgifter ärvt dessa inställningar från projekt- och uppgiftsinställningarna som angetts på systemnivå.</p> <p>Om du skapar en mall- eller malluppgift utan en grupp, till exempel från sidan Huvudmallar, ärvs inställningarna ovan från projekt- och uppgiftsinställningarna på systemnivå. Om du senare tilldelar en grupp till mallen eller malluppgiften påverkas den inte av gruppens inställningar.</p> </td> 
   <td> <p>Förhandsversion: 26 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Ta reda på vilka anpassade formulär som använder ett anpassat fält</a> </p> <p>Nu är det enklare att ändra ett anpassat fält i ett anpassat formulär. Med ett enda klick i det anpassade formuläret kan du ta reda på mer om andra anpassade formulär som också använder fältet. Det är viktigt att du kontrollerar om dessa formulär behöver justeras för att de ska fortsätta fungera korrekt när du har gjort ändringen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 19 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nytt för gruppadministratörer: Lås och lås upp projekt-, uppgifts- och utgivningsinställningar för en grupp</a> </p> <p>Nu kan du se till att alla i gruppen och dess undergrupper använder samma inställning för ett projekt, en uppgift eller en utgåva. När en Workfront-administratör har låst upp en inställning på systemnivå kan du konfigurera den och sedan låsa den för din grupp. Även om du fortfarande kan konfigurera om en låst gruppinställning, kan inte administratörer av lägre undergrupper göra detta separat för sina grupper.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 12 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nytt för gruppadministratörer: Skapa och redigera mallar från gruppområdet</a> </p> <p>Vi fortsätter att göra det enklare att hantera dina grupper och tillhörande objekt på ett och samma ställe. Nu kan du visa och arbeta med en grupps mallar från området Grupper i Konfigurera. På så sätt slipper du gå till mallområdet för att hantera en grupps mallar. Listan med gruppmallar som du arbetar med hålls åtskild från övriga i systemet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 12 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">Ange och spara information i ett anpassat formulär i taget</a> </p> <p>Nu är det enklare att ange information i informationsavsnittet för ett objekt: Skriv och spara information i ett enda anpassat fält eller utökningsbart område (t.ex. Översikt och Ekonomi), även om obligatoriska fält i andra anpassade formulär för objektet ännu inte har fyllts i.</p> <p>Tidigare när du angav information i ett anpassat formulär eller utökningsbart område för ett objekt, gick alla anpassade formulär som var kopplade till objektet in i redigeringsläge och alla obligatoriska fält för dem måste fyllas i innan du kunde spara ändringarna. Detta var ett problem om du inte kunde fylla i ett obligatoriskt fält eftersom det var avsett för en annan användare.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 22 juli 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">Nytt för gruppadministratörer: Skapa och hantera status för en grupp på alla nivåer</a> </p> <p>För att göra det enklare för alla nivåer i en organisation att hantera och styra sina arbetsflöden oberoende av varandra har vi introducerat möjligheten att skapa och hantera statusar för undergrupper. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 3 juni 2021 (under 21.3-versionen)<br></p> <p>Produktionsrelease: 22 juli 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Nytt för Workfront-administratörer: Migrera layoutmallar från Workfront Classic till den nya Workfront-upplevelsen på egen hand</a> </p> <p>För att hjälpa dig att hantera layoutmallar medan användarna växlar till den nya Workfront-upplevelsen har vi skapat en knapp som du kan använda för att migrera layoutmallar från Workfront Classic till den nya upplevelsen utan att behöva använda Workfront kundsupport.</p> <p>Tidigare var det bara Workfront kundsupport som kunde migrera dina layoutmallar från Workfront Classic till nya Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 1 juli 2021<br></p> <p>Produktionsrelease: 15 juli 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">När du associerar en mall med en grupp väljer du en process för gruppgodkännande i Köinformation och Köämnen </a> </p> <p>Vi har lagt till ett nytt alternativ i processen att koppla en mall till en grupp. Nu kan du välja gruppspecifika godkännandeprocesser för problem i mallens köinformation eller i något av dess köämnen.</p> <p>I 21.3, när vi lade till möjligheten att associera en gruppmall med en grupp, kan du välja en gruppspecifik godkännandeprocess i mallen, men det kan du inte göra i mallens köinformation eller köämnen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 1 juli 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">Inkludera bilder i uppdateringar</a> </p> <p>På fliken Uppdateringar för ett objekt kan du nu lägga till bilder genom att klicka på ikonen Bild i verktygsfältet. Du kan också dra och släppa en bild i uppdateringsområdet. Observera att Workfront-administratören måste aktivera bildtillägg innan du kan se bildikonen.</p> <p>Du kan lägga till bilder i både uppdateringar och svar. En miniatyrbild i uppdateringen anger att mottagarna kan förhandsgranska bilden i webbläsaren eller hämta den, och e-post- och appmeddelanden visar att bilder är kopplade till uppdateringen.</p> <p>Tidigare var det enda sättet att dela en bild i Workfront att bifoga den till ett objekt som ett dokument. Bilder som läggs till på fliken Uppdateringar är bara tillgängliga på den fliken och inte på fliken Dokument.</p> <p>Innan Workfront-användare kan inkludera bilder i uppdateringar måste den här funktionen först aktiveras av Adobe Workfront-administratören.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Uppdaterad algoritm för smarta tilldelningar</a> </p> <p>Vi har förbättrat algoritmen som används för smarta tilldelningar. Med den nya förbättringen tittar Workfront på de 30 senaste uppdragen som gjorts av den inloggade användaren för att ge förslag när de tilldelar uppgifter och ärenden. Listan med förslag kan innehålla upp till 50 användare. </p> <p>Före den här förbättringen övervägde Workfront tilldelningarna för de överordnade uppgifterna och andra användarattribut som är relaterade till tilldelningarna när de föreslog användare.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny upplevelse när du skapar ett projekt från en mall</a> </p> <p>Vi har gjort om gränssnittet för att skapa ett projekt från en mall så att du kan använda Workfront på ett sätt som är förenligt med den nya Workfront-upplevelsen. Funktionen för att skapa ett projekt med en mall har inte ändrats. Några av förbättringarna i det nya gränssnittet är dock följande:</p> 
    <ul> 
     <li> <p>Förhandsgranska mallinformation innan den bifogas</p> </li> 
     <li> <p>Lägga till mallar i en lista med favoriter när projektet skapas</p> </li> 
    </ul> <p>Vi har uppdaterat gränssnittet för att skapa projektet både när du skapar det från både projektet och mallområdet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Ny upplevelse när mallar bifogas till projekt</a> </p> <p>För att din användning av Workfront ska vara förenlig med den nya Workfront-upplevelsen har vi gjort om gränssnittet för att bifoga en mall till ett projekt. Funktionen för att bifoga en mall har inte ändrats. Det finns dock några förbättringar i det nya gränssnittet som innehåller följande:</p> 
    <ul> 
     <li> <p>Förhandsgranska mallinformation innan den bifogas</p> </li> 
     <li> <p>Lägga till mallar i en lista med favoriter under bilageprocessen</p> </li> 
     <li> <p>Visa alla alternativ för att hantera mall- och projektinställningar på en sammanhängande sida</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 26 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}">Enhetliga värden för varaktighet och varaktighet för aktiviteter</a> </p> <p>För en renare och mer strömlinjeformad användarupplevelse har värdet för fältet Varaktighet sammanfogats med tidsenheten. Före den här förbättringen visas tidsenheten i ett separat nedrullningsbart fält efter fältet Varaktighet.</p> <p>Förutom varaktighetsfälten i rutorna Uppgiftsinformation, Redigera uppgifter och Ny uppgift uppdaterar vi även följande fält så att de matchar den här funktionen:</p> 
    <ul> 
     <li> <p>Varaktighetsfält vid avancerade tilldelningar</p> </li> 
     <li> <p>Fältet Nivåfördröjning när du skapar eller redigerar en uppgift</p> </li> 
     <li> <p>Frekvensfält när en återkommande uppgift skapas (tillgängligt snart)</p> </li> 
     <li> <p>Laga fält när en föregångare läggs till (tillgängligt snart)</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 19 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">Inaktivera infogning av fel i projekt</a> </p> <p>För att säkerställa att användarna ger korrekt information när de lägger till problem i projekt genom att fylla i ett utgivningsformulär har vi infört en ny inställning som gör att du kan hantera om de kan lägga till problem i ett projekt eller dess uppgifter internt. Den här inställningen är aktiverad som standard i området för nya inställningar för problem i rutan Redigera projekt. Om du inaktiverar det nedtonas alternativet Lägg till fler problem i avsnittet Problem i ett projekt så att användarna inte kan lägga till fler problem i listan. Användarna kan fortfarande lägga till problem i projekten genom att använda alternativet Nytt problem i avsnittet Problem eller genom att använda en frågekö om en sådan har konfigurerats för projektet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 5 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">Förbättrad visning av anpassade fält för kryssrutor och alternativknappar</a> </p> <p>Det har blivit enklare att visa och markera kryssrutor och alternativknappar i anpassade formulär - ett anpassat fält med många kryssrutor och alternativknappar visas nu i flera kolumner på sidan. Tidigare visades de i en enda kolumn, vilket krävde extra bläddring för användare som fyller i formuläret.</p> <p>Detta beror på hur du placerar fälten i det anpassade formuläret. Om du placerar ett annat fält på samma rad med kryssrutan eller alternativknappsfältet kan det hända att alternativen bara har tillräckligt mycket vågrätt utrymme för att visas i en enda kolumn.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 29 juli 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">Gör snabba tilldelningar i arbetsbelastningsutjämnaren</a> </p> <p>Nu kan du effektivt balansera resurser i Utjämning av arbetsbelastning med minsta möjliga klick genom att dra ett objekt från området Ej tilldelat och släppa det på en användares rad i området Tilldelad. Med dra och släpp kan du också ta bort tilldelning av objekt från användare och flytta dem tillbaka till området Ej tilldelade samt flytta dem till andra användare. </p> <p>Före den här förbättringen kunde du bara tilldela objekt genom att klicka på Mer-menyn för en uppgift eller ett problem och sedan använda alternativet Tilldela. Nu uppdateras de planerade timmarna som tilldelats användaren i realtid medan uppgifterna dras.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt standardalternativ för belastningsutjämnare för arbetsbelastning</a> </p> <p>Som en del av vår strävan att ta bort schemaläggningen och göra Workfront viktigaste resurstilldelningsverktyg för arbetsbelastningsutjämning, har vi gjort Workfront Balancer till standardalternativet för alla nya användare. Schemaläggning är för närvarande standardalternativet. Den här ändringen gäller för alla områden där du kan komma åt Schemaläggning från vilka du kan använda området Resurser (i den nya Adobe Workfront-upplevelsen) eller i området Personer (i Adobe Workfront Classic), samt projekt- och teamnivå.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Ny filterupplevelse i arbetsbelastningsutjämnaren</a> </p> <p>Vi har gjort om filterupplevelsen i arbetsbelastningsutjämnaren så att den innehåller följande extra funktioner:</p> 
    <ul> 
     <li> <p>Enklare och effektivare användargränssnitt som matchar den nya Workfront-upplevelsen</p> </li> 
     <li> <p>Ytterligare fält som du kan filtrera efter</p> </li> 
     <li> <p>Kan duplicera ett filter</p> </li> 
     <li> <p>Dela filter med andra användare</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 16 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Flexibla förbättringar {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Användartilldelningar på Kanban- och Scrum-tavlor</a> </p> <p>Vi har uppdaterat artikelkorten på Kanban- och Scrum-tavlor för att göra det enklare att tilldela en användare till artikeln. Nu kan du klicka på ett team eller en avatar för användare för att lägga till ett uppdrag när artikelkortet är utökat. Tidigare var du tvungen att leta upp och klicka på en separat plusteckenikon.</p> </td> 
   <td> <p>Förhandsversion: 9 september 2021 <br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Konfigurera hur datum tillämpas när arbetsobjekt läggs till i en upprepning</a> </p> <p>När du lägger till en arbetsuppgift i en iteration ändras som standard det planerade startdatumet och det planerade slutförandedatumet för arbetsuppsättningen så att de matchar upprepningens startdatum och datum. Nu kan du välja att behålla det ursprungliga planerade startdatumet och det planerade slutförandedatumet för alla arbetsobjekt för ett team.</p> <p>Det här alternativet gäller endast för Scrum-team och inte för Kanban-team.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">Ändringar i Agile-vyn i projekt</a> </p> <p>Som en del av version 21.3 har vi förbättrat Agile-kortets rubrik och artikeltavlor (se <a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">Uppdateringar för Agile-kortets rubrik och artikelanslagstavla</a>). Uppdateringarna gäller både iterationer och Agile-vyn i projekt.</p> <p>I version 21.4 återställer vi dessa förbättringar för Agile-vyn i projekt. Inga ändringar görs i Agile-iterationer.</p> <p>Följande ändringar återställs när det gäller Agile-vyn i projekt:</p> 
    <ul> 
     <li> <p>Artikelkorten och kortspalterna har justerbar bredd.</p> </li> 
     <li> <p>Kolumner har ingen bakgrundsskuggning.</p> </li> 
     <li> <p>Kort saknar identifieringsetiketter (överordnad artikel, underuppgift, artikel, uppgift eller utgåva).</p> </li> 
     <li> <p>Kolumnen Överordnad artikel har bytt namn till Artiklar.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 16 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Lägg till nya artiklar och utgåvor från Kanban-tavlan</a> </p> <p>Nu kan du skapa en ny artikel eller utgåva direkt från Kanban-tavlan. Det gör det enklare att snabbt lägga till en ny artikel utan att behöva gå till ett projekt, en rapport eller en kontrollpanel för att skapa en uppgift.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 22 juli 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Rapportförbättringar {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt utseende och ny känsla för fältet Uppdrag i uppdaterade listor och rapporter</a> </p> <p>För att matcha det moderna utseendet i andra områden i den nya Workfront-upplevelsen har formatet ändrats för fältet Uppdrag i uppdaterade listor och rapporter. Omdesignen innehåller en ny ikon för jobbroll, en ny ikon för personer för avancerade uppdrag, en ny ikon för begränsad åtkomst med mera.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 april 2021 (med version 21.2)<br></p> <p>Produktionsversion: 15 juli 2021 <span class="uitext" style="color: #dc143c;"> (ursprungligen släppt till Production med version 21.2)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt utseende och ny känsla för typsnittsfält i uppdaterade listor och rapporter</a> </p> <p>För att matcha det moderna utseendet i andra områden i den nya Workfront-upplevelsen har formateringen ändrats för typsnittsfält i uppdaterade listor och rapporter. Dessa ändringar innehåller olika förbättringar.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 april 2021 (med version 21.2)<br></p> <p>Produktionsversion: 15 juli 2021 <span class="uitext" style="color: #dc143c;"> (ursprungligen släppt till Production med version 21.2)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrade begäranden {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Förbättrad sökning efter förfrågningar innehåller nu specialtecken</a> </p> <p>För att det ska gå snabbare och enklare att hitta begärandeköer när begäranden skickas har vi förbättrat sökalgoritmen så att det nu går att hitta köer som kan innehålla specialtecken.</p> <p>Du kan till exempel hitta en frågekö med namnet "*Workfront" genom att skriva "*Workfront" eller "Workfront" i fältet Typ av begäran.</p> <p>Alla specialtecken stöds.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt utseende och ny känsla för inbäddade begärandeköer i den nya Workfront-upplevelsen</a> </p> <p>För att bevara utseendet och känslan för att skicka in begäranden på samma sätt överallt i den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att lägga till begäranden i en inbäddad frågekö. Före den här förbättringen matchade gränssnittet för att lägga till begäranden från en kontrollpanel Workfront Classic-miljön.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 26 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Förbättrade korrekturfunktioner för granskare och beställare</a> </p> <p>För att skapa en mer integrerad upplevelse mellan Workfront och Korrektur har vi gjort flera förbättringar när det gäller korrekturfunktioner för granskare och beställare:</p> 
    <ul> 
     <li> <p>Du kan tilldela moderator- eller författarroller till alla användare i Workfront, oavsett om de har en korrekturlicens eller ger dem ytterligare behörigheter, som att tillämpa åtgärder eller lösa kommentarer.</p> </li> 
     <li> <p>Du kan lägga till granskare och begärande till korrektur som kräver en inloggning eller som behöver signeras elektroniskt.</p> </li> 
     <li> <p>Alla användare kan också dra nytta av den förbättrade anslutningen mellan Workfront och Korrektur. När du inaktiverar en användare eller uppdaterar en användares e-postadress visas dina uppdateringar korrekt i korrektur när de ändras i Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 5 augusti 2021 <br></p> <p>Produktionsrelease: Med version 21.4 <span class="uitext" style="color: #dc143c;"> (borttagen från förhandsgranskning och produktion den 20 oktober 2021). Ursprungligen endast för helintegrerade EMEA-kunder. Den här funktionen återinförs till alla kunder vid ett senare tillfälle.)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">Länka dokument från Dropbox Business</a> </p> <p>Vi har lagt till Dropbox Business som en tillgänglig dokumentintegrering. Nu kan du få tillgång till dokument som du har sparat i Dropbox Business direkt inifrån Workfront.</p> <p>Med Dropbox Business kan du länka delade dokument och överföra dokument till delade mappar. Dropbox (inte Dropbox Business) tillåter endast dokumentägaren att visa dokumentet i Workfront.</p> <p>Din Workfront-administratör kan aktivera integreringen för din organisation.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Uppdateringar av Workfront för Slack</a> </p> <p>Följande uppdateringar är nu synliga i Workfront för Slack-integrering:</p> <p>Integreringen av Workfront för Slack har nu ett nytt utseende och en ny känsla. Nu får du även meddelanden från Workfront för Slack i realtid. </p> <p>Om du till exempel har tilldelats en uppgift får du det meddelandet så snart du har tilldelats. </p> <p>Tidigare kunde det dröja innan meddelandet visades i Slack.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 29 juli 2021<br></p> <p>Produktionsrelease: 29 juli 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">Mer tydlig information om kontoåtkomst när du godkänner Adobe Workfront-integreringar</a> </p> <p>Medgivandeskärmarna för Adobe Workfront-integreringar har nu uppdaterats. Nu kan du se de specifika åtgärder och områden som integreringarna har tillgång till, så att du bättre kan förstå vad du tillåter integreringen eller programmet att komma åt.</p> <p>Den här nya godkännandeskärmen gäller för alla Adobe Workfront-integreringar som använder OAuth 2.0. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 29 juli 2021<br></p> <p>Produktionsrelease: 29 juli 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}">API-nyckelautentisering behövs inte längre för integreringar</a> </p> <p>Workfront integreringar har nyligen börjat använda OAuth2 för bättre säkerhet och användbarhet. Som en del av detta kräver Workfront inte längre API-nycklar för integreringsautentisering.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 5 augusti 2021<br></p> <p>Produktionsrelease: 5 augusti 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">Granska och godkänn korrektur i mobilappen</a> </p> <p>I Adobe Workfront mobilapp visas nu alla korrekturgodkännanden som du har tilldelats i din lista över godkännanden i Mitt arbete. Du kan granska ett korrekturdokument direkt i appen och fatta ett beslut om det.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: 11 oktober 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>iOS App Store</p> </li> 
     <li> <p>Android App Store</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Skapa en ny begäran från mobilappens hemsida</a> </p> <p>Nu kan du skapa en ny begäran från hemsidan i Adobe Workfront mobilapp. Om du trycker på knappen "lägg till" i det flytande navigeringsfältet visas ett alternativ för Begäran förutom Aktivitet. Tidigare var du tvungen att navigera till sidan med förfrågningar för att skapa en förfrågan.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: 4 augusti 2021</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>iOS App Store</p> </li> 
     <li> <p>Android App Store</p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya kortkommandon för indrag och utdrag i listor</a> </p> <p>För att alla användare av systemet ska få en hjälpmedelsupplevelse som är kompatibel och som uppfyller standardprinciperna för tangentbordsnavigering har tangentbordskommandona för indrag/utdrag ändrats. </p> <p>I Mac trycker du på Alt + &gt; för att dra in ett listobjekt och Alt + &lt; för att dra ut. </p> <p>I Windows trycker du på Alt + &gt; för att dra in ett listobjekt och Alt + &lt; för att dra ut.</p> <p>Tidigare var kortkommandot för indrag i en lista Tabb och utdrag var Skift + Tabb. Om du däremot använder tabbtangenten för indrag och utdrag gick det inte att tabba igenom alla aktiva fält i gränssnittet.</p> <p>Den här ändringen gäller endast för uppdaterade listor och inte för äldre listor. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 12 augusti 2021<br></p> <p>Produktionsrelease: Med version 21.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än 21.4. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

## Förbättringar av Workfront Scenario Planner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

Nya funktioner kommer till Workfront Scenario Planner i version 21.4. Mer information om de här nya funktionerna som nu är tillgängliga i förhandsgranskningen finns i [Versionsaktivitet för Adobe Workfront Scenario Planner](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
-->

## Förbättringar av Workfront-mål

Det finns inga Workfront Goals-uppdateringar just nu i den här versionen. Det här området uppdateras när det finns uppdateringar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API-version 14

För API-version 14 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 14](../../../wf-api/api/new-api-version-14.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md).

## 21.4 Release Webinar

Workfront 21.4 Release Webinar presenterades den 23 september 2021. Du kan visa webbinariet på sidan [Händelser på Workfront One](https://one.workfront.com/s/event).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns på sidan [Uppdateringar om utbildningsversioner](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

## Funktionen stöds inte längre

### Internet Explorer 11

Nu när stödet för Internet Explorer har tagits bort stöder Workfront officiellt Microsoft Edge.

Mer information om vilka webbläsare som stöds finns i [Adobe Workfront webbläsarkrav](../../../workfront-basics/workfront-browser-requirements.md).
