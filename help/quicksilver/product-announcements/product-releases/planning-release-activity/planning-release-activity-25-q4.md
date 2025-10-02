---
content-type: release-notes
title: Versionsaktivitet fjärde kvartalet 2025 för Adobe Workfront Planning
description: Detta är lanseringsaktiviteten för Adobe Workfront Planning-produkten för fjärde kvartalet 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f75f44c3c5ea4c281c0c9fe916ea8261d3500fb0
workflow-type: tm+mt
source-wordcount: '2508'
ht-degree: 0%

---

# Versionsaktivitet fjärde kvartalet 2025 för Adobe Workfront Planning

I den här artikeln beskrivs funktionerna som lanseras för Workfront Planning i den fjärde utgåvan av kvartal 2025.

<!--keep the sentence below for all future quarterly release pages-->

En lista över alla funktioner som släppts för Adobe Workfront Planning finns i [Versionsaktivitet för Adobe Workfront Planning: artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--## Centralized record types

>[!NOTE]
>
>Preview: October 2, 2025
>Production fast release: October 15, 2025
>Production for everyone:  October 16, 2025

When implementing Workfront Planning for a multi-team organization with common workflows, you might need to define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work.  

 Also, you might need each team's work to roll up to a central level.  

 In such a workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everything to one workspace, or everyone in the organization to every workspace. You can use centralized record types to achieve this. 

You can now enable record types to be centralized and use them across multiple workspaces. Users can use the same field structure and connections that are already configured in a central workspace.  

For more information, see the following articles:  

* [Cross-workspace record type overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) 

* [Configure record type cross-workspace capabilities](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) 

* [Add existing record types from another workspace](help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## New limit for connection fields for one record type

>[!NOTE]
>
>Preview: October 2, 2025
>Production fast release: October 15, 2025
>Production for everyone:  October 16, 2025

We have introduced a limit of 30 connection fields for each record type.  

If your organization currently has more than 30 connection fields for one record type, the additional connections will be inherited going forward. However, you cannot add more connection fields. For new record types, the new limit of 30 connection fields will be enforced.  

For more information, see [Connected Record Types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).-->

## Förbättringar av förfrågningar om formulär i Workfront Planning

>[!NOTE]
>
>Förhandsgranska: 2 oktober 2025
>&#x200B;>Production fast release: 15 oktober 2025
>&#x200B;>Produktion för alla: 16 oktober 2025

För att förenkla förfrågningsprocessen har vi gjort några förbättringar av förfrågningsformulären. När du konfigurerar ett begärandeformulär kan du nu konfigurera följande:

* Aktivera ett alternativ om du bara vill tillåta ett beslut när en begäran har flera godkännare.
* Konfigurera när begäranden som skapas från formuläret automatiskt markeras som slutförda. Du kan ange att begäran ska markeras som slutförd när det begärda objektet skapas, eller när det begärda objektet är färdigt baserat på de villkor du anger.
* Ställ in en automatisering som aktiveras när en begäran skickas från formuläret. För närvarande kan du automatiskt skapa poster när en förfrågan skickas.

Mer information om hur du skapar ett begärandeformulär och konfigurerar dessa alternativ finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Dra och släpp-funktionen i tidslinjen och kalendervyer

>[!NOTE]
>
>Förhandsgranska: 2 oktober 2025
>&#x200B;>Production fast release: 15 oktober 2025
>&#x200B;>Produktion för alla: 16 oktober 2025


Nu kan du dra och släppa poster i tidslinjen och kalendervyer. Om du drar posterna i en annan tidsram uppdateras automatiskt start- och slutdatumen.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Kommentera begäranden i Workfront Planning

>[!NOTE]
>
>Förhandsgranska: 2 oktober 2025
>&#x200B;>Production fast release: 15 oktober 2025
>&#x200B;>Produktion för alla: 16 oktober 2025

För att förenkla kommunikationen av förfrågningar i Workfront Planning har vi lagt till ett kommentarsområde på sidan Begär information. Detta är användbart om personen som begäran är tilldelad har frågor till personen som gjorde begäran.

Det gick inte att kommentera begäranden tidigare i Workfront Planning.

Mer information om hur du gör begäranden, inklusive kommentarer, finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

<!--## Approve a Workfront Planning request in the My Approvals widget

>[!NOTE]
>
>Preview: October 2, 2025
>Production fast release: October 15, 2025
>Production for everyone:  October 16, 2025

To make it easier to approve Workfront Planning requests, we've added them to the My Approvals widget in Home. Now, you can approve or reject these requests directly from the widget, allowing you to manage these approvals without leaving Home.

Previously, Workfront approvals could be managed only within Workfront Planning.

For more information on approving requests, see [Approve a request in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).-->

## Inline redigera Workfront-projekt på postens sida för kopplade poster

>[!NOTE]
>
>Förhandsgranska: 25 september 2025
>&#x200B;>Production fast release: 15 oktober 2025
>&#x200B;>Produktion: 16 oktober 2025

Nu kan du infoga redigering av Workfront-anslutna projekt på sidan Anslutna poster. Du kan också skapa projekt utan en mall från den anslutna postsidan.

Mer information finns i [Hantera postsidan](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Unified request form list now available

>[!NOTE]
>
>* Preview: September 4, 2025
>* Production fast release: September 11, 2025
>* Production all: October 16, 2025

To make it easier to find the request form you're looking for in Workfront Planning, we've created a unified list for request forms. Now, all request forms that you have access to can be found in a single list, regardless of the object they were created for. Clicking on a form in this list brings you to the request form's page, where you can edit, preview, or publish and unpublish the form.

Previously, request forms were located only on the object for which they were created.

For more information on request forms, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). -->

## Utforma om verktygsfälten och åtkomstpunkterna för planeringsvyer

>[!NOTE]
>
>* Förhandsgranska: 25 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion: 16 oktober 2025

Vi har gjort om hur du visar, får åtkomst till och hanterar vyer på en posttypssida.

Följande förbättringar ingår i den här uppdateringen:

* Vyflikarna har ersatts av en listruta i det övre vänstra hörnet av posttypssidan. Menyn innehåller nu en lista med alla vyer.
* Du kan ändra ordningen på vyerna genom att dra och släppa dem i den ordning som du vill.
* De flesta verktygsfältsikonerna, förutom helskärmsläget, har flyttats från höger sida till vänster på sidan.
* Sökrutan har flyttats till höger om verktygsfältet.
Funktionen för varje vy har inte ändrats.

Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

<!--## Enhancements to request forms in Workfront Planning

>[!NOTE]
>
>* Preview: September 25, 2025
>* Production fast release: October 15, 2025
>* Production all: October 16, 2025

To make the request process simpler, we've made some enhancements to request forms. Now, when configuring a request form, you can configure the following:

* Configure when requests created from the form will be automatically marked complete. You can set the request to be marked complete when the requested object is created, or when the requested object is complete based on criteria you specify.
* Set up an automation that is triggered when a request is submitted from the form. Currently, you can automatically create records when the request is submitted. 

For more information on creating a request form and configuring these options, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). -->

## Ändra storlek på poster i kalenderns veckovy

>[!NOTE]
>
>* Förhandsgranska: 25 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion: 16 oktober 2025

I vyn för veckokalendrar på en posttypsida kan du nu klicka och hålla ned en posts vänstra eller högra marginal för att ändra dess varaktighet.

När du flyttar en posts marginaler ändras också dess start- och slutdatum omedelbart.

En disposition visas som vägleder dig till den nya platsen innan händelsens storlek ändras.

Den här funktionen finns redan i kalenderns månadsvy.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Ny inställning som förhindrar att en dubbelriktad anslutning skapas från en posttyp

>[!NOTE]
>
>* Förhandsgranska: 18 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion: 16 oktober 2025

För att förhindra att alltför många anslutningsfält skapas och eventuellt påverka prestanda har vi infört en ny inställning som gör att arbetsytehanterare kan skapa motsvarande anslutna fält på en ansluten posttyp. När det här alternativet är aktiverat räknas anslutningar av båda posterna, vilket ökar risken för att 500-anslutningsgränsen uppnås. För att undvika det rekommenderar vi att du inte aktiverar den här inställningen, särskilt när du länkar till taxonomiska posttyper.

Följande funktioner ingår i den här förbättringen:

* En ny inställning för&quot;Skapa motsvarande fält för länkad posttyp&quot; har lagts till på fliken Ny anslutning.

* Området Anslutningstyp på fliken Ny anslutning har fått en ny utformning.

* Det finns en gräns på 500 anslutningar för varje posttyp.

* Den nya inställningen kan ändras när en ny anslutning har skapats och sparats.



Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

## Ny informationsruta visas när du ändrar eller tar bort ett fält

>[!NOTE]
>
>* Förhandsgranska: 11 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion: 16 oktober 2025

När du uppdaterar ett formelfält eller ett fält som kan påverka det visas ett varningsmeddelande om hur ändringen påverkar dig. Varningen visas i följande fall:

* När du uppdaterar ett formelfält (exklusive ändringar av namn och beskrivning) när det fältet har beroende formelfält eller uppslagsfält. Aviseringen visar de beroende fälten och frågar om du vill fortsätta.

* När du tar bort ett fält som används i ett formeluttryck eller som ett uppslagsfält. Varningen visar de beroende formeln och sökfälten och frågar om du vill fortsätta med borttagningen.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Integrering mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing

>[!NOTE]
>
>Förhandsgranska: 11 september 2025
>&#x200B;>Produktion för alla kunder: 11 september 2025
>&#x200B;>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Om er organisation använder både Adobe Workfront Planning och Adobe GenStudio for Performance Marketing kanske ni vill definiera mer detaljerade marknadsföringskoncept som Campaigns, Products och Personas än vad GenStudio stöder som standard.

Tack vare den nya integreringen mellan GenStudio for Performance Marketing och Workfront Planning kan ni nu hantera de kampanjer, produkter, personuppgifter, aktiveringar, kanaler och regioner som används i GenStudio for Performance Marketing i Workfront Planning. Tack vare integreringen kan du även konfigurera GenStudio for Performance Marketing så att det refererar till befintliga posttyper från Workfront Planning, vilket skapar ett mer uppkopplat och enhetligt arbetsflöde för marknadsföring.

GenStudio for Performance Marketing arbetsyta är nu tillgänglig i Adobe Workfront Planning när ditt företag har köpt båda produkterna.
Tack vare integrationen mellan Workfront Planning och GenStudio for Performance Marketing kan du

* Visa arbetsytan i GenStudio i Workfront Planning.
* Modifiera kampanjer, produkter, profiler och aktiveringar i GenStudio for Performance Marketing och få uppdateringar i realtid av samma information i Workfront Planning.
* Ändra kampanjer, produkter, personligheter och aktiveringar i Workfront Planning och ha realtid
* Undvik dubblettinmatning.
* Bibehåll enhetligheten i planeringen och aktiveringen.

Mer information finns i [Kom igång med integreringen mellan Adobe Workfront Planning och Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Ändra storlek på poster i kalenderns månadsvy

>[!NOTE]
>
>* Förhandsgranska: 4 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion: 16 oktober 2025

I kalendervyn på en posttypsida kan du nu klicka, dra och släppa en posts vänstra eller högra marginal för att ändra dess varaktighet.

När du flyttar en posts marginaler ändras också dess start- och slutdatum omedelbart.

En disposition visas som vägleder dig till den nya platsen innan händelsens storlek ändras.

Det går bara att ändra storlek på poster i kalendervyn om vyn visas per månad.

Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Skapa poster i kalendervyn

>[!NOTE]
>
>* Förhandsgranska: 4 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion för alla kunder: 16 oktober 2025

Nu kan du skapa poster i kalendervyn av en posttyp genom att dubbelklicka var som helst i kalendern.

Du kan välja datumintervall för posten eller öppna postens sida för att redigera all information.

Före den här förbättringen kunde du bara lägga till nya poster från kalendervyn med knappen Ny post.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Ändra storlek på poster i tidslinjevyn

>[!NOTE]
>
>* Förhandsgranska: 4 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion för alla kunder: 16 oktober 2025

I tidslinjevyn på en posttypsida kan du nu klicka, dra och släppa en posts vänster- eller högermarginal för att ändra dess varaktighet.

När du flyttar en posts marginaler ändras också dess start- och slutdatum omedelbart.

En disposition visas som vägleder dig till den nya platsen innan händelsens storlek ändras.

>[!NOTE]
>
>Det går att ändra storlek på poster i tidslinjevyn när vyn visas varje år, varje kvartal eller varje månad.


Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Styr hur många poster som ska visas i kalendervyn

>[!NOTE]
>
>* Förhandsgranska: 4 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion för alla kunder: 16 oktober 2025

Vi har lagt till inställningen Radhöjd i verktygsfältet i kalendervyn på en postsida. Du kan nu välja hur många poster som ska visas i en kalendercell genom att välja något av följande alternativ för vyns radhöjd:

* Kort
* Standard
* Medium
* Hög
* Anpassa till innehåll

Inställningen är bara tillgänglig när kalendervyn visas per månad. Inställningen är inte tillgänglig när kalendern visas per vecka.

Mer information, inklusive begränsningar för varje alternativ, finns i [Hantera kalendervyn](/help/quicksilver/planning/views/manage-the-calendar-view.md).


## Lägg till ett nytt alternativ för urvalsfält i tabellvyn

>[!NOTE]
>
>* Förhandsgranska: 4 september 2025
>* Production fast release: 15 oktober 2025
>* Produktion för alla kunder: 16 oktober 2025

Du kan nu lägga till ett nytt alternativ i ett enskilt- eller flervalsfält när du uppdaterar fältvärdet i tabellvyn. Om du till exempel har tre alternativ för ett envalsfält för Status och vill ha ett fjärde alternativ, kan du lägga till det när du redigerar statusfältet för en post i tabellvyn.

Före den här förbättringen kan du bara lägga till nya alternativ genom att redigera fältet.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig när du uppdaterar fältvärden i tabellvyn.


Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).

## Ny kombinerad statuskolumn i listan för enhetliga begäranden

>[!NOTE]
>
>* Förhandsgranska: 28 augusti 2025
>* Production fast release: 11 september 2025
>* Produktion för alla kunder: 16 oktober 2025

För att förenkla den enhetliga upplevelsen av begäranden visas nu både begärandestatus och godkännandestatus i statuskolumnen, beroende på vilket som gäller för en viss begäran.

Mer information om hur du skapar begäranden finns i:

* För Workfront: [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* För Workfront Planning: [Skicka in Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md)

## Nya gränser för formelfält

>[!NOTE]
>
>* Förhandsgranska: 28 augusti 2025
>* Production fast release: 11 september 2025
>* Produktion för alla kunder: 16 oktober 2025

Vi har satt följande gränser för formelfält:

* Det finns en gräns på 20 formelfält per posttyp
* Ett formeluttryck får innehålla högst 50 000 tecken

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Visa fel när formelvärden inte kan matchas

>[!NOTE]
>
>* Förhandsgranska: 28 augusti 2025
>* Production fast release: 11 september 2025
>* Produktion för alla kunder: 16 oktober 2025

Fältet visas nu som &quot;#ERROR!&quot; för att visa att det inte går att lösa ett formelfält i något av följande fall:

* När ett fält som används i en formel tas bort.

* När ett fält som används i ett aggregerat uppslagsfält visas som #ERROR!.

* När ett formelvärde inte kan visas i det valda formatet.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

## Nya uttryck har lagts till i formelfält i Planning

>[!NOTE]
>
>Förhandsgranska: 7 augusti 2025
>&#x200B;>Produktion för alla kunder: augusti 2025
>&#x200B;>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Vi har lagt till nya uttryck med följande användning i formelfält i Workfront Planning och i beräknade anpassade fält i Workfront:

* **REMOVEACCENTS(string)**: Tar bort diakritiska tecken från alla tecken med accent i indatasträngen.
* **REPLACEPATTERN (sträng, mönster, ersättningssträng)**: Ersätter matchningarna för det angivna mönstret med ersättningssträngen.
* **PASCAL(string)**: Konverterar indatasträngen till PascalCase genom att ändra den första bokstaven i varje ord till versal och ta bort alla blanksteg.

Mer information finns i [Översikt över beräknade datauttryck](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Lägga till Maximera och Minimera-knappar i fönstret där formelfält skapas

>[!NOTE]
>
>Förhandsgranska: 31 juli 2025
>&#x200B;>Produktion för alla kunder: 31 juli 2025
>&#x200B;>[!BADGE Frånschemat &#x200B;]{type=Neutral}

Vi har lagt till knappen Maximera för att förstora formelfältet när du skapar eller redigerar fältet i en posttabellvy. Dessutom har vi lagt till en Minimera-knapp i det nya förstorade fönstret för att återgå till rutan för att skapa fält.

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Sidan Anslutna poster är nu tillgänglig i en posts förhandsgranskningsområde

>[!NOTE]
>
>* Förhandsgranska: 31 juli 2025
>* Production fast release: 14 augusti 2025
>* Produktion för alla kunder: 16 oktober 2025

Vi har nu gjort så att upplevelsen på den anslutna postsidan i förhandsvisningsrutan matchar den på sidan på hela sidan i en posts informationsområde.

Före den här förbättringen var det endast möjligt att visa anslutna poster på en sida med anslutna poster på hela sidan i en posts informationsområde.

Mer information finns i [Hantera postsidans layout](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Skapa poster i tidslinjevyn

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Nu kan du skapa poster i tidslinjevyn för en posttyp genom att dubbelklicka någonstans på tidslinjen.

Du kan välja datumintervall för posten eller öppna postens sida för att redigera all information.

Före den här förbättringen kunde du bara lägga till nya poster med knappen Ny post eller textbunden i tabellvyn.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Alternativet Lägg till delning på menyn Mer för ett posttypskort

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Du kan nu dela en posttyp på menyn Mer på posttypskortet på arbetsytesidan. Före den här förbättringen var alternativet Dela bara tillgängligt på posttypssidan.

Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).

## Visa alla Workfront Planning-vyer i helskärmsläge

>[!NOTE]
>
>Förhandsgranska: 24 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Nu kan du visa alla Workfront Planning-vyer (tabell, tidslinje och kalender) i helskärmsläge. Visningsfunktionen bevaras och du kan även ändra vyn i helskärmsläge.

Före den här förbättringen fanns inte den här funktionen.

Mer information finns i [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md).

## Lägg till team som godkännare i planeringsförfrågningsformulär

>[!NOTE]
>
>Förhandsgranska: 22 juli 2025
>&#x200B;>Production for fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

För att göra godkännandeprocessen mer flexibel har vi lagt till möjligheten att lägga till team som godkännare i planeringsförfrågningsformulär. Nu kan du ange och välja teamnamn när du ställer in godkännare. Alla teammedlemmar kan fatta ett beslut som räknas som ett godkännandebeslut för hela teamet.

Tidigare kunde bara enskilda användare tilldelas godkännare.

Mer information finns i [Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Nya fält för att visa information om postgodkännande

>[!NOTE]
>
>Förhandsgranska: 17 juli 2025
>&#x200B;>Production for fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025

Vi introducerar följande fält för att samla in godkännandeinformation för poster som skapats genom att skicka en begäran med ett godkännande:

* Godkänd av
* Godkännandedatum

Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

## Fyll i fält automatiskt baserat på använda grupperingar

>[!NOTE]
>
>Förhandsgranska: 10 juli 2025
>&#x200B;>Production fast release: 14 augusti 2025
>&#x200B;>Produktion för alla kunder: 16 oktober 2025


När du har använt grupperingar i en tabellvy fylls de fält som är kopplade till de grupperingar du lägger till posten i automatiskt i när du lägger till en post i tabellen.

Om du har använt flera grupperingar fylls fälten som är kopplade till alla grupperingar i automatiskt när du lägger till posten i slutet av listan i det sista grupperingsvillkoret.

Före den här förbättringen behövde du uppdatera fälten som var kopplade till grupperingar manuellt.

Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
