---
product-area: documents
navigation-topic: approvals
title: Skapa ett dokumentgodkännande
description: Du kan begära godkännande från andra användare för ett dokument i Adobe Workfront.
author: Nolan
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Skapa en begäran om dokumentgodkännande

Du kan begära godkännande från andra användare eller team för ett dokument i Adobe Workfront, eller begära att de granskar ett dokument utan att behöva godkänna det.

>[!IMPORTANT]
>
>Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, mallar, Portfolio, program, rapporter, kontrollpaneler och kalendrar, dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till objektet som är associerat med åtkomstbegäran eller godkännandet </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa ett dokumentgodkännande från dokumentsidan

1. Gå till dokumentsidan genom att klicka på dokumentets namn och välj sedan den version av dokumentet som du vill skapa ett godkännande för i versionsmenyn. Den senaste versionen väljs som standard.

1. Välj **Godkännanden** i den vänstra rutan.

1. Om du vill lägga till en godkännare måste du se till att **Godkännare** kryssrutan är markerad och börjar sedan skriva i **Granskare** textruta. Du kan lägga till Workfront-användare eller -team efter namn. Om du vill lägga till en granskare istället avmarkerar du **Godkännare** innan du skriver.

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.

## Skapa ett dokumentgodkännande från rutan Dokumentsammanfattning

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningsrutan för det dokumentet.

1. Välj den version av dokumentet som du vill skapa ett godkännande för i listrutan. Den senaste versionen väljs som standard.

1. Bläddra nedåt till **Godkännanden** i rutan Dokumentsammanfattning. Om du vill lägga till en godkännare måste du se till att **Godkännare** kryssrutan är markerad och börjar sedan skriva i **Granskare** textruta. Du kan lägga till Workfront-användare eller -team efter namn. Om du vill lägga till en granskare istället avmarkerar du **Godkännare** innan du skriver.

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
