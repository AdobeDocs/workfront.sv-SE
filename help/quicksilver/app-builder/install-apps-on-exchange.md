---
title: Hämta och installera program från Adobe Exchange
description: Med Workfront UI Extensions, som drivs av Adobe App Builder, kan kunder och partner skapa skräddarsydda användarupplevelser.
author: Courtney
feature: Digital Content and Documents
source-git-commit: 0a90da6978fc9b380d237dab74af1f14eabb857a
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---


# Hämta och installera program från Adobe Exchange

Du kan nu installera partnerbyggda program för Workfront direkt från Adobe Exchange. Detta kopplar samman kunderna med ett växande antal av Adobe partners som levererar specialbyggda verktyg som förbättrar produktiviteten, effektiviserar verksamheten och utökar Workfront funktionalitet. Genom Adobe Exchange kan kunderna upptäcka och installera appar som sömlöst integreras i Workfront med hjälp av UI-tillägg.

Adobe Exchange är den centrala marknadsplatsen för tredjepartsprogram, tillägg och integreringar i Adobe Experience Cloud - inklusive Adobe Workfront. För Workfront-kunder är det den perfekta målplatsen att upptäcka och installera program som förbättrar funktionaliteten, effektiviserar arbetsflödena och integreras med externa system.

## Adobe partnerappar

Workfront Partner Network är ett växande ekosystem av teknikpartners - oberoende programvaruleverantörer (ISV) som bygger skalbara, säkra och utbyggbara appar med Adobe App Builder och Workfront UI Extensions.

Workfront partners utnyttjar Workfront UI Extensions, ett kraftfullt ramverk som gör att appar kan bäddas in direkt i Workfront gränssnitt. När du har installerat dem från Adobe Exchange kan Workfront-administratörer lägga till dem i layoutmallar, så att de blir synliga och tillgängliga för användare i deras dagliga arbetsflöden. Denna smidiga integrering säkerställer att användarna kan interagera med verktyg som skapats av partners - som kontrollpaneler, godkännandeflöden eller kampanjspårare - utan att lämna Workfront-miljön.

### AtApp

#### Resultat i realtid direkt i Adobe Workfront

Vi samarbetar med Adobe Workfront-kunder för att förvandla vardagliga flaskhalsar till repeterbara lösningar med förutsägbara resultat. Vårt växande bibliotek med lösningar hjälper er att öka noggrannheten, hastigheten och ansvarsskyldigheten med hjälp av livedata från den plats där människor arbetar. Ni kan hjälpa ledarna att se vad som händer nu och planera vad som ska hända härnäst. Utforska de Adobe Exchange-appar i AtAppStore som är tillgängliga och klara att installera, välj sedan de som matchar dina aktuella prioriteringar och skala sedan efter behov.

