---
content-type: release-notes
keywords: noteringar,kvartalsvis,uppdatera
navigation-topic: product-releases
title: 21.1 Förbättrad projektledning
description: Den här sidan beskriver alla projekthanteringsförbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# 21.1 Förbättrad projektledning

Den här sidan beskriver alla projekthanteringsförbättringar som gjorts i version 21.1 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön den 15 februari 2021.

En lista över alla ändringar som är tillgängliga i version 21.1 finns i [21.1 - versionsöversikt](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Export finns nu i avsnittet Metrics i ett projekt

Om du enklare vill dela status och förlopp för ett projekt kan du nu exportera hela kontrollpanelen i avsnittet Metrisk i ett projekt till en PNG-fil.

Mer information finns i [Översikt över projektstatistik](../../../manage-work/projects/manage-projects/project-metrics.md).

Den här funktionen ingår nu i [Grundläggande om planering för den nya Workfront-upplevelsen, del 3: Hantera ett projekt](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) utbildningsväg på Workfront One.

## Uppdatera utleveransprocent slutfört när projektet eller aktiviteten konverterades från utleveransuppdateringen

Vi har uppdaterat hur procentandelen slutförda problem fungerar för problem som har konverterats till projekt eller uppgifter. När ett problem konverteras till en aktivitet eller ett projekt uppdateras procentandelen slutfört av problemet synkroniserat med procentandelen slutfört för den åtgärd eller det projekt som åtgärdas när inställningen&quot;Uppdatera lösningsstatus automatiskt när statusen för det objekt som löses ändras&quot; aktiveras från konfigurationen.

Mer information om hur du konverterar problem finns i [Översikt över upplösta och upplösta objekt](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Lista över nya skickade begäranden

För att du ska kunna hantera dina skickade begäranden på ett enklare och mer konsekvent sätt har vi tagit bort avsnitten Begäranden som jag har skickat och Alla begäranden i området Begäranden och ersatt dem med en ny skickad lista. Listan har en välbekant utseende som matchar alla andra listor i systemet, vilket gör att du kan filtrera efter olika kategorier av skickade begäranden och snabbt söka efter en begäran som kan vara svår att hitta.

Mer information om hur du söker efter skickade begäranden finns i [Sök efter skickade begäranden](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Den här funktionen ingår nu i [Collaborator Fundamentals för nya Workfront Experience](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) utbildningsväg på Workfront One.

Den här funktionen ingår nu i [Begäranden i den nya Workfront-upplevelsen](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) utbildningsväg på Workfront One.

## Fält som tagits bort från sidan Ny begäran

>[!NOTE]
>
>Borttagen från release.

Som en del av omdesignen av sidan Ny begäran har vi uppdaterat de nya fält för problem som har konfigurerats i avsnittet Köinställningar i ett projekt.

Följande fält för nya problem visas bara när du skapar ett problem i projektets avsnitt Problem. De visas inte när ett problem skickas med en frågekö i området Begäranden:

* Allvarlighetsgrad
* Planerade timmar
* Planerat startdatum
* URL
* Tilldelad till
* Jobbroll
* Team

Vi har ersatt fälten Tilldelad till, Jobbroll och Team med det nya fältet Uppdrag på sidan Ny begäran, för att effektivt utse en användare, jobbroll eller team i ett gemensamt fält när du skickar en ny begäran.

Mer information om hur du definierar nya fält för problem i ett projekt finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Ny upplevelse när begäranden skickas i området Förfrågningar

>[!NOTE]
>
>Borttagen från version; kommer att finnas kvar i Förhandsgranska och distribueras till Produktion med 21.2.

För att skapa enhetlighet med den nya Workfront-upplevelsen och för att effektivisera när du skickar in begäranden har vi gjort om rutan Ny begäran i området Begäranden. Nedan följer några av förbättringarna:

* Ett enhetligt användargränssnitt med resten av den nya Workfront-upplevelsen
* Eliminerade området med nya förfrågningar för en enklare och mer intuitiv upplevelse
* Ett nytt, effektivare sätt att bifoga dokument

Möjlighet att dela en länk till begärandekön, ämnesgruppen eller köämnet när du anger begäran.

Mer information om hur du skickar begäranden finns i [Skapa och skicka Workfront-förfrågningar](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Dela en länk till en begärandekö när du skickar en begäran

>[!NOTE]
>
>Borttagen från version; kommer att finnas kvar i Förhandsgranska och distribueras till Produktion med 21.2.

Vi har nu gjort det möjligt att dela en länk till en begärandekö, en ämnesgrupp eller ett köämne medan du skapar en begäran.

Innan du skickar en ny begäran kan du kopiera en länk till begärandekön, ämnesgruppen eller köämnet för begäran och dela den med andra användare, eller bädda in den i en instrumentpanel.

Mer information om hur du delar en länk till en begärandekö när du skickar en begäran finns i [Dela en länk till en begärandekö](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Söka efter en grupp som du vill tilldela ett projekt och visa information om den

Nu är det enklare att se till att du identifierar rätt grupp när du tilldelar en grupp till ett projekt. Håll muspekaren över namnet på en grupp som du hittar i grupprutan och klicka sedan på infoikonen som visas bredvid namnet för att visa verktygstipset Gruppinformation.

Det här verktygstipset innehåller hierarkin med grupper ovanför gruppen, om sådan finns, och gruppens administratörer.

Beroende på den information som konfigurerats för gruppen kan du även se gruppens företagsledare och beskrivning.

Med den här informationen kan du vara säker på att du väljer rätt grupp för projektet.

Mer information finns i [Hantera information i projektöversiktsområdet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Ny delegeringsrapport för användare

Tidigare kunde information för delegering av uppgifter, utgåvor och projektgodkännande endast visas av delegaten i hemområdet. Om du vill att andra användare ska kunna se den här informationen kan plananvändarna nu skapa rapporten för användardelegering, som innehåller följande information:

* Vem har delegerat godkännandena till en annan användare
* Vilken användare har delegerats dessa godkännanden
* Start- och slutdatum för dessa delegationer

Mer information finns på [Skapa en delegeringsrapport för användare](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
