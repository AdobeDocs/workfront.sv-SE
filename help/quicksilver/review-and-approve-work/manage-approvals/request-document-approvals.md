---
product-area: documents
navigation-topic: approvals
title: Begär dokumentgodkännanden
description: Du kan begära godkännande från chefer eller andra användare för ett dokument i Adobe Workfront. Du kan också begära dokumentgodkännanden från personer utan Workfront-konton om Workfront-administratören har aktiverat den funktionen, enligt beskrivningen i Konfigurera systemsäkerhetsinställningar.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 2503b6e628e4860a5652c620d8e4d0eea2414443
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Begär dokumentgodkännanden

Du kan begära godkännande från chefer eller andra användare för ett dokument i Adobe Workfront. Du kan också begära dokumentgodkännanden från personer utan Workfront-konton om Workfront-administratören har aktiverat den här funktionen, enligt beskrivningen i [Konfigurera systemsäkerhetsinställningar](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

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
   <p>Contribute eller högre</p>
   <p>Granska eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, mallar, portföljer, program, rapporter, instrumentpaneler och kalendrar, dokument</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till objektet som är associerat med åtkomstbegäran eller godkännandet </p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begär godkännande av dokument

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Hitta det dokument du behöver.

1. Bläddra ned till avsnittet **Godkännanden** i Sammanfattning och börja skriva i textrutan **Lägg till godkännare**. Du kan lägga till Workfront-användare efter namn eller externa användare via e-post.

1. Om Adobe Workfront-administratören har aktiverat möjligheten att samarbeta med personer som inte använder Workfront, vilket beskrivs i [Konfigurera systemsäkerhetsinställningar](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), kan du skriva deras e-postadresser så att de inkluderas.

   Du kan inte begära godkännande från team eller grupper.

1. Upprepa föregående steg om du vill lägga till andra godkännare.

## Skicka ett godkännande på nytt för en ny version

Beslut om dokumentgodkännande återställs inte automatiskt när du överför en ny version. Om dokumentet till exempel godkänns med ändringar visas&quot;ändringar&quot; som beslut, även om du överför en ny version med de angivna ändringarna. Du kan rensa beslutet om en ny version om du skickar in godkännandet manuellt igen.

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Hitta det dokument du behöver.

1. Bläddra ned till avsnittet **Godkännanden** i sammanfattningen, klicka på ikonen Mer och klicka sedan på Skicka igen.

   ![Skicka godkännande igen](assets/nwe-resubmit-approval-350x149.png)

## Ta bort en begäran om dokumentgodkännande

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Hitta det dokument du behöver.

1. Bläddra ned till avsnittet **Godkännanden** i Sammanfattning, klicka på menyn **Mer** inline med godkännarens namn och välj **Ta bort**.

   Godkännandebegäran tas bort och godkännaren får ett meddelande om att deras godkännande inte längre behövs. Deras godkännanderelaterade resursåtkomst tas också bort.

## Skicka en påminnelse till en godkännare

Du kan skicka ett meddelande för att påminna en godkännare om att du väntar på deras feedback.

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Hitta det dokument du behöver.

1. Bläddra ned till avsnittet **Godkännanden** i Sammanfattning, klicka på menyn **Mer** inline med godkännarens namn och välj **Påminn**.

   Godkännaren får ett meddelande som informerar dem om att godkännandet fortfarande väntar. De kan även få en påminnelse via e-post om de har aktiverat detta.
