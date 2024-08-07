---
content-type: reference
navigation-topic: betas
title: 'Reporting Canvas beta: översikt'
description: Information om betaprogrammet för det kommande verktyget Reporting Canvas för Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
hide: true
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 0%

---

# Betaversion av arbetsyta för rapportering: översikt

## Arbetsyta för rapportering

Den nya rapportfunktionen i Workfront är under utveckling. När vi utformade Reporting Canvas har vi arbetat hårt med att skapa en upplevelse som ger maximal flexibilitet i kombination med en intuitiv, modulär design, så att användare som du på bästa sätt kan utnyttja dina egna data när de skapar och delar rapporter. Tack vare en ny, enhetlig rapporttyp som gör att du kan dra och släppa nästan alla element på en obegränsad arbetsyta blir det snart enklare än någonsin att skapa ett visuellt datamasterverk.

Den här artikeln innehåller information om den aktuella privata betaversionen, som är begränsad till specifika kunder. Nya rapportfunktioner för arbetsytan distribueras nu via Canvas Dashboards. Mer information finns i **Utvecklingsplan** nedan.

### Utvecklingsplan

Vi är i slutskedet när det gäller att lösa ett problem med datakvalitet som vi observerade tidigt i betaversionen av Reporting Canvas. Vi kommer snart att återuppta arbetet med att ta fram nya visualiseringar, utvidga urvalet av rapporteringspliktiga Workfront-objekt och förbättra upplevelserna av att skapa och distribuera rapporter, som alla är viktiga för att förverkliga våra mål för Rapportera arbetsyta.

Vi kommer att leverera dessa nya upplevelser stegvis, från och med version 23.2, via den nya sidan Canvas Dashboards som nu är tillgänglig i din förhandsvisningsmiljö. På arbetsytans kontrollpaneler kan du visa befintliga rapporter tillsammans med de nya rapporteringsfunktionerna som vi håller på att skapa, och de kommer att fungera som vår primära miljö för driftsättning och testning av nya funktioner för Reporting Canvas. Mer information om hur du aktiverar och använder arbetsytans kontrollpaneler finns i [Översikt över arbetsytans kontrollpaneler](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Delta i betaversionen

>[!IMPORTANT]
>
>Betaversionsinformationen nedan är till för administratörer som redan har inkluderats i betaversionen av Reporting Canvas, som inte längre accepterar nya deltagare. Om du vill testa de nya funktionerna i Rapportera arbetsyta när de läggs till kan du läsa **Utvecklingsplan** ovan för information om hur du aktiverar Canvas-instrumentpaneler.

### Tillgänglighet

Betaversionen av Reporting Canvas är tillgänglig för alla organisationer på AWS, oavsett region.

### Gå med i betaversionen

Betaversionen av Reporting Canvas är helt valfri, men kan bara väljas av en Workfront-administratör. Så här väljer du systemadministratör:

1. Välj ikonen **Rapportering (beta)** på huvudmenyn för din Workfront-instans.
1. Klicka på **Acceptera** för att acceptera villkoren.
1. Tillåt att organisationens data läggs till i rapportarbetsytan (detta kan ta upp till några timmar).
1. Börja använda Rapportera arbetsyta.

När data har lagts till i Rapporteringsarbetsyta kan andra systemadministratörer välja att gå med på individuell basis på samma sätt (utan att vänta på att data ska läggas till igen).

Så här väljer du andra användare som inte är Workfront-administratörer:

1. Välj ikonen **Rapportering (beta)** på huvudmenyn för din Workfront-instans.
1. Klicka på **Rapportera arbetsytebehörigheter**.
1. Sök efter och välj de användare du vill delta i.

   >[!IMPORTANT]
   >
   >Användare som du ger åtkomst till Reporting Canvas får tillgång till **alla**-data i systemet i skrivskyddad kapacitet, oavsett deras standardbehörigheter för att visa dessa data.

1. Klicka på **Spara**.
1. Lägg till ikonen **Rapportering (beta)** i huvudlayoutmallen för varje användare som har valts. Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Varje användare måste sedan navigera individuellt till ikonen **Rapportering (beta)** på huvudmenyn och acceptera villkoren.

### Skicka feedback

Så här skickar du feedback om betaversionen:

1. Klicka på knappen **Skicka feedback** när du är i Reporting Canvas i Workfront.
1. Fyll i formuläret och klicka sedan på **Skicka**.

## BETA FAQ

+++Kan jag migrera mina äldre rapporter till Reporting Canvas?

Sammanfattningsvis är migrering av äldre rapporter inte tillgängligt under betaversionen. Det är dock en planerad funktion (med några kavattar som beskrivs nedan) för den officiella lanseringen.

Hindringen att skapa nya rapporter har minskat avsevärt med Reporting Canvas, men vi förstår att det går snabbare att ta över några av dina befintliga rapporter och kontrollpaneler. Därför vill vi tillhandahålla de verktyg och resurser som behövs för att säkerställa att du kan ta över alla relevanta äldre objekt så att du kan börja till höger i Rapportera arbetsyta. Eftersom Reporting Canvas är en så genomgripande förändring av hur den aktuella rapporteringen fungerar skulle det dock vara omöjligt att migrera alla rapporter och kontrollpaneler precis som i dag.

Vår nuvarande strategi för migrering i den officiella versionen är att göra följande:

1. Identifiera relevanta rapporter och instrumentpaneler

   1. Ge dig möjlighet att exportera en CSV-fil med alla rapporter och kontrollpaneler i systemet tillsammans med relevant spårningsinformation (antal vyer, när och av vem).
   1. Exportera rapporter som har konfigurerats med schemalagda leveranser tillsammans med mottagarna.

1. Markera de rapporter och instrumentpaneler som du vill migrera och klicka sedan på **Migrera**

   Det här är en enkelriktad migrering. Den skapar en kopia av de markerade rapporterna och kontrollpanelerna till Rapporteringsarbetsyta och lämnar den äldre rapporten eller kontrollpanelen oförändrad i det aktuella rapportverktyget.

   Du kan migrera samma rapport eller kontrollpanel så många gånger du vill.

1. I Rapportera arbetsyta kontrollerar du att alla rapporter och instrumentpaneler som du har valt har migrerats.
+++

+++Varför kan jag inte se alla objekt jag normalt gör?

För att kunna ge våra kunder betaversionen så tidigt som möjligt har vi bara släppt den med en delmängd av de många objekttyper som finns i Workfront idag. Nedan finns de objekttyper som stöds i betaversionen:

* Tilldelning
* Dokument
* Godkännande av dokument
* Utgift
* Timme
* Problem
* Anteckning
* Portfolio
* Projekt
* Program
* Uppgift
* Tidrapport
* Arbetsobjekt
+++

+++Om något går fel i Reporting Canvas under betatestningen, kommer data från min organisation att påverkas?

Nej. Betaversionen använder en kopia av organisationens data som fylls i i Reporting Canvas. Detta innebär att du kan experimentera under betaversionen utan risk för att påverka viktiga data, men det innebär också att redigering online av data i Reporting Canvas inte är tillgängligt förrän den officiella starten.
+++

+++Kan jag avanmäla mig från betaversionen när jag väl har gått med?

En Workfront-administratör kan inte avanmäla sig från betaversionen, men andra administratörer kan tas bort genom att göra följande:

1. Logga in som systemadministratör.
1. Navigera till Rapporteringsarbetsyta.
1. Klicka på Rapportera arbetsyta **behörigheter**.
1. Ta bort de användare som du vill avanmäla från betaversionen från listan som har valts in.
1. Klicka på **Spara**.
+++
