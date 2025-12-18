---
title: Första utgåvan, kvartal 2026, översikt
description: Den här sidan innehåller information om de funktioner som ingår i den första utgåvan av kvartalet 2026. Dessa förbättringar planeras bli tillgängliga i produktionsmiljön under hela kvartalet.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: bed931281d7d0b3184914ed7649d9cb889bcf39a
workflow-type: tm+mt
source-wordcount: '2888'
ht-degree: 0%

---

# Första utgåvan, kvartal 2026, översikt

Den här sidan innehåller information om de funktioner som ingår i den första utgåvan av kvartal 2026, som är planerad till januari 2026.

Förbättringarna på den här sidan är tillgängliga i förhandsvisningsmiljön. Den här sidan kommer att uppdateras med ytterligare förbättringar eftersom den planerade produktionsversionen för första kvartalet 2026 närmar sig den.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Månads- och kvartalsvisa releaser planeras vara tillgängliga torsdagen den andra hela veckan i månaden, om inte annat anges.
>
>| Månadsrelease | Kvartalsvis utgivning |
>|----|----|
>| <ul><li>25.11 (13 november 2025)</li><li>25.12 (11 december 2025)</li><li>26.1 (14 januari 2026)</li></ul> | <ul><li>26.1 (15 januari 2026)</li></ul> |
>
>Observera att för den slutliga utgåvan av varje kvartal (26.1 i det här kvartalet) kommer användare som har den snabba releasen att få releasen en dag i början (14 januari 2026).
>
>Mer information om processen för snabb släppning finns i [Aktivera eller inaktivera processen för snabb släppning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-förbättringar

* [Administratörsförbättringar](#administrator-enhancements)
* [Förbättringar av dokument och godkännanden](#documents-and-approvals-enhancements)
* [Integration enhancements](#integration-enhancements)
* [Projektförbättringar](#project-enhancements)
* [Rapportförbättringar](#reporting-enhancements)
* [Förbättrade begäranden](#requests-enhancements)
* [Andra förbättringar](#other-enhancements)

### Administratörsförbättringar

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Hantera prioriteringar i layoutmallen</a>
            <p>Du kan nu aktivera eller inaktivera prioriteter för specifika användare i layoutmallen. Om du tidigare har inaktiverat prioriteter för din organisation förblir den inaktiverad i layoutmallen med den här ändringen.</p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2025</td>
        <td>15 januari 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Sök efter konflikter för flera formulär för beräknade anpassade fält</a>
            <p>Vi har lagt till ett alternativ för att kontrollera om det finns konflikter, så att du kan se vilka objekt som kan påverkas när du redigerar ett uttryck i anpassade fält. I den här dialogrutan visas alla objekt som kan påverkas av att formeln ändras, grupperade efter objekttyp. Du kan navigera till informationen för varje objekt och granska fälten för att bestämma om fältet ska tas bort från något av formulären eller om uttrycket ska förbli oförändrat.</p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2025</td>
        <td>15 januari 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Anmälningsdatum och Angivet av ID lagras på anpassade objekt</a><p>[!BADGE Off schema]{type=Neutral}</p>
            <p>Anmälningsdatumet och det angivna ID:t lagras nu i anpassade formulär, fält och avsnitt. Du kan använda dessa dataalternativ i rapporter som filter, vyer eller grupperingar. Om du vill visa dem i listan med anpassade formulär, fält eller avsnitt i installationsprogrammet lägger du till anmälningsdatum och anges av: Namnge som kolumner i en ny eller befintlig vy.</p>
        </td>
        <td>13 november 2025</td>
        <td>13 november 2025</td>
        <td>13 november 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av knappnamn vid redigering av en layoutmall</a>
            <p>För att skapa större enhetlighet med andra delar av installationsprogrammet, t.ex. den anpassade formulärdesignern, har de knappar du ser när du redigerar en layoutmall ändrats till Använd, Spara och stäng samt Avbryt. Med det nya alternativet Använd kan du spara ändringarna i layoutmallen och fortsätta redigera. Tidigare var alternativen Spara och Avbryt. </p>
        </td>
        <td>30 oktober 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Förbättrad fälthantering med aktiv flagga i anpassade fält </a>
            <p>När du har ett stort antal anpassade fält i systemet kan det vara svårt att hantera dessa fält i anpassade formulär och rapporter. Du kan nu markera anpassade fält som inaktiva med den nya flaggan <b>Aktiv</b>. Den här flaggan är tillgänglig när du arbetar med ett fält i ett anpassat formulär eller när du lägger till eller redigerar ett fält från fältlistan. </p>
        </td>
        <td>30 oktober 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
    </tr>   
  </tbody>
</table>

### Förbättringar av dokument och godkännanden

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Välj ett Workfront-projekt när du skickar en granskning i Creative Cloud Express<p>[!BADGE Off schema]{type=Neutral}</p> </a>
            <p>Du kan välja ett Workfront-projekt att skicka ett korrektur till. Detta hjälper till att hålla alla relaterade resurser och korrektur välorganiserade i samma projekt.</p>
        </td>
        <td>15 december 2025</td>
        <td>15 december 2025</td>
        <td>15 december 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Organisationsövergripande stöd för Adobe Express med Workfront Proofing<p>[!BADGE Off schema]{type=Neutral}</p> </a>
            <p>Vi introducerar stöd för flera organisationer för Adobe Express med Workfront Proofing. Förbättringen gör det möjligt för kunder som arbetar i flera IMS-organisationer att smidigt använda och hantera korrekturarbetsflöden.</p>
        </td>
        <td>13 november 2025</td>
        <td>13 november 2025</td>
        <td>13 november 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager är nu tillgängligt med Frame.io-integrering <p>[!BADGE Off schema]{type=Neutral}</p> </a>
            <p>Nu kan ni använda Experience Manager Assets ​ för att hantera och lagra era digitala resurser som gått igenom gransknings- och godkännandecykeln. Tack vare integreringen kan ni utnyttja funktionerna i Adobe Experience Manager, Frame.io och Workfront för att effektivisera innehållshanteringen och samarbetet. </p>
        </td>
        <td>30 oktober 2025</td>
        <td>30 oktober 2025</td>
        <td>30 oktober 2025</td>
    </tr>   
  </tbody>
</table>



### Integration enhancements

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">Uppdatera till widgeten Mentions i Home</a>
            <p>Vi har gjort följande förbättringar av widgeten Mentions i hemmet: <ul><li>Samma upplevelse i uppdateringsområdet för de flesta Workfront-objekt finns nu även i widgeten Mentions i Home. </li><li>Widgeten Mentions innehåller nu de kommentarer som användaren har gjort eller har taggat in de senaste två veckorna</li><ul></p>
        </td>
        <td>17 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>   
  </tbody>
</table>

### Integration enhancements

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Välj ett Workfront-projekt när du skickar en granskning i Creative Cloud Express</a><p>![!BADGE Off schedule]{type=Neutral}</p>
            <p>Du kan välja ett Workfront-projekt att skicka ett korrektur till. Detta hjälper till att hålla alla relaterade resurser och korrektur välorganiserade i samma projekt. </p>
        </td>
        <td>15 december 2025</td>
        <td>15 december 2025</td>
        <td>15 december 2025</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Uppdaterad resursväljare för inbyggd integrering för Adobe Workfront för Experience Manager Assets </a>
            <p>Vi har uppgraderat resursväljaren i Adobe Workfront för Experience Manager Assets-integrering. Med den här uppgraderingen kan du nu välja och hämta AEM Collections direkt till Workfront. </p>
        </td>
        <td>20 november 2025</td>
        <td>11 december 2025</td>
        <td>15 januari 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Ny version av Salesforce-integrering är nu tillgänglig </a>
            <p>För att hålla oss uppdaterade med de senaste ändringarna av Workfront API har vi skapat en ny Salesforce-integrering. Den nya integreringen har samma funktioner som den tidigare versionen och har uppdaterats för att undvika att förlora funktioner som är inaktuella i API:t.</p><p>Obs! Integreringen av Workfront för Salesforce, inklusive den nya versionen, kommer inte att vara tillgänglig efter den 28 februari 2026**. </p>
        </td>
        <td>30 oktober 2025</td>
        <td>30 oktober 2025</td>
        <td>30 oktober 2025</td>
    </tr>   
  </tbody>
</table>

### Projektförbättringar

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Ljusanvändare kan logga tid i projekt</a>
            <p>Ljusanvändare kan nu logga tiden direkt i projekt. Tidigare var det bara användare med Standard-licenser som kunde logga timmar i projekt.</p>
        </td>
        <td>11 december 2025</td>
        <td>15 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>   
  </tbody>
</table>

### Rapportförbättringar

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
 <!--    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Currency updates in Canvas Dashboards</a>
            <p>We have made the following updates for currency fields:<ul><li>When multiple currencies are defined in Workfront, you can now choose a default currency for the dashboard during creation. </li><li>When creating a report, you can lock a currency field. This ensures that the dashboard-level currency preference does not affect the display of these values.</li><li>When viewing a dashboard, users can toggle between any defined currencies in Workfront. These changes apply to the entire dashboard with the exception of locked currency fields</li></ul></p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr>-->
 <!--    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}"> Quick search table results in Canvas Dashboards</a>
            <p>We have added a quick search to Table reports. This search works across all pages, so you can find data even if it's not currently visible.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr>-->
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nytt alternativ för Visa totalt för Cirkeldiagram</a>
            <p>Vi har introducerat ett nytt alternativ för Visa totalt som konverterar cirkeldiagram till matrisdiagram. Med den här funktionen kan användare visa ett centralt värde som representerar summan av alla segment i diagrammet.</p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nya konfigurationsalternativ för cirkeldiagram på arbetsytans kontrollpaneler</a>
            <p>Vi har introducerat två nya konfigurationsalternativ för cirkeldiagram: <ul><li>Dölj segmentetiketter: Du kan nu välja att dölja segmentetiketter i ett cirkeldiagram om de är för långa och påverkar diagrammets läsbarhet.</li><li>Dölj och flytta diagramförklaringen: Du kan nu välja att dölja cirkeldiagramförklaringen. Du kan också ange teckenförklaringens placering till höger (standard), vänster, överst eller nederst i diagrammet. </li></ul></p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Förbättrat grupperingsantal på arbetsytans kontrollpaneler</a>
            <p>Vi har uppdaterat grupperingsfältet på arbetsytans kontrollpaneler för att visa antalet poster för den aktuella sidan och det totala antalet poster för grupperingen på alla sidor. </p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Ny referensradfunktion i rapporter på arbetsytans kontrollpaneler</a>
            <p>Nu kan du definiera en referensrad i Bar-, Column- och Line-diagram för att ange ett mål eller tröskelvärde för fyra dina seriebaserade rapporter. </p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Anpassa axeletiketter i diagramrapporter på arbetsytans kontrollpaneler</a>
            <p>Nu kan du anpassa axeletiketterna i diagramrapporter. Med den här nya funktionen kan du ange en ersättningsaxeletikett som ska visas i stället för standardobjektet och fältsökvägen. Dessutom kan du välja att helt dölja axeletiketterna.</p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Duplicera en rapport på en arbetsytans kontrollpanel</a><p>![!BADGE Off schedule]{type=Neutral}</p>
            <p>Du kan nu duplicera en KPI-, tabell- eller diagramrapport på en Canvas Dashboard när den har skapats. När du har duplicerat rapporten kan du redigera den efter behov innan du sparar den.</p>
        </td>
        <td>23 oktober 2025</td>
        <td>23 oktober 2025</td>
        <td>23 oktober 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Tar bort fältalternativ från rapportfilter</a>
            <p>Vi har tagit bort följande fältalternativ som tidigare var tillgängliga när ett filter tillämpades på en rapport:
            <ul>
            <li>Andra grupp-ID</li>
            <li>Andra roller-ID</li>
            <li>Andra team-ID</li>
            </ul>
            </p>
        </td>
        <td>6 november 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Förbättrad visning av antalet grupperingar på arbetsytans kontrollpaneler</a>
            <p>När en tabellrapport har flera resultatsidor och tabellen är konfigurerad med grupperingar, visar nu tabellen både postmängden för den aktuella sidan och det totala antalet poster för alla sidor. Om tabellrapporten till exempel har 7 grupperingar och den första sidan visar 3, visas 3 av 7.</p>
        </td>
       <td>6 november 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nya skyddsytor som förbättrar inläsningstiden på arbetsytans kontrollpaneler</a>
            <p>För att undvika tidsfördröjningar vid inläsning och förbättra övergripande prestanda på arbetsytans kontrollpaneler har vi tillämpat begränsningar för hur många kontrollpanelskomponenter som kan läggas till på en kontrollpanel:
            <ul>
            <li>Rapporter per kontrollpanel: 25 gräns</li>
            <li>Grupperingar i tabellvyer: 5 gräns</li>
            <li>Avstånd från rapportens basobjekt: 10-gräns</li>
            <li>Kolumner i en tabellvy: 25 gräns</li>
            <li>Filteruppmaningar på kontrollpanelnivå: 10 gräns</li>
            </ul></p>
        </td>
       <td>6 november 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
    </tr>   
  </tbody>
</table>

### Förbättrade begäranden

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Objektlänkar som skapats är nu tillgängliga i området Begäranden och widgeten Mina förfrågningar</a>
            <p>För att göra det enklare för dig att gå till objektet som skapats av en viss begäran har vi lagt till länkar i kolumnen Skapat objekt. Nu kan du klicka på länken i den här kolumnen för att gå direkt till det skapade objektets sida./p&gt;
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr> 
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Lägg till anpassade fält i listan över förfrågningar och widgeten Mina förfrågningar</a>
            <p>För att göra det enklare för dig att se den information du behöver har vi lagt till möjligheten att lägga till anpassade fält som kolumner i listan över förfrågningar och widgeten Mina förfrågningar i Hem. Nu kan du lägga till fält från anpassade formulär som en kolumn, och förfrågningar som har information i det fältet visar den informationen i listan eller widgeten.</p><p>Den här funktionen är bara tillgänglig i den nya upplevelsen av begäranden.</p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Aktuellt jokertecken för användare är nu tillgängligt i begärandefiltret</a>
            <p>För att göra det enklare att filtrera efter förfrågningar som gäller dig har vi skapat ett jokertecken för den aktuella användaren. När du filtrerar kan du nu välja "Jag (inloggad användare)". Filtret gäller sedan den användare som visar listan med förfrågningar.   </p>
        </td>
        <td>18 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Formulärfyllning från AI är nu tillgänglig för begäranden</a>
            <p>För att förenkla skapandet av förfrågningar har vi skapat en formulärfyllning som bygger på AI. Nu kan du klistra in i en dialogruta eller överföra ett dokument till ett begärandeformulär, så tar AI ut relevant information och fyller i formuläret.  </p>
        </td>
        <td>11 december 2025</td>
        <td>11 december 2025</td>
        <td>11 december 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Dela vyer i området Förfrågningar och i widgeten Mina förfrågningar</a>
            <p>För att göra det enklare att se den information du behöver har vi lagt till möjligheten att dela vyer till den nya rapportupplevelsen. Nu kan du dela vyer med andra användare, team eller grupper. </p>
        </td>
        <td>4 december 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Spara utkast av begäranden i den nya begärande upplevelsen</a>
            <p>För att göra det enklare att skapa och skicka begäranden har vi lagt till möjligheten att spara utkast till den nya begärandeupplevelsen. När du nu börjar fylla i en begäran och stänger den, sparas den i utkaststatus och finns på det begärandeformulär som användes för att skapa utkastet. Du kan sedan öppna, uppdatera och skicka utkastet när det passar. </p>
        </td>
        <td>20 november 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Ta bort skickade begäranden i den nya begärandeupplevelsen</a>
            <p>För att göra det enklare att hålla ordning på och reda på dina förfrågningar har vi lagt till möjligheten att ta bort förfrågningar till den nya begärande upplevelsen. Nu kan du ta bort begäranden som du har skickat in. Workfront-administratörer och Workfront Planning Workspace-administratörer kan även ta bort begäranden.</p>
        </td>
        <td>20 november 2025</td>
        <td>14 januari 2026</td>
        <td>15 januari 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Skapa nya begäranden genom att kopiera tidigare skickade begäranden i den nya begärande upplevelsen</a>
            <p>För att förenkla inlämningen av begäranden har vi lagt till möjligheten att kopiera förfrågningar till den nya begärande upplevelsen. Nu kan du kopiera en förfrågan, redigera fält och skicka in den som en ny begäran. </p>
        </td>
        <td>20 november 2025</td>
        <td>11 december 2025</td>
        <td>15 januari 2026</td>
    </tr>    
  </tbody>
</table>

### Andra förbättringar

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Förhandsgranska</strong></td>
        <td><strong>Snabb release</strong></td>
        <td><strong>kvartalsvis</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Uppdateringar av utseende och känsla under tidsramen för den första utgåvan av kvartal 2026</a>
                        <p>Mindre uppdateringar av utseendet och känslan i olika delar av Adobe Workfront-programmet görs inom tidsramen för den första utgåvan av kvartal 2026. </p>
                    </td>
                    <td><p>Under tidsperioden för den första utgåvan i kvartal 2026<br /></p>
                    <td colspan="2"><p>Snabbredigering: Minst en vecka efter att du släppt till Förhandsgranska (om inget annat anges)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Markeringsgränser för flervalsfält </a>
              <p>Fält som tillåter flera val, t.ex. kryssrutor och flervalslistrutor, är nu begränsade till 5 000 val när en användare fyller i formuläret.</p>
             </td>
        <td>30 oktober 2025</td>
        <td>13 november 2025</td>
        <td>15 januari 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience finns nu för fler Workfront-organisationer</a><p></p>
            <p>För att ge företag och organisationer tillgång till fördelarna med Adobe Unified Experience fortsätter vi att göra den tillgänglig för befintliga Workfront-kunder.</p>
        </td>
        <td><p>11 december 2025</p></td>
        <td><p>15 januari 2026</p></td>
        <td><p>15 januari 2026</p></td>
    <tr>
            </tbody>
        </table>


### Funktioner som snart ska tas bort från Workfront

#### Borttagning av åsidosättningsvalutan i jobbroller med version 25.11

Som en del av förenklingen av den finansiella modellen kommer åsidosättningsvalutan för jobbroller i förhandsversionen den 30 oktober och i produktionen för alla kunder med version 25.11. Den här ändringen påverkar hur valutor och frekvenser konfigureras för jobbroller i inställningsområdet.

* Fälten **Åsidosätt valuta** i en jobbroll är inte längre tillgängliga.
* Varje jobbroll har en valuta med tillhörande kostnad och faktureringsfrekvens.
* Alla befintliga åsidosättningsvalutor och deras kursvärden migreras automatiskt till den enda valutan och valutorna för den jobbrollen.

## Modernisering av gränssnitt

Vi uppdaterar gränssnittet i hela Adobe Workfront för att förbättra användarupplevelsen och sammanföra det med andra Adobe-program. Dessa ändringar släpps utanför standardreleaseplanen. En lista över de här ändringarna finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Versionsinformation för andra områden

### Workfront Fusion-förbättringar

Nya funktioner i Workfront Fusion finns i Production på en cadence som ligger utanför standardreleaseprogrammet. Mer information om de senaste funktionerna finns i [Adobe Workfront Fusion-versionsaktivitet](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Förbättringar av Workfront Planning

Nya funktioner i Workfront Planning finns i Production. Mer information om de senaste funktionerna finns i [Första utgåvan av kvartal 2026 för Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Det finns inga uppdateringar för följande i den här versionen:

* Scenarioplan
* Korrektur
* Mål

## Uppdateringar för korrekturläsare för datorer

### Version 2.1.54

**Produktionsrelease för alla kunder: 11 december 2025**

Desktop Proofing Viewer har uppdaterats till 2.1.52 till 2.1.54. Uppdateringen innehöll interna verktygsuppdateringar och påverkade inte slutanvändarnas funktioner.

Version 2.1.53 innehåller även interna verktygsändringar.

Uppdateringen gäller både Mac och Windows.

### Version 2.1.52

**Produktionsrelease för alla kunder: 31 juli 2025**

Desktop Proofing Viewer har uppdaterats till version 2.1.52 som åtgärdar felkorrigeringar.

2.1.51-uppdateringen inkluderade interna verktygsuppdateringar och påverkade inte slutanvändarnas funktioner.

Uppdateringen gäller både Mac och Windows.

## Meddelanden

### API version 21

Workfront API version 21 släpptes 23 oktober 2025. För API-version 21 har vi ändrat vissa resurser och slutpunkter. Vissa av ändringarna har stöd för nya funktioner och andra gör det enklare för dig att använda informationen som är tillgänglig via API:t.

>[!IMPORTANT]
>
>Denna API-version innehåller en brytningsändring som kan påverka dina befintliga API-anrop. Detta beror på att API version 21 använder Event Subscriptions version 2.
>
> För flervalsfält skickas alltid Event Subscriptions version 2 som en array. Version 1 skickade en array om mer än ett värde har valts. Om bara ett värde valdes, skickades en sträng.

Information om nyheter och uppdateringar finns i [Nyheter i API-version 21](/help/quicksilver/wf-api/api/new-api-version-21.md).

Mer information om API-versioner finns i [API-versionshantering och supportschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Ny version av Workfront för Microsoft Teams

När [Microsoft övergår till New Teams-klienten](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) är Classic Teams-klienten inte längre tillgänglig efter 1 juli 2025. För att kunna fortsätta använda Microsoft Teams och integrerade program som Workfront måste kunderna gå över till nya Teams-klienten före detta datum.

Den uppdaterade Workfront-integreringen är nu tillgänglig och helt kompatibel med New Teams. I de flesta fall visas Workfront automatiskt när användaren har gått över. Om så inte är fallet kan integreringen installeras manuellt från Microsoft Teams App Store. Information om hur du installerar eller verifierar Workfront-integreringen i klienten New Teams finns i [Installera [!DNL Adobe Workfront] för Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront för Microsoft Outlook

[Microsoft håller på att inaktivera stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), som för närvarande används av Workfront Outlook-tillägget för autentisering. Denna förändring från Microsoft har redan börjat påverka kunderna och kommer att fortsätta att gälla i faser fram till oktober 2025.

* **När Microsoft har inaktiverat alla dessa variabler fungerar inte längre integreringen med Workfront för Microsoft Outlook.**

Som en del av den här ändringen har Microsoft beslutat att ändra hur tokens återaktiveras. Efter den **30 juni 2025** kan administratörer inte längre återaktivera tokens själva. Det är bara Microsoft Support som kan bevilja undantag. **Den 1 oktober 2025 inaktiveras äldre token för alla innehavare. Undantag beviljas inte.**

### Andra integreringsövergångar för Workfront

För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen är följande integreringar inte tillgängliga efter **28 februari 2026**:

* Workfront for G Suite
* Workfront för Jira
* Workfront för Salesforce.

Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Google Workspace.
En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Underhållsuppdateringar för Workfront

Mer information om underhållsuppdateringar som gjordes under den första utgåvan av kvartal 2025 finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Uppdateringar

Upptäck de senaste uppdateringarna av utbildningsprogram, utbildningsvägar, videor och guider för varje Adobe Workfront-produktrelease. Mer information finns i avsnittet Nyheter på [Workfront-sidan &#x200B;](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
