---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Projektförbättringar
description: Den här sidan beskriver alla ändringar som gjorts i Project-förbättringar i version 2019.3. Den gjordes tillgänglig i produktionsmiljön den 19 augusti 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# 2019.3 Projektförbättringar

Den här sidan beskriver alla ändringar som gjorts i Project-förbättringar i version 2019.3. Den gjordes tillgänglig i produktionsmiljön den 19 augusti 2019.

En lista över alla ändringar som gjorts under 2019.3 finns i [Översikt över versionsaktiviteten för 2019.3 ](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Ändra visningstypen för ett fält i ett anpassat formulär

Nu kan du ändra visningstypen för ett fält i ett anpassat formulär.

Om du t.ex. har skapat ett kryssrutefält kan du ändra det till ett nedrullningsbart fält eller ett alternativknappsfält. Dessa tre fälttyper är utbytbara.

Om du har skapat ett textfält med en rad kan du ändra det till ett textfält med en rad. Dessa två fälttyper är utbytbara.

Tidigare var du tvungen att skapa ett nytt fält och ta bort det gamla för att ändra visningstypen för ett anpassat fält. Detta krävde överföring av data, som ofta var tidskrävande.

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 9 augusti 2019
>
>Produktionstillgänglighet: 30 augusti 2019

## Skapa tid för kalendrar och rapporter

Nu kan du se användarens ledig tid för bättre planering och körning. Du kan också lägga till ny tid med rapporter och kalendrar på kontrollpanelerna för att få en realtidsbild av användarnas tillgänglighet.

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 9 augusti 2019
>
>Produktionstillgänglighet: 30 augusti 2019

## Filtret Öppna visar nu fler resultat i en lista över problem

När du tillämpar filtret Öppna på en lista med problem, innehåller listan problem som:

* Har stängts - väntar på godkännandestatus
* Är associerade med ett matchande objekt

Före den här ändringen togs inte dessa problem med i listan när filtret Öppna användes.

## Ny upplevelse vid infogad redigering av information i listor

När du infogar redigeringsinformation i de nya listorna tonas de rader som har redigerats ned, men informationen visas inte. Före den här ändringen var de redigerade raderna nedtonade och informationen var inte synlig.

De nya listorna finns i följande områden i Workfront:

* Projekt- och uppgiftslistor
* Fliken Timmar för projekt, uppgifter och ärenden

## Uppdaterade listor för flikarna Projekt, Uppgift och Antal ärenden

De förbättrade listvyerna är nu tillgängliga på fliken Timmar för projekt, uppgifter och ärenden.

Före den här förbättringen tillämpades de nya listorna endast på följande:

* En lista med uppgifter
* En lista med projekt

Mer information om hur du visar objekt i en lista finns i [Kom igång med listor i Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Redigera Gantt utan att aktivera ett särskilt redigeringsläge

Nu kan du redigera Gantt-schemat för uppgiftslistan när Spara automatiskt är aktiverat eller inte. Du kan inte ångra ändringar när växeln är aktiverad. I det här fallet sparas de ändringar du gör i projektet automatiskt.

Mer information om hur du redigerar Gantt-schemat för uppgiftslistor finns i [Uppdatera information i Gantt-schemat för uppgiftslistor](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Ta bort fliken Problem från Kanban-tavlan

Fliken Problem tas bort från Kanban-tavlan i produktionsutgåvan 19.3. Du kan fortfarande komma åt fliken Problem från Backlog på Kanban-tavlan.

## Ta bort flikarna Dokument och Problem från sidan med upprepningsinformation

>[!NOTE]
>
>Den här ändringen kommer att ske i Production med version 2019.3. Den kommer inte att göras i förhandsvisningsmiljön före produktionsreleasen.

Flikarna Dokument och problem tas bort från sidan Agile-information om upprepning:

* **Dokument:** Alla dokument som lagras på fliken Dokument måste flyttas före produktionsversionen. Om du inte flyttar dokumenten har du inte längre åtkomst till dem.
* **Problem:** Den här fliken finns vanligtvis i listrutan Mer. Du kan fortfarande komma åt fliken Problem på fliken Arbetsobjekt i iteration.

## Överväg eller ignorera användartid i aktivitetsdatum

Du kan nu bestämma om tidsplanen för den primära tilldelaren av en uppgift ska tillåtas för att justera planerade datum.

Du kan fatta det här beslutet antingen på systemnivå, som Workfront-administratör eller på projektnivå som projektledare.

Före den här ändringen har tiden för den primära tilldelaren alltid justerat aktivitetens planerade datum, om aktivitetsbegränsningen tillåter att datumen ändras.

Mer information om inställning för användartid på systemnivå finns i [Konfigurera systemomfattande projektinställningar](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Mer information om inställningen för användartid av projektnivå finns i [Redigera projekt](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 22 juli 2019
>
>Produktionstillgänglighet: 9 augusti 2019

## Anpassade villkor

Nu kan du göra följande för att anpassa de villkor du använder för projekt, uppgifter och ärenden och bättre uppfylla organisationens behov:

* Skapa anpassade villkor med egna etiketter och färger.
* Ändra villkorens ordning i listrutorna där användarna markerar dem.
* Använd anpassade villkor som du skapar i stället för de inbyggda standardvillkoren som Workfront automatiskt tilldelar arbetsobjekt.
* Ändra namn och färger för de inbyggda standardvillkoren för projekt, uppgifter och ärenden.

Om du har behörighet att redigera en uppgift eller ett problem, men inte har tilldelats någon uppgift (kanske för att du övervakar den), kan du nu ändra dess villkor med kolumnen Villkor i en listvy.

Tidigare gick det inte att anpassa eller ändra villkoren, och bara användare kunde ändra villkoret för en uppgift eller ett problem om de hade tilldelats till den.

Mer information finns i [Anpassade villkor](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 4 juli 2019
>
>Produktionstillgänglighet: slutet av september eller början av oktober

## Nytt e-postmeddelande för team

Det finns ett nytt e-posthändelsemeddelande för team. Teammedlemmar får ett e-postmeddelande när ett projekt med uppgifter tilldelade till deras team blir aktivt. Den här inställningen är inaktiverad som standard.

Tidigare kunde teammedlemmarna inte meddelas när de var aktiva.

Mer information finns i Meddelanden: Information om projekt som jag är på.

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 4 juli 2019
>
>Produktionstillgänglighet: 18 juli 2019

## Dokumentuppdateringar visas nu för det associerade objektet och projektet

När du kommenterar ett dokument visas uppdateringen nu på fliken Uppdateringar både för dokumentet och för objektet som dokumentet är bifogat till.

Om objektet är en del av ett projekt visas kommentaren i dokumentet även på fliken Uppdateringar för projektet.

Tidigare visades bara uppdateringskommentarer på fliken Uppdateringar för dokumentet.

Mer information finns i avsnittet [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) i artikeln [Uppdatera arbete](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 6 juni 2019
>
>Produktionstillgänglighet: 20 juni 2019

## Synlighet i tidsgränsschemat för en användare när han eller hon tilldelar dem till uppgifter och ärenden

När du tilldelar en användare till en aktivitet eller ett problem kan du nu se en textbunden varning om den valda användaren har en tid utanför schemalagd tid mellan de planerade datumen för aktiviteten eller utgåvan.

Mer information om hur du tilldelar uppgifter finns i [Tilldela uppgifter](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Mer information om ledig tid finns i [Konfigurera personlig tid ](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 30 maj 2019
>
>Produktionstillgänglighet: 13 juni 2019

## Lägg till fält som representerar objekt i anpassad Forms

Vi har skapat en ny fälttyp i den anpassade formulärbyggaren som kallas Typeahead. I det här fältet kan du lägga till fält som representerar objekt i dina anpassade formulär. För närvarande är User-objektet aktiverat med Typeahead och andra objekt kommer i framtiden.

Tidigare var administratörer tvungna att manuellt underhålla användare som enskilda alternativ på anpassade formulärmenyer.

>[!NOTE]
>
>Tillgänglighet för förhandsgranskning: 30 maj 2019
>
>Produktionstillgänglighet: 13 juni 2019
>
>Före produktionsreleasedatum stöds inte de nya anpassade fälten i Mobile, Outlook, MS Teams och Salesforce-integreringen.
>
>I Production stöds nu Outlook och MS Teams. Mobilt stöds från slutet av juni eller början av juli. Salesforce-integreringar stöds från och med juni.

## Det nya ämnesfältet för begäran har bytt namn till Namn

>[!NOTE]
>
>Den här funktionen har tagits bort och kommer inte att ingå i version 2019.3.

När du skickar en ny begäran till en begärandekö anger du namnet på begäran i fältet Namn i det nya begärandeformuläret.

Före den här ändringen anger du namnet på begäran i fältet Ämne.

Mer information om hur du skapar begäranden finns i [Skapa och skicka Workfront-begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

