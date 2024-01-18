---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatering,release
navigation-topic: 2021-2-release-activity
title: 21.2 Projektförbättringar
description: Den här sidan beskriver alla projektförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i versionsöversikt 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4e954d79-da5a-42f5-b43f-b1fdd17316d2
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1650'
ht-degree: 0%

---

# 21.2 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 21.2 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 10 maj 2021. En lista över alla ändringar som är tillgängliga i version 21.2 finns i [21.2 Versionsöversikt](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Nytt gränssnitt för att skapa och redigera återkommande uppgifter

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Som en del av omdesignen av rutorna Ny och Redigera uppgift har vi lagt till möjligheten att göra en ny uppgift återkommande samt att redigera den överordnade för en återkommande uppgift. Den här funktionen ingick inte i den tidigare versionen av rutan Ny och redigera uppgift.

Mer information finns i [Skapa återkommande uppgifter](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

Den här funktionen ingår nu i [Grundläggande om planering för den nya Workfront-upplevelsen, del 2: Planera ett projekt](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-MCDUWIMXC3JRAAFGHX7QYIN2BVDI) utbildningsväg på Workfront One.

## Nya knappar tillgängliga i projekthuvudet

>[!NOTE]
>
>Den här funktionen är ännu inte tillgänglig i förhandsvisning. Den släpps i förhandsvisningsmiljön den 29 april 2021.

För att du snabbt ska kunna filtrera listan över projekt på sidan Projekt finns det två nya knappar i huvudet som gör att du snabbt kan använda filtret Projekt jag är på eller Projekt jag äger.

Den här funktionen ingår nu i [Grundläggande om planering för den nya Workfront-upplevelsen, del 1: Skapa ett projekt](https://one.workfront.com/s/learningpath5/planner-fundamentals-for-the-new-workfront-experience-MCTOONVRZDLRD3FAIX6SQYSUAHDE) utbildningsväg på Workfront One.

## Flytta eller ta bort en artikel eller ett problem från Urklipp

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Nu kan du flytta en artikel eller ett problem från din Scrum-panel genom att klicka på ikonen Mer på en artikel eller ett frågekort och välja Flytta till. Om du har definierat framtida iterationer kan du flytta objektet till en annan iteration. Du kan också flytta objektet till teamets eftersläpning.

Du kan också ta bort en artikel eller ett problem direkt från din Scrum-panel genom att klicka på ikonen Mer på ett kort och sedan välja Ta bort. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.

Mer information finns i [Hantera artiklar och problem på Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/manage-scrum-board.md).

## Ny ruta för redigeringsproblem

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Som en del av uppdateringen av utseendet och känslan i den nya Workfront-upplevelsen har vi gjort om rutan Redigera problem. Du kan öppna den nya rutan Redigera problem från ett enskilt ärende eller när du redigerar ett enstaka ärende från en lista.

Förutom att utseendet och känslan har uppdaterats är följande ändringar även tillgängliga i rutan Ärendeuppgift:

* Du kan anpassa layoutmallen en gång och spegla anpassningarna både på sidan Detaljer och i rutan Redigera problem.
* Enskilda anpassade formulärnamn finns nu på den vänstra panelen i rutan Redigera problem och du kan snabbt komma åt de olika formulären därifrån.
* Vi har lagt till fältet Planerade timmar i uppdragsavsnittet för att göra det enklare att uppdatera tiden det kan ta för att slutföra problemet.
* Vi har tagit bort kommentarsfunktionen från skärmen Redigera problem för att eliminera redundans i uppdateringsavsnittet.

## Flyttade knapparna Spara och Avbryt för rutorna Redigera och Nytt objekt

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Baserat på användarfeedback har vi flyttat knapparna Spara och Avbryt till det nedre vänstra hörnet i rutorna Redigera objekt och Nytt objekt för projekt och uppgifter.

Före den här förbättringen fanns de här knapparna i det övre högra hörnet av rutorna.

Mer information om hur du redigerar projekt och uppgifter finns i följande artiklar:

* [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md)

![](assets/pasted-image-4-5-2021-0-350x278.png)

## Förbättrade anpassade formulär

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För en bättre upplevelse när du fyller i ett anpassat formulär har vi förbättrat sättet som långa anpassade fältetiketter visas på. När det finns tillräckligt med vågrätt utrymme för att visa dem i sin helhet trunkeras inte längre dessa etiketter.

Mer information om hur du fyller i anpassade formulär finns i [Redigera information i anpassade formulärfält](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Den primära kontakten för ett problem visas nu i området Projektinformation

>[!NOTE]
>
>Den här funktionen släpptes till produktionsmiljön den 10 mars 2020.

När en utgåva konverteras till ett projekt överförs den som har begärt utgåvan till projektet och visas i fältet Originator för det konverterade utgåvan. Du kan visa det här fältet i området Projektinformation, liksom i projektrapporter och listor. Den här informationen visas även för uppgifter, endast i rapporter och listor.

Du måste aktivera det här fältet i din layoutmall för att kunna visa det i den nya Adobe Workfront-upplevelsen för projekt.

Mer information om hur du konverterar problem finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Visa information om en grupp som du vill tilldela en portfölj, ett program eller ett team

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

När du tilldelar en grupp till en portfölj, ett program eller ett team har det blivit enklare att se till att du har rätt grupp. Du kan klicka på informationsikonen bredvid namnet på gruppen om du vill visa ett verktygstips som innehåller hierarkin med grupper ovanför den, tillsammans med gruppens administratörer. Beroende på den information som konfigurerats för gruppen kan du även se gruppens företagsledare och beskrivning.

Det här är samma funktioner som nyligen släpptes för att hjälpa dig att identifiera en grupp som du måste tilldela ett projekt, vilket förklaras i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Mer information finns i följande artiklar:

* [Skapa en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)
* [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)
* [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)

## Textformatering i anpassade fält visas nu i alla listor och rapporter i Workfront Classic

>[!NOTE]
>
>Den här funktionen är endast tillgänglig i Adobe Workfront Classic.

Användarna kan nu se textformatering som fet stil, punktlistor och hyperlänkar i anpassade fält när de visar listor och rapporter.

Tidigare i Workfront Classic var textformateringen bara synlig i listorna Projekt, Aktivitet och Timme.

Mer information om textformatering i anpassade fält finns i [Skapa ett anpassat formulär](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FAdministration_and_Setup%2FCustomize_Workfront%2FCreate_manage_Custom_Forms%2Fcreate-a-custom-form.html).

Mer information om hur du visar information i listor finns i [Kom igång med listor](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWorkfront_basics%2FNavigate_Workfront%2FWorkfront_Navigation%2Fview-items-in-a-list.html&amp;_LANG=en).

## Ny åtgärdsruta för redigering

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Som en del av uppdateringen av utseendet på den nya Workfront-upplevelsen har vi gjort om rutan Redigera uppgift. Du kan öppna den nya rutan Redigera uppgift från en enskild uppgift eller när du redigerar en enstaka uppgift från en lista.

>[!NOTE]
>
>Som en del av den här uppdateringen kommer fältet Resursomfång att tas bort från den nya Adobe Workfront-upplevelsen.

Förutom ett uppdaterat utseende och känsla finns följande ändringar även i rutan Redigera uppgift:

* Du kan anpassa layoutmallen en gång och återge anpassningarna både på sidan Detaljer och i rutan Redigera uppgift.
* Enskilda namn på anpassade formulär finns nu på den vänstra panelen i rutan Redigera åtgärd och du kan snabbt komma åt formulären därifrån.
* Vi har lagt till fälten Varaktighet, Varaktighet och Planerade timmar i uppdragsavsnittet för att skapa konsekvens när tilldelningar uppdateras för olika varaktighetstyper och hur länge eller hur länge de används för uppgiften.
* Vi har tagit bort kommentarsfunktionerna från redigeringsskärmen för att eliminera redundans med uppdateringsavsnittet.

Mer information om den nya rutan Redigera uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Ny aktivitetsruta

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

Som en del av uppdateringen av utseendet på den nya Workfront-upplevelsen har vi gjort om rutan Ny uppgift. Du kommer åt rutan Ny uppgift när du lägger till en uppgift i ett projekt genom att klicka på Ny uppgift högst upp i uppgiftslistan.

>[!NOTE]
>
>Som en del av den här uppdateringen kommer fältet Resursomfång att tas bort från den nya Adobe Workfront-upplevelsen.

Förutom ett uppdaterat utseende och känsla finns följande ändringar även i arbetsflödet Ny uppgift:

* En mindre skärm med nya uppgifter visas när du först klickar på Ny uppgift i en projektlista med ett begränsat antal fält som ska uppdateras, vilket sparar tid när du snabbt vill lägga till uppgifter i projekt. Du kommer åt det fullständiga nya aktivitetsformuläret som innehåller alla aktivitetsfält som vi har ändrat namn till Skapa uppgift.
* Du kan anpassa layoutmallen en gång och återge anpassningarna både på sidan Detaljer och i rutan Ny uppgift.
* Vi har lagt till fälten Varaktighet, Varaktighet och Planerade timmar i uppdragsavsnittet för att ge konsekvens när tilldelningar uppdateras och hur lång tid eller varaktighet de lägger på uppgiften.

Mer information om den nya aktivitetsrutan finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

## Inaktivera team som inte längre används

>[!NOTE]
>
>Den här funktionen lanseras i Production den 15 april 2021, före version 21.2.

Nu kan du inaktivera team som du inte längre använder. När du inaktiverar ett team visas det inte längre i de flesta typsnitt, sökfält eller vanliga menyer i Workfront. Historiska data som är kopplade till teamet sparas dock.

Mer information finns i [Inaktivera ett team](../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md).

## Uppdatera till inställning som tillåter användare att ta bort uppgifter och problem med loggade timmar

>[!NOTE]
>
>Finns endast i nya Adobe Workfront.

För att ge dig en sammanhängande upplevelse av alla objekt har vi ändrat det sätt på vilket inställningen&quot;Tillåt användare att ta bort uppgifter och problem med loggade timmar&quot; fungerar i Workfront. När nu din Workfront- eller gruppadministratör inaktiverar inställningen Aktivitet och problem kan du inte längre ta bort projekt som innehåller uppgifter eller problem med loggade timmar.

Innan den här ändringen utfördes hindrades användarna från att ta bort aktiviteter eller problem, inte projekt, bara om inställningen inaktiverades.

Mer information finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

