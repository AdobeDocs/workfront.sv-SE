---
title: 21.3 Projektförbättringar
description: 21.3 Projektförbättringar
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3 Projektförbättringar

Den här sidan beskriver alla projektförbättringar som gjorts i version 21.3 till förhandsvisningsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 21 juli 2021.

En lista över alla ändringar som är tillgängliga i version 21.3 finns i [21.3 Versionsöversikt](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Koppla en mall till en grupp

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Vi har lagt till möjligheten att tilldela en grupp till en projektmall för att hjälpa dig att effektivisera projektskapandet - och för att hjälpa dig att enklare identifiera och rapportera vilka grupper som äger vilka projektmallar.

När du tilldelar en grupp till en projektmall kopplas alla projekt som skapas från mallen automatiskt till mallgruppen. Mer information finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Du kan även koppla en process för gruppgodkännande till en mall och dess malluppgifter om mallen är kopplad till gruppen. Mer information finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Enklare redigering av fält i detaljavsnittet

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Med följande förbättringar kan du enklare redigera information i detaljavsnittet för alla objekt:

* En grå kontur runt ett fält när du hovrar över det visar att det är redigerbart.
* Du kan redigera fält genom att klicka på dem en gång.

Före den här förbättringen var det inte klart vilka fält som kunde redigeras och du var tvungen att dubbelklicka för att redigera ett fält.

## Överväg om du vill använda en föregående projektövergripande beräkning vid beräkning av datum för överlämning

I och med den nya förbättringen av hur Adobe Workfront beräknar leveransdatum för arbetsmoment har man nu tagit hänsyn till projektövergripande beroenden.

Tidigare beräknades datum för överlämnande endast baserat på föregående aktiviteter för aktiviteten från samma projekt.

För att vara säker på att du alltid har rätt datum för en åtgärd med en föregångare mellan projekt måste du beräkna om tidslinjen för den efterföljande uppgiftens projekt. När tidslinjen har räknats om beräknas datum för när uppgiften har överlämnats med hänsyn till aktiviteternas projektövergripande beroenden.

Mer information om leveransdatum finns i [Översikt över datum för aktivitetsleverans](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Lägg till befintliga artiklar och utgåvor från Scrum board

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Nu kan du lägga till en befintlig artikel eller ett befintligt problem direkt från Scrum board. Det gör det enklare att lägga till befintliga artiklar i den aktuella upprepningen utan att behöva gå till eftersläpningssidan.

Mer information finns i [Lägga till artiklar och utgåvor från Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Lägg till nya artiklar och utgåvor från Scrum board

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Nu kan du skapa en ny artikel eller ett nytt problem direkt från Scrum board. Det gör det enklare att snabbt lägga till en ny artikel i den aktuella upprepningen.

Mer information finns i [Lägga till artiklar och utgåvor från Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Ta bort artikel eller utleverans från Kanban-tavlan

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Du kan nu ta bort en artikel eller ett problem direkt från din Kanban-panel genom att klicka på ikonen Mer på en artikel eller ett utgivningskort och välja Ta bort. När du tar bort en artikel eller ett problem flyttas den till papperskorgen i 30 dagar och kan endast återställas av systemadministratören.

Mer information finns i [Ta bort artiklar eller utgåvor från Kanban-tavlan](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Uppdateringar av Agile-kortets rubrik och anslagstavla

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

På Kanban- och Scrum-paneler finns nu följande förbättringar:

* Artikelkorten och kortspalterna har fast bredd så att kortstorlekarna inte ändras om du justerar storleken på webbläsarfönstret.
* Namnet på kolumnen Artiklar har ändrats till Överordnad artikel.
* Varje kort har en etikett högst upp som identifierar det som en överordnad artikel, underuppgift (kopplad till en överordnad artikel), artikel (inte kopplad till en överordnad artikel) eller utgåva.
* Bakgrundsskuggning skiljer kolumnerna åt visuellt.

Mer information finns i [Översikt över iterationer](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Inställningar för gruppera projekt, uppgift och ärende

Som vi meddelade tidigare introducerade vi anpassningar på gruppnivå för projekt, uppgifter och utgåvor i faser fram till 24 juni 2021. Nu är utrullningen klar och finns tillgänglig i Production för alla kunder.

Mer information finns i följande artiklar:

* [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Tillåt externa användare att godkänna ett dokument

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Nu kan du använda externa e-postadresser för att tilldela godkännare till ett dokument i den nya Workfront-upplevelsen.

Tidigare kunde du bara lägga till externa användare via e-postadresser i Workfront Classic.

Mer information finns i [Begär dokumentgodkännanden](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exportera information från detaljavsnittet i en portfölj eller ett program

>[!NOTE]
>
>Den här funktionen släpptes till förhandsvisningsmiljön den 20 maj 2021. Den kommer att släppas ut i produktionsmiljön den 3 juni 2021.

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Du kan nu exportera till en PDF-filinformation från detaljavsnittet för portföljer och program. Före den här förbättringen kunde du bara exportera information från informationsavsnittet från projekt, uppgifter och problem.

Mer information om hur du exporterar anpassade formulär från ett objekt finns i [Exportera anpassade formulär och objektinformation](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Tidsstämpel för planerat slutförandedatum har lagts till i objektets rubrik

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

För att underlätta åtkomst, bekvämlighet och exakthet har vi lagt till alternativet att välja en tidsstämpel i fältet Planerat slutförandedatum för projekt, uppgifter eller problem.

Före den här förbättringen valde Workfront midnatt som standardtid när du uppdaterade ett objekts planerade slutförandedatum. Nu kan du anpassa både tid och slutdatum.

Mer information om objektrubrikerna i den nya Workfront-upplevelsen finns i [Nya objektrubriker](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Lägga till ett anpassat formulär i ett objekt utan att redigera det

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen.

Vi har gjort det enklare att lägga till ett anpassat formulär som någon annan kan fylla i - eller som du senare ska fylla i - i ett objekt. Formuläret försätts inte längre i redigeringsläge automatiskt när du lägger till det. Du kan bara spara det tomma formuläret i objektet.

Tidigare när du lade till ett anpassat formulär till ett objekt, övergick sidan till redigeringsläge och du var tvungen att fylla i alla obligatoriska fält i formuläret innan du kunde spara det till objektet. Detta var inte praktiskt när formuläret var avsett för en annan användare att fylla i, eller när du ännu inte visste vad som skulle läggas in i ett obligatoriskt fält i formuläret.

Mer information om hur du lägger till ett anpassat formulär till ett objekt finns i [Lägga till ett anpassat formulär i ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

