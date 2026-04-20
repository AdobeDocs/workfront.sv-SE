---
product-area: documents
navigation-topic: approvals
title: Kom igång med Workfront Content Reviewer
description: Använd Workfront Content Reviewer AI Collaborator för att utvärdera innehåll mot varumärkesriktlinjer under gransknings- och godkännandearbetsflöden.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 72fa86e6dc653905181603e0111f65eb0ca5965b
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Kom igång med Workfront Content Reviewer

Content Reviewer är en AI-samarbetspartner, en typ av AI-agent som kan läggas till i projekt, uppgifter och dokument. AI-samarbetspartners kan konfigureras under Konfigurera och tilldelas precis som användare.

I Workfront hjälper Content Reviewer till att öka innehållets hastighet och förbättra varumärkesefterlevnaden under gransknings- och godkännandeprocessen. Du kan lägga till innehållsgranskare i godkännandemallar eller inkludera dem i enskilda gransknings- och godkännandebegäranden.

## Åtkomstkrav

Om du vill konfigurera innehållsgranskare i Workfront måste du vara systemadministratör.

Alla användare kan lägga till Content Reviewer i en gransknings- och godkännandebegäran.

## Krav

* Enhetliga godkännanden måste vara aktiverat för din Workfront-instans.
* Din organisation måste ha GenStudio Foundation.
   * Content Reviewer i Workfront innehåller de funktioner som är tillgängliga i GenStudio Foundation för granskning och godkännande av resurser. Du behöver inte komma åt GenStudio Foundation direkt för att slutföra arbetet. Din åtkomst till GenStudio Foundation-funktioner via Content Reviewer följer villkoren i ditt Workfront-avtal.
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands.
Mer information om hur du signerar avtalet finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* Content Reviewer är inte tillgängligt i sandlådemiljöer.


## Filtyper som stöds {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Filtypen stöds inte"
>abstract="Denna Content Reviewer stöder inte den valda filtypen. Överför en filtyp som stöds eller ta bort Content Reviewer för att skicka begäran."

Content Reviewer kan granska följande filtyper:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* Icke-animerad GIF (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Om du överför en filtyp som inte stöds är alternativet Content Reviewer inte tillgängligt när du skapar ett arbetsflöde för godkännande.

## Ställ in varumärkesriktlinjer

Workfront Content Reviewer använder varumärkesriktlinjerna när du granskar ditt innehåll. Workfront-administratörer kan ange riktlinjer för varumärken under Konfigurera i Workfront. Varumärken som skapats i GenStudio Foundation finns också i Workfront.

För att kunna följa varumärkesriktlinjerna måste systemadministratören

1. [Ge åtkomst till varumärkesbehörigheter](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Skapa och hantera varumärken för Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Skapa innehållsgranskare

När minst ett varumärke har konfigurerats kan Workfront-administratörer börja skapa Content Reviewers under Setup. Du kan skapa flera innehållsgranskare som fokuserar på olika riktlinjer:

* **Bild**: Den här Content Reviewer granskar resursen mot de riktlinjer för bildvarumärken som du har konfigurerat i Workfront. [!BADGE Beta]{type=Positive tooltip="Den här funktionen är för närvarande i betaversion."}
   * Systemadministratörer måste signera betaavtalet för att aktivera den här funktionen.
* **Varumärkesröst**: Content Reviewer granskar resursen mot de riktlinjer för varumärkesröst som du har ställt in i Workfront.

Granskarna kan sedan tilldelas till mallar för godkännande och enskilda gransknings- och godkännandebegäranden.

Mer information finns i [Konfigurera AI-medarbetare](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Lägg till innehållsgranskare för att granska och godkänna förfrågningar

Användare kan lägga till innehållsgranskare i befintliga godkännandemallar eller i enskilda gransknings- och godkännandebegäranden.

### Godkännandemallar

Om din organisation ofta lägger till samma personer för att granska och godkänna begäranden, kan standardlicensanvändare skapa godkännandemallar under Konfigurera i Workfront.

Användare kan lägga till innehållsgranskare i godkännandemallar för att automatiskt kontrollera varumärkesefterlevnaden när en mall används för att skapa en begäran.

När du har skapat en mall för godkännande kan du använda den för resurser i området Dokument i ett projekt, en uppgift eller en utgåva.

Mer information finns i [Skapa en arbetsflödesmall för godkännande för dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![malllista med AI-granskare](assets/ai-review-templates.png)

### Individuell begäran om granskning och godkännande

När användare skapar enskilda gransknings- och godkännandeförfrågningar kan de lägga till en Content Reviewer i med andra deltagare eller skapa en enda förfrågan med enbart Content Reviewer för att kontrollera varumärkesefterlevnaden.

Mer information finns i [Skapa ett arbetsflöde för dokumentgodkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Innehållsgranskare har lagts till i en enskild godkännandebegäran](assets/new-stage.png)

## Visa Content Reviewer-poäng och feedback

Sekunder efter att gransknings- och godkännandebegäran med en Content Reviewer har skickats är poängen och kommentarerna från Content Reviewer tillgängliga på panelen Dokumentsammanfattning, även om andra deltagare fortfarande granskar och fattar beslut.

Godkännandeägare får också ett e-postmeddelande som meddelar dem om att en granskning har slutförts av resursen. Klicka på **Gå till granskning** i e-postmeddelandet och se poängen och feedback i Workfront.

Content Reviewer är inte avsedd som beslutsfattare i arbetsflödet för granskning och godkännande. Det ger bara poäng och rekommendationer för att anpassa resursen efter de angivna varumärkeskraven.

Om resursen inte uppfyller varumärkesriktlinjerna kan den som skapar resursen överföra en ny version och den som ansvarar för godkännandet kan skapa en andra gransknings- och godkännandebegäran med Content Reviewer.

Mer information om hur du visar bakgrundsmusik och feedback finns i [Visa bakgrundsmusik och feedback för Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

