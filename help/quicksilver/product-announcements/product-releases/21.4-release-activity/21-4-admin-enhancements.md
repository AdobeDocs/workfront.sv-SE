---
title: 21.4 Administratörsförbättringar
description: 21.4 Administratörsförbättringar
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 21.4 Administratörsförbättringar

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 21.4 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 4 oktober 2021.

En lista över alla ändringar som är tillgängliga i version 21.4 finns i [21.4 Versionsöversikt](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## För administratörer: Se vilka grupper som är kopplade till en godkännandeprocess

För att du ska få reda på vilka grupper som är kopplade till godkännandeprocesserna i ditt system har vi lagt till en gruppnamnskolumn i standardvyn på sidan Godkännanden i Inställningar. Nu kan du visa den här informationen utan att behöva skapa en anpassad vy.

Mer information om godkännandeprocesser finns i [Översikt över godkännandeprocessen](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Mer information om hur du hanterar gruppgodkännandeprocesser finns i [Godkännandeprocesser på gruppnivå](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Nytt för administratörer: Grupper kan konfigurera sina egna inställningar för tidrapport och timma

>[!NOTE]
>
>I Production kommer denna funktionalitet till att börja med att vara tillgänglig som en del av en fasad lansering endast för kunder i kluster 4. Den här anteckningen uppdateras när funktionen blir tillgänglig för andra kluster.

I en stor organisation kan vissa grupper behöva konfigurera tidrapport- och timinställningar separat för att passa sina unika arbetsflöden, i stället för att ärva inställningarna som konfigurerats av en administratör på systemnivå. Nu kan Workfront-administratörer låsa upp en tidrapport och timinställning för alla grupper i systemet så att de själva kan konfigurera den.

Den här funktionen lades också till nyligen för projektinställningar och för inställningar för uppgifter och utgåvor.

Mer information om hur en Workfront-administratör låser upp en tidrapport och timinställning finns i avsnittet [Lås upp tidrapport och timinställningar för grupper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) i artikeln [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Mer information om hur en gruppadministratör konfigurerar olåsta uppgifter och utfärdar inställningar för en grupp finns i [Konfigurera tidrapport och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Nytt för Workfront-administratörer: Konfigurera layoutmallar för användare med automatisk etablering i den nya Workfront-upplevelsen

Nu kan du konfigurera layoutmallar i den nya Workfront-upplevelsen för användare som etablerats automatiskt. I listrutan Workfront-användarattribut, där du mappar användarattribut (Inställningar > System > Enkel inloggning), finns nu ett nytt menyalternativ på menyn Ny layoutmall som du kan använda för att göra den här konfigurationen. Tidigare kunde du bara konfigurera layoutmallar för användare med automatisk etablering i Workfront Classic.

Instruktioner om hur du mappar användarattribut finns i [Mappa användarattribut och autodistribuera nya användare](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Nytt fält visar de grupper som användarna tillhör

Nu är det enkelt att ta reda på vilka grupper användarna tillhör. I en rapport eller vy som listar användare kan du skapa en kolumn med hjälp av det nya fältet Andra grupper. I det här fältet visas de grupper där varje användare är medlem.

Mer information om hur du använder rapporter och vyer finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) och [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Sidan med information om utkast visar nu en bild

På informationssidan för varje plan visas nu en bild av projektmallen som installeras tillsammans med ritningen. Bilden innehåller en förhandsvisning av det blå innehållet så att du vet vad du ska installera. Du kan också förhandsvisa hela bilden i webbläsaren eller hämta bilden.

Mer information finns i [Översikt över utkast](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Inställningar för utkast av nya utgåvor

Nya inställningar för utgåvor finns nu för vissa utkast. De installeras som standard, men du kan välja att inte installera inställningarna när du konfigurerar installationsinformationen.

Inställningarna omfattar ämnesgrupper i kön, köämnen och routningsregler för att samla in korrekt information när ett problem eller en förfrågan skickas och skicka ärendet eller förfrågan till rätt jobbroll eller team. Inställningarna gör att du kan skapa ett konsekvent sätt att hantera nya utgåvor eller förfrågningar i dina projekt.

Observera att när du använder dessa inställningar konverteras inte projekt som skapats från mallen till begärandeköer.

Mer information finns i [Konfigurera en plan](../../../administration-and-setup/blueprints/configure-template-package.md).

## Nytt för gruppadministratörer: Visa och hantera nyligen borttagna och återställda objekt i en grupp

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Vi fortsätter att göra det enklare att hantera dina grupper och tillhörande objekt på ett och samma ställe. Nu kan du visa och arbeta med en grupps nyligen borttagna och återställda objekt i gruppområdet. Detta gör att du inte behöver gå till området Senast borttaget eller Senast återställt i installationsprogrammet för att hantera dessa objekt. Listan med gruppobjekt som du arbetar med hålls åtskild från andra borttagna och återställda objekt i systemet.

Mer information finns i [Visa och hantera nyligen borttagna objekt i en grupp](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) och [Visa och hantera nyligen återställda objekt i en grupp](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Nytt för gruppadministratörer: Gruppinställningar påverkar nu gruppmallar

Nu är det enklare att se till att gruppens projektmallar motsvarar gruppens behov. När du tilldelar en ny projektmall till en grupp samtidigt som du skapar den, ärver mallen följande inställningar från gruppens projekt- och uppgiftsinställningar:

* Resultatindexmetod
* Villkorstyp
* Schemalägg från
* Användartid ledig
* Uppdateringstyp
* Inställningar för åtkomstsektion

När du skapar en ny malluppgift i en projektmall som är associerad med en grupp, ärver malluppgiften följande inställningar från gruppens uppgiftsinställningar:

* Typ av varaktighet
* Intäktstyp
* Kostnadstyp

Tidigare har projektmallar och projektmallsuppgifter ärvt dessa inställningar från projekt- och uppgiftsinställningarna som angetts på systemnivå.

Om du skapar en mall- eller malluppgift utan en grupp, till exempel från sidan Huvudmallar, ärvs inställningarna ovan från projekt- och uppgiftsinställningarna på systemnivå. Om du senare tilldelar en grupp till mallen eller malluppgiften påverkas den inte av gruppens inställningar.

Mer information finns i avsnittet Använda inställningar för mallar och malluppgifter i artikeln [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Nytt för administratörer: Ta reda på vilka anpassade formulär som använder ett anpassat fält

Nu är det enklare att ändra ett anpassat fält i ett anpassat formulär. Med ett enda klick i det anpassade formuläret kan du ta reda på mer om andra anpassade formulär som också använder fältet. Det är viktigt att du kontrollerar om dessa formulär behöver justeras för att de ska fortsätta fungera korrekt när du har gjort ändringen.

Mer information finns i [Visa alla anpassade formulär som använder ett visst anpassat fält eller en viss widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Nytt för gruppadministratörer: Låsa och låsa upp projekt-, uppgifts- och utgivningsinställningar för en grupp

Nu kan du se till att alla i undergrupperna under gruppen använder samma inställningar eller låta dem konfigurera en inställning för sina unika arbetsflöden.

* När en Workfront-administratör har låst upp en inställning på systemnivå kan du konfigurera och sedan låsa den för alla undergrupper under gruppen. Även om du fortfarande kan konfigurera om den låsta inställningen kan inte administratörer av undergrupper göra det för sina grupper.

   Omvänt kan du låsa upp en inställning för gruppen. Detta gör att undergruppsadministratörer kan konfigurera den för sina användares unika arbetsflödesbehov för projekt, uppgifter eller utgåvor.

   Mer information finns i [Låsa eller låsa upp ett projekt, en uppgift eller en utleverans för undergrupper](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Om du är Workfront-administratör behöver du inte gå till gruppområdet för att konfigurera en undergrupps inställningar. Under Projektinställningar, Åtgärder och ärenden, eller Inställningar för tidrapporter och timmar, kan du använda sökrutan längst upp på sidan för att hitta undergruppen och konfigurera dess inställningar.

   Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Nytt för gruppadministratörer: Skapa och redigera mallar från området Grupper

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Workfront-upplevelsen.

Vi fortsätter att göra det enklare att hantera dina grupper och tillhörande objekt på ett och samma ställe. Nu kan du visa och arbeta med en grupps mallar från området Grupper i Konfigurera. På så sätt slipper du gå till mallområdet för att hantera en grupps mallar. Listan med gruppmallar som du arbetar med hålls åtskild från övriga i systemet.

Mer information finns i [Skapa och ändra en grupps projektmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Ange och spara information i ett bifogat anpassat formulär i taget

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Nu är det enklare att ange information i detaljavsnittet för ett objekt: Skriv och spara information i ett enda anpassat fält eller utökningsbart område (t.ex. Översikt och Ekonomi), även om obligatoriska fält i andra anpassade formulär på objektet ännu inte är ifyllda.

Tidigare när du angav information i ett anpassat formulär eller utökningsbart område för ett objekt, gick alla anpassade formulär som var kopplade till objektet in i redigeringsläge och alla obligatoriska fält för dem måste fyllas i innan du kunde spara ändringarna. Detta var ett problem om du inte kunde fylla i ett obligatoriskt fält eftersom det var avsett för en annan användare.

Om du vill redigera alla anpassade formulär och utökningsbara områden i detaljavsnittet för ett objekt kan du klicka på Redigera alla på den nya Redigera-menyn som vi lade till i redigeringsikonen. Du kan också klicka på ett namn på samma meny för att bläddra till det anpassade formuläret eller avsnittet där du vill göra ändringarna

>[!NOTE]
>
>Den här funktionen släpptes ursprungligen för förhandsgranskning i version 21.3.

För att göra det enklare för alla nivåer i en organisation att hantera och styra sina arbetsflöden oberoende av varandra har vi introducerat möjligheten att skapa och hantera statusar för undergrupper. Från avsnittet Grupper i Setup kan du nu göra följande för grupper som du administrerar på alla nivåer:

* Skapa, redigera, ta bort och dölja en status för en grupp
* Lås en status för en grupp så att alla undre undergrupper kan använda den på samma sätt
* Lås upp en status för en grupp så att administratörer av undergrupper kan anpassa den efter deras unika behov
* Ange en gruppstatus som standardstatus
* Ändra ordning på och dölja visningen av gruppstatus för objekt

Workfront-administratörer kan även göra detta (för alla grupper).

Tidigare var den här funktionen bara tillgänglig för grupper på den översta nivån.

Mer information finns i [Hantera gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Nytt för Workfront-administratörer: Migrera layoutmallar från Workfront Classic till den nya Workfront-upplevelsen på egen hand

>[!NOTE]
>
>Den här funktionen släpptes till förhandsvisningsmiljön den 1 juli 2021. Den kommer att släppas ut i produktionsmiljön den 15 juli 2021.

För att hjälpa dig att hantera layoutmallar medan användarna växlar till den nya Workfront-upplevelsen har vi skapat en knapp som du kan använda för att migrera layoutmallar från Workfront Classic till den nya upplevelsen utan att behöva använda Workfront kundsupport.

Tidigare var det bara Workfront kundsupport som kunde migrera dina layoutmallar från Workfront Classic till den nya Workfront-upplevelsen.

## När du associerar en mall med en grupp väljer du en process för gruppgodkännande i Köinformation och Köämnen

Vi har lagt till ett nytt alternativ i processen att koppla en mall till en grupp. Nu kan du välja gruppspecifika godkännandeprocesser för problem i mallens köinformation eller i något av dess köämnen.

I 21.3, när vi lade till möjligheten att associera en gruppmall med en grupp, kan du välja en gruppspecifik godkännandeprocess i mallen, men det kan du inte göra i mallens köinformation eller köämnen.

Mer information finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
