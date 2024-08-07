---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 3 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2018.1 av Beta 3. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 7 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i början av 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# 2018.1 Beta 3 - versionsaktivitet

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i version 2018.1 av Beta 3. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 7 januari 2018. Den kommer att göras tillgänglig i produktionsmiljön i början av 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.1 finns på  [Aktivitetsöversikt för version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 3 innehåller förbättringar för både Workfront-administratörer och andra användare:

**För administratörer**

* [Förbättringar av gruppadministratörer](#group-administrator-improvements)

**För alla användare**

* [Förbättringar av korrekturläsaren för HTML5](#html5-proofing-viewer-improvements)
* [Korrekturförbättringar i Workfront](#proofing-improvements-within-workfront)
* [Förbättringar av hemområdet](#home-area-improvements) 
* [Agile Improvements](#agile-improvements)
* [Förbättringar av Gantt-schema](#gantt-chart-improvements)
* [Förbättringar av resursplanering](#resource-planner-improvements)

## Förbättringar av gruppadministratörer {#group-administrator-improvements}

* [Återställ användargränssnittet för lösenord har uppdaterats för gruppadministratörer](#reset-password-ui-updated-for-group-administrators)
* [Alternativ för åtkomstnivåinställningar för gruppadministratörer](#access-level-setup-options-for-group-administrators)
* [Skapa tidrapportprofiler för grupper](#create-timesheet-profiles-for-groups)
* [Återställ borttagna objekt för användare som gruppadministratör](#recover-deleted-items-for-users-as-a-group-administrator)

### Återställ användargränssnittet för lösenord har uppdaterats för gruppadministratörer {#reset-password-ui-updated-for-group-administrators}

När du återställer lösenordet för en annan användare uppmanas du som gruppadministratör att ange ditt eget lösenord innan du kan ändra lösenordet. Gränssnittet har uppdaterats för att återspegla den här funktionen. Innan den här ändringen utfördes visades att Workfront administratörslösenord krävs.

Mer information om hur du återställer lösenord för andra användare finns i [Redigera en användares profil](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Mer information om funktionerna för en gruppadministratör finns i avsnittet &quot;Capabilities of group administrators&quot; i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Alternativ för åtkomstnivåinställningar för gruppadministratörer {#access-level-setup-options-for-group-administrators}

Som Workfront-administratör kan du nu styra om gruppadministratörer kan logga in som andra användare eller om de kan återställa lösenord för andra användare. Vi har lagt till en ny inställning på åtkomstnivån för att aktivera eller inaktivera åtkomsten. Före den här ändringen kunde alla gruppadministratörer logga in som andra användare och återställa andra användares lösenord som standard. Den här ändringen påverkar bara åtkomstnivån för planerare.

Mer information om hur du konfigurerar åtkomstnivå för användare finns i [Bevilja åtkomst för användare](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Mer information om funktionerna för en gruppadministratör finns i avsnittet &quot;Capabilities of group administrators&quot; i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Skapa tidrapportprofiler för grupper {#create-timesheet-profiles-for-groups}

Som gruppadministratör kan du nu skapa tidrapportprofiler för de grupper som du administrerar och associera dem med grupper som du administrerar, eller användare från dessa grupper. Tidrapportprofiler säkerställer att tidrapporter skapas automatiskt för de användare som är associerade med dem.

Före den här ändringen kunde bara en Workfront-administratör skapa tidrapportprofiler.

Mer information om hur du skapar tidrapportprofiler finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Mer information om funktionerna för en gruppadministratör finns i avsnittet &quot;Capabilities of group administrators&quot; i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Återställ borttagna objekt för användare som gruppadministratör {#recover-deleted-items-for-users-as-a-group-administrator}

Om ett projekt är kopplat till en grupp som du är gruppadministratör för, kan du återställa projektet eller någon av dess borttagna uppgifter, utleveranser eller dokument från Papperskorgen. Före den här ändringen kunde bara en Workfront-administratör återställa objekt från papperskorgen.

Mer information om hur du återställer borttagna objekt i Workfront finns i [Återställa borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Mer information om funktionerna för en gruppadministratör finns i avsnittet &quot;Capabilities of group administrators&quot; i [Skapa en grupp](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Förbättringar av korrekturläsaren för HTML5  {#html5-proofing-viewer-improvements}

* [Jämför läge](#compare-mode)
* [Filtrera kommentarlistan](#filter-the-comment-list)
* [Kommentarlistan genomsöks efter det första tecknet har angetts](#comment-list-is-searched-after-the-first-character-is-entered)

### Jämför läge {#compare-mode}

Nu kan du använda jämförelseläget i korrekturläsaren för HTML 5 när du visar statiskt korrektur och videokorrektur. 

Jämförelseläget i korrekturläsaren för HTML5 skiljer sig från det äldre språkvisningsprogrammet på följande sätt:

* När du startar jämförelseläget flyttas den nyare versionen till höger, med den version du jämför till vänster.

  Tidigare flyttades den nyare versionen till vänster, med den version du jämför till höger.

* Du kan välja vilken version av ett korrektur du vill jämföra direkt i korrekturläsaren. 
* Den aktuella zoomnivån och positionen för korrektur i korrekturläsaren bibehålls vid samtidig navigering.
* Nytt alternativ för Återställ när samtidig navigering används.
* När du avslutar jämförelseläget kan du välja vilket korrektur du vill stänga. 

  Tidigare var den äldre versionen alltid stängd.

* Olika förbättringar av utseende, känsla och användbarhet.

Mer information finns i [Jämför korrektur i korrekturläsaren](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrera kommentarlistan {#filter-the-comment-list}

Nu kan du filtrera kommentarer i kommentarlistan. Du kan filtrera efter användare, åtgärder, olästa med mera.

### Kommentarlistan genomsöks efter det första tecknet har angetts {#comment-list-is-searched-after-the-first-character-is-entered}

När du söker i kommentarlistan filtreras listan automatiskt efter att du har skrivit det första tecknet.

Före den här ändringen var du tvungen att skriva minst tre tecken i sökfältet innan kommentarlistan filtrerades.

Mer information finns i .

## Förbättringar av korrektur i Workfront {#proofing-improvements-within-workfront}

* [Länka korrektur från Workfront Proof till Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Kan inte längre ta bort ett korrektur från ett dokument](#can-no-longer-remove-a-proof-from-a-document)
* [Uppdaterad look och känsla vid generering och öppning av korrektur](#updated-look-and-feel-when-generating-and-opening-proofs)

### Länka korrektur från Workfront Proof till Workfront {#link-proofs-from-workfront-proof-to-workfront}

Nu kan du länka dokumentkorrektur som redan finns i ditt Workfront Proof-konto till Workfront.

Före den här ändringen kunde du inte komma åt korrektur som redan fanns i Workfront Proof i Workfront. 

Mer information finns i [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) i [Länka dokument från externa program](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Kan inte längre ta bort ett korrektur från ett dokument {#can-no-longer-remove-a-proof-from-a-document}

Du kan inte längre ta bort ett korrektur från ett dokument. Om du vill ta bort ett korrektur måste du i stället ta bort hela dokumentet.

Den här förbättringen minskar risken för att användare oavsiktligt tar bort alla versioner av ett korrekturdokument. 

Mer information om hur du tar bort ett dokument finns i [Ta bort ett korrektur](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) i [Ta bort ett korrektur](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Uppdaterad look och känsla vid generering och öppning av korrektur {#updated-look-and-feel-when-generating-and-opening-proofs}

Det finns nu en uppdaterad animeringssnurra när ett korrektur genereras.

## Förbättringar av hemområdet {#home-area-improvements}

Följande förbättringar har gjorts i hemområdet:

* [Visa korrekturgodkännanden från hemområdet](#view-proof-approvals-from-the-home-area)
* [Standardfält visas när layoutmallen för objekt i hemområdet konfigureras](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Visa korrekturgodkännanden från hemområdet {#view-proof-approvals-from-the-home-area}

Nu kan du visa korrekturgodkännanden på Hem-området, förutom standardgodkännanden.

Tidigare kunde du visa Workfront-godkännanden, men du kunde inte visa godkännanden för ett korrektur.  

Mer information finns i [Använda hemområdet](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Standardfält visas när layoutmallen för objekt i hemområdet konfigureras {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Tidigare var standardfälten inte synliga från layoutmallen.

Mer information finns i&quot;Skapa och hantera layoutmallar&quot;.

## Flexibla förbättringar {#agile-improvements}

* [Lägg till aktiviteter och problem i iterationen direkt från aktivitets- eller ärendeinformationssidan](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Inkludera problem i Scrum Backlog och Story Board för ett Agile Team](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Använd grupperingar och filter i eftersläpningen för ett Agile Team](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Skapa en tom iteration och uppdatera den senare](#create-a-blank-iteration-and-update-it-later)
* [Fälten &quot;Fokus&quot; och &quot;Capacity&quot; fylls i i förväg när en interaktion skapas](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Lägg till uppgifter och problem i iterationen direkt från sidan Aktivitets- eller Ärendeinformation {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Nu kan du lägga till uppgifter och ärenden som för närvarande är tilldelade ett smidigt team till en iteration direkt från uppgiften eller utgåvan.

Tidigare kunde du bara lägga till uppgifter i en iteration från efterloggen. 

Mer information finns i [Skapa en iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) i [Skapa en iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Inkludera problem i Scrum Backlog och Story Board för ett Agile Team {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Problem inkluderas nu som standard i eftersläpningen för ditt mobila team när Scrum-metoden används (utgåvor visas inte i eftersläpningen för ett rörligt team när Kanban-metoden används).

Före den här ändringen kunde bara uppgifter läggas till i efterloggen. Om du ville lägga till ett problem var du först tvungen att konvertera problemet till en uppgift innan det kunde läggas till.

Mer information om hur du använder problem i eftersläpningen finns i  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Använda grupperingar och filter i eftersläpningen för ett Agile-team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Grupperings- och filteralternativen är nu tillgängliga i den flexibla eftersläpningen, så att du kan ordna din eftersläpning efter grupperingar samt filtrera efter specifika uppgifter och problem.

Före den här ändringen kan du tillämpa på vyer på den flexibla eftersläpningen.

Mer information finns i  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) i  [Hantera den flexibla eftersläpningen](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Skapa en tom iteration och uppdatera den senare {#create-a-blank-iteration-and-update-it-later}

Du behöver inte längre lägga till en uppgift eller ett problem i en iteration för att kunna skapa den. Du kan skapa en tom upprepning och lägga till uppgifter och utgåvor vid ett senare tillfälle.

Mer information finns i [Skapa en iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Fälten &quot;Fokus&quot; och &quot;Capacity&quot; fylls i i förväg när en interaktion skapas {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

När du skapar en iteration fylls nu fälten&quot;Fokus&quot; och&quot;Kapacitet&quot; i automatiskt med de genomsnittliga värdena för alla tidigare iterationer som ditt team har skapat. Om ditt team inte har skapat några tidigare iterationer visas dessa fält som 0.

Tidigare var dessa fält alltid inställda på 0.

Mer information finns i [Skapa en iteration](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Förbättringar av Gantt-schema {#gantt-chart-improvements}

* [Aktivera redigeringsläge i Gantt-schema](#enable-edit-mode-in-the-gantt-chart)
* [Ta bort föregående när Gantt-schemat redigeras](#remove-predecessors-when-editing-the-gantt-chart)

### Aktivera redigeringsläge i Gantt-schema {#enable-edit-mode-in-the-gantt-chart}

När du aktiverar redigeringsläget i Gantt-diagrammet kan du ändra informationen i diagrammet. Det gick inte att redigera informationen i Gantt-diagrammet före den här ändringen. Du kan bara redigera uppgiftsinformation i uppgiftslistan.

Mer information om hur du redigerar Gantt-schemat finns i [Uppdatera information i Gantt-schemat för uppgiftslistan](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Ta bort föregående när Gantt-schemat redigeras {#remove-predecessors-when-editing-the-gantt-chart}

Med redigeringsläget för Gantt-schemat kan du nu ta bort tidigare relationer mellan aktiviteter i Gantt-schemat för ett projekt. Före den här förbättringen kan du ta bort den föregående relationen endast i uppgiftslistan eller på aktivitetsnivån.

Mer information om hur du redigerar Gantt-schemat finns i [Uppdatera information i Gantt-schemat för uppgiftslistan](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Förbättringar av resursplanering {#resource-planner-improvements}

* [Budget med noll varaktighet i resursplaneraren](#budget-with-zero-duration-in-the-resource-planner)

* [Visa data efter kostnad i resursplaneraren](#show-data-by-cost-in-the-resource-planner)

### Budget med noll varaktighet i resursplaneraren {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Den här funktionen har tagits bort från förhandsvisningsmiljön och släpps i version 18.1.

Du kan nu budgetera dina resurser i resursplaneraren för valfritt datum, inom eller utanför projektets tidsram. Före den här förbättringen kunde du bara budgetera dina resurser för datum inom projektets tidsram.

Mer information om budgeteringsresurser i resursplaneraren finns i avsnittet Budgeteringsresurser i resursplaneraren i [Översikt över resursplaneraren](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Visa data efter kostnad i resursplaneraren {#show-data-by-cost-in-the-resource-planner}

Du kan nu visa informationen i resursplaneraren efter kostnad, förutom timvärden och FTE-värden. Du kan visa kostnader i resursplaneraren när du visar dem i vyerna Visa efter projekt eller Visa efter roll. Du kan inte visa kostnader när du visar resursplaneraren i vyn Visa efter användare.

Mer information om hur du visar resursplaneraren efter timmar, FTE eller kostnadsvärden finns i [Navigeringsöversikt för resursplanering](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
