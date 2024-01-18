---
title: 2.1 Förbättringar av administratören
description: 2.1 Förbättringar av administratören
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 2.1 Förbättringar av administratören

Den här sidan beskriver alla administratörsförbättringar som gjorts i version 2.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

veckan 17 januari 2022.

En lista över alla ändringar som är tillgängliga i version 2.1 finns i [2.1 Versionsöversikt](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Dokumenthämtningar som är loggade i uppdateringsområdet

För att hjälpa dina användare att spåra nedladdningar av dokument som de lagrar i Workfront loggar systemet nu in i uppdateringsområdet för ett dokument när någon laddar ned det.

>[!NOTE]
>
>Vi rekommenderar att du testar den här funktionen i Förhandsgranska för ett nyligen överfört dokument.

Information om hur Workfront loggar automatiska uppdateringar av objekt finns i [Systemspårade uppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Bevilja åtkomst för team med åtkomstnivåer

Ett nytt avsnitt i området Åtkomstnivåer ger dig mer detaljerade kontroller för att hantera användarnas åtkomst till team. Nu kan du avgöra vilka som kan skapa, redigera och visa team.

Detta ändrar inte användarnas befintliga åtkomst till team.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Gruppmappning finns nu i utkast

Vissa utkast innehåller nu grupper som du kan anpassa innan du installerar ritningen. Du kan mappa en grupp i planen till en befintlig grupp i din Workfront-instans eller skapa en ny grupp om det behövs.

Mer information finns i [Konfigurera en plan](../../../administration-and-setup/blueprints/configure-template-package.md).

## Formatuppdateringar i området Anpassade Forms

Området Anpassade Forms har en ny stil och känsla som gör den uppdaterad med många andra områden i den nya Workfront-upplevelsen.

Mer information om hur du skapar ett anpassat formulär finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Många förbättringar för att skapa beräknade anpassade fält

Det är nu mycket enklare att skapa beräknade anpassade fält med dessa tillägg i den nya beräkningsredigeraren:

* Du kan hovra över vilket uttryck som helst i beräkningen för att visa information om det, inklusive en beskrivning, ett exempel på hur det kan användas och en länk till mer information i en hjälpartikeln.
* Varje uttryck som du lägger till är färgkodat, beroende på vilken typ det är. Det gör det enklare att identifiera dina uttryck och omedelbart identifiera deras typ.
* Med radnummer kan du identifiera och referera till funktioner i en lång beräkning.
* När du börjar skriva ett uttryck eller fältnamn visas en lista med tillgängliga objekt så att du kan välja det du vill använda. När du skriver en öppen parentes läggs den avslutande parentesen till automatiskt.
* Du kan förhandsgranska resultatet av beräkningen med ett befintligt objekt utan att lämna beräkningsredigeraren.

I den anpassningsbara hovringstexten &quot;Instruktioner&quot; för ett beräknat anpassat fält kan du visa eller dölja fältets formel. Detta är användbart om du tror att de användare som ska fylla i det anpassade formuläret inte kommer att behöva den informationen.

Mer information om hur du skapar ett beräknat anpassat fält finns i [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Visa granskningsloggsinformation om status och företag

Nu kan du enklare felsöka incidenter som rör status och företag genom att visa information om dem i området Granskningsloggar under Konfigurera.

Exempel:

* Du kan ta reda på vem som har bytt namn, låst eller gömt en status och när de gjorde det.
* Du kan ta reda på vem som har tagit bort några medlemmar eller jobbroller från ett företag, och när de gjorde det.

Mer information om hur du visar granskningsloggsinformation finns i [Visa och exportera granskningsloggar](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Företagsmappning med utkast och andra förbättringar

Följande förbättringar av utkast är nu tillgängliga:

* Vissa ritningar innehåller nu företag som du kan anpassa innan du installerar ritningen. Du kan mappa ett företag i planen till ett befintligt företag i din Workfront-instans eller skapa ett nytt företag om det behövs.
* Nu finns en ny ritningstyp, Organisationsstruktur. Vissa utkast innehåller element från flera typer (till exempel Projektmall och Organisationsstruktur). Du kan filtrera med hjälp av en ritningstyp på katalogsidan.
* Avsnitten Installera inställningar och Mallägande på konfigurationssidan har kombinerats till Mallinställningar för att bli enklare.

Mer information finns i [Konfigurera en plan](../../../administration-and-setup/blueprints/configure-template-package.md).

## Hantera företagsmedlemskap enklare

I området Företag gör ett uppdaterat verktygsfält det enkelt att lägga till befintliga Workfront-användare i ett företag och att ta bort företagsmedlemmar.

Tidigare var dessa åtgärder bara tillgängliga i rutan Redigera företag.

Det uppdaterade verktygsfältet innehåller även alla åtgärder som var tillgängliga i det föregående verktygsfältet, t.ex. redigering av medlemmarnas användarprofilinformation och inaktivering av dem i systemet.

Mer information finns i [Hantera företagsmedlemskap](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Välj uttryck och fält i det nya fönstret för beräkningsfält

Vi fortsätter att göra det enklare att skapa ett beräknat fält i en anpassad form. När du klickar på Maximera för att öppna den nya beräkningsredigeraren kan du nu hitta och välja de uttryck och fält som du behöver.

Mer information finns i [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Grupper kan konfigurera sina egna inställningar för tidrapport och timma

>[!NOTE]
>
>Den här funktionen var ursprungligen endast tillgänglig som en del av en fasad lansering för kunder i kluster 4 som en del av version 21.4. Den här funktionen kommer att vara tillgänglig för alla återstående kluster i produktion den 8 november 2021.

I en stor organisation kan vissa grupper behöva konfigurera tidrapport- och timinställningar separat för att passa sina unika arbetsflöden, i stället för att ärva inställningarna som konfigurerats av en administratör på systemnivå. Nu kan Workfront-administratörer låsa upp en tidrapport och timinställning för alla grupper i systemet så att de själva kan konfigurera den.

Den här funktionen lades också till nyligen för projektinställningar och för inställningar för uppgifter och utgåvor.

Mer information om hur en Workfront-administratör låser upp en tidrapport och timinställning finns i avsnittet [Lås upp tidrapport och timinställningar för grupper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) i artikeln [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Mer information om hur en gruppadministratör konfigurerar olåsta uppgifter och utfärdar inställningar för en grupp finns i [Konfigurera tidrapport och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Välj flera meddelanden som du vill låsa upp eller låsa upp för grupper

Det är nu snabbare och enklare att låsa upp eller låsa upp e-postmeddelanden för grupper. Nu kan du välja flera meddelanden, kontrollera dina val för att se till att de är korrekta och sedan klicka på den nya knappen Lås upp eller Lås som visas i verktygsfältet.

Tidigare var du tvungen att låsa upp och låsa upp meddelanden igen en i taget. Workfront har för närvarande 95 meddelanden, så det här tog en stund om du var tvungen att göra det för alla eller många av dem.

Mer information finns i [Lås upp eller lås konfigurationen av händelsemeddelanden för alla grupper](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## För gruppadministratörer: Det är enklare att välja en ersättningsgrupp när du tar bort en grupp

När du tar bort en grupp är det två förbättringar i rutan Ta bort grupp som gör det enklare att markera den ersättningsgrupp som du vill behålla den borttagna gruppens användare, arbetsobjekt och undergrupper:

* Du kan börja skriva namnet på gruppen för att snabbt hitta den. Tidigare fanns det bara en nedrullningsbar lista som du inte kunde skriva in. Detta var ett problem för organisationer med många grupper eftersom du var tvungen att bläddra igenom listan för att hitta den grupp du ville ha. Listrutan hade också en objektgräns, så det var möjligt att den önskade gruppen inte visades.
* Du kan använda den nya informationsikonen för att kontrollera att du väljer den ersättningsgrupp du vill använda. När du hovrar över ikonen visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför den och namnen på dess administratörer.

Mer information finns i [Ta bort en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Större yta för att skapa beräknade fält

Nu är det enklare att skapa komplexa beräkningsfält i ett anpassat formulär. Klicka på knappen Maximera för att öppna ett stort redigeringsfönster där du kan skapa beräkningen. När du är klar klickar du på Minimera för att fortsätta arbeta med det anpassade formuläret.

Mer information finns i [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Lägga till anpassade formulär i grupper

Anpassade formulär stöds nu för Group-objektet. Detta gör det enklare för grupper i organisationen att samla in och dela information som passar deras specifika behov och arbetsflöden. Användare kan göra följande för en grupp på samma sätt som för andra Workfront-objekt:

* Skapa ett anpassat formulär
* Bifoga ett eget formulär
* Spara anpassade formulärdata
* Ta bort ett anpassat formulär
* Redigera anpassade data från listor och, i den nya Workfront-upplevelsen, från gruppsidan

Mer information om anpassade formulär finns i [Egna formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Skapa OAuth2-appar för att integrera program med Workfront

Nu kan du integrera Workfront med andra program som Workfront inte erbjuder någon inbyggd integrering för. Genom att skapa en OAuth2-app för programmet som du vill integrera med kan du ge programmet åtkomst till Workfront, samtidigt som du vet att dina data skyddas av det säkra, branschledande OAuth2-autentiseringsprotokollet.

Tidigare kunde du bara integrera med andra program via inbyggda integreringar, Workfront Fusion eller Workfront API.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Förbättrat gränssnitt i företagsområdet

I området Företag i installationsprogrammet är det enklare att hantera företagsmedlemskap att använda nya bekräftelsemeddelanden och smärre ändringar av ordalydelsen. Avsnittsnamnet&quot;Personer&quot; i den vänstra panelen är nu&quot;Företagsmedlemmar&quot;.

Mer information om hur du hanterar företagsmedlemskap finns i [Hantera företagsmedlemskap](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
