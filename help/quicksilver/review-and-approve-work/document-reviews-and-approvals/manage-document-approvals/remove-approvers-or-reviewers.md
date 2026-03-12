---
product-area: documents
navigation-topic: approvals
title: Ta bort godkännare eller granskare från ett arbetsflöde för dokumentgodkännande
description: Du kan ta bort enskilda godkännare eller granskare från ett dokument.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Ta bort godkännare eller granskare från ett arbetsflöde för dokumentgodkännande

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Du kan ta bort enskilda godkännare eller granskare från en resurs eller ett dokument när de har tilldelats.

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
   <td> <p>Hantera åtkomst till objektet som är associerat med åtkomstbegäran eller godkännandet </p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Ta bort godkännare eller granskare från sidan Dokumentinformation i produktionsmiljön

1. Gå till dokumentsidan genom att klicka på dokumentets namn och markera sedan den version av dokumentet som du vill ta bort ett godkännande för i versionslistan. Den senaste versionen är markerad som standard.

1. Välj **Godkännanden** på den vänstra panelen.

1. Håll muspekaren över namnet på den godkännare eller granskare som du vill ta bort och klicka sedan på ikonen **Ta bort** ![Ta bort &#x200B;](../assets/delete.png) som visas efter namnet.

   Godkännandet eller granskningsbegäran tas bort och godkännaren får ett meddelande om att deras godkännande inte längre behövs. Deras godkännanderelaterade resursåtkomst tas också bort.

1. (Valfritt) Om du vill nedgradera en godkännare till en granskare i stället för att ta bort dem helt, avmarkerar du kryssrutan **Godkännare** enligt deras namn.

1. Upprepa föregående steg om du vill ta bort ytterligare godkännare eller granskare.

## Ta bort godkännare eller granskare från dokumentsammanfattningen i produktionsmiljön

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningspanelen för det dokumentet.

1. Välj den version av dokumentet som du vill ta bort en godkännare eller granskare för i listrutan för version. Den senaste versionen är markerad som standard.

1. Bläddra ned till avsnittet **Godkännanden** på panelen Dokumentsammanfattning. Håll muspekaren över namnet på den godkännare eller granskare som du vill ta bort och klicka sedan på ikonen **Ta bort** ![Ta bort &#x200B;](../assets/delete.png) som visas efter namnet.

   Godkännandet eller granskningsbegäran tas bort och godkännaren får ett meddelande om att deras godkännande inte längre behövs. Deras godkännanderelaterade resursåtkomst tas också bort.

1. (Valfritt) Om du vill nedgradera en godkännare till en granskare i stället för att ta bort dem helt, avmarkerar du kryssrutan **Godkännare** enligt deras namn.

1. Upprepa föregående steg om du vill ta bort ytterligare godkännare eller granskare.


<div class="preview">

## Ta bort godkännare eller granskare från ett arbetsflöde för godkännande i förhandsgranskningsmiljön i det äldre dokumentområdet

Om ditt företag använder Workfront-lagring visas det äldre dokumentområdet när du öppnar dokument i Workfront. Mer information om Workfront-lagring finns i [Workfront-lagring jämfört med Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Så här tar du bort godkännare eller granskare från ett arbetsflöde för godkännande:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.

1. Klicka på det dokument du behöver så öppnas dokumentsammanfattningspanelen för det dokumentet.

1. Bläddra ned till avsnittet **Godkännanden** på panelen Dokumentsammanfattning.

1. Klicka på **Redigera arbetsflöde**.

1. Leta reda på deltagaren som du vill ta bort och klicka sedan på ikonen **Ta bort** bredvid namnet.

   Godkännandet eller granskningsbegäran tas bort och godkännaren får ett meddelande om att deras godkännande inte längre behövs. Deras godkännanderelaterade resursåtkomst tas också bort.

   ![redigera arbetsflöde för godkännande](assets/edit-approval-in-legacy.png)

1. (Valfritt) Om du vill ändra rollen för en godkännare till en granskare, eller vice versa, klickar du på den nedrullningsbara menyn bredvid användarnamnet och väljer den nya rollen.

1. Upprepa föregående steg om du vill ta bort ytterligare godkännare eller granskare.

</div>


## Ta bort godkännare eller granskare från ett arbetsflöde för godkännande i det nya dokumentområdet

Om ditt företag använder Enterprise-lagring visas det nya dokumentområdet när du öppnar dokument i Workfront. Mer information om Enterprise-lagring finns i [Översikt över Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

Så här skapar du ett arbetsflöde för godkännande:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument** i den vänstra panelen.

1. Klicka på dokumentet och sedan på ikonen **Godkännanden** till höger på sidan.

   ![Lägg till godkännare i dokumentsammanfattning](assets/approvals-icon-new.png)


1. Klicka på **Redigera arbetsflöde**.

1. Leta reda på deltagaren som du vill ta bort och klicka sedan på ikonen **Ta bort** bredvid namnet.

   Godkännandet eller granskningsbegäran tas bort och godkännaren får ett meddelande om att deras godkännande inte längre behövs.

1. (Valfritt) Om du vill ändra rollen för en godkännare till en granskare, eller vice versa, klickar du på den nedrullningsbara menyn bredvid användarnamnet och väljer den nya rollen.

1. Upprepa föregående steg om du vill ta bort ytterligare godkännare eller granskare.

   ![ta bort deltagare från en scen](assets/add-or-remove-participants.png)
1. Klicka på **Spara**.