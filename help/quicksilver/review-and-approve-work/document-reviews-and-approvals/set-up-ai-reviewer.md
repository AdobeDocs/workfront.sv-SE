---
product-area: documents
navigation-topic: approvals
title: Skapa AI-granskare
description: När du har konfigurerat minst ett varumärke i Workfront kan du skapa flera AI-granskare, som du sedan kan tilldela till godkännandemallar och individuella gransknings- och godkännandeförfrågningar.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 551f316bcfd5e0a1390e7be4679e06cd6808e969
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Skapa AI-granskare

>[!NOTE]
>
>Den här funktionen är för närvarande i betaversion.

När du har konfigurerat minst ett varumärke i Workfront kan du skapa flera AI-granskare, som du sedan kan tilldela till godkännandemallar och individuella gransknings- och godkännandeförfrågningar.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara systemadministratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du ange riktlinjer för bildvarumärken i Workfront. Mer information finns i [Skapa och hantera varumärken för Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Lägg till en AI Reviewer

>[!NOTE]
>
>AI Reviewer är inte avsedd som beslutsfattare i arbetsflödet för granskning och godkännande. Det ger bara poäng och rekommendationer för att anpassa resursen efter de angivna varumärkeskraven.

Så här lägger du till en Content Reviewer:

{{step-1-to-setup}}

1. Gå till **Granska och godkänn** > **AI-granskare** i den vänstra panelen.
1. Klicka på **Lägg till ny**.
1. Ge granskaren ett namn.
1. Välj ett **varumärke**.
1. Välj något av följande i listrutan **Stödlinjetyp**:
   * **Bild**: AI Reviewer granskar resursen mot de riktlinjer för bildvarumärken som du har konfigurerat i Workfront.
   * **Varumärkesröst**: AI Reviewer granskar resursen mot de riktlinjer för varumärkesröst som du har ställt in i Workfront.
1. Klicka på **Skapa**.

   När AI Reviewer har skapats kan användare lägga till AI Reviewer i godkännandemallar eller individuella godkännanden.

   Mer information finns i

   * [Skapa en arbetsflödesmall för godkännande av dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Skapa ett arbetsflöde för dokumentgodkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
