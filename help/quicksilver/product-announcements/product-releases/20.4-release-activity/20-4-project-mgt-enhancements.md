---
title: 20.4 Förbättrad projektledning
description: 20.4 Förbättrad projektledning
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 66659813798d330bb441b32c692693b54d4cfad6
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 0%

---

# 20.4 Förbättrad projektledning

Den här sidan beskriver alla projekthanteringsförbättringar som gjorts i version 20.4 till förhandsvisningsmiljön. Dessa förbättringar kommer att bli tillgängliga i produktionsmiljön den 9 november 2020.

En lista över alla ändringar som är tillgängliga i version 20.4 finns i [20.4 versionsöversikt](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nytt för administratörer: Styr hur ett anpassat fält delas

För att du ska få större kontroll över vem som kan redigera, ta bort och använda anpassade fält som du skapar har vi lagt till möjligheten att konfigurera exakt hur du vill att de ska delas.

Fram tills nu, när du skapade ett anpassat fält, var det redigerbart av alla i systemet. Detta är fortfarande standardtillståndet för ett anpassat fält, men nu kan du begränsa delningen av ett anpassat fält till vissa användare, roller, team, grupper och företag. Och du kan avgöra om mottagarna kan hantera eller bara visa det anpassade fältet.

För att göra den här upplevelsen bekant för dig har vi utformat användargränssnittet för den här funktionen så att det liknar andra objektområden som delas i Workfront.

## Nytt för administratörer: Standardanpassad formulärdelning

Vi har standardiserat delning för anpassade Forms så att du kan använda samma Workfront-process för objektdelning som du redan känner till. Och den nya delningsfunktionen ger dig större kontroll över vem som kan redigera, ta bort och använda anpassade Forms som du skapar. Du kan begränsa delning för ett anpassat formulär till vissa användare, roller, team, grupper och företag. Du kan även avgöra om mottagarna kan visa eller hantera det anpassade formuläret.

Mer information finns i [Dela ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportera anpassade formulär och översiktsinformation från detaljavsnittet för ett projekt, en uppgift eller ett ärende

Nu kan du exportera den anpassade formulärinformationen till en PDF-fil. Du kan exportera anpassade formulär från projekt, uppgifter eller utgåvor när du öppnar formuläret i objektets detaljavsnitt.

Förutom att exportera anpassade former av projekt, uppgifter och utgåvor kan du nu även inkludera området Översikt i den exporterade PDF-filen.

Mer information om hur du exporterar anpassade formulär från ett objekt finns i [Exportera anpassade formulär och objektinformation](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Lägg snabbt till en upprepning

>[!NOTE]
>
>Den här funktionen har tillfälligt tagits bort från produktionsmiljön. Den här sidan uppdateras när funktionen blir tillgänglig.

För att förenkla upplevelsen av att skapa en iteration har vi lagt till en ny knapp som gör att du kan lägga till en iteration från fliken iterationer. Här kan du skapa en iteration och sedan lägga till uppgifter och problem senare.

Du kan fortfarande skapa en iteration på eftersläpningstaggen som tidigare.

Mer information finns i [Skapa en iteration](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nytt metadataavsnitt som är tillgängligt i projekt

För att spara tid och öka förståelsen för ett projekts övergripande hälsa finns det nu ett metrisk avsnitt i ett projekt som innehåller information om följande:

* Fullständigt, ofullständigt, försenat och kommande arbete
* Aktivitets- och utleveransbelopp grupperade efter status eller prioritet
* Arbetsinsats som tilldelats varje användare

Du kan göra markeringar i diagrammen för att visa olika aspekter av uppgifter och problem i ett projekt och klicka på vissa element för att visa aktivitetsinformation.

<!--This feature is now included in the [Planner Fundamentals, Part 3 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) on Workfront One. -->

## Nytt för administratörer: Tilldela en företagsledare till en grupp

För att du bättre ska kunna organisera och definiera dina grupper har vi lagt till möjligheten att utse en användare till affärsledare för en grupp (eller undergrupp). En företagsledare är en Workfront-användare som fattar affärsbeslut för en grupp.

Det nya fältet Business Leader kan användas i rapportfilter, vyer och grupperingar. Du kan t.ex. filtrera efter en viss affärsledare för att endast visa de grupper som personen har tilldelats i den rollen.

Mer information finns i [Översikt över företagsledare](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Den här funktionen ingår nu i [Administratörsgrunderna, del 1 utbildningsväg](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) på Workfront One.

## Nytt för administratörer: Associera portföljer, program och företag med grupper

När Workfront-administratörer skapar eller redigerar en portfölj, ett program eller ett företag kan de tilldela den till en grupp. Med grupper tilldelade till dessa objekt är det enkelt att identifiera gruppens ansvar för dem.

Du kan t.ex. lista alla organisationens portföljer i en rapport och titta i kolumnen Grupp för att se vilka som din grupp arbetar med.

Mer information finns i avsnittet Om att associera en grupp med ett objekt i artikeln [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Den här funktionen ingår nu i [Administratörsgrunderna, del 1 utbildningsväg](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) på Workfront One.

## Nytt för administratörer: Administratörer för en grupp som tilldelats ett företag kan hantera företaget

Vi har gjort det enkelt för en gruppadministratör att hantera ett företag som är kopplat till sin grupp i Workfront. Åtkomst att hantera företaget är automatiskt tillgänglig när associationen görs. Detta är särskilt viktigt när gruppadministratören inte har administrativ åtkomst till företag.

Mer information finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Mer information om administrativ åtkomst till företag finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Den här funktionen ingår nu i [Administratörsgrunderna, del 1 utbildningsväg](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) på Workfront One.

## Ersätta knappen Work On It (Arbeta på) med en Start-knapp

För att hjälpa till att hämta det datum och den tid då arbetet faktiskt startar på en arbetsuppgift kan användare ersätta knappen Arbeta på den med knappen Start som automatiskt uppdaterar arbetsuppgiftens status och faktiska startdatum.

Uppdaterades den 24 september: När du klickat på Starta uppgift eller Starta utgåva kan du nu välja att återställa ditt val och ange att du kanske inte är redo att börja arbeta med en arbetsuppgift genom att klicka på Ångra. Arbetsuppgiften återgår till statusen Nytt och datumet för implementering och det faktiska startdatumet tas bort. Alternativet Ångra visas mycket kort och tas bort när du navigerar bort från eller uppdaterar sidan.

Mer information om hur du konfigurerar det här alternativet finns i [Ersätt knappen Arbeta på med en Start-knapp](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Den här funktionen ingår nu i [Grundläggande kursväg för arbetare](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) och [Grundläggande för administratörer, del 1 utbildningsväg](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) på Workfront One.

## Tillåt flera utkast för ett köämne

För att du ska få större frihet när du arbetar med begäranden finns det inte längre någon gräns för hur många utkast du kan spara för ett köämne. När du skapar en ny begäran kan du välja ett befintligt utkast från en lista med utkast för samma köämne, skriva över det och skicka det som en ny begäran eller skapa en ny begäran från början.

Före den här förbättringen sparade Workfront endast ett utkast för varje köämne i din begärandekö.

Mer information om hur du skickar begäranden finns i [Skapa och skicka Workfront-begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Tilldela en grupp till ett team

För att göra det enklare att hantera och rapportera om de team som är kopplade till en grupp kan du nu tilldela vilken grupp som helst till ett team som du har tillgång till för redigering.

När du tilldelar ett team till en grupp kan dess gruppadministratörer hantera teamet utan att vara medlem i det. På sidan Teaminformation kan de se vilka team som har tilldelats till de grupper som de hanterar. Och de kan köra en rapport för att lista alla team som är kopplade till en viss grupp.

Mer information finns i [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Den här funktionen ingår nu i [Administratörsgrunderna, del 1 utbildningsväg](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) på Workfront One.

## Med nya fält kan du rapportera data för en grupp på den översta nivån och alla dess undergrupper

För att du lättare ska kunna identifiera data som är kopplade till en grupp på den översta nivån och dess undergrupper har vi lagt till ett nytt fält för överordnat ID som du kan använda i Filter, Vyer och grupperingar när du skapar rapporter om gruppobjekt.

Det här fältet bör vara särskilt användbart för gruppadministratörer som hanterar grupper som innehåller flera undergrupper.

Tänk dig att ni hanterar en grupp som heter Marknadsföring och som har undergrupperna Field Marketing och Digital Marketing. Du kan lista projekt som tillhör alla tre grupperna genom att skapa ett projektområdesfilter med följande filterregel:
<pre>Grupp: Överordnat namn &gt; Lika &gt; Marknadsföring</pre>Vi har också lagt till ett nytt fält för överordnat namn som du kan använda för att identifiera data som är kopplade till grupper på den översta nivån i vyer (inte i filter eller grupperingar).

Mer information om hur du använder fält i listor och rapporter finns i [Ordlista för Adobe Workfront-terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nytt alternativ för att avbryta åtgärden när ett utkast av en begäran ignoreras

När du tar bort ett sparat utkast kan du nu klicka på Avbryt på bekräftelsemeddelandet som informerar dig om att utkastet kommer att tas bort. På så sätt förlorar du inte utkastet om du skulle ångra dig.

Den här funktionen är bara tillgänglig i den nya Workfront-upplevelsen. Mer information finns i [Skapa och skicka Workfront-begäranden](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

