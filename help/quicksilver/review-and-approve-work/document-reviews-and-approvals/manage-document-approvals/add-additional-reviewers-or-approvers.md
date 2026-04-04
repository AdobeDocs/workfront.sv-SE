---
product-area: documents
navigation-topic: approvals
title: Lägga till ytterligare godkännare eller granskare i ett arbetsflöde för dokumentgodkännande
description: Du kan lägga till ytterligare godkännare eller granskare i ett dokument som redan har väntande godkännanden.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Lägga till ytterligare godkännare eller granskare i ett arbetsflöde för dokumentgodkännande

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Du kan lägga till ytterligare godkännare eller granskare i ett arbetsflöde för dokumentgodkännande som redan har väntande godkännanden.

>[!IMPORTANT]
>
>Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
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
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, mallar, portföljer, program, rapporter, instrumentpaneler, kalendrar och dokument</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller öka åtkomsten till objektet som är associerat med åtkomstbegäran eller godkännandet </p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Lägg till ytterligare godkännare eller granskare från sidan Dokumentinformation i produktionsmiljön

1. Gå till dokumentsidan genom att klicka på dokumentets namn och markera sedan den version av dokumentet som du vill lägga till en godkännare eller granskare i den nedrullningsbara menyn version. Den senaste versionen är markerad som standard.

1. Välj **Godkännanden** på den vänstra panelen. Alla befintliga godkännare och granskare listas här.

1. Om du vill lägga till en godkännare markerar du kryssrutan **Godkännare** och börjar sedan skriva i textrutan **Granskare**. Du kan lägga till Workfront-användare eller -team efter namn. Om du vill lägga till en granskare i stället avmarkerar du kryssrutan **Godkännare** innan du skriver.

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.

## Lägg till ytterligare godkännare eller granskare från Dokumentsammanfattning i produktionsmiljön

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningspanelen.

1. Välj den version av dokumentet som du vill lägga till en godkännare eller granskare i listrutan för versionen. Den senaste versionen är markerad som standard.

1. Bläddra ned till avsnittet **Godkännanden** på panelen Dokumentsammanfattning, där alla befintliga godkännare och granskare listas. Om du vill lägga till en godkännare markerar du kryssrutan **Godkännare** och börjar sedan skriva i textrutan **Granskare**. Du kan lägga till Workfront-användare eller -team efter namn. Om du vill lägga till en granskare i stället avmarkerar du kryssrutan **Godkännare** innan du skriver.

1. Upprepa föregående steg om du vill lägga till ytterligare godkännare eller granskare.

<div class="preview">

## Lägg till ytterligare godkännare eller granskare från dokumentsammanfattningen i förhandsgranskningsmiljön i det äldre dokumentområdet

Om ditt företag använder Workfront-lagring visas det äldre dokumentområdet när du öppnar dokument i Workfront. Mer information om Workfront-lagring finns i [Workfront-lagring jämfört med Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Så här lägger du till ytterligare godkännare eller granskare från Dokumentsammanfattning:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningspanelen för det dokumentet.

1. Välj den version av dokumentet som du vill lägga till en godkännare eller granskare i listrutan för versionen. Den senaste versionen är markerad som standard.

1. Bläddra ned till avsnittet **Godkännanden** och klicka sedan på **Redigera arbetsflöde**.

   ![redigera arbetsflöde för godkännande](assets/edit-approval-in-legacy.png)

1. Leta reda på den scen som du vill lägga till godkännare eller granskare i och lägg sedan till användarens namn eller e-postadress i textrutan. Du kan även lägga till ett helt team vid behov.

1. När namnet har lagts till väljer du om de är godkännare eller granskare.

   ![listrutan Godkännare eller granskare](assets/choose-approver-or-reviewer.png)

1. Upprepa steg 5-6 för att lägga till ytterligare godkännare eller granskare.
När du har sparat får deltagarna som lagts till ett e-postmeddelande om att de behöver godkänna eller granska dokumentet.

</div>


## Lägg till ytterligare godkännare eller granskare från dokumentsammanfattningen i området för nya dokument

Om ditt företag använder Enterprise-lagring visas det nya dokumentområdet när du öppnar dokument i Workfront. Mer information om Enterprise-lagring finns i [Översikt över Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.

1. Klicka på dokumentet och sedan på ikonen **Godkännanden** till höger på sidan.

   ![Lägg till godkännare i dokumentsammanfattning](assets/approvals-icon-new.png)


1. Klicka på **Redigera arbetsflöde**.

1. Leta reda på den scen som du vill lägga till godkännare eller granskare i och lägg sedan till användarens namn eller e-postadress i textrutan. Du kan även lägga till ett helt team vid behov.

1. När namnet har lagts till väljer du om de är godkännare eller granskare.

   ![listrutan Godkännare eller granskare](assets/choose-approver-or-reviewer.png)

1. Upprepa steg 5-6 för att lägga till ytterligare godkännare eller granskare.
När du har sparat får deltagarna som lagts till ett e-postmeddelande om att de behöver godkänna eller granska dokumentet.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
