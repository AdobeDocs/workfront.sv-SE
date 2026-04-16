---
product-area: documents
navigation-topic: approvals
title: Ta bort godkännare eller granskare från ett arbetsflöde för dokumentgodkännande
description: Du kan ta bort enskilda godkännare eller granskare från ett dokument.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Ta bort godkännare eller granskare från ett arbetsflöde för dokumentgodkännande

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


## Ta bort godkännare eller granskare från ett arbetsflöde för godkännande i det äldre dokumentområdet

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