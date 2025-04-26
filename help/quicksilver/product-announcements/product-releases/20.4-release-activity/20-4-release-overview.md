---
content-type: release-notes
navigation-topic: product-releases
title: 20.4 versionsöversikt
description: 20.4-utgåvan gjordes tillgänglig i produktionsmiljön den 9 november 2020. Specifika releasedatum och -tider för varje kluster finns på Workfront statuswebbplats.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7cf7f6ed-fe85-4c86-bb4b-dd93197338cf
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3695'
ht-degree: 0%

---

# 20.4 versionsöversikt

20.4-utgåvan gjordes tillgänglig i produktionsmiljön den 9 november 2020.

Den här sidan innehåller information om funktionaliteten för både Adobe Workfront Classic och den nya Adobe Workfront-upplevelsen som ingår i version 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 20.4 release nears its planned Production release, this page will be updated with all functionality included with 20.4.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of November 9, 2020. For specific release dates and times for each cluster, see the <a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>. </p>
-->

## Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättringar av resurshantering](#resource-management-enhancements)
* [Förbättringar av projekthantering](#project-management-enhancements)
* [Förbättrad analys](#enhanced-analytics)
* [Språkförbättringar](#proofing-enhancements)
* [Förbättringar av mobiler och integrering](#mobile-and-integration-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Kontrollera hur ett anpassat fält delas</a> </p> <p>För att du ska få större kontroll över vem som kan redigera, ta bort och använda anpassade fält som du skapar har vi lagt till möjligheten att konfigurera exakt hur du vill att de ska delas.</p> <p>Fram tills nu, när du skapade ett anpassat fält, var det redigerbart av alla i systemet. Detta är fortfarande standardtillståndet för ett anpassat fält, men nu kan du begränsa delningen av ett anpassat fält till vissa användare, roller, team, grupper och företag. Och du kan avgöra om mottagarna kan hantera eller bara visa det anpassade fältet.</p> <p>För att göra den här upplevelsen bekant för dig har vi utformat användargränssnittet för den här funktionen så att det liknar andra objektområden som delas i Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Standardanpassad formulärdelning</a> </p> <p>Vi har standardiserat delning för anpassade Forms så att du kan använda samma Workfront-process för objektdelning som du redan känner till. Och den nya delningsfunktionen ger dig större kontroll över vem som kan redigera, ta bort och använda anpassade Forms som du skapar. Du kan begränsa delning för ett anpassat formulär till vissa användare, roller, team, grupper och företag. Du kan även avgöra om mottagarna kan visa eller hantera det anpassade formuläret.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Byt alternativ för Workfront-miljö tillgängligt</a> </p> <p>För en effektivare och smidigare upplevelse kan gruppadministratörer och Workfront-administratörer nu snabbt växla mellan olika Workfront-miljöer från vilken sida som helst i Workfront utan att behöva logga ut.</p> <p>I den nya Workfront-versionen visas alternativet Växla till klassisk på huvudmenyn.</p> <p>I Workfront Classic visas alternativet Växla till den nya upplevelsen på den meny som visas när du klickar på profilbilden i det övre högra hörnet av det globala navigeringsfältet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Administratörer för en grupp som tilldelats ett företag kan hantera företaget</a> </p> <p>Vi har gjort det enkelt för en gruppadministratör att hantera ett företag som är kopplat till sin grupp i Workfront. Åtkomst att hantera företaget är automatiskt tillgänglig när associationen görs. Detta är särskilt viktigt när gruppadministratören inte har administrativ åtkomst till företag.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Förbättringar av e-postmeddelanden</a> </p> <p>Med ett enda klick kan du nu aktivera eller inaktivera ett e-postmeddelande för en händelse i installationsprogrammet. Klicka bara på På/Av bredvid meddelandets namn.</p> <p>Observera också att vår moderna formatering nu förbättrar upplevelsen av att konfigurera händelsemeddelanden i området E-postmeddelanden.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Associera portföljer, program och företag med grupper</a> </p> <p>När Workfront-administratörer skapar eller redigerar en portfölj, ett program eller ett företag kan de tilldela den till en grupp. Med grupper tilldelade till dessa objekt är det enkelt att identifiera gruppens ansvar för dem. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 25 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Tilldela en grupp till ett team</a> </p> <p>För att göra det enklare att hantera och rapportera om de team som är kopplade till en grupp kan du nu tilldela vilken grupp som helst till ett team som du har tillgång till för redigering.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 29 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt för administratörer: Tilldela en företagsledare till en grupp</a> </p> <p>För att du bättre ska kunna organisera och definiera dina grupper har vi lagt till möjligheten att utse en användare till affärsledare för en grupp (eller undergrupp). En företagsledare är en Workfront-användare som fattar affärsbeslut för en grupp.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 21 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Vi presenterar Workfront för MobileIron</a> </p> <p>Workfront samarbetar med MobileIron, en plattform för hantering av mobila enheter (MDM), för att ge företag en säkrare och mer kontrollerad mobilupplevelse.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsrelease: 21 augusti 2020</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#plan" class="MCXref xref" xrefformat="{para}">Planera arbete med hjälp av Arbetskraft i stället för planerade timmar</a> </p> <p>För att ge dig flexibilitet när du planerar att arbeta med dina projekt har vi introducerat det nya konceptet med arbetsinsatser för uppgifter. Du kan uppskatta om arbetsinsatsen för en uppgift är liten, medelstor eller stor utan att manuellt uppskatta antalet planerade timmar för uppgiften. Varje ansträngningsnivå beräknas utifrån en procentandel av tiden från de vanliga timmarna per dag som konfigurerats i din instans.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#project" class="MCXref xref" xrefformat="{para}">Projektstatusbaserade färger för arbetsobjekt i arbetsbelastningsutjämnaren</a> </p> <p>För bättre synlighet och ökad anpassning av din upplevelse i Utjämning av arbetsbelastning kan du nu ändra färgerna för projekten och deras arbetsobjekt så att de matchar statusen för projekten. Färgerna motsvarar projektstatus på gruppnivå eller systemnivå. De färger som visas kan motsvara både system- och anpassad projektstatus.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#adjust" class="MCXref xref" xrefformat="{para}">Justera användarallokering med hjälp av procentvärden i Utjämning av arbetsbelastning</a> </p> <p>Nu kan du hantera användarnas tilldelningar i Utjämning av arbetsbelastning med procentandelar i stället för timmar.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny ikon för växling mellan timmar- och procentvärden, eller allokerad och återstående tid i Utjämning av arbetsbelastning</a> <p>Vi har lagt till en ny inställning som gör att du kan växla mellan tilldelade timmar och procentvärden när du visar Utjämning av arbetsbelastning. Med den här nya ikonen har vi även tagit bort avsnittet Användararbetsbelastning på panelen Inställningar. I Utjämning av arbetsbelastning visas tilldelad tid som standard, och vi har flyttat inställningen Återstående timmar till den nya ikonen Procentandel eller Timmar.</p></td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 25 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Ett nytt inbyggt filter för Utjämning av arbetsbelastning: Användare i projekt</a> </p> <p>Vi har lagt till ett nytt inbyggt filter på arbetsytan Tilldelad arbetsyta för att göra din filtreringsupplevelse i belastningsutjämnaren mer effektiv. Du kan nu använda filtret Användare i projekt som visar användare som har tilldelats uppgifter och ärenden i de projekt du anger.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 25 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#visualiz" class="MCXref xref" xrefformat="{para}">Visa slutfört arbete i arbetsbelastningsutjämnaren</a> </p> <p>För att du enkelt ska kunna identifiera arbete som redan har slutförts så att du kan hantera användartilldelningar på rätt sätt har vi aktiverat en visuell indikator i belastningsutjämnaren som visar när objekt för en vald tidsram har slutförts. Nu kan du se en grön bockmarkering för uppgifter, utgåvor när de är klara. I projektet visas även den gröna bockmarkeringen när arbetsobjekt har slutförts under den tidsram som visas på skärmen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 11 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt standardfilter för den tilldelade arbetsytan i Utjämning av arbetsbelastning</a> </p> <p>Standardfiltret för området Tilldelat arbete i Utjämning av arbetsbelastning visar nu endast användare som är medlemmar i alla team som du, som är inloggad användare, är kopplad till. Det nya filtret visar nu den mest relevanta informationen som standard.</p> <p>Innan den här förbättringen visades alla användare som du hade åtkomst till i det här området. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 11 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Användarallokeringsdiagram i belastningsutjämnaren</a> </p> <p>För att du ska kunna ha en visuell representation på hög nivå av användarens allokering inom en given tidsram, aktiverar nu en ny inställning en diagramvy för hur allokeringarna visas i Utjämning av arbetsbelastning. Om du aktiverar den här inställningen visas användarens tilldelning i ett linjediagram som anger överbeläggningar i röda block och underbeläggningar i blått. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 29 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#show" class="MCXref xref" xrefformat="{para}">Visa eller dölj slutfört arbete i arbetsbelastningsutjämnaren</a> </p> <p>Med en ny inställning kan du nu visa eller dölja slutförda arbetsobjekt i Utjämning av arbetsbelastning. Inställningen är aktiverad som standard och slutförda arbetsobjekt som matchar filtervillkoren och den valda tidsramen visas i arbetsbelastningsutjämnaren. </p> <p>Före den här förbättringen visas alltid slutförda arbetsobjekt i arbetsbelastningsutjämnaren.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 21 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#usabilit" class="MCXref xref" xrefformat="{para}">Användbarhetsförbättringar i belastningsutjämnaren</a> </p> <p>För att säkerställa en smidig och användarvänlig upplevelse när du hanterar dina resurser i Utjämning av arbetsbelastning finns det nu olika förbättringar av användbarheten.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 21 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Exportera anpassade formulär och översiktsinformation från detaljavsnittet för ett projekt, en uppgift eller ett problem</a> </p> <p>Nu kan du exportera den anpassade formulärinformationen till en PDF-fil. Du kan exportera anpassade formulär från projekt, uppgifter eller utgåvor när du öppnar formuläret i objektets detaljavsnitt. </p> <p>Förutom att exportera anpassade former av projekt, uppgifter och utgåvor kan du nu även inkludera området Översikt i den exporterade PDF-filen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020 (export av översiktsområdet lades till 3 november 2020)</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#quickly" class="MCXref xref" xrefformat="{para}">Lägg snabbt till en iteration</a> </p> <p>För att förenkla upplevelsen av att skapa en iteration har vi lagt till en ny knapp som gör att du kan lägga till en iteration från fliken iterationer. Här kan du skapa en iteration och sedan lägga till uppgifter och problem senare.</p> <p>Du kan fortfarande skapa en iteration på eftersläpningstaggen som tidigare.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020</p> <p>Produktionsrelease: Med version 20.4 <span style="color: #dc143c; font-weight: bold;">inte tillgänglig</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nytt metadataavsnitt är tillgängligt i projekt</a> </p> <p>För att spara tid och öka förståelsen för ett projekts övergripande hälsa finns det nu ett metrisk avsnitt i ett projekt som innehåller information om följande:</p> 
    <ul> 
     <li>Fullständigt, ofullständigt, försenat och kommande arbete</li> 
     <li>Aktivitets- och utleveransbelopp grupperade efter status eller prioritet</li> 
     <li>Arbetsinsats som tilldelats varje användare</li> 
    </ul> <p>Du kan göra markeringar i diagrammen för att visa olika aspekter av uppgifter och problem i ett projekt och klicka på vissa element för att visa aktivitetsinformation.</p> <p>Mer information finns i <a href="../../../manage-work/projects/manage-projects/project-metrics.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Översikt över projektstatistik</a>.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 23 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nytt alternativ för att avbryta åtgärden när du ignorerar ett begärandeutkast</a> <p>När du tar bort ett sparat utkast kan du nu klicka på Avbryt på bekräftelsemeddelandet som informerar dig om att utkastet kommer att tas bort. På så sätt förlorar du inte utkastet om du skulle ångra dig.</p></td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 25 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#replace" class="MCXref xref" xrefformat="{para}">Ersätt knappen Arbeta med med knappen Start</a> </p> <p>För att hjälpa till att hämta det datum och den tid då arbetet faktiskt startar på en arbetsuppgift kan användare ersätta knappen Arbeta på den med knappen Start som automatiskt uppdaterar arbetsuppgiftens status och faktiska startdatum.</p> </td> 
   <td> <p><strong>Tillgängligt på följande datum:</strong> </p> <p>Beta Preview-version: 20 augusti 2020</p> <p>Produktionsversion: 8 oktober 2020</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Med nya fält kan du rapportera data för en grupp på den översta nivån och alla dess undergrupper</a> </p> <p>För att du lättare ska kunna identifiera data som är kopplade till en grupp på den översta nivån och dess undergrupper har vi lagt till ett nytt fält för överordnat ID som du kan använda i Filter, Vyer och grupperingar när du skapar rapporter om gruppobjekt.</p> <p>Det här fältet bör vara särskilt användbart för gruppadministratörer som hanterar grupper som innehåller flera undergrupper.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 29 augusti 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#allow" class="MCXref xref" xrefformat="{para}">Tillåt flera utkast för ett köämne</a> </p> <p>För att du ska få större frihet när du arbetar med begäranden finns det inte längre någon gräns för hur många utkast du kan spara för ett köämne. När du skapar en ny begäran kan du välja ett befintligt utkast från en lista med utkast för samma köämne, skriva över det och skicka det som en ny begäran eller skapa en ny begäran från början. </p> <p>Före den här förbättringen sparade Workfront endast ett utkast för varje köämne i din begärandekö. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 21 augusti 2020</p> <p>Produktionsrelease: 17 september 2020</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrad analys  {#enhanced-analytics}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-analytics-enhancements.md#paginati" class="MCXref xref" xrefformat="{para}">Sidnumrering och sortering har lagts till i Förbättrad analys</a> </p> <p>För att du ska kunna visa den information du vill se utan att använda begränsande filter har vi lagt till alternativ för sidnumrering och sortering för varje diagram i området Förbättrad analys.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">Överför det befintliga korrekturarbetsflödet när en ny version genereras</a> </p> <p>Det befintliga korrekturarbetsflödet överförs nu till alla nya versioner du skapar, oavsett vilken metod de skapas i.</p> <p>Tidigare fanns det en liten skillnad i hur korrekturarbetsflödet överfördes beroende på var du skapade dem i Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 8 oktober 2020</p> <p>Produktionsrelease: Med version 20.4 <span class="uitext" style="color: #dc143c;"> (uppskjuten till mars 2021)</span></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#auto-gen" class="MCXref xref" xrefformat="{para}">Generera ett korrektur automatiskt när en dokumentinställning överförs inaktiverat som standard</a> </p> <p>Alternativet i användarprofilen att automatiskt generera korrektur när dokument överförs är nu inaktiverat som standard för nya korrekturanvändare. Den här ändringen påverkar inte aktuella användare. Om du har aktiverat den här inställningen kommer den att vara så stor.</p> <p>Tidigare var den här inställningen aktiverad för nya användare som standard.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 18 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#document" class="MCXref xref" xrefformat="{para}">Knappar för dokumentgodkännande är tillgängliga i korrekturläsaren</a> </p> <p>Dokumentets godkännandeknappar är nu tillgängliga i korrekturläsaren i den nya Adobe Workfront-versionen för att anpassas till korrekturvyn i Classic.</p> <p>Tidigare kunde du bara godkänna ett dokument från området Dokumentinformation.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 9 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättringar av mobiler och integrering {#mobile-and-integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#added" class="MCXref xref" xrefformat="{para}">Lagt till funktioner i Microsoft Teams-meddelanden </a> </p> <p>För att göra det enklare för dig att använda Workfront via Microsoft Teams har vi lagt till nya funktioner i Microsoft Teams-meddelanden som skickas från Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: TBD</p> <p>Produktionsrelease: Med version 20.4 <strong> (uppskjuten till december 2020 eller början av 2021)</strong></p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#get" class="MCXref xref" xrefformat="{para}">Få hjälp med kommandona för den virtuella assistenten på Workfront Mobile</a> </p> <p>I mobilappen kan du be den virtuella assistenten att hjälpa dig med kommandon genom att säga Vad kan jag göra?" en"Hjälp mig med kommandon".</p> <p>Dessa kommandon visar en lista med de olika saker du kan fråga assistenten om.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsrelease: Med version 20.4 </p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Skapa en uppgift snabbt i Workfront mobilapp</a> </p> <p>Använd det nya snabbuppgiftsalternativet i Workfront mobilapp för att snabbt skapa uppgifter. Ange bara uppgiftens namn och bifoga eventuella dokument. Du kan fortfarande fylla i ytterligare fält som beskrivningar och tilldelningar om det behövs. Klicka bara på pilen till höger om aktivitetens namn.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 18 september 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Förbättrad kryptering för Workfront Proof</a> </p> <p>Vi gör några ändringar för att förbättra styrkan på kryptering av data-i-rörelse i Workfront korrekturprogram. De svaga TLS-lärarna kommer att bli inaktuella den 11 november 2020.</p> <p>Kontrollera att du använder en webbläsare som stöds när du använder Workfront. </p> <p> </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 20 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nytt utseende och känsla för 3 e-postmallar</a> </p> <p>Följande e-postmallar har ett nytt utseende och en ny känsla för att förbättra läsbarheten och den övergripande upplevelsen</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nya e-postmeddelanden för team</a> </p> <p>Vi har lagt till två nya e-postmeddelanden för team: när en enskild föregångare till en uppgift som har tilldelats ditt team har slutförts och när alla föregående för en uppgift som har tilldelats ditt team har slutförts.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 15 oktober 2020</p> <p>Produktionsrelease: Med version 20.4</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya API-objekt som utlöser händelseprenumerationsuppdateringar</a> </p> <p>Två nya API-objekt, documentVersion och proofApproval, skapades och har konfigurerats för att utlösa uppdateringar av händelseprenumerationer när ett dokument versionsindelas eller godkänns. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Beta Preview-version: 11 september 2020</p> <p>Produktionsrelease: Med version 20.4 till produktion</p> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## Förbättringar av Workfront Scenario Planner

De flesta nya funktionerna i Workfront Scenario Planner i version 20.4. Information om de här nya funktionerna som nu finns i Förhandsgranska finns i [Workfront Scenario Planner med version 20.4 - 14 oktober 2020](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-20-4.md).

## Förbättringar av Workfront-mål

De flesta nya funktionerna som kommer till Workfront Goals-versionen i version 20.4. Mer information om de här nya funktionerna som nu finns i Förhandsgranska finns i [Workfront-mål med version 20.4](../../../product-announcements/product-releases/goals-release-activity/goals-release-20-4.md).

## Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än 20.4. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)

## API-förbättringar

API-version 12 är nu tillgänglig med version 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Mer information om nyheter och uppdateringar finns i [Nyheter i API-version 12](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/new-api-version-12).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjorts under version 20.3 finns i [Workfront Maintenance Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Meddelanden

* [Flash-borttagning](#flash-deprecation)
* [20.4 Release Webinar](#20-4-release-webinar)
* [Ändra i förhandsgranskningsversionsstatus](#change-in-preview-release-cadence)
* [Tillåtelselista av ytterligare domäner som krävs för åtkomst till Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Workfront One](#workfront-one)

### Borttagning av Flash {#flash-deprecation}

I slutet av 2020 slutförde Adobe och alla större webbläsare borttagningen av Adobe Flash-teknik, vilket innebär att dessa verktyg inte längre fungerar.

Workfront hjälper er att gå över till den nyare tekniken genom att tillhandahålla en serie nya lösningar som inte bygger på Flash. Läs mer om ersättningslösningar för varje specifikt Flash-baserat verktyg i följande artikel: [Ersättning av Flash-baserade verktyg i Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

Alla Flash-baserade verktyg tas bort från alla produkter den 19 november 2020. Vi rekommenderar att du börjar använda de nya verktygen och drar tillbaka Flash-verktygen innan dess för att öka säkerheten för instansen. Om du vill att vi ska inaktivera Flash-verktygen före 19 november kan du kontakta kundsupport.

### 20.4 Release Webinar {#20-4-release-webinar}

Workfront 20.4 Release Webinar presenteras onsdagen den 28 oktober 2020 kl. 11.00 EDT. Registrera dig för webbinariet [här](https://webinars.on24.com/workfront/204release?partnerref=CXnewsletter).

### Ändringar i förhandsgranskningsversionsstatus {#change-in-preview-release-cadence}

Från och med den 20 maj 2020 började Workfront att tillgängliggöra funktioner i förhandsvisningsmiljön varje vecka. Före den här ändringen släpptes funktionen vanligtvis till förhandsvisningsmiljön varannan vecka.

Mer information finns i [Förändringar i Workfront förhandsgranskningsversion - frågor och svar](https://experienceleague.adobe.com/en/docs/workfront/using/home)

### Tillåtelselista av ytterligare domäner som krävs för åtkomst till Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Om din organisation använder en brandvägg måste du lägga till följande ytterligare domäner i tillåtelselista för att säkerställa oavbruten åtkomst till Workfront:

* event.split.io
* sdk.split.io

Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

Med Workfront One hittar du det viktigaste innehållet, resurserna och nyheterna från Workfront - allt på ett och samma ställe, med en enda inloggning. Vi har samlat webbplatserna för upplevelser, community och utbildning, vilket gör det enklare att hitta det du söker.

[Läs mer om Workfront One](https://business.adobe.com/products/workfront.html).
