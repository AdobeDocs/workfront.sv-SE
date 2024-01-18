---
title: 2.1 Versionsöversikt
description: 2.1 Versionsöversikt
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: daf977fe-957a-40ad-a37f-1c164cb4ada3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '4757'
ht-degree: 0%

---

# 2.1 Versionsöversikt

Den här sidan innehåller information om de funktioner som finns i version 22.1. Alla funktioner finns i nya Adobe Workfront. Vissa funktioner är också tillgängliga i Adobe Workfront Classic, men [Workfront Classic upphör i mars 2022](https://one.workfront.com/s/new-workfront-experience), följt av utgånget för Workfront Classic i juli 2022.

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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.1 release nears its planned Production release the week of January 17, 2022
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.1. </p>
-->

Dessa förbättringar har gjorts tillgängliga i produktionsmiljön den 17 januari 2022.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of January 17, 2022, unless otherwise specifiedthe week of May 10, 2021
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on
<a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times
</MadCap:conditionalText>
-->

.

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Förbättrad resurshantering](#resource-management-enhancements)
* [Förbättrade begäranden](#requests-enhancements)
* [Förbättringar av korrektur](#proofing-enhancements)
* [Andra förbättringar](#other-enhancements)
* [Mobilförbättringar](#mobile-enhancements)

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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#document" class="MCXref xref" xrefformat="{para}">Dokumenthämtningar som är loggade i uppdateringsområdet</a> </p> <p>För att hjälpa dina användare att spåra nedladdningar av dokument som de lagrar i Workfront loggar systemet nu in i uppdateringsområdet för ett dokument när någon laddar ned det.</p> <p>Vi rekommenderar att du testar den här funktionen i Förhandsgranska för ett nyligen överfört dokument.</p> </td> 
   <td> <p>Förhandsversion: 16 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Skapa OAuth2-appar för att integrera program med Workfront</a> </p> <p>Nu kan du integrera Workfront med andra program som Workfront inte erbjuder någon inbyggd integrering för. Genom att skapa en OAuth2-app för programmet som du vill integrera med kan du ge programmet åtkomst till Workfront, samtidigt som du vet att dina data skyddas av det säkra, branschledande OAuth2-autentiseringsprotokollet.</p> <p>Tidigare kunde du bara integrera med andra program via inbyggda integreringar, Workfront Fusion eller Workfront API.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">Förbättrat gränssnitt i företagsområdet</a> </p> <p>I området Företag i installationsprogrammet är det enklare att hantera företagsmedlemskap att använda nya bekräftelsemeddelanden och smärre ändringar av ordalydelsen. Avsnittsnamnet"Personer" i den vänstra panelen är nu"Företagsmedlemmar".</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Lägga till anpassade formulär i grupper</a> </p> <p>Anpassade formulär stöds nu för Group-objektet. Detta gör det enklare för grupper i organisationen att samla in och dela information som passar deras specifika behov och arbetsflöden. Användare kan göra samma åtgärder för en grupp som de kan för andra Workfront-objekt, till exempel skapa ett anpassat formulär, bifoga ett anpassat formulär och spara ett anpassat formulär.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#styling" class="MCXref xref" xrefformat="{para}">Formatuppdateringar i området Anpassade Forms</a> </p> <p>Området Anpassade Forms har en ny stil och känsla som gör den uppdaterad med många andra områden i den nya Workfront-upplevelsen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#many" class="MCXref xref" xrefformat="{para}">Många förbättringar för att skapa beräknade anpassade fält</a> </p> <p>Det är nu mycket enklare att skapa beräknade anpassade fält med dessa tillägg i den nya beräkningsredigeraren:</p> 
    <ul> 
     <li> <p>Du kan hovra över vilket uttryck som helst i beräkningen för att visa information om det, inklusive en beskrivning, ett exempel på hur det kan användas och en länk till mer information i en hjälpartikeln.</p> </li> 
     <li> <p>Varje uttryck som du lägger till är färgkodat, beroende på vilken typ det är. Det gör det enklare att identifiera dina uttryck och omedelbart identifiera deras typ.</p> </li> 
     <li> <p> Med radnummer kan du identifiera och referera till funktioner i en lång beräkning.</p> </li> 
     <li> <p>När du börjar skriva ett uttryck eller fältnamn visas en lista med tillgängliga objekt så att du kan välja det du vill använda. När du skriver en öppen parentes läggs den avslutande parentesen till automatiskt.</p> </li> 
     <li> <p>Du kan förhandsgranska resultatet av beräkningen med ett befintligt objekt utan att lämna beräkningsredigeraren.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: 3 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Välj uttryck och fält i det nya fönstret för beräkningsfält</a> </p> <p>Vi fortsätter att göra det enklare att skapa ett beräknat fält i en anpassad form. När du klickar på Maximera för att öppna den nya beräkningsredigeraren kan du nu hitta och välja de uttryck och fält som du behöver.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 21 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#larger" class="MCXref xref" xrefformat="{para}">Större yta för att skapa beräknade fält</a> </p> <p>Nu är det enklare att skapa komplexa beräkningsfält i ett anpassat formulär. Klicka på knappen Maximera för att öppna ett stort redigeringsfönster där du kan skapa beräkningen. När du är klar klickar du på Minimera för att fortsätta arbeta med det anpassade formuläret.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 14 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#grant" class="MCXref xref" xrefformat="{para}">Bevilja åtkomst för team med åtkomstnivåer</a> </p> <p>Ett nytt avsnitt i området Åtkomstnivåer ger dig mer detaljerade kontroller för att hantera användarnas åtkomst till team. Nu kan du avgöra vilka som kan skapa, redigera och visa team.</p> <p>Detta ändrar inte användarnas befintliga åtkomst till team.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#group" class="MCXref xref" xrefformat="{para}">Gruppmappning finns nu i utkast</a> </p> <p>Vissa utkast innehåller nu grupper som du kan anpassa innan du installerar ritningen. Du kan mappa en grupp i planen till en befintlig grupp i din Workfront-instans eller skapa en ny grupp om det behövs.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Företagsmappning med utkast och andra förbättringar</a> </p> <p>Vissa ritningar innehåller nu företag som du kan anpassa innan du installerar ritningen. Du kan mappa ett företag i planen till ett befintligt företag i din Workfront-instans eller skapa ett nytt företag om det behövs.</p> <p>Det finns även andra förbättringar av utkast.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: 11 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Visa granskningsloggsinformation om status och företag</a> </p> <p>Nu kan du enklare felsöka incidenter som rör status och företag genom att visa information om dem i området Granskningsloggar under Konfigurera.</p> <p>Exempel:</p> 
    <ul> 
     <li> <p>Du kan ta reda på vem som har bytt namn, låst eller gömt en status och när de gjorde det.</p> </li> 
     <li> <p>Du kan ta reda på vem som har tagit bort några medlemmar eller jobbroller från ett företag, och när de gjorde det.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: 3 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#manage" class="MCXref xref" xrefformat="{para}">Hantera företagsmedlemskap enklare</a> </p> <p>I området Företag gör ett uppdaterat verktygsfält det enkelt att lägga till befintliga Workfront-användare i ett företag och att ta bort företagsmedlemmar. </p> <p>Tidigare var dessa åtgärder bara tillgängliga i rutan Redigera företag.</p> <p>Det uppdaterade verktygsfältet innehåller även alla åtgärder som var tillgängliga i det föregående verktygsfältet, t.ex. redigering av medlemmarnas användarprofilinformation och inaktivering av dem i systemet.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 4 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#groups" class="MCXref xref" xrefformat="{para}">Grupper kan konfigurera sina egna inställningar för tidrapport och timma</a> </p> <p>I en stor organisation kan vissa grupper behöva konfigurera tidrapport- och timinställningar separat för att passa sina unika arbetsflöden, i stället för att ärva inställningarna som konfigurerats av en administratör på systemnivå. Nu kan Workfront-administratörer låsa upp en tidrapport och timinställning för alla grupper i systemet så att de själva kan konfigurera den.</p> <p>Den här funktionen lades också till nyligen för projektinställningar och för inställningar för uppgifter och utgåvor. </p> </td> 
   <td> <p><b>Tillgängligt på följande datum:</b> </p> <p>Förhandsversion: 9 september 2021<br></p> <p>Produktionsrelease: 8 november 2021 <span style="color: #ff0000;">(Den här funktionen var endast tillgänglig i Production för kunder i kluster 4 med version 21.4; den gjordes tillgänglig för alla andra kluster i Production den 8 november 2021.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select2" class="MCXref xref" xrefformat="{para}">Välj flera meddelanden som du vill låsa upp eller låsa upp för grupper</a> </p> <p>Det är nu snabbare och enklare att låsa upp eller låsa upp e-postmeddelanden för grupper. Nu kan du välja flera meddelanden, kontrollera dina val för att se till att de är korrekta och sedan klicka på den nya knappen Lås upp eller Lås som visas i verktygsfältet.</p> <p>Tidigare var du tvungen att låsa upp och låsa upp meddelanden igen en i taget. Workfront har för närvarande 95 meddelanden, så det här tog en stund om du var tvungen att göra det för alla eller många av dem.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 14 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">För gruppadministratörer: Det är enklare att välja en ersättningsgrupp när du tar bort en grupp</a> </p> <p>När du tar bort en grupp är det två förbättringar i rutan Ta bort grupp som gör det enklare att markera den ersättningsgrupp som du vill behålla den borttagna gruppens användare, arbetsobjekt och undergrupper:</p> 
    <ul> 
     <li> <p>Du kan börja skriva namnet på gruppen för att snabbt hitta den. </p> </li> 
     <li> <p>Du kan använda den nya informationsikonen för att kontrollera att du väljer den ersättningsgrupp du vill använda.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 14 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Dela en dokumentmapp</a> </p> <p>Nu kan du dela en dokumentmapp och dess innehåll från området Dokument. Tidigare var detta inte möjligt - du var tvungen att dela varje dokument i en mapp separat.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 16 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#limit" class="MCXref xref" xrefformat="{para}">Begränsa möjligheten att lägga till dokument i en mall som du delar</a> </p> <p>Ibland lägger man till dokument i en projektmall som tror att de läggs till i ett projekt. Nu kan du förhindra detta - när du delar en mall med Visa-åtkomst kan du inaktivera den nya avancerade inställningen Lägg till dokument. Detta gör att mottagarna inte kan lägga till dokument i mallen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 14 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Uppdaterat verktygsfält i instrumentpanelslistan och rapporter i instrumentpaneler</a> </p> <p>Verktygsfältet på fyra kontrollpanelssidor har nu ett modernt utseende som matchar andra Workfront-listor som projekt, uppgifter och problem. Det här intuitiva verktygsfältet gör det nu enklare att lägga till, redigera, dela, kopiera och ta bort kontrollpaneler.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Lägga till och redigera en anpassad formulärsammanfattningspanel för dokument</a> </p> <p>Nu kan du lägga till och redigera anpassade formulär direkt i dokumentsammanfattningspanelen.</p> <p>Med den här ändringen får du också ett nytt utseende och en ny känsla i dokumentsammanfattningen. Det finns ett nytt avsnitt, Översikt, som innehåller både miniatyrbilden och dokumentinformationen. Du kan även checka in och ut dokument i dokumentinformationsavsnittet.</p> <p>Tidigare var du tvungen att gå till fliken Egna formulär i Dokumentinformation för att göra ändringar eller lägga till anpassade formulär.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 18 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#filter" class="MCXref xref" xrefformat="{para}">Filtrera efter användarlista på flexibla anslagstavlor visar användare med de flesta tilldelningar först</a> </p> <p>Nu visar filtret de användare som har de flesta uppdrag först så att de blir lättare att hitta utan att bläddra igenom listan.</p> <p>Tidigare visades listan för filtrering efter användare på både Kanban- och Scrum-tavlor i alfabetisk ordning. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: 11 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 <b style="color: #ff0000;">(Borttagen från version 2.1. Inte längre tillgängligt i Förhandsgranska.)</b></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#change" class="MCXref xref" xrefformat="{para}">Ändra standardalternativet för föregående aktiviteter när uppgifter kopieras eller flyttas</a> </p> <p>För att minimera antalet manuella steg när du kopierar eller flyttar uppgifter har vi uppdaterat informationen som kopieras eller flyttas med uppgiften som standard. Nu kopieras eller flyttas alla föregångare med uppgiften som standard, eftersom alternativet Alla föregående användare är markerat som standard. </p> <p>Före den här förbättringen avmarkerades alternativet Alla föregående som standard när en uppgift kopierades eller flyttades.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Ny upplevelse vid kopiering av en eller flera uppgifter</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Adobe Workfront-upplevelsen har vi omdesignat gränssnittet när du kopierar en uppgift. Detta är för närvarande tillgängligt när du kopierar en uppgift på aktivitetsnivå eller kopierar en uppgift eller flera uppgifter i en lista.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 18 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Ny upplevelse när du flyttar en eller flera uppgifter från en lista</a> </p> <p>För att ge en konsekvent upplevelse när vi utför samma uppgift har vi nu uppdaterat gränssnittet för att flytta en eller flera uppgifter från en lista så att de matchar upplevelsen när aktiviteten flyttas på aktivitetsnivå. (Vi har uppdaterat upplevelsen av att flytta en uppgift på aktivitetsnivå i en tidigare förhandsversion.)</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 4 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Ny upplevelse när en uppgift flyttas på aktivitetsnivå</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att flytta en uppgift. Detta är för närvarande tillgängligt när du flyttar en uppgift på aktivitetsnivå. I nästa version kommer vi att utöka den här designen till att flytta en uppgift från en lista.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 21 oktober 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Ny upplevelse vid konvertering av ett ärende till ett projekt med hjälp av en mall på problemnivå</a> </p> <p>För att få din användning av Workfront att överensstämma med den nya Workfront-upplevelsen har vi omdesignat gränssnittet för att konvertera ett problem till ett projekt när du använder en mall när du konverterar det från problemsidan.</p> <p>Nu är det enklare att komma åt din lista med favoriter direkt efter att du har valt att konvertera utgåvan.</p> <p>Det omdesignade gränssnittet matchar upplevelsen när du skapar ett projekt från en mall som vi också har uppdaterat nyligen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 <span style="color: #ff0000; font-weight: bold;">(Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Detta finns nu i Förhandsgranska och produktion för alla kunder.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Konvertera ärenden till projekt med en mall från listor, rapporter och kontrollpaneler</a> </p> <p>För att effektivisera arbetet och göra det enklare för dig att konvertera utgåvor i en snabbpaketerad miljö har vi lagt till möjligheten att konvertera ett problem till ett projekt med hjälp av en mall från en lista, rapport eller en kontrollpanel.</p> <p>Före den här förbättringen fanns den här funktionen bara när du konverterade problemet från sidan med utgåvor.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 <span style="color: #ff0000; font-weight: bold;">(Den här funktionen togs tillfälligt bort från produktionsmiljön den 4 mars 2022. Den släpptes senare i en fasad utrullning från den 28 april 2022. Utbyggnaden slutfördes den 5 maj 2022. Detta finns nu i Förhandsgranska och produktion för alla kunder.)</span></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Förbättringar av panelen Inställningar och möjligheten att färgkoda projekt och deras uppgifter i Utjämning av arbetsbelastning</a> </p> <p>För att förbättra din upplevelse när du använder belastningsutjämnaren har vi infört följande förbättringar:</p> 
    <ul> 
     <li> <p>Panelen Inställningar har gjorts om så att den innehåller alternativ som tidigare fanns i verktygsfältet. Detta förbättrar användningen av utrymmet i verktygsfältet.</p> </li> 
     <li> <p>Lagt till möjlighet att anpassa färgtemat efter projekt. När du väljer att färgkoda efter projekt visas varje projekt och dess arbetsobjekt i samma färg. Färgerna är unika för varje projekt. Före den här förbättringen kunde du bara färgkoda efter projektstatus.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Tilldela flera arbeten med hjälp av belastningsutjämnaren</a> </p> <p>Vi fortsätter vårt arbete med att ta bort schemaläggningsverktygen och ersätta dem med arbetsbelastningsutjämnaren. Vi har lagt till möjligheten att hantera grupptilldelningar. Du kan nu tilldela flera arbetsposter samtidigt till flera användare, ersätta användare från flera arbetsposter med andra användare och ta bort användartilldelningar från flera objekt samtidigt. Du kan utföra alla dessa med en åtgärd genom att använda den nya funktionen Grupptilldelning i Utjämning av arbetsbelastning.</p> <p>Före den här förbättringen kunde du bara tilldela en användare till ett arbetsobjekt manuellt eller genom att dra och släppa.</p> <p>De nya grupptilldelningarna innehåller även nya filtreringsfunktioner per projekt och aktivitetsstatus, utöver Namn.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#override" class="MCXref xref" xrefformat="{para}">Åsidosätt valuta vid hantering av jobbroller</a> </p> <p>För att du enkelt ska kunna hantera kostnader och faktureringstaxor i globala organisationer har vi implementerat åsidosättande av valutan för en jobbroll. Med den här funktionen kan du nu ange kostnads- och faktureringssatser för jobbroller i den valuta som matchar jobbrollens plats. Detta åsidosätter systemvalutan i alla ekonomiska beräkningar för jobbrollen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">Gränssnittsförbättring för användare som inte har behörighet att skapa begäranden</a> </p> <p>För att förbättra användarnas upplevelse när de arbetar med förfrågningar har vi infört en förbättring av gränssnittet som anger för den inloggade användaren att de inte har tillgång till att skapa förfrågningar. I och med den här förbättringen är knappen Ny begäran nedtonad för användare som inte har åtkomst till att skapa problem. När du hovrar över den nedtonade knappen visas ett verktygstips som förklarar att Workfront-administratören har begränsat den aktuella användarens åtkomst för att skapa begäranden. </p> <p>Före den här förbättringen visades inte knappen Ny begäran i området Begäranden för dessa användare. Kopiering och inlämning av en begäran som ny är också begränsad.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#copy" class="MCXref xref" xrefformat="{para}">Kopiera och skicka begäranden</a> </p> <p>För att optimera processen för att skicka in begäranden introducerar vi nya funktioner som gör att du kan kopiera en befintlig begäran och skicka den som en ny begäran. Detta är praktiskt när du ofta skickar in liknande förfrågningar. I det här fallet kan du återanvända en befintlig begäran, göra några ändringar och sedan skicka den som en ny begäran.</p> <p>Med den här ändringen kan användare som kan visa förfrågningar som andra har skickat även kopiera dessa förfrågningar och skicka dem som nya. Du kan förhindra detta genom att uppdatera följande inställning i begärandeköprojektet: Personer från samma företag ärver samma behörigheter för alla begäranden.</p> <p>Du kan inte kopiera och skicka om utgåvor som har skickats till en begärandekö utan ett köämne innan den här funktionen släpptes.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 18 november 2021 <br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Uppdaterad sammanfattning i avsnittet Skickat i området Begäranden</a> </p> <p>För att förbättra synligheten och interaktionen med panelen Sammanfattning har vi lagt till en etikett till ikonen Öppna sammanfattning i avsnittet Skickat i området Begäranden. Etiketten är nu dynamisk och uppdateras beroende på om panelen är öppen eller stängd. </p> <p>När du öppnar panelen Sammanfattning utan att först markera en begäran visas nu en mer användarvänlig bild som tydligt instruerar användaren att markera ett objekt innan panelen öppnas. </p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 4 november 2021<br></p> <p>Produktionsrelease: Med version 2.1 </p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Förbättrade korrekturfunktioner för granskare och beställare</a> </p> <p>För att skapa en mer integrerad upplevelse mellan Workfront och Korrektur har vi gjort flera förbättringar när det gäller korrekturfunktioner för granskare och beställare:</p> 
    <ul> 
     <li> <p>Du kan tilldela moderator- eller författarroller till alla användare i Workfront, oavsett om de har en korrekturlicens eller ger dem ytterligare behörigheter, som att tillämpa åtgärder eller lösa kommentarer.</p> </li> 
     <li> <p>Du kan lägga till granskare och begärande till korrektur som kräver en inloggning eller som behöver signeras elektroniskt.</p> </li> 
     <li> <p>Alla användare kan också dra nytta av den förbättrade anslutningen mellan Workfront och Korrektur. När du inaktiverar en användare eller uppdaterar en användares e-postadress visas dina uppdateringar korrekt i korrektur när de ändras i Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021 <b style="color: #ff0000;">(Endast tillgängligt för EMEA-kunder med integrerad korrekturläsning, tillgängligt för alla återstående kunder den 17 januari 2022)</b><br></p> <p>Produktionsrelease: 21 december 2021 <b style="color: #ff0000;">(Endast tillgängligt för EMEA-kunder med integrerad korrekturläsning, tillgängligt för alla återstående kunder 3 februari 2022)</b><br></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#electron" class="MCXref xref" xrefformat="{para}">Förbättringar av elektroniska signaturer för korrektur</a> </p> <p>Vi har gjort det enklare för användare att signera korrektur elektroniskt. Nu kan användare använda sina Workfront-inloggningsuppgifter för att signera ett beslut om ett bevis.</p> <p>Om du vill signera ett korrektur elektroniskt med inloggningsuppgifter för enkel inloggning måste du konfigurera enkel inloggning i Workfront Proof. </p> <p>Tidigare var man tvungen att använda Workfront Proof-inloggningsuppgifterna, som skiljer sig från inloggningsuppgifterna för Workfront.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021 <b style="color: #ff0000;">(Tillgängligt för både EMEA- och USA-kunder)</b><br></p> <p>Produktionsrelease: TBD <b style="color: #ff0000;">(Tillgängligt för kunder i EMEA den 21 december 2021; tillgängligt för alla återstående kunder den 3 februari 2022)</b></p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#desktop" class="MCXref xref" xrefformat="{para}">Uppgradering av Desktop Viewer</a> </p> <p>Vi har uppgraderat Desktop Proofing Viewer med stöd för upp till Chrome version 91 för bättre kompatibilitet med interaktiva korrektur.</p> <p>Windows-användare måste installera om Desktop Viewer manuellt för att uppgradera till den senaste versionen. Därefter kommer framtida uppdateringar av Desktop Proofing Viewer att vara automatiska.</p> <p>Mac-användare uppgraderas automatiskt till den senaste versionen.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: 2 december 2021</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nytt verktygsfält för användarlistor</a> </p> <p>Ett modernare och mer intuitivt verktygsfält gör det enklare att hantera användare i en användarlista. Med verktygsfältsknapparna kan du snabbt lägga till personer i Workfront, påminna dem om att registrera sig och hantera deras profiler. Du kan också exportera en användarlista.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 8 december 2021<br></p> <p>Produktionsrelease: Med version 2.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#default" class="MCXref xref" xrefformat="{para}">Standardstigande ordning för planerat slutförandedatum och möjlighet att gruppera efter planerat startdatum i hemarbetslistan</a> </p> <p>För att göra det enklare och snabbare att hitta objekt som kräver din uppmärksamhet har vi lagt till två förbättringar som gör att du kan se dina tidigaste förfallna objekt visas överst i din arbetslista som standard och att du kan gruppera dina uppgifter och ärenden efter planerat startdatum. </p> <p>Före dessa förbättringar kan du bara gruppera dina objekt efter planerat slutförandedatum och efter implementeringsdatum.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Lägg till området Mina uppdateringar för alla licensierade användare</a> </p> <p>Som en del av vårt arbete med att skapa paritet mellan Workfront Classic och den nya Workfront-upplevelsen har vi återinfört området Mina uppdateringar för alla användare.</p> <p>Som ett resultat av den här uppdateringen kan Granska-användare hitta det här området som sin standardlandningssida, såvida de inte har tilldelats en layoutmall.</p> <p>En Workfront- eller gruppadministratör kan lägga till det här området i alla användares huvudmeny och övre navigering med hjälp av en layoutmall.</p> <p>När du öppnar området Mina uppdateringar kan du snabbt hitta följande information:</p> 
    <ul> 
     <li> <p>Godkännanden som väntar på ditt beslut visas på den första halvan av sidan Mina uppdateringar. Du kan godkänna, avvisa, föreslå ändringar, bevilja åtkomst eller delegera dina godkännanden till andra.</p> </li> 
     <li> <p>Kommentarer som du har inkluderats i visas i den nedre delen av sidan Mina uppdateringar i avsnittet Meningar.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Förbättringar av tidrapporter</a> </p> <p>För att förbättra upplevelsen för alla som hanterar tid i Workfront introducerar vi olika uppdateringar av tidrapporter.</p> <p>Några av uppdateringarna är:</p> 
    <ul> 
     <li> <p>När en användare har en aktuell tidrapport öppnas området Tidrapporter nu för den aktuella tidrapporten, vilket sparar tid för sökning och klickning på en aktuell tidrapport. När det inte finns några aktuella tidrapporter visas avsnittet Mina tidrapporter fortfarande i området Tidrapporter, precis som i dag.</p> </li> 
     <li> <p>Raden som du hovrar över eller klickar på för att ange tid markeras för att öka synligheten.</p> </li> 
     <li> <p>Sidfoten som innehåller tidrapportknapparna är nu fäst så att du alltid kan spara och avbryta utan att bläddra längst ned på sidan. Vi har också lagt till en ny knapp från början till början i det här området för att snabbt gå tillbaka till sidans övre del.</p> </li> 
     <li> <p>Ett nytt varningsmeddelande varnar dig nu om osparade ändringar för att förhindra att information går förlorad när du navigerar bort från tidrapporten.</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsversion: 2 december 2021<br></p> <p>Produktionsrelease: Med version 2.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic upphör i mars 2022</a>, följt av utgånget för Workfront Classic i juli 2022.)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Uppdaterad hjälpmeny</a> </p> <p>När du klickar på hjälplänken i det övre navigeringsfältet visas en uppdaterad, mer strömlinjeformad meny. Den nya menyn innehåller samma information, men med färre navigeringsnivåer, vilket kräver färre klick för att se relevant innehåll.</p> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: Med version 2.1</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>Nya Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Förbättrade korrekturfunktioner i mobilappar</a> </p> <p>I Adobe Workfront mobilapp kan du nu:</p> 
    <ul> 
     <li> <p>Dela korrektur med interna och externa mottagare</p> </li> 
     <li> <p>Visa korrekturkommentarer</p> </li> 
     <li> <p>Ladda ned korrektur</p> </li> 
    </ul> </td> 
   <td><strong>Tillgängligt på följande datum:</strong> <p>Förhandsgranskningsversion: Ej tillämpligt<br></p> <p>Produktionsrelease: tidig februari 2022</p> <p><strong>Finns i följande miljöer:</strong> </p> <p>iOS mobilapp</p> <p>Android-mobilapp</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production vid en senare tidpunkt än 2.1-versionen. Mer information om de senaste funktionerna finns i [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Förbättringar av Workfront Scenario Planner

Det finns för närvarande inga uppdateringar av scenarioplanen i den här versionen. Det här området uppdateras när det finns uppdateringar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Förbättringar av Workfront-korrektur

Nu finns nya funktioner i Workfront Proof. Mer information finns i [Workfront korrekturutgivningsaktivitet: 29 november 2021](../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md).

## Förbättringar av Workfront-mål

Det finns inga Workfront Goals-uppdateringar just nu i den här versionen. Det här området uppdateras när det finns uppdateringar.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API-version 14

För API-version 14 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

Information om nyheter och uppdateringar finns på [Nyheter i API-version 14](../../../wf-api/api/new-api-version-14.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](../../../wf-api/api/api-version-support-schedule.md).

## Workfront Maintenance Updates

Mer information om underhållsuppdateringar som gjordes i version 22.1 finns i [Workfront Maintenance Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 22.1 Release Webinar

Workfront 22.1 Release Webinar presenterades den 12 januari 2022. Du kan visa webbinariet på [Evenemangssida på Workfront One](https://one.workfront.com/s/event).

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

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i [Uppdateringssida för utbildningsversioner](https://one.workfront.com/s/training-release-updates).

## Funktionen stöds inte längre

### Internet Explorer 11

Nu när stödet för Internet Explorer har tagits bort har Workfront officiellt stöd för Microsoft Edge.

Mer information om vilka webbläsare som stöds finns i [Krav för Adobe Workfront webbläsare](../../../workfront-basics/workfront-browser-requirements.md).
