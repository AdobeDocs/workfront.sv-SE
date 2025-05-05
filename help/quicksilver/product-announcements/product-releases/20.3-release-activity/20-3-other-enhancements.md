---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 andra förbättringar
description: Den här sidan beskriver alla andra förbättringar som gjorts i version 20.3 i produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3 andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i version 20.3 i produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.

En lista över alla ändringar som är tillgängliga i version 20.3 finns i [20.3 versionsöversikt](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Dela en kalender med en privat länk

För att förenkla arbetet med att dela kalendrar i Workfront kan du dela en privat länk som tar användarna direkt till kalendern. Kalendern måste delas med användaren och användaren måste logga in för att kunna visa den.

Tidigare kunde du dela en offentlig URL som inte krävde inloggning för att kunna visa.

Mer information finns i [Dela en kalenderrapport](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Området Nya utkast när begäranden skapas

För att du ska kunna arbeta mer flexibelt med förfrågningar sparar Workfront nu automatiskt alla förfrågningar du skapar som utkast i det nya området Utkast. Om du inte har all information som krävs för att slutföra den nya begäran kan du lämna den som ett utkast, gå tillbaka till den och slutföra den senare. Workfront sparar en begäran per ämne i kön i området Utkast. Utkastbegäranden kan sparas så länge du behöver dem tills du är redo att slutföra och skicka dem. Du kan också ta bort eller flytta området Utkast på den vänstra panelen med hjälp av en layoutmall.

Mer information om hur du skapar begäranden finns i [Skapa och skicka Workfront-begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Om du har tilldelats en anpassad layoutmall i förhandsgranskningsversionen måste du lägga till området Utkast för dina begäranden genom att ändra layoutmallen.

## Expandera eller komprimera objekt på tidrapporten

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

För att du enkelt ska kunna hantera tidrapporter med flera objekt kan du nu expandera eller komprimera alla objekt genom att klicka på en knapp.

Tidigare var du tvungen att klicka på varje objekt för sig.

Mer information finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignorera faktiska datum i Workfront-kalendrar

>[!NOTE]
>
>Den här funktionen släpptes till förhandsvisningsmiljön den 5 juni 2020. Det kommer att finnas i produktionsmiljön den 19 juni 2020.

Om du vill ha större kontroll över hur objekt visas i kalenderrapporter kan du välja att ignorera faktiska datum även när de är tillgängliga.

Tidigare användes faktiska datum automatiskt i kalendern när de var tillgängliga.

Mer information finns i [Översikt över kalenderrapporter](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Använd anpassade datumfält i kalenderrapporter

>[!NOTE]
>
>Den här funktionen släpptes till förhandsvisningsmiljön den 29 maj 2020. Det kommer att finnas i produktionsmiljön den 12 juni 2020.

För att du bättre ska kunna visualisera och hantera ditt dagliga arbete med kalendrar finns nu anpassade datumfält som datumalternativ.

Tidigare kunde du bara hantera din kalender med projicerade, planerade när faktiska datum inte var tillgängliga.

Mer information finns i [Använd anpassade datumfält i en kalenderrapport](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (eller om du använder Workfront Classic, se [Använd anpassade datumfält i en kalenderrapport](https://experienceleague.adobe.com/sv/docs/workfront/using/home)).

## E-poständringar

**Ändringar i utgående e-post:** Alla e-postmeddelanden från Workfront kommer från notifications@my.workfront.com. Detta inkluderar automatiska varningar och kommunikation mellan användare.

Tidigare kunde systemadministratörer lägga till en anpassad e-postadress i området E-postinställningar.

**Ändringar i POP-svar för inkommande e-post:** Systemadministratörer kan inte längre konfigurera en anpassad POP-e-postserver för inkommande e-postsvar till meddelanden.

Mer information finns i [E-postförfalskning och POP-svar, e-poständringar](https://experienceleague.adobe.com/sv/docs/workfront/using/home).

## DomainKeys Identified Mail (DKIM) ingår nu i utgående Workfront-e-postmeddelanden

En teknik för e-postautentisering (DKIM) kommer att inkluderas i alla utgående e-postmeddelanden. Den här DKIM-signaturen är inte synlig för slutanvändaren, men tillåter validering på servernivå och stärker vårt befintliga autentiseringsramverk.

## Uppdateringar av registreringen i nya Workfront

Gruppadministratörer har nu åtkomst till att registrera och avregistrera användare som tillhör de grupper som de hanterar för att göra användarregistreringen i den nya Workfront-upplevelsen mer hanterbar.

Det finns nu även en länk för användarinformation som visar följande användarinformation:

* Namn
* Jobbroll
* E-postadress
* Profilbild

## Nytt för administratörer: varumärke-Workfront för specifika grupper, team, jobbroller och användare

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

Nu kan du använda en layoutmall för att ändra logotyperna i det övre navigeringsområdet och på huvudmenyn för specifika grupper, team, jobbroller och användare med egna varumärken.

Mer information finns i [Förse din Adobe Workfront-instans](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Gruppadministratörer kan skapa och hantera godkännandeprocesser

För att ge mer självbestämmande och kontroll över gruppernas arbetsflöden kan en gruppadministratör nu komma åt godkännandeprocessområdet i Inställningar och skapa och redigera godkännandeprocesser för en grupp som han eller hon hanterar. Dessa godkännandeprocesser baseras på gruppens status.

För att vara säker på att gruppadministratörer inte oavsiktligt redigerar godkännandeprocesser som används i hela systemet eller som har skapats av andra grupper, kan de bara komma åt de godkännandeprocesser som är kopplade till de grupper de hanterar.

Mer information finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## För administratörer: Sidan Nya grupper gör det enklare att skapa och hantera grupper

Gruppadministratörer kan enklare hantera grupper nu när allt de behöver finns på den nya gruppsidan. Du behöver inte längre navigera mellan olika övertäckningsrutor och konfigurationssidor för att skapa och ändra grupper.

Här är de viktigaste högdagrarna:

* Gruppinformation: Visa och redigera grundläggande information om gruppen, till exempel gruppens namn, beskrivning, gruppadministratörernas namn och om gruppen är offentlig eller privat.
* Lista med gruppmedlemmar: Visa alla gruppmedlemmar och använd det nya verktygsfältet för att snabbt lägga till, ta bort, exportera, aktivera och inaktivera medlemskap. Du kan också redigera medlemmarnas profiler och skicka dem Uppdatera kommentarer.
* Fältet Gruppadministratör i rubriken: När du visar en grupp som du hanterar kan du snabbt tilldela eller ta bort en gruppmedlem som administratör för gruppen. Du kan också göra detta i listan med gruppmedlemmar med hjälp av den nya kolumnen Grupproll.
* Lista med undergrupper: Visa, redigera, kopiera, exportera och ta bort undergrupper i en grupp som du hanterar.
* Statuslista: Visa och hantera gruppens status.

Mer information finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Nytt för administratörer: Skapa upp till 14 nivåer med undergrupper

För att göra det enklare att ordna dina Workfront-grupper så att de matchar din organisationshierarki har vi ökat nivån på undergrupper som du kan skapa i en grupp mellan 3 och 14.

Mer information finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Nytt för administratörer: Nytt sidofält för installationsprogrammet

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

Det vänstra sidofältet i installationsprogrammet är nu snabbare och enklare att använda och utnyttjar den grundläggande layout och funktionalitet som du redan känner till. Tillsammans med ett modernare utseende och känsla är det här något annat nytt:

* En ny benvit bakgrund i sidofältet gör det enklare att skilja sig från resten av inställningsområdet.
* Ikonerna i sidlisten är lite större och vissa har fått en ny design som tydligare visar vad alternativet gör.
* Mer lodrätt utrymme mellan sidofältobjekt gör dem lättare att läsa.
* Du kan komprimera sidofältet när du behöver utrymme i huvudområdet för att se och göra mer, till exempel visa ytterligare kolumner. Och du kan expandera sidofältet igen när du behöver se funktionsnamnen.
* När sidofältet är komprimerat visas bara ikonerna för varje funktion. Om du vill visa underobjekten under ett sidofältsobjekt för du pekaren över dess ikon för att visa dem i en utfällbar meny. Du kan till exempel hålla muspekaren över ikonen Processer för att visa en meny som innehåller godkännande- och milstolpe-banor.
* Du kan komma åt de två alternativen Snabbstart (Importera data och Exportera data) en klickning snabbare. De har flyttats ut från under System för att visas på sidofältens huvudnivå.

Mer information om hur du använder inställningsområdet finns i [Administration och konfiguration](../../../administration-and-setup/administration-and-setup.md).

## Inkludera klusternummer i området Kundinformation

Som Workfront-administratör kan du nu enkelt hitta klusternumret i Workfront utan att behöva lägga ned mer tid och kraft på att få det från vårt supportteam. Vi lade till ett klusterinställningsfält i området Kundinformation i installationsprogrammet.

Mer information om området Kundinformation finns i [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Base64-kodning för händelseprenumerationer

base64Encoding-fältet är ett valfritt fält som används för att aktivera Base64-kodning av händelseprenumerationsnyttolaster. Om en begäran görs med fältet base64Encoding inställt på true, levereras objekten newState och oldState i nyttolasten som Base64-kodningssträngar. Den här funktionen kan vara användbar om ditt nätverk är konfigurerat på ett sådant sätt att det inte tillåter specialtecken i händelseprenumerationer.

Mer information finns i [API för händelseprenumeration](../../../wf-api/general/event-subs-api.md).

## Möjlighet att skapa duplicerade händelseprenumerationer har tagits bort

Du kan inte längre skapa dubblettprenumerationer för att förhindra att dubblettmeddelanden levereras. Dessutom har dubblettprenumerationer som skapats tidigare tagits bort.

Mer information finns i [Vanliga frågor och svar - Händelseabonnemang](../../../wf-api/general/event-subs-faq.md).
