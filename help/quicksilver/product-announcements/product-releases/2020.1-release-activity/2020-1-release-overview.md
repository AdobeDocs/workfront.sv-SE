---
content-type: release-notes
navigation-topic: product-releases
title: Översikt över version 2020.1
description: 2020.1-utgåvan gjordes tillgänglig i produktionsmiljön under veckan av . Den här sidan innehåller information om de funktioner som ingår i version 2020.1.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4162cfb7-d5e1-4152-857a-fc4a6eb09cd7
source-git-commit: 255b4b83b6d1d37bb6ffff975f1b1f44130170bc
workflow-type: tm+mt
source-wordcount: '2556'
ht-degree: 0%

---

# Översikt över version 2020.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 2020.1 release was made available in the Production environment the week of . This page provides information about the functionality included in the 2020.1 release.</p>
-->

Den här sidan innehåller information om de funktioner som ingår i version 2020.1.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 2020.1 release nears its planned Production release, this page will be updated with all functionality included with 2020.1.</p>
-->

Dessa förbättringar är för närvarande tillgängliga i förhandsvisningsmiljön och kommer att vara tillgängliga i produktionsmiljön den 30 mars 2020.

<!--To download this page in PDF format, go [here](https://documentation.my.workfront.com/library/a/9f5c9e44-c9a9-4f33-beec-9e5dc2e0fdc2).-->

Vissa funktioner släpptes före version 2020.1. Om du vill se vad som släpptes före version 2020.1 ska du läsa [Andra Workfront Classic-funktioner som släpptes i Production före version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/prior-to-2020-1.md).

## Förbättringar för administratörer

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#limit" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Begränsa användarnas möjlighet att redigera filtrerings-, vy- och grupperingskontroller för listor och rapporter</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Limit users' ability to edit Filter, View, and Grouping controls on lists and reports</a>
     --> </p> <p>Nu kan du använda en åtkomstnivå för att begränsa användarnas möjlighet att redigera kontrollerna Filter, Visa och Gruppering i listor och rapporter. Detta är användbart om du har anpassade fält som du bara vill ska vara synliga för användare på en viss åtkomstnivå.</p> </td> 
   <td> <p>Beta Preview-version: 17 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förbättringar för alla användare

* [Listförbättringar](#list-enhancements)
* [Förbättringar av resurshantering](#resource-management-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Språkförbättringar](#proofing-enhancements)
* [Mobila förbättringar](#mobile-enhancements)
* [Andra förbättringar](#other-enhancements)

### Listförbättringar {#list-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#new" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Nytt sparningsläge när du gör ändringar i en uppgiftslista: tidslinjens planeringsläge</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">New saving mode when making changes in a task list: the Timeline Planning mode</a>
     --> </p> <p>Beroende på projektets storlek och komplexitet kan det ta längre tid än du önskar att uppdatera uppgiftslistan, särskilt datum och varaktighet. För att göra redigeringarna mycket snabbare har vi introducerat ett nytt sparalternativ när vi redigerar uppgifter i en lista som kallas tidslinjeplaneringsläge. Före det här läget kan du spara ändringarna i uppgiftslistorna automatiskt med Spara automatiskt eller manuellt när du inaktiverar flyttningen automatiskt.</p> </td> 
   <td> <p>Beta Preview-version: 14 mars 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#improved" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Förbättrad navigering i alla nya listor med tydlig grupperingsdifferentiering</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Improved navigation of all new lists with clear grouping differentiation</a>
     --> </p> <p>Nu kan du se skillnaden mellan flera lager med grupperingar i listor med ett nytt färgschema tydligare. Grupperingsresultaten visas också tydligare i en separat ram. Den här ändringen har tillämpats på alla nya listor.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#highligh" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Markera matchande objekt i listor när du använder snabbfilter</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Highlight matching items in lists when using the quick filters</a>
     --> </p> <p>Det går nu snabbare att hitta objekt i listor: när du söker efter ett objekt med snabbfilter markeras de matchande fälten med gult i resultaten så att du tydligt kan se vilket fältvärde som matchar nyckelordet. Fälten markeras med gult i fristående fält, liksom delade kolumner och komplexa fält. Exempel på komplexa fält är uppdrag, uppdrag och status, Procent färdigt, Föregående, Godkännare och status, Resurshanterare, Kategorier, Villkor, Uppdatera villkor osv.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#new4" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Nytt alternativ för att ange hur grupperingsresultat ska visas i listor</a> <!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">New option for indicating how to display grouping results in lists</a>
     --><span style="color: #ff0000;">Borttaget från release</span></p> <p>För att du ska få större kontroll över hur du visar listresultaten kan du nu ange om du vill att resultaten i grupperingen ska expanderas eller komprimeras som standard när listan eller rapporten visas. Det här alternativet är tillgängligt i grupperingsverktyget i en lista eller rapport.</p> </td> 
   <td> <p>Beta Preview-version: 17 januari 2020</p> <p>Produktionsrelease: Ej tillämpligt</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#display" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Visa kolumnrubriker i listor och rapporter i meningsfullt fall</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Display column headers of lists and reports in sentence case</a>
     --> </p> <p>I en tidigare version har vi gjort en ändring som visar alla kolumnrubriker med versaler när du visar en lista eller rapport. Baserat på den feedback vi har fått återställer vi nu den här ändringen. Med den här ändringen visas nu alla kolumnrubriker med inledande versal.</p> </td> 
   <td> <p>Beta Preview-version: 17 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#new2" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ny Mer-meny i uppdateringsområdet</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">New More menu in the Updates area</a>
     --> </p> <p>Använd menyn Mer på en uppdatering för att kopiera brödtexten i en uppdatering, kopiera direktlänken till en uppdatering eller ta bort uppdateringen.</p> </td> 
   <td> <p>Beta Preview-version: 8 januari 2020</p> <p>Produktionsrelease: 8 januari 2020</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#new3" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ny förloppsindikator i uppdateringsområdet</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">New progress bar in the Updates area</a>
     --> </p> <p>Förloppsindikatorn för procent färdigt i uppdateringsområdet har ett nytt utseende. Klicka och dra om du vill uppdatera procentvärdet eller dubbelklicka om du vill ange talet manuellt.</p> </td> 
   <td> <p>Beta Preview-version: 8 januari 2020</p> <p>Produktionsrelease: 8 januari 2020</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-list-enhancements.md#updated" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Uppdaterat utseende och känsla för nya listor</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-List-Enhancements-1190593809?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Updated look and feel of new lists</a>
     --><span style="color: #ff0000;">(Vissa listuppdateringar togs bort från versionen)</span> </p> <p>Listorna Projekt, Uppgifter och Timmar har nu ett uppdaterat utseende och känsla. </p> <p>När de här funktionerna ursprungligen släpptes för förhandsgranskning var de tillgängliga för alla rapporter och listor utom listorna i inställnings- och rapportområdena. De här funktionerna är nu bara tillgängliga för projekt-, uppgifts- och timlistor.</p> </td> 
   <td> <p>Beta Preview-version: 20 december 2019</p> <p>Planerad produktionsrelease: Med version 2020.1</p> </td> 
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
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-resource-management-enhancements.md#show2" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Visa daglig planerad tid för uppgifter och otillgängliga objekt i arbetsytan Ej tilldelat i arbetsbelastningsutjämnaren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Resource-Management-enhancements-1967535178?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Show daily Planned Hours for projects, tasks, and inaccessible items in the Unassigned Work area of the Workload Balancer</a>
     --> </p> <p>För att du lättare ska förstå hur enskilda projekt, uppgifter eller otillgängliga objekt påverkar arbetsbelastningen för dina användare hanterar inställningen Visa allokeringar nu vilken information som visas i området Ej tilldelat arbete i Utjämning av arbetsbelastning. </p> </td> 
   <td> <p>Beta Preview-version: 14 mars 2020</p> <p>Produktionsrelease: TBD (Den här funktionen kommer att vara tillgänglig i produktionsmiljön någon gång efter version 2020.1.)</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-resource-management-enhancements.md#show" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Visa planerade timmar per dag för projekt, uppgifter och otillgängliga objekt i arbetsytan Tilldelad arbetsyta i arbetsbelastningsutjämnaren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Resource-Management-enhancements-1967535178?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Show daily Planned Hours for projects, tasks, and inaccessible items in the Assigned Work area of the Workload Balancer</a>
     --> </p> <p>För att du ska få en förståelse för hur enskilda projekt, uppgifter eller otillgängliga objekt bidrar till arbetsbelastningen för dina användare och för att kunna fatta korrekta beslut om omfördelning i belastningsutjämnaren har vi infört en inställning som gör att du kan visa timfördelningen för enskilda projekt, uppgifter och otillgängliga objekt.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-resource-management-enhancements.md#adjust" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Justera varaktighet för tidslinjen i arbetsbelastningsutjämnaren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Resource-Management-enhancements-1967535178?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Adjust timeline duration in the Workload Balancer</a>
     --> </p> <p>Du kan nu välja hur många veckor du vill visa i Utjämning av arbetsbelastning: du kan välja mellan 2, 4 eller 6 veckor. Tidigare var antalet veckor som standard 4.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-resource-management-enhancements.md#improved" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Förbättrad navigering i arbetsbelastningsutjämnaren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Resource-Management-enhancements-1967535178?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Improved navigation in the Workload Balancer</a>
     --> </p> <p>Nu kan du navigera fram och tillbaka i belastningsutjämnaren en gång i taget. Före den här förbättringen när du klickade på ikonerna för bakåt och framåt flyttades tidsramen med fyra tidsperioder i taget.</p> </td> 
   <td> <p>Beta Preview-version: 31 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-resource-management-enhancements.md#the" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Inställningen Visa faktiska timmar har tagits bort från resursplaneraren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Resource-Management-enhancements-1967535178?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">The Display Actual Hours setting removed from the Resource Planner</a>
     --> </p> <p>För att det ska vara enklare att visa faktiska timmar i resursplaneraren har vi tagit bort inställningen Visa faktiska timmar från resursplaneraren. </p> </td> 
   <td> <p>Beta Preview-version: 17 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
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
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#more" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Se enklare vem som är taggad i en uppdatering</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">More easily see who is tagged in an update</a>
     --> </p> <p>Det är nu enklare att se vilka användare som är taggade i en uppdatering. Det taggade användarnamnet visas i blått och länkar till användarprofilen.</p> <p>Taggade användare visas också i kommentarsrutan. </p> </td> 
   <td> <p>Beta Preview-version: 14 mars 2020</p> <p>Produktionsrelease: 26 mars 2020</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ta med och identifiera citerad text i en uppdateringskommentar eller svar</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=3&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Include and identify quoted text in an update comment or reply</a>
     --> </p> <p>När du skriver en kommentar kan du markera en del av kommentaren som citerad text för att skilja den från din egen kommentar. Använd knappen Blockcitat i HTML Editor.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: 26 mars 2020</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#quote" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Citera en tidigare kommentar i en uppdateringskommentar eller svara</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Quote a previous comment in an update comment or reply</a>
     --> </p> <p>När du kommenterar i en uppdateringstråd kan du snabbt ta med text från en tidigare kommentar i kopplingen. Leta efter alternativet Offertsvar på menyn Mer bredvid kommentaren som du vill citera.</p> </td> 
   <td> <p>Beta Preview-version: 14 mars 2020</p> <p>Produktionsrelease: 26 mars 2020</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ytterligare riskinformation </a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Additional risks information</a>
     --> </p> <p>För att du bättre ska kunna förstå riskerna med dina projekt kan du nu se vilka och när en risk angavs och när den uppdaterades i ett projekt. Du kan få tillgång till den här informationen i en riskvy och via det offentliga Workfront-API:t. Dessa fält är tillgängliga med API-version 11, som släpps med 2020.1 Production.</p> </td> 
   <td> <p>Beta Preview-version: 14 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#addition2" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ytterligare fält har lagts till i baslinjer och baslinjeaktiviteter</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Additional fields added to Baselines and Baseline Tasks</a>
     --> </p> <p>För att du bättre ska kunna förstå de ekonomiska framstegen i dina projekt kan du nu inkludera ytterligare kostnads- och intäktsinformation i en baslinje- eller en baslinjeaktivitetsrapport. Den ytterligare ekonomiska informationen läggs inte till i de baslinjer som du har sparat, men den läggs till för nya baslinjer.</p> </td> 
   <td> <p>Beta Preview-version: 31 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-project-enhancements.md#issues" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Problem med statusen "Stängt och väntar på godkännande" anses vara ofullständiga</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Project-enhancements-1509887664?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Issues in "Closed-Pending Approval" status are considered incomplete</a>
     --> </p> <p>Hur Workfront hanterar problem i statusen"Slutför väntande godkännande" har ändrats. Nu uppfattas dessa problem som öppna och projektet kan inte markeras som fullständigt förrän godkännandet är löst. </p> </td> 
   <td> <p>Beta Preview-version: 6 december 2019</p> <p>Planerad produktionsrelease: Med version 2020.1</p> </td> 
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
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-proofing-enhancements.md#updates" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Uppdateringar av mätverktyget i korrekturläsaren</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Proofing-enhancements-1999580039?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Updates to the measurement tool in the proofing viewer</a>
     --> </p> <p>För att tillgodose behoven hos användare inom regelefterlevnad och reglerade branscher där strikta riktlinjer gäller finns det nu olika förbättringar i korrekturläsaren som är kopplade till mätverktyget.</p> </td> 
   <td> <p>Beta Preview-version: 6 mars 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Förbättrade inställningsetiketter i områden för automatiserat arbetsflöde</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Proofing-enhancements-1999580039?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Improved setting labels in Automated Workflow areas</a>
     --> </p> <p>Nu när du ställer in tidsgräns och aktiveringsinställningar för ett automatiserat arbetsflöde är etiketterna i användargränssnittet enklare att förstå.</p> <p>Namnet på sceninställningarna är nu konsekvent från en automatiserad arbetsflödesaktivitet till en annan.</p> </td> 
   <td> <p>Beta Preview-version: 17 januari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-proofing-enhancements.md#add" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Lägg till en tidszon i en mall för automatiserat arbetsflöde</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Proofing-enhancements-1999580039?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Add a timezone to an Automated Workflow template</a>
     --> </p> <p>När du skapar eller ändrar en mall för automatiserat arbetsflöde för dina användares korrektur kan du nu ange tidszonen för de användare som ska skapa eller arbeta med korrekturet.</p> </td> 
   <td> <p>Beta Preview-version: 6 december 2019</p> <p>Planerad produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-proofing-enhancements.md#document" class="MCXref xref" xrefformat="{para}">Dokumentikonen har tagits bort från korrekturläsaren</a> </p> <p>Dokumentikonen har tagits bort i linje med korrekturnamnet i korrekturläsaren. Den här ikonen tog dig till dokumentinformationen.</p> <p>Nu kan du klicka på namnet på korrekturet för att gå till sidan med dokumentinformation.</p> <p>Den här ikonen togs bort på grund av en förändring i den nya Workfront-upplevelsen: länk till versionsinformation för vägbeskrivningar.</p> </td> 
   <td> <p>Beta Preview-version: 30 januari 2020</p> <p>Planerad produktionsrelease: Med version 2020.1</p> </td> 
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
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-mobile-enhancements.md#seamless" class="MCXref xref" xrefformat="{para}">Smidig upplevelse mellan mobilappen och webben</a> </p> <p>För att göra upplevelsen mer enhetlig när du använder Workfront i både mobilappen och på webben återspeglas automatiskt en anpassning av den vänstra panelens sekundära navigering i de nya eller befintliga layoutmallarna i mobilappen.</p> </td> 
   <td> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-mobile-enhancements.md#like" class="MCXref xref" xrefformat="{para}">Gilla uppdateringar i mobilappen</a> </p> <p>Använd den nya Gilla-knappen på fliken Uppdateringar för att gilla en uppdatering</p> </td> 
   <td> <p>Beta Preview-version: Ej tillämpligt</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
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
   <td> <p><strong>Releasedatum</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-other-enhancements.md#change" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Ändra krävs för att lägga till korrektur i tillåtelselista</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Other-enhancements-1407923545?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Change required for whitelisting proofs</a>
     --> </p> <p>Korrekturdomänen ändras from proofhq.com till workfront.com. </p> </td> 
   <td> <p>Beta Preview-version: 10 mars 2020</p> <p>Produktionsrelease: Med version 2020.1 <span style="color: #ff0000;">(borttagen från version)</span></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-other-enhancements.md#the" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Flash Portfolio Optimizer har tagits bort</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Other-enhancements-1407923545?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">The Flash Portfolio Optimizer has been removed</a>
     --> </p> <p>Vi har tagit bort möjligheten att växla mellan det nya och det gamla (baserat på FlashFlash-baserade) Portfolio Optimizer från Workfront Classic-miljön för alla kunder. Äldre Portfolio Optimizer är en föråldrad funktion och de nya verktygen har samma funktionalitet idag.</p> </td> 
   <td> <p>Beta Preview-version: 27 februari 2020</p> <p>Produktionsrelease: Med version 2020.1</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-other-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Workfront cookie-beteende har uppdaterats för att bibehålla kompatibilitet med Chrome</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Other-enhancements-1407923545?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Workfront cookie behavior updated to maintain compatibility with Chrome</a>
     --> </p> <p>För att bibehålla kompatibiliteten med en kommande Google Chrome-uppdatering (Chrome v80) har vi uppdaterat Workfront-plattformen så att cookies skickas på rätt sätt med begäranden. </p> <p>Den här Chrome-uppdateringen ändrar standardvärdet för cookie-attributet SameSite. Om du vill testa hur din Workfront-instans fungerar efter Google Chrome-uppdateringen justerar du flaggorna i Chrome och aktiverar följande alternativ: </p> 
    <ul> 
     <li>"SameSite som standard cookies" </li> 
     <li>"Cookies utan SameSite måste vara säkra"</li> 
    </ul> </td> 
   <td> <p>Beta Preview-version: 29 januari 2020</p> <p>Produktionsrelease: 30 januari 2020</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../product-announcements/product-releases/2020.1-release-activity/2020-1-other-enhancements.md#workfron2" class="MCXref xref" xrefformat="{para}" data-mc-conditions="OnlineOrPDF.OnlineOnly">Workfront-kommentarer synkroniseras till Jira</a><!--
      <a href="https://experience.workfront.com/s/article/2020-1-Other-enhancements-1407923545?language=en_US&amp;r=13&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">Workfront comments sync to Jira</a>
     --> </p> <p>Integreringen av Workfront för Jira synkroniserar nu dina Workfront-kommentarer till Jiras inbyggda kommentarström.</p> <p>Mer information finns i <a href="../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md" class="MCXref xref" xrefformat="{para}">Konfigurera Adobe Workfront för Jira</a>.</p> </td> 
   <td> <p>Beta Preview-version: 20 december 2019</p> <p>Produktionsrelease: 20 december 2019</p> </td> 
  </tr> 
 </tbody> 
</table>

## API-förbättringar

API version 11 släppt med version 2020.1. Information om nyheter och uppdateringar finns i [Nyheter i API-version 11](../../../wf-api/api/new-api-version-11.md) [Nyheter i API-version 11](https://experience.workfront.com/s/article/What-s-new-in-API-version-11-1760875145).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md) [API-versionens utgåva och supportschema](https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1).

## Funktionen stöds inte längre

### Äldre arbetsdagskalender stöds inte längre efter version 2020.1

Den gamla arbetskalendern stöds inte längre i version 2020.1 och kommer att tas bort i version 2020.2. Mer information om den äldre kalendern finns i [Använda den äldre arbetskalendern för team](https://experience.workfront.com/s/article/Using-the-Legacy-Working-On-Calendar-for-Teams-1516477096?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1).

Efter version 2020.2 kommer team som använder den äldre funktionen Arbeta med kalender automatiskt att växla till resursplaneringsverktygen på fliken Schemaläggning i Teams-området.

Resursplaneringsverktygen har samma funktioner som den gamla funktionen Arbeta med kalender, men innehåller ytterligare funktioner och förbättringar. Mer information finns i &quot;Resursschemaläggning&quot;.

>[!NOTE]
>
>Resursplaneringen har tagits bort och ersatts från Workfront.


## Underhållsuppdateringar för Workfront

Mer information om underhållsuppdateringar som gjordes i version 2020.1 finns i [Workfront Maintenance Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Meddelanden

* [Lägger till ytterligare domäner till tillåtelselista som krävs för åtkomst till Workfront](#adding-additional-domains-to-the-allowlist-required-for-accessing-workfront)
* [Workfront One](#workfront-one)
* [2020.1 versionswebbseminarium](#2020-1-release-webinar)
* [Q1 Product Roadmap Webinar](#q1-product-roadmap-webinar)
* [Olika alternativ för enkel inloggning som ska tas bort](#various-single-sign-on-options-to-be-removed)
* [Stöd för TLS 1.0 och 1.1 upphör](#tls-1-0-and-1-1-support-is-ending)
* [Borttagning av Flash-program](#flash-application-removal)

### Lägga till ytterligare domäner till tillåtelselista som krävs för åtkomst till Workfront {#adding-additional-domains-to-the-allowlist-required-for-accessing-workfront}

Om din organisation använder en brandvägg måste du lägga till följande ytterligare domäner i tillåtelselista för att säkerställa oavbruten åtkomst till Workfront:

* event.split.io
* sdk.split.io

Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

Med Workfront One hittar du det viktigaste innehållet, resurserna och nyheterna från Workfront - allt på ett och samma ställe, med en enda inloggning. Vi har samlat webbplatserna för upplevelser, community och utbildning, vilket gör det enklare att hitta det du söker.

[Läs mer om Workfront One](https://business.adobe.com/products/workfront.html).

### 2020.1 Release Webinar {#2020-1-release-webinar}

Se inspelningen av webbinariet 2020.1 här.

### Q1 Product Roadmap Webinar {#q1-product-roadmap-webinar}

Läs mer om vad som kommer att hända under [Q1 Roadmap-webbinariet](https://webinars.on24.com/workfront/product_roadmap032620?partnerref=announcementcenter). Det här webbinariet kommer att hållas den 26 mars 2020 kl. 9:00a. MT. Klicka på länken för att registrera

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
and watch the recording on demand
</MadCap:conditionalText>
-->

.

### Olika alternativ för enkel inloggning som ska tas bort {#various-single-sign-on-options-to-be-removed}

Följande SSO-alternativ (Single Sign-On) stöds nu endast i begränsad kapacitet. De kommer att tas bort från produkten under andra halvåret 2019:

* LDAP

  Mer information om LDAP med Workfront finns i [Konfigurera Adobe Workfront med LDAP](../../../administration-and-setup/manage-workfront/security/removal-various-sso-options.md)

  <!--
  <MadCap:conditionalText data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">
  Configuring Workfront with LDAP
  </MadCap:conditionalText>

  ](https://experience.workfront.com/s/article/Configuring-Workfront-with-LDAP-1449733049).
  -->

* Active Directory

  Mer information om hur du använder Active Directory med Workfront finns i [Konfigurera Adobe Workfront med Active Directory](../../../administration-and-setup/manage-workfront/security/removal-various-sso-options.md)

  <!--
  <MadCap:conditionalText data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">
  Configuring Workfront with Active Directory
  </MadCap:conditionalText>

  ](https://experience.workfront.com/s/article/Configuring-Workfront-with-Active-Directory-899157379).
  -->

* SAML 1.1

  Mer information om hur du använder SAML 1.1 med Workfront finns i [Konfigurera Adobe Workfront med SAML 1.1](../../../administration-and-setup/manage-workfront/security/removal-various-sso-options.md)

  <!--
  <MadCap:conditionalText data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">
  Configuring Workfront with SAML 1.1
  </MadCap:conditionalText>

  ](https://experience.workfront.com/s/article/Configuring-Workfront-with-SAML-1-1-1062120191).
  -->

Nedan visas borttagningstidslinjen för dessa SSO-alternativ:

* Begränsat stöd: augusti 2018-januari 2019

  Stora problem som skickas in under den här tiden kommer att åtgärdas, och mindre allvarliga problem kommer inte att åtgärdas.

* Borttagning: januari 2019-november 2019 (med version 2019.4)

  Stöds inte.

* Finns inte längre i Workfront för nya konfigurationer: november 2019
* Nödvändig migrering för befintliga kunder: början av 2020

### Stöd för TLS 1.0 och 1.1 upphör {#tls-1-0-and-1-1-support-is-ending}

För att ge optimal säkerhet kräver Workfront att alla integreringar och all webbtrafik som använder TLS 1.1 eller tidigare ska uppgraderas till TLS 1.2. I förhandsvisningsmiljön är TLS 1.0 redan inaktiverat.

Mer information finns i [TLS 1.2 krävs i Adobe Workfront](../../../product-announcements/announcements/announcement-archive/tls-1-disabled.md).

### Borttagning av Flash-program {#flash-application-removal}

Alla funktioner som bygger på Flash-teknik har tagits bort från Workfront sedan version 2018.3 och ersatts med en ny lösning.

Mer information om de äldre Flash-verktygen och deras ersättningar finns i [Ersättning av Flash-baserade verktyg i Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

<!--
<a href="https://experience.workfront.com/s/article/Replacement-of-Flash-Based-Tools-in-Workfront-194935493" target="_blank" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<MadCap:conditionalText data-mc-conditions="OnlineOrPDF.PrintOnly">
Replacement of Flash-based tools in Workfront
</MadCap:conditionalText></a>
-->
