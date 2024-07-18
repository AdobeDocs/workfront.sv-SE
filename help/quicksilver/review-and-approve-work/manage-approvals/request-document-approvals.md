---
product-area: documents
navigation-topic: approvals
title: Begär dokumentgodkännanden
description: Du kan begära godkännande från chefer eller andra användare för ett dokument i Adobe Workfront. Du kan också begära dokumentgodkännanden från personer utan Workfront-konton om Workfront-administratören har aktiverat den funktionen, enligt beskrivningen i Konfigurera systemsäkerhetsinställningar.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Begär dokumentgodkännanden

Du kan begära godkännande från chefer eller andra användare för ett dokument i Adobe Workfront. Du kan också begära dokumentgodkännanden från personer utan Workfront-konton om Workfront-administratören har aktiverat den här funktionen, enligt beskrivningen i [Konfigurera systemsäkerhetsinställningar](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

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
   <td> <p>Visa eller ge senare åtkomst till projekt, uppgifter, ärenden, mallar, Portfolio, program, rapporter, kontrollpaneler och kalendrar, dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till objektet som är associerat med åtkomstbegäran eller godkännandet </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

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

   ![](assets/nwe-resubmit-approval-350x149.png)

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
