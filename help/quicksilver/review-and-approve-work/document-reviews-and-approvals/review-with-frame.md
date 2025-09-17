---
product-area: documents
navigation-topic: approvals
title: Granska och godkänn med Frame.io-visningsprogrammet
description: Lär dig hur du granskar och godkänner dokument med Frame.io-visningsprogrammet.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 601285fdbf26365dcaea14f990904d049816af21
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---


# Granska och godkänn med Frame.io-visningsprogrammet

Du kan granska och godkänna dokument i Workfront med Frame.io-visningsprogrammet.

Genom att granska Workfront-dokument med Frame.io-visningsprogrammet kan du lämna kommentarer eller kommentera i specifika delar av ett dokument, en bild eller en video för att samarbeta effektivt med teamet och säkerställa att det går att ge tydlig och tydlig feedback.

<!--For more information on the Frame.io integration with Workfront, see [Frame.io integration overview](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Begäran eller senare</p>
   <p>Medarbetare eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till objektet som är associerat med dokumentet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Granska ett dokument

Som granskare kan du lägga till kommentarer och markera resurser. När du är klar kan du markera granskningen som slutförd i Workfront. Att markera granskningen som slutförd krävs inte för att resursen ska gå framåt i godkännandeprocessen.

1. Gå till e-postmeddelandet för din granskning och klicka på **Gå till granskning**.
eller
Gå till Workfront hemsida, leta upp widgeten Mina godkännanden och klicka sedan på **Öppna granskning**.

   >[!NOTE]
   > 
   >Du kan behöva lägga till widgeten Mina godkännanden på hemsidan. Mer information finns i [Lägga till, redigera eller ta bort widgetar i Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).

1. I Frame.io använder du kommentarverktygen för att lämna feedback eller ställa frågor.
Kommentarer och resursmarkeringar visas bara i Frame.io-visningsprogrammet. Mer information om hur du använder Frame.io-visningsprogrammet finns i [Kommentera på dina media](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. När du är nöjd med dokumentet går du tillbaka till sidan Dokumentinformation i Workfront och markerar granskningen som slutförd.

   ![Markeringsgranskningen är klar](assets/mark-review-complete.png)

## Godkänn ett dokument

Som godkännare kan du lägga till kommentarer och kommentera resurser. Du måste fatta ett beslut om att flytta godkännandeprocessen framåt.

Dokumentet flyttas inte till en godkänd status förrän alla tilldelade godkännare väljer&quot;Godkänd&quot;.

Så här fattar du ett beslut om ett dokument:

1. Gå till e-postmeddelandet för din granskning och klicka på **Gå till granskning**.
eller
Gå till Workfront hemsida, leta upp widgeten Mina godkännanden och klicka sedan på **Öppna granskning**.

   >[!NOTE]
   > 
   >Du kan behöva lägga till widgeten Mina godkännanden på hemsidan. Mer information finns i [Lägga till, redigera eller ta bort widgetar i Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).


1. I Frame.io använder du kommentarverktygen för att lämna feedback eller ställa frågor.
Kommentarer och resursmarkeringar visas bara i Frame.io-visningsprogrammet. Mer information om hur du använder Frame.io-visningsprogrammet finns i [Kommentera på dina media](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. När du är nöjd med dokumentet kan du välja något av följande i Frame.io-visningsprogrammet:

   * **Godkänn**: Resursen behöver inte ändras och är klar att användas.
   * **Behöver arbete**: Resursen behöver ändras och är inte klar att användas. När de angivna ändringarna har gjorts måste resursen överföras som en ny version och gå igenom en ny godkännandeomgång. Mer information finns i [Överföra en ny dokumentversion och begära ett godkännande](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md). <!--do they need to tell someone it was uploaded via comment tagging?-->

   När du har fattat ett beslut meddelas dokumentägaren via e-post.

   Mer information om beslut i Workfront finns i [Översikt över dokumentets beslutsstatus](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

   ![Bildrutevisningsprogram och -beslut](assets/make-decision-frame.png)



<!--is document owner the correct term?-->

