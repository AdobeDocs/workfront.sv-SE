---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 4
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i R1.4-versionen. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 15 februari 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1 Preview 4

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i R1.4-versionen. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 15 februari 2017.

En lista över alla ändringar som gjorts i R1 finns i [Workfront R1-utgåvan](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Uppdaterade projekt-, uppgifts- och godkännandeprocesser

När du skapar godkännandeprocesser för projekt-, uppgifts- och godkännandeprocesser är följande förbättringar och ändringar nu tillgängliga: 

* Godkännandet&quot;Steg&quot; kallas nu för godkännande&quot;Steg&quot;.
* Inkludera flera typer av godkännare per fas.\
  Detta inkluderar användare, team och jobbroller.\
  Före den här ändringen kan du endast inkludera flera godkännare av samma typ. Du kan till exempel inkludera flera jobbroller, men inte en jobbroll och ett team.

* Följande begränsningar som tidigare fanns för att ändra befintliga globala godkännandeprocesser har tagits bort:

   * Den ändrade godkännandeprocessen återspeglas endast på objekt i hela systemet där godkännandeprocessen antingen inte har startats än eller där godkännandeprocessen inte har ändrats. Objekt där godkännandeprocessen redan har startats eller där godkännandeprocessen har ändrats uppdateras inte med dina ändringar.
   * Du kan inte ändra den status som bestämmer när godkännandet startar.

* Uppdaterat utseende och känsla.

Mer information om hur du skapar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

När du kopplar en godkännandeprocess till ett projekt, en uppgift eller ett ärende finns nu följande förbättringar och ändringar:

* Uppdaterat utseende och känsla.
* Godkännandediagrammet visas på fliken Godkännanden och visar en visuell representation av föregående, aktuella och framtida steg för godkännande.

Mer information om hur du associerar godkännanden med projekt, uppgifter och ärenden finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Ändra status för ett projekt direkt från projektsidan

Du behöver inte längre redigera ett projekt för att kunna ändra projektstatus. Du kan nu ändra status för ett projekt direkt från projektets huvudsida.

Mer information finns i [Ändra status för ett projekt](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Schemalägg användare för inaktivering

Du kan nu schemalägga användare att inaktiveras vid ett framtida datum.

Före den här förbättringen kunde du bara inaktivera en användare manuellt direkt.

Att schemalägga en användare som ska inaktiveras kan vara användbart i många olika scenarier. Om du till exempel skapar användare i Workfront som tillfälligt anställs kan du konfigurera dem så att de inaktiveras när deras kontrakt upphör.

Den här funktionen är även tillgänglig när användare gruppredigeras. 

Mer information om schemaläggning av användare för inaktivering finns i [Inaktivera eller återaktivera en användare](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) och [Lägg till användare](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nya alternativ för e-postsammandrag för&quot;Åtgärder krävs&quot;

Leveransalternativet Daglig sammandrag är nu tillgängligt i området Åtgärd krävs i meddelandeinställningarna.

Mer information finns i [Ändra dina egna e-postmeddelanden](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Kom ihåg att uppdatera e-postadressen som är kopplad till ditt konto för att kunna testa den här funktionen. Detta är obligatoriskt eftersom förhandsvisningssandlådan rensar e-postadresserna för alla användare.

## Förbättring av papperskorgen: Inspelat i uppdateringsströmmen och Ta emot e-postmeddelande

Följande förbättringar lades till vid återställning av borttagna projekt, uppgifter och problem:

* Du får nu ett e-postmeddelande när du har återställt ett objekt.\
  Som Workfront-administratör får du nu ett e-postmeddelande när du har återställt ett projekt, en uppgift eller ett problem som tidigare har tagits bort. Du får ett e-postmeddelande med information om återställningsprocessens status.\
  Mer information om hur du återställer objekt i Workfront finns i [Återställa borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* När objektet återställs registreras borttagningen och återställningen av objektet i objektets uppdateringsström och i det överordnade objektets uppdateringsström.\
  Tidigare spelades endast borttagningen in i det överordnade objektets uppdateringsström.\
  När uppgiften återställs läggs till exempel ett meddelande till i uppdateringsströmmen för både projektet och själva aktiviteten, vilket anger att uppgiften återställdes. (Borttagningar och återställningar registreras inte för underaktiviteter. Information om borttagning och återställning av underaktiviteter är bara tillgänglig för överordnade uppgifter.)\
  Mer information finns i [Återställ borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Uppdaterad dialogruta för hantering av gruppmedlemskap

Det finns ett nytt gränssnitt för hantering av grupper och undergrupper som ger en enklare och mer användarvänlig upplevelse.

Fältet Gruppägare och fältet Gruppmedlemmar kombineras nu till ett enda fält med en lista över gruppmedlemmar som listas nedan. Dessutom kan du filtrera listan med gruppmedlemmar och ändra om de är ägare eller medlem. 

Mer information om hur du lägger till undergrupper i grupper samt anger användare som medlemmar eller gruppägare i grupper finns i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) och [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Kopiera text i mobilappen

Du kan kopiera text i följande fält för alla objekt som är synliga i mobilappen:

* Namn
* Beskrivning
* Referensnummer
* Kommentar

Den här funktionaliteten bör lanseras i både iOS- och Android-appbutikerna den 13 februari.
