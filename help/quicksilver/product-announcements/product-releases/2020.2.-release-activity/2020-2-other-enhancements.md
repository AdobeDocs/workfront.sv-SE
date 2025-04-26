---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 andra förbättringar
description: Den här sidan beskriver alla andra förbättringar som gjorts i 2020.2-versionen av produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i 2020.2-versionen av produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 maj 2020.

En lista över alla ändringar som är tillgängliga i version 2020.2 finns i [2020.2 versionsöversikt](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## För Workfront-administratörer: Nyare layoutmallar som skapats i Workfront Classic finns nu i den nya Workfront-upplevelsen

Layoutmallar som skapats i Workfront Classic efter hösten 2019 finns nu i den nya Workfront-upplevelsen. Det är en bra idé att uppdatera dessa layoutmallar i den nya Workfront-upplevelsen för att utnyttja de nya funktionerna och göra dem så användbara som möjligt för användare i den miljön.

Mer information finns i [Layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront

## Gruppspecifika godkännandeprocesser är tillgängliga för alla objekt

Om du vill utnyttja gruppspecifika godkännandeprocesser fullt ut kan du nu lägga till dem i uppgifter, ärenden och projekt när du redigerar dessa objekt.

Du kan också automatiskt koppla en gruppspecifik godkännandeprocess till en uppgift i området Åtgärder i rutan Redigera projekt, samt till problem, när du konfigurerar begärandeköer eller Köämnen i ett projekt.

Mer information om hur du lägger till godkännandeprocesser till projekt, uppgifter och problem finns i följande artiklar:

* [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Redigera problem](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Skapa godkännandeprocesser för grupper med anpassade statusvärden

För att göra det enklare för grupper att hantera sina egna unika arbetsflöden kan du nu använda gruppspecifika anpassade statusvärden i godkännandeprocesser.

Tidigare kunde en grupp inte använda sina egna anpassade statusvärden med sina gruppspecifika godkännandeprocesser. Det fanns bara systemomfattande statusar tillgängliga och dessa passade inte alltid in i gruppens godkännandeprocesser.

Anpassade statusvärden kan nu användas både i enstaka och i systemomfattande godkännandeprocesser:

* Skapa en godkännandeprocess för ett objekt (projekt, uppgift eller utgåva) och basera den på statusvärden som är kopplade till gruppen som arbetar med objektet. Detta inkluderar alla anpassade statusvärden som är associerade med gruppen.
* Skapa en global godkännandeprocess och gör den tillgänglig endast för gruppen eller för alla i systemet.

För användare med administrativ åtkomst till godkännandeprocesser finns information om hur du konfigurerar godkännandeprocesser i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (eller om du använder Adobe Workfront Classic, se [Skapa godkännandeprocesser](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

Information om hur du associerar godkännandeprocesser med arbetsobjekt finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (eller om du använder Adobe Workfront Classic, se [Associera en ny eller befintlig godkännandeprocess med arbete](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Tillgängligt i dessa miljöer:**

* Adobe Workfront Classic
* Nya Adobe Workfront

## Nya överläggssidor för sökning

För att användarna enklare ska kunna navigera fram och tillbaka mellan söksidor och tidigare sidor i den nya Workfront-upplevelsen har vi lagt till en sökövertäckningssida som delvis täcker skärmen.

När du klickar på Avancerad sökning på menyn Sök eller utför en grundläggande sökning öppnas nu en sida från skärmens högra sida.

Mer information finns i [Sök i Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Tillgängligt i dessa miljöer:**

* Nya Adobe Workfront

## Uppdateringar av händelseprenumerationer

För att göra det lättare för användare att trigga, felsöka och lösa problem har vi ändrat beteendet och lagt till mer data i API:t för händelseprenumerationer. Vi har även gjort följande ändringar:

* Migrerad underliggande meddelandeteknik
* Ombyggt tjänsten så att den har mindre komplexa beroenden och därmed skalas mer effektivt
* Förbättrade övervaknings- och varningsfunktioner

Mer information finns i [Vanliga frågor och svar - Evenemangsprenumerationer](../../../wf-api/general/event-subs-faq.md) och [Bästa tillvägagångssätt för händelseteckning](../../../wf-api/general/event-sub-best-practice.md).
