---
product-area: documents
navigation-topic: approvals
title: Skapa en begäran om dokumentgranskning eller godkännande
description: Du kan begära godkännande från andra användare för ett dokument i Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Skapa en begäran om dokumentgranskning eller godkännande

Du kan begära godkännande från andra användare eller team för ett dokument i Adobe Workfront, eller begära att de granskar ett dokument utan att behöva godkänna det.

>[!IMPORTANT]
>
>Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <td>
   <p>Medarbetare eller högre</p>
   <p>Granska eller högre</p>
   <p>Om du använder Frame.io-integreringen måste du ha en standardlicens för att skapa arbetsflöden för godkännande.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, mallar, portföljer, program, rapporter, instrumentpaneler och kalendrar, dokument</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till objektet som är associerat med åtkomstbegäran eller godkännandet </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en dokumentgranskning eller godkännandebegäran från dokumentsidan

1. Håll muspekaren över dokumentet och klicka sedan på Dokumentinformation.
   ![Dokumentinformation](assets/doc-details.png)

1. I närheten av dokumentnamnet väljer du den version av dokumentet som du vill skapa ett godkännande för i listrutan. Den senaste versionen väljs som standard.

1. Klicka på **Godkännanden** i den vänstra rutan.

1. (Valfritt) Ange en tidsgräns för godkännandet. Användare och team meddelas via e-post 72 timmar, sedan 24 timmar före den angivna tidsgränsen.

1. Om du vill lägga till en godkännare klickar du på **Godkännaren** och börjar skriva in ett användar- eller teamnamn.

1. Om du vill lägga till en granskare klickar du på kryssrutan **Granskare** och börjar skriva in ett användar- eller teamnamn.

   ![Lägg till godkännare och deadline](assets/add-approver-and-deadline.png)

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.

## Skapa en dokumentgranskning eller godkännandebegäran från panelen Dokumentsammanfattning

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningsrutan för det dokumentet.

1. Välj den version av dokumentet som du vill skapa ett godkännande för i listrutan. Den senaste versionen väljs som standard.

1. Bläddra ned till avsnittet **Godkännanden** i rutan Dokumentsammanfattning och klicka sedan på **Lägg till**.

![Lägg till godkännare i dokumentsammanfattning](assets/doc-summary-add-approvers.png)

1. (Valfritt) Ange en tidsgräns för godkännandet. Användare och team meddelas via e-post 72 timmar, sedan 24 timmar före den angivna tidsgränsen.

1. Om du vill lägga till en godkännare klickar du på **Godkännaren** och börjar skriva in ett användar- eller teamnamn.

1. Om du vill lägga till en granskare klickar du på kryssrutan **Granskare** och börjar skriva in ett användar- eller teamnamn.

   ![Lägg till godkännare och deadline](assets/add-approver-and-deadline.png)

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
