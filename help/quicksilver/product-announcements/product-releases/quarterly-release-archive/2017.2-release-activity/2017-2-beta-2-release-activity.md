---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2 - versionsaktivitet
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 24 maj 2017. Den kommer att finnas tillgänglig i produktionsmiljön mellan slutet av juli och början av augusti 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 2017.2 Beta 2 - versionsaktivitet

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön i 2017.2 Beta 2. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 24 maj 2017. Den kommer att finnas tillgänglig i produktionsmiljön mellan slutet av juli och början av augusti 2017.

>[!IMPORTANT]
>
>Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2017.2 finns i [Översikt över versionsaktivitet för 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

2017.2 Beta 2 innehåller förbättringar både för Workfront-administratörer och andra användare:

**För administratörer:**

* [API-förbättring: händelseprenumerationer](#api-enhancement-event-subscriptions)

**För alla användare:**

* [Prenumerera på projekt](#subscribe-to-projects)
* [Avbeställ utskick från e-post](#unsubscribe-from-items-from-email)
* [Konfigurera hur milstolpar visas i Gantt-schemat](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Resurspoolmallar](#resource-pools-templates)
* [Visa versioner av korrekturdokument i Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nytt begäranobjekt i korrekturgodkännanderapport](#new-requester-object-in-proof-approval-report)

## API-förbättring: händelseprenumerationer {#api-enhancement-event-subscriptions}

När en åtgärd inträffar för ett Workfront-objekt som stöds av händelseprenumerationer, kan du nu konfigurera Workfront att skicka ett svar till önskad slutpunkt. Det innebär att integreringarna kan interagera med Workfront API i realtid.

Mer information finns i [API för händelseprenumeration](../../../../wf-api/general/event-subs-api.md). 

## Prenumerera på projekt {#subscribe-to-projects}

Nu kan du prenumerera på nya kommentarer i projekt som du inte är en del av projektteamet för. Före den här versionen kunde du bara prenumerera på kommentarer om problem och uppgifter.

Mer information om att prenumerera på objekt finns i [Prenumerera på objekt i Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Avbeställ utskick från e-post {#unsubscribe-from-items-from-email}

Du kan avbeställa prenumerationer via länken &quot;Avbeställ&quot; i prenumerationens mejl. Tidigare kunde du bara avbryta prenumerationen på ett objekt från Workfront-gränssnittet.

Mer information om hur du avbryter prenumerationen på e-postmeddelanden finns i avsnittet om att välja bort e-postmeddelanden i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Konfigurera hur milstolpar visas i Gantt-schemat {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***KORRIGERING &#x200B;**: Den här funktionen finns inte i förhandsvisningssandlådemiljön. Den planeras släppas vid ett senare datum, under juni 2017.*

Det finns nu två alternativ för att visa information om milstolpar i ett Gantt-schema. Du kan konfigurera någon av eller båda följande milstolpeindikatorer:

* Milstolpediamanter (ikon)

  Den här ikonen visas i Gantt-schemat efter en uppgift som är associerad med en milstolpe.

* Milstolpslinjer

  En linje visas efter en uppgift som är associerad med milstolpen, för alla uppgifter i Gantt-schemat.

Före den här ändringen fanns det bara ett alternativ för att aktivera att milstolpar visas i ett Gantt-schema, som kallas&quot;milstolpar&quot;. Med det här alternativet aktiverades både milstolpdiamantikonen och milstolpslinjen. Dessa indikatorer kunde inte separeras. De två alternativen är nu tillgängliga för alla Gantt-scheman, inklusive alla projektlistor och rapporter. 

Mer information om hur du konfigurerar hur information visas i Gantt-schemat finns i [Konfigurera hur information visas i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Resurspoolmallar {#resource-pools-templates}

Nu kan du ange resurspooler för mallar. Före den här versionen kunde du bara associera resurspooler med användare och projekt.

Mer information om resurspooler finns i [Översikt över resurspooler](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Visa versioner av korrekturdokument i Workfront {#view-versions-of-proofed-documents-within-workfront}

Nu kan du visa korrektur från alla versioner av ett korrekturdokument i Workfront gränssnitt. 

Före den här ändringen kunde du bara visa den senaste versionen av det korrekturlästa dokumentet.

Användare utan korrekturlicens kan:

* Öppna ett korrektur på en tidigare version av ett korrekturdokument

Användare med korrekturlicens kan göra något av följande:

* Öppna ett korrektur på en tidigare version av ett korrekturdokument
* Visa korrekturinformation om en tidigare version av ett korrekturdokument

Mer information finns i [Hantera dokumentversioner](../../../../documents/managing-documents/manage-document-versions.md) i [Hantera dokumentversioner](../../../../documents/managing-documents/manage-document-versions.md).

## Nytt begäranobjekt i korrekturgodkännanderapport {#new-requester-object-in-proof-approval-report}

När du skapar en korrekturgodkännanderapport finns det nu ett nytt begärandeobjekt. Med det här objektet kan du rapportera information om den användare som begärde korrekturgodkännandet. 

Det nya begärandeobjektet i rapporten för korrektur av godkännande innehåller alla fält som är tillgängliga med det befintliga användarobjektet i andra typer av objektrapporter.

>[!NOTE]
>
> Den här informationen är endast tillgänglig i rapporten från den tidpunkt då den här funktionen först introducerades i respektive förhandsgransknings- eller produktionsmiljö. Information i rapporter om objektet Requester innan den här funktionen introducerades är inte tillgänglig.

Du får åtkomst till objektet Begär när du skapar en rapport för godkännande av korrektur, vilket beskrivs i [Skapa en anpassad rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Mer information om objektrapporten för korrekturgodkännanden finns i avsnittet [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) i [Förstå objekt i Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