* [Excel Updater](https://exchange.adobe.com/apps/ec/abtt1rq7o9/atapp-excel-updater): Med Excel Updater-lösningen får du ett kostnadseffektivt sätt att integrera data i Workfront utan att du behöver lära dig API:t, skriva kod eller konfigurera en server, och den är idealisk för både engångs- och återkommande datainläsningar.

* [Återanvänd hjälp](https://exchange.adobe.com/apps/ec/abv755903t/atapp-recalc-helper): Med den här lösningen kan du snabbt beräkna om anpassade formulärberäknade uttryck, projekttidslinjer eller projektekonomi för alla objekt som matchar ett valt filter, direkt från Workfront.

* UberTimesheet: UberTimesheet-lösningen kan förbättra och utöka användarnas användning av Workfront genom att göra det enkelt och bekvämt för alla att spåra tiden från webbläsaren, surfplattan eller smarttelefonen, efter det att de gjort det.

### Arbetsfokus

Workfocus ger avancerade automatiserings- och integrationslösningar för Workfront. Deras appar fokuserar på:

* Effektivisera tidslinjer

* Automatisera Fusion-arbetsflöden

* Möjliggör samarbete mellan instanser

Arbetsfokusappar är utformade för att fungera direkt i Workfront och utnyttjar UI-tillägg för att ge användarna kraftfulla verktyg som förbättrar produktiviteten och minskar den manuella arbetsinsatsen.

## Förutsättningar och behörigheter

**App Builder Provisioning**

* Kunder måste ha App Builder etablerat i sin Adobe Admin Console. Detta är en nödvändig förutsättning för att installera program från Adobe Exchange.

**Företagsorganisationsadministratörer eller utvecklare**

* Du kan söka efter appar, klicka på **Hämta** och fortsätta med installationen.

* Om appen redan har hämtats av någon i organisationen kan de se **Starta installationen** eller **Hantera** i stället.

**Användare som inte är administratörer**

* Kan starta förvärvet men uppmanas att logga in och kan stöta på begränsningar om appen kräver administratörsgodkännande eller särskild licensiering.

## Hämta och installera program från Adobe Exchange

Adobe-kunder kan bläddra bland, söka efter och installera program direkt från Adobe Exchange Marketplace och använda dem i Workfront.

Appar som skapats med Adobe App Builder listas som _App Builder-program_ på Adobe Exchange. Varje programlista innehåller dokumentation, skärmdumpar och användningsanvisningar som hjälper kunderna att förstå appens värde.

Om du vill visa program för Workfront går du till Adobe Exchange och söker efter Workfront-kompatibla program. Du kan även filtrera listor för Workfront App Builder-program:

1. Klicka på **Experience Cloud** i den vänstra panelen.
1. I den vänstra panelen söker du efter **Produkt** och väljer sedan **Workfront**.
1. Expandera **apptyp** och välj sedan **App Builder**.

### Hämta appar

Appar kan kräva köp från Adobe Exchange eller tillåta installation, men kräver licens från apputvecklaren.

Så här skaffar du en app

1. Klicka på appens namn.
1. Klicka på knappen längst upp till höger i programlistan.
1. Klicka på **Ja, fortsätt** och godkänn sedan slutanvändarlicensavtalet.
   ![bekräfta licensavtalet](assets/2-aquire-application.png)

### Åtgärder för systemadministratörer

När en användare köper ett program från Adobe Exchange kan det visas följande meddelande: _Systemadministratören måste godkänna köpet innan du kan installera och använda programmet._

Det innebär att programmet måste godkännas på administratörsnivå innan installationen kan fortsätta. Systemadministratörer kan hitta begäran från följande områden:

**Meddelanden**

Systemadministratörer meddelas vanligtvis via e-post när en användare i organisationen köper en app.

**Admin Console**

Systemadministratörer kan logga in på Admin Console på [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/) och navigera till Produkter > Programintegreringar för att visa alla hämtade eller begärda program.

När en systemadministratör har åtkomst till förfrågningarna kan de granska och godkänna programmet. Vissa appar kan uppmana administratören att ge sitt medgivande till dataåtkomst och tilldela appen till produktprofiler eller specifika användare.

När appen godkänts blir den tillgänglig för installation.

![granska och godkänna appar](assets/3-manage.png)

## Installera program

När en app har köpts kan den installeras direkt i Workfront. Administratörer kan hantera installerade program via Workfront-gränssnittet för att säkerställa att de är korrekt konfigurerade och tillgängliga för användarna.

1. Hitta det program du vill installera och öppna Åtgärder-menyn till höger på skärmen.
1. Klicka på Visa appinformation.
1. Välj en miljö till vänster på skärmen eller lägg till en ny.
1. Klicka på **Distribuera**.
   ![distribuera app](assets/10-env-details-2.png)
1. Tilldela installations- eller användningsbehörighet (om det behövs).

   Om organisationen styr appåtkomst via produktprofiler eller användargrupper tilldelar du appen till rätt profil eller grupp så att användarna kan fortsätta med installationen och använda den.

## Lägg till i layoutmall

När partnerappen har distribuerats är den tillgänglig i Workfront layoutmall. Du kan lägga till appen i primär eller sekundär navigering som ska användas i Workfront.

Om du vill lägga till programmet i layoutmallen öppnar du layoutmallen och går till huvudmenyn eller sekundära menyområden. Lägg till appen med ikonen Lägg till.

![lägg till app i layoutmallen](assets/add-to-lt.png)

## Kontakta appsupport

Tillägg som installeras från Adobe Exchange stöds av appägarna. Från Hantera program kan du klicka på **Få support** för att få hjälp med eventuella problem.