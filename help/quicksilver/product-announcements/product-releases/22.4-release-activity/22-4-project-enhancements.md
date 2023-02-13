---
title: 2.4 Projektförbättringar
description: 2.4 Projektförbättringar
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 2.4 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 22.4 till förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga den 3 oktober 2022.

En lista över alla ändringar som är tillgängliga i version 22.4 finns i [22.4 Versionsöversikt](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Nu finns information om föregående

Om du vill visa information om en uppgifts föregångare kan du nu hålla muspekaren över föregående nummer i kolumnen Föregående. I informationsrutan visas föregående aktivitet och projekt som refereras, planerade start- och slutdatum för föregående aktivitet samt antalet föregående aktiviteter och efterföljande aktiviteter. Du kan expandera projektinformationen om du vill ha mer information om projektet. Ytterligare information finns för projektövergripande föregångare.

Mer information finns i [Skapa en föregående relation i uppgiftslistan](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Tilldela flera team till en uppgift eller ett ärende

För att du ska kunna hantera uppgifter och ärenden på ett mycket flexiblare sätt har vi gjort det möjligt att tilldela flera team till en uppgift eller ett problem. Tidigare kunde bara ett team tilldelas en uppgift eller ett problem.

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i Utjämning av arbetsbelastning i Teams-området.

Mer information finns i [Tilldela uppgifter](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) och [Tilldela ärenden](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Smart användarval för projektroller i områdena Redigera och Detaljer

Vi har förbättrat sättet som användare visas på när du lägger till dem i följande projektfält i rutan Redigera och i avsnittet Detaljer i projektet:

* Projektägare

* Projektsponsorer

* Resurshanteraren

När du nu lägger till en användare i något av dessa fält i områdena Redigera eller Detaljer visas även användarens primära roll och e-postadress, förutom namn och avatar. Detta gör det lättare att skilja mellan flera användare med liknande eller identiska namn.

Mer information finns i [Redigera projekt](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

OBS! Ytterligare användarfält för projekt, uppgifter och utgåvor kommer att uppdateras med den här funktionen i framtida versioner.

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Beräknade datumfält sparas alltid baserat på UTC (Coordinated Universal Time)

Nu kan du vara säker på att alla datumfunktioner i beräkningsfält fungerar på ett konsekvent sätt och ger samma resultat för alla, oavsett hur ett anpassat datauttryck uppdateras eller var användare samarbetar med objektet över hela världen.

Alla beräkningar beräknas och sparas nu med en standard - UTC (Coordinated Universal Time) - inte med de tidszonskonfigurationer som angetts för organisationens instans och din individuella användarprofil. Beräkningar visas emellertid i ett anpassat formulär baserat på varje användares enskilda tidszoner som angetts i webbläsaren.

Tidigare orsakade tidsinställningar i beräkningar förvirring när de varierade i dessa situationer:

* Om någon omberäknade ett beräknat fältuttryck med Uppdatera tidigare beräkningar i formulärbyggaren, bestämdes datumfunktionsresultaten av organisationens UTC-tidszon.

* Om någon redigerade objektet och det gjorde att beräkningsfältuttrycket beräknades om, bestämdes datumfunktionsresultaten av användarens lokala tidszon. Resultat av beräkningsdatumfält i det här scenariot beräknas också baserat på UTC.

Mer information finns i [Arbeta över tidszoner](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Förbättringar av anpassade formulär: Adobe XD och snabbfiltret

Baserat på din feedback har vi introducerat följande förbättringar för att förbättra din upplevelse när du hanterar anpassade formulär:

* Lägg till en Adobe XD-fil för att göra ett anpassat formulär mer visuellt och informativt. När formuläret är kopplat till ett objekt kan användare som arbetar med objektet visa och interagera med den XD filen inifrån formuläret.

   Mer information finns i [Lägga till eller redigera en bild eller en annan resurswidget i ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Använd snabbfiltret för att enkelt hitta objekt i den moderniserade listan med anpassade formulär och fält. Du får också ett bättre utseende och en bättre känsla när du hanterar formulär och fält.

   Mer information om snabbfiltret finns i [Använda snabbfiltret på en lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Allmän betaversion - ny filterupplevelse för projekt, uppgifter och problem

Filtrering av projekt-, uppgifts- och problemlistor har gjorts om så att du snabbt kan skapa och dela filter. Funktioner:

* Ett intuitivt gränssnitt för betaversion som skapar ett nytt filter

* Möjlighet att markera ett filter som en favorit

* Filterstackning (tillämpa fler än ett sparat filter)

* Duplicera filter

* Delningsfilter

* Ta bort filter som delas med dig


Den nya filterupplevelsen finns även i tidrapportlistor och scenarioplaneraren.

Textläget är fortfarande tillgängligt för avancerad filterredigering, och systemadministratörer kan fortfarande tilldela standardfilter till alla användare via layoutmallarna.

### Var finns den här?

* Projekt/uppgifter/Ärendelistor

* Scenarioplan

* Tidrapporter


### Vi vill ha din feedback!

Med denna allmänna betaversion får användarna möjlighet att skicka feedback direkt till teamet som arbetar med filterupplevelsen genom att klicka på knappen för feedback. Vi ser fram emot att få höra av dig och dina användare om den nya filterupplevelsen i betaversionen. Om ditt team vill träffa en produkt direkt för att ge mer feedback kan du planera ett möte här: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Vad kommer härnäst?

* Ny upplevelse av grupperingar och vyer (kallas även kolumner)

   Vi börjar arbeta med den nya upplevelsen för grupperingar och vyer (kallas även kolumner) så att den blir konsekvent med den nya filterupplevelsen och har några av samma bra funktioner som den nya filterupplevelsen.

* Implementera nya filter i andra delar av Adobe Workfront

   Vi kommer att samarbeta med team i hela produkten för att implementera den nya filterupplevelsen inom andra områden i Workfront.


Vi vill leverera värde till er iterativt, så vi kommer att fortsätta leverera när de nya upplevelserna och andra områden är klara. Håll dig uppdaterad och få mer spännande uppdateringar.

Mer information finns i [Översikt över filter i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) och [Skapa eller redigera filter i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Visa en videodemonstration av den här funktionen.](https://video.tv.adobe.com/v/3412391/)
