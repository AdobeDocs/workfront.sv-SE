---
title: 22.2 Versionsöversikt
description: 22.2 Versionsöversikt
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3974'
ht-degree: 0%

---

# 22.2 Versionsöversikt

Den här sidan innehåller information om de funktioner som finns i version 22.2. Alla funktioner i listan är tillgängliga i den nya Adobe Workfront-upplevelsen. Vissa funktioner är också tillgängliga i Adobe Workfront Classic, men [Workfront Classic kommer att upphöra i mars 2022](https://experienceleague.adobe.com/sv/docs/workfront/using/home), som kommer att följas inom kort efter det datum då Workfront Classic slutar gälla i juli 2022.

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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 4 april 2022.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättringar av resurshantering](#resource-management-enhancements)
* [Hem-förbättringar](#home-enhancements)
* [Mobila förbättringar](#mobile-enhancements)
* [Integrationsförbättringar](#integrations-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Konfigurera ett anpassat formulär som ska fungera med flera objekttyper</a> </p> <p>Nu kan du konfigurera ett nytt eller befintligt anpassat formulär så att det fungerar med flera objekttyper, vilket gör formuläret mycket mer användbart. Användarna kan bifoga och fylla i formuläret på objekt av alla typer som du konfigurerar det för.</p> <p>Tidigare kunde du konfigurera ett anpassat formulär så att det bara fungerar med en objekttyp.</p> <p>Den här funktionen fungerar med alla anpassade formulär som skapats tidigare i Workfront. Om du till exempel redan har ett anpassat formulär som har skapats för objekttypen Task kan du nu konfigurera det så att det även fungerar med andra objekttyper, till exempel Projekt och Problem.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Katalogen med utkast är tillgänglig för alla användare, och administratörer kan tillåta begäranden</a> </p> <p>Alla Adobe Workfront-användare kan nu bläddra i katalogen med tillgängliga ritningar. </p> <p>Dessutom kan systemadministratören ge användare åtkomst att begära installation av ritningar. Om du tilldelar en begärandekö för att lagra begäranden kan användarna göra förfrågningar från katalogen med utkast. </p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Lägg till en bild i ett anpassat formulär</a> </p> <p>I ett anpassat formulär som du skapar eller redigerar kan du nu lägga till en bild och inkludera ett informativt eller instruktivt verktygstips som användare kan läsa när de för muspekaren över den.</p> <p>Det kan vara praktiskt att t.ex. visa varumärken för en ny produkt eller för att ge visuell information som människor behöver när de fyller i formuläret.</p> <p>Tidigare var anpassade formulär helt textbaserade.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Inaktivera en grupp</a> </p> <p>När de interna organisationerna förändras kan du behöva sluta använda vissa grupper i Workfront och skapa nya. För att underlätta detta har vi lagt till möjligheten att inaktivera en grupp utan att förlora sina historiska data. För vanliga användare som inte behöver se dem rensas inaktiva grupper från grupptypsnittsfält.</p> <p>Du kan fortfarande hitta och konfigurera alternativ, inställningar och objektassociationer för inaktiva grupper som du hanterar. Om du inaktiverar en grupp ändras inte något om objekten som gruppen är kopplad till.</p> <p>Tidigare var det inte möjligt att inaktivera en grupp.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nya standardkonfigurationer för åtkomstnivå</a> </p> <p>För att bättre passa behoven hos de flesta administratörer som skapar åtkomstnivåer har vi ändrat standardkonfigurationen för flera av alternativen"Finjustera dina inställningar" som visas när du klickar på kugghjulsikonen på en redigeringsknapp.</p> <p>Alternativen som tidigare aktiverats som standard är nu inaktiverade. Om detta inte passar organisationens behov kan du aktivera dem när du skapar en ny åtkomstnivå eller när som helst senare.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 27 januari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/sv/docs/workfront/using/home" target="_blank">Workfront Classic kommer att upphöra i mars 2022</a>, följt av livscykeldatumet för Workfront Classic i juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Förbättringar i installationshistoriken för utkast</a> </p> <p>När du installerar en plan visar ett meddelande nu de specifika objekt (t.ex. roller, team eller grupper) som har installerats med planen och eventuella objekt som inte gick att installera. Du kan även visa listan över installerade objekt på sidan Information om utkast genom att klicka på Visa detaljer bredvid en specifik installation i tabellen över installationshistorik.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">En varning visas nu när du installerar en plan som bara är för förhandsgranskning i Production</a> </p> <p>Vissa utkast är bara tillgängliga för installation i förhandsvisningsmiljön i testsyfte.</p> <p>Om du har tillgång till innehåll som bara är för förhandsgranskning i din produktionsmiljö, i sandlåda 1 eller i sandlåda 2, är installationsknappen inte aktiv, och du kan se ett varningsmeddelande.</p> </td> 
   <td><b>Tillgängligt på följande datum:</b> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront Boards finns nu att köpa! </a> </p> <p>Styrelserna är flexibla verktyg som ger teamsamarbete genom att ge åtkomst till en delad anslagstavla som innehåller kolumner och kort. </p> <p>Med anslagstavlor kan du snabbt ställa in en anslagstavla med flera kolumner, konfigurera kolumner så att en status eller kategori visas, lägga till andra användare på anslagstavlan och tilldela dem till kort, med mera.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">Ytterligare förbättringar i Workfront Boards</a></p> <p>Följande ytterligare förbättringar är nu tillgängliga för Workfront Boards:</p> 
    <ul> 
     <li> <p>Tagga kort på anslagstavlor</p> </li> 
     <li> <p>Flytta kort</p> </li> 
     <li> <p>Kopiera kort</p> </li> 
     <li> <p>Sök på anslagstavlor</p> </li> 
     <li> <p>Ange ett förfallodatum för ett kort i en bok</p> </li> 
    </ul> </td> 
   <td><b>Tillgängligt på följande datum:</b> 
    <ul> 
     <li> <p>Förhandsversion: 24 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">Ångra-alternativ för uppdateringsposter</a> </p> <p>Det är nu enklare att fånga upp misstag när en uppdatering publiceras. När du slutför en kommentar på objektets uppdateringsflik skapas nu ett popup-fönster i 7 sekunder som gör att du kan avbryta inlägget och återgå till redigering - innan systemet tidsstämplar det eller skickar e-postmeddelanden och meddelanden i programmet. Om du stänger popup-fönstret, lämnar sidan eller väntar i 7 sekunder på att fönstret ska timeout, kommer inlägget att göras normalt.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny upplevelse vid kopiering av ett projekt</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet för att kopiera projekt. Detta är för närvarande tillgängligt när du kopierar ett projekt från projektsidan eller när du kopierar ett projekt från en lista eller rapport. Före den här uppdateringen kunde du bara kopiera ett projekt från projektsidan.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">Möjlighet att hantera projekt från listor och rapporter på en ny Mer-meny</a> </p> <p>Vi har lagt till en ny Mer-meny i projektlistor och rapporter så att du kan utföra följande åtgärder från dessa områden:</p> 
    <ul> 
     <li> <p>För flera projekt i taget:</p> </li> 
     <li> <p>Beräkna om tidslinje</p> </li> 
     <li> <p>Beräkna om ekonomi</p> </li> 
     <li> <p>Beräkna om anpassade uttryck</p> </li> 
     <li> <p>För ett enskilt projekt:</p> </li> 
     <li> <p>Bifoga mall</p> </li> 
     <li> <p>Exportera till MS-projekt</p> </li> 
     <li> <p>Prenumerera</p> </li> 
    </ul> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Ny upplevelse vid konvertering av ett problem till ett projekt med hjälp av en mall på emissionsnivå</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att konvertera ett problem till ett projekt när du använder en mall när du konverterar det från problemsidan.</p> <p>Nu är det enklare att komma åt din lista med favoriter direkt efter att du har valt att konvertera utgåvan.</p> <p>Det omdesignade gränssnittet matchar upplevelsen när du skapar ett projekt från en mall som vi också har uppdaterat nyligen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 8 december 2021<br></p> </li> 
     <li> <p>Produktionsversion: Med version 22.1 <span style="color: #ff0000; font-weight: bold;">Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Detta är nu tillgängligt i Förhandsgranska och produktion för alla kunder.</span></p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Konvertera problem till projekt med en mall från listor, rapporter och kontrollpaneler</a> </p> <p>För att effektivisera arbetet och göra det enklare för dig att konvertera utgåvor i en snabbpaketerad miljö har vi lagt till möjligheten att konvertera ett problem till ett projekt med hjälp av en mall från en lista, rapport eller en kontrollpanel.</p> <p>Före den här förbättringen fanns den här funktionen bara när du konverterade problemet från sidan med utgåvor.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 8 december 2021<br></p> </li> 
     <li> <p>Produktionsversion: Med version 22.1 <span style="color: #ff0000; font-weight: bold;">Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Detta är nu tillgängligt i Förhandsgranska och produktion för alla kunder.</span></p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Uppdaterad upplevelse vid kopiering och flytt av problem</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet för att kopiera och flytta problem. Detta är för närvarande tillgängligt när du kopierar eller flyttar ett enstaka problem eller när du kopierar eller flyttar flera utgåvor samtidigt från en lista eller rapport.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 18 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">Behåll användare på kontrollpanelen, listan eller rapporten efter konvertering av problem till projekt</a> </p> <p>För att öka effektiviteten och eliminera antalet klick har vi släppt en förbättring när vi konverterar problem till projekt från en lista, rapport eller kontrollpanel.</p> <p>Användarna finns kvar på listan, rapporten eller kontrollpanelen efter att ha konverterat ett problem till ett projekt i stället för att omdirigeras till projektets sida. Ett meddelande om att projektet lyckades med länken till projektet visas när konverteringen är klar, så att du enkelt kan navigera till projektet, om det behövs. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: 24 februari 2022</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Allokeringstider tas inte längre bort när du ändrar tilldelningar</a> </p> <p>För att dina data ska bli korrekta har vi gjort en ändring som bevarar tilldelningstimmar och behåller planerad tid för aktiviteten oförändrad när du ändrar tilldelningar för aktiviteten.</p> <p>Följande ändringar har gjorts för aktiviteter med en enkel varaktighetstyp:</p> 
    <ul> 
     <li> <p>Enskilda tilldelningar bevaras när användare och roller ersätts.</p> </li> 
     <li> <p>Enskilda tilldelningar bevaras för rollen när användaren tas bort.</p> </li> 
     <li> <p>Planerade timmar bevaras när alla tilldelningar tas bort. <span style="color: #ff0000;">(Borttagen från version. Planerade timmar anges till 0 när alla tilldelningar har tagits bort.)</span></p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022<br></p> </li> 
     <li> <p>Produktionsversion: Med version 2.2 <span style="color: #ff0000; font-weight: bold;">Den här funktionen släpps till produktion strax efter version 22.2</span></p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/sv/docs/workfront/using/home" target="_blank">Workfront Classic kommer att upphöra i mars 2022</a>, följt av livscykeldatumet för Workfront Classic i juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Dela mappar endast på de fem översta nivåerna i en mapphierarki</a> </p> <p>För att säkerställa bästa prestanda för användare som delar mappar begränsar vi för närvarande delningen till de fem högsta nivåerna i en mapphierarki på ett objekt.</p> <p>Varje mapp på sjätte nivån eller tidigare ärver sina delningskonfigurationer från mappen direkt ovanför den.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022<br></p> </li> 
     <li> <p>Produktionsversion: Med version 2.2 <span style="color: #ff0000; font-weight: bold;">Den här funktionen är inte tillgänglig för tillfället. Den här sidan uppdateras när funktionen är tillgänglig i produktion.</span></p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/sv/docs/workfront/using/home" target="_blank">Workfront Classic kommer att upphöra i mars 2022</a>, följt av livscykeldatumet för Workfront Classic i juli 2022.)</p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Förbättringar av navigeringen för belastningsutjämnare för arbetsbelastning</a> </p> <p>För att förbättra din upplevelse när du använder belastningsutjämnaren har vi infört följande förbättringar:</p> 
    <ul> 
     <li> <p>Knapparna Avbryt och Spara när du justerar tilldelningar är nu fortfarande kvar, även när uppgiften är längre än den tidsram som finns på skärmen eller när panelen Sammanfattning visas.</p> </li> 
     <li> <p>Den vänstra panelen som visar namnen på användare och arbetsobjekt är nu fast så att du kan rulla vågrätt under längre tidsramar och fortfarande kunna läsa namnen på objekten som visas på panelen.</p> </li> 
     <li> <p>Du kan komprimera och expandera alla objekt i den vänstra panelen med ett klick i stället för på användar- eller projektnivå.</p> </li> 
     <li> <p>Nu går det även att ändra storlek på den vänstra panelen.</p> </li> 
     <li> <p>Det finns nu ett helskärmsläge för Utjämning av arbetsbelastning.</p> </li> 
    </ul> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">Få åtkomst till avancerade tilldelningar i arbetsbelastningsutjämnaren</a> </p> <p>Om du vill göra det enklare och exaktare att tilldela arbetsobjekt kan du nu göra avancerade uppdrag när du tilldelar arbetsobjekt manuellt i Arbetsbelastningsutjämnaren. Före den här förbättringen har du åtkomst till avancerade uppdrag när du redigerar objekt, objektens rubriker eller i listor.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny formel för beräkning av användartillgänglighet när inställningen Standardschema har valts</a> </p> <p>För att kunna ge mer korrekt information i resurshanteringsverktygen har vi ändrat formeln som Workfront använder för att beräkna användartillgänglighet när Workfront-administratören väljer Standardschema i Resurshanteringsinställningar. I den nya uppdateringen använder Workfront följande formel för att beräkna användartillgänglighet:</p> <p>Tillgängliga timmar för användare = (standardtimmar för schema - undantag) * FTE - ledig tid</p> <p>Före den här uppdateringen använde Workfront följande formel för att beräkna användartillgänglighet när Standardschema valdes:</p> <p>Tillgängliga timmar för användare = (standardtimmar för schema - (schemalagda undantag + ledig tid) * Användarens FTE-värde</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/sv/docs/workfront/using/home" target="_blank">Workfront Classic kommer att upphöra i mars 2022</a>, följt av livscykeldatumet för Workfront Classic i juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hemförbättringar {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Förbättringar av filter i hemarbetslistan</a> </p> <p>För att få större kontroll över och fokus på din arbetslista har vi implementerat flera förbättringar av filtren i Hem-området. Med de nya förbättringarna kan du välja filter efter objekttyp och ytterligare begränsa resultatet efter arbetsobjektens status (t.ex. Klar att börja, Arbeta på eller Begärt). De nya Home-filtren ger nu ett korrekt antal uppgifter, ärenden, personliga arbetsobjekt och godkännanden när du tillämpar en kombination av objekttyp- och arbetsobjektsstatusfilter.</p> <p>Tidigare gav filtren i Hem inte korrekt antal arbetsobjekt i listan när du markerade ett eller flera filter och de skapade förvirring om arbetsobjektens status.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">Ritningar och kommentarer om korrekturdokument i mobilappen</a></p> <p>Med Adobe Workfront mobilapp kan du nu lägga till ritningar och kommentarer i korrekturdokument. Ett nytt verktygsfält i korrekturet innehåller ritverktyg för former. Du kan välja inställningar som färg och linjetjocklek för varje form. När du ritar en form på korrekturet kopplas din kommentar till det området i korrekturdokumentet.</p> <p>Du kan också svara på kommentarer som andra har gjort i korrekturet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> </li> 
     <li> <p>Produktionsrelease: från mitten till slutet av april 2022 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>iOS mobilapp</p> </li> 
     <li> <p>Android mobilapp</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Förbättringar av korrekturfunktionen i mobilappen</a> </p> <p>I Adobe Workfront mobilapp kan du nu:</p> 
    <ul> 
     <li> <p>Dela korrektur med interna och externa mottagare</p> </li> 
     <li> <p>Visa korrekturkommentarer</p> </li> 
     <li> <p>Ladda ned korrektur</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> </li> 
     <li> <p>Produktionsrelease: Tidig februari 2022 (dessa förbättringar kommunicerades ursprungligen med version 22.1).</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>iOS mobilapp</p> </li> 
     <li> <p>Android mobilapp</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Förbättrade integreringar {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Releasedatum och miljöer</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront med Anaplan-integrering är nu tillgänglig</a> </p> <p>Workfront kan nu integreras med ditt Anaplan-konto för att ge dig större flexibilitet och insikt i de ekonomiska aspekterna av dina Workfront-projekt. Genom att länka Workfront-objekt till Anaplan-objekt kan du uppdatera information mellan de båda kontona automatiskt, så att informationen i båda är aktuell och identisk. </p> <p>Du kan också aktivera automatiserade processer i Anaplan baserat på åtgärder i Workfront (eller vice versa).</p> <p>Du kan till exempel skapa en kampanj i Anaplan och sedan skapa ett Workfront-projekt eller -program som är länkat till kampanjen. Alla kostnader som spåras i Workfront kan sedan överföras tillbaka till Anaplan för att granska kampanjens resultat.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront för Experience Manager förbättrade anslutningsuppdateringar</a> </p> <p>Workfront för Experience Manager förbättrade anslutningsprogram innehåller nu följande uppdateringar:</p> 
    <ul> 
     <li> <p>Nu kan du skapa länkade mappar mellan Adobe Workfront och Adobe Experience Manager Assets as a Cloud Service även om det finns flera projektlänkade mappkonfigurationer.</p> </li> 
     <li> <p>Stöd för sidnumrering av händelseabonnemang har lagts till</p> </li> 
     <li> <p>Stöd för AEM 6.4.x har lagts till</p> </li> 
     <li> <p>Stöd för proxymiljöer har lagts till</p> </li> 
     <li> <p>Flera felkorrigeringar baseras på feedback från partner och kunder</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> </li> 
     <li> <p>Produktionsrelease: 28 mars 2022</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">Se information om klienthemlighet för anpassade OAuth2- eller JWT-integreringar</a> </p> <p>För att skapa transparens i användningen av era anpassade OAuth2- och JWT-integreringar har vi gjort det möjligt för er att se information om de kundhemligheter som era integreringar använder. Nu kan du se de datum då klienthemligheten skapades och senast användes. Du kan också lägga till och visa dina egna anteckningar om klienthemligheten.</p> <p>Tidigare var dessa uppgifter inte tillgängliga.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 3 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">Adobe Creative Cloud-integreringar använder nu OAuth2</a> </p> <p>För större säkerhet och för att skapa en mer enhetlig upplevelse i alla integreringar har vi uppdaterat Adobe Creative Cloud-integreringarna så att de använder OAuth2-autentisering, ett branschstandardsätt att autentisera användare. När användarna loggar in kan de nu se de specifika åtgärder och områden som integreringarna har tillgång till och tillåta åtkomst till. Därefter behöver de inte logga in så ofta.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 24 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">Se autentiseringstypen i listan över anpassade OAuth2-program</a> </p> <p>När du nu visar listan över anpassade OAuth2-program i din organisation kan du se om respektive program använder användarautentisering eller serverautentisering.</p> <p>Tidigare kunde du bara se den här informationen genom att gå till redigeringsalternativen för varje program.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 17 februari 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">Ange förfallodatum för uppdateringstoken i dina anpassade OAuth2-integreringar</a> </p> <p>För att få bättre kontroll över åtkomst och säkerhet för dina anpassade OAuth2-integreringar kan du nu anpassa uppdateringstokenernas livslängd. När en användares uppdateringstoken har upphört att gälla, måste användaren logga in på integreringen igen.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022 <br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">Använd offentliga och privata nycklar i dina anpassade OAuth2-integreringar för server-till-server-appar</a> </p> <p>Nu kan du konfigurera OAuth2-program server-till-server i dina anpassade integreringar. Genom att ställa in offentliga och privata nycklar kan du tillåta att Workfront kommunicerar med ett annat program utan att använda inloggningsuppgifter.</p> <p>Tidigare användes användarens inloggningsuppgifter för all autentisering i dina anpassade OAuth2-program.</p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> 
    <ul> 
     <li> <p>Förhandsversion: 10 februari 2022 <br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2 </p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under tidsramen för version 22.2</a> </p> <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för version 2.2. De här förbättringarna kommer att göras tillgängliga i produktionsmiljön minst två veckor efter att förhandsvisningen släppts. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsgranskningsversion: Under hela tidsramen för version 22.2<br></p> </li> 
     <li> <p>Produktionsrelease: Minst två veckor efter lanseringen till Förhandsgranska</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Förbättringar av det övre navigeringsfältet</a> </p> <p>Vi har gjort flera förbättringar av navigeringsfältet längst upp i Adobe Workfront.</p> 
    <ul> 
     <li> <p>Favoriter och Senaste har nu separata ikoner i det övre navigeringsfältet. Alla innehåller fortfarande samma innehåll (sidor som du har markerat som favoriter och sidor som du nyligen har besökt), och du kan fortsätta lägga till och ta bort favoritsidor på samma sätt.</p> </li> 
     <li> <p>Utseendet och känslan hos både punkter och huvudmenyn har uppdaterats till Adobe designstandarder, inklusive färger och teckensnitt. Det sätt som du lägger till och tar bort punkter och de områden du har tillgång till på huvudmenyn har inte ändrats.</p> </li> 
     <li> <p>Ikonerna till höger om det övre navigeringsfältet har ordnats om för att bli mer intuitiva. Ikonordningen är: hjälplänk, meddelanden, favoriter, senaste, sökning, huvudmeny.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">Omformade tidrapportlistor</a> </p> <p>Vi har gjort om tidrapportlistorna i området Tidrapporter för att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen. Du kan förvänta dig samma funktioner i tidrapportlistan, men bara med en renare och smidigare användarupplevelse.</p> <p>Några av nydesignens högdagrar är:</p> 
    <ul> 
     <li> <p>Tidrapportlistan matchar nu upplevelsen i alla andra listor i Workfront.</p> </li> 
     <li> <p>Filterupplevelsen matchar nu filtren i alla andra listor. Du får större flexibilitet att skapa egna filter med de fält och attribut som passar dig bäst, samt att dela dem med andra användare.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> 
    <ul> 
     <li> <p>Förhandsversion: 10 mars 2022<br></p> </li> 
     <li> <p>Produktionsrelease: Med version 2.2</p> </li> 
    </ul> <p><strong>Tillgängligt i dessa miljöer:</strong> </p> 
    <ul> 
     <li> <p>Nya Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än 2.2-versionen. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

## Förbättringar av Workfront Scenario Planner

Det finns för närvarande inga uppdateringar av scenarioplanen i den här versionen. Det här området uppdateras när det finns uppdateringar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof-förbättringar

Det finns inga Workfront Proof-uppdateringar just nu. Det här området uppdateras när det finns uppdateringar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
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

## Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjorts under version 2.2 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/sv/docs/workfront-known-issues/releases/current-updates).

## 22.2 Release Webinar

Workfront 22.2 Release Webinar presenteras den 24 mars 2022 kl. 8.00 MST. Du kan registrera dig för händelsen på [eventsidan på Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
-->

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

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns på sidan [Uppdateringar om utbildningsversioner](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/home).

## Funktionen stöds inte längre

### Internet Explorer 11

Nu när stödet för Internet Explorer har tagits bort stöder Workfront officiellt Microsoft Edge.

Mer information om vilka webbläsare som stöds finns i [Adobe Workfront webbläsarkrav](../../../workfront-basics/workfront-browser-requirements.md).
