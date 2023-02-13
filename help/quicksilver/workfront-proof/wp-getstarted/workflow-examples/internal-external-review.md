---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: Intern och extern granskning i [!DNL Workfront Proof]
description: Om din organisation slutför interna granskningar innan han/hon delar korrektur med kunden föreslår vi två sätt att du kan använda [!DNL Workfront Proof] för att förbättra arbetsflödet - REDIGERA MIG.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: bf6c6c497d98d91ca78f892606a52f82ee4b5666
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Intern och extern granskning i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om din organisation slutför interna granskningar innan han/hon delar korrektur med kunden föreslår vi två sätt att du kan använda [!DNL Workfront Proof] för att förbättra arbetsflödet:

## Klienter ser interna kommentarer

Det här alternativet illustrerar ett arbetsflöde där klienterna kan se alla interna kommentarer.

Designern delar korrekturet med projektledaren (och andra kollegor) först. Kollegorna granskar korrekturet och om de godkänner det kan du använda delningsfunktionen för att dela korrekturet med dina kunder. Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

![internal_external_-_option_A.png](assets/internal-external---option-a-350x86.png)

1. **Skapa ett nytt korrektur** - formgivaren skapar ett nytt korrektur i [!DNL Workfront Proof] och delar med sig av detta till interna granskare. Designern gör projektledaren till ägare av beviset.
1. **Intern granskning** - projektledaren och andra kollegor granskar korrekturet.
1. **Dela korrektur** - projektledaren delar korrekturet med kunden.
1. **Nytt korrekturmeddelande** - klienten får ett e-postmeddelande om det nya korrekturet med [!UICONTROL Go to proof] länk. Mer information finns i [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **Granska korrektur** - kunden granskar korrekturet, lägger till kommentarer och fattar ett beslut.
1. **E-postavisering** - projektledaren får en e-postavisering (beroende på inställningarna för korrekturet). Mer information finns i [Konfigurera e-postmeddelandeinställningar i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

1. **Ändringsbegäran** - projektledaren låter designern få information om ändringsbegäranden. Detta kan du göra med funktionen Skriv ut kommentarer. Mer information finns i [Skriv ut och exportera kommentarer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Ny version** (om det behövs) - designern ändrar filen och överför den till [!DNL Workfront Proof] som en ny version. Mer information finns i .

Du kan upprepa den här processen tills korrekturet har godkänts.

## Kunden ser bara sin egen version

Det här alternativet illustrerar ett arbetsflöde där korrekturläsningsprocessen hanteras av projektledaren som skapar nya versioner (efter behov) och delar korrekturet med kunden. Designern behöver inte delta i granskningsprocessen.)

![internal_external_-_option_B.png](assets/internal-external---option-b-350x86.png)

1. **Skapa ett nytt korrektur** - Designern skapar ett nytt korrektur i [!DNL Workfront Proof] och delar med sig av detta till interna granskare. Designern gör projektledaren till ägare av beviset eller ger honom rollen som [!UICONTROL Author] på korrekturet (se [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

1. **Intern granskning** - projektledaren och andra kollegor granskar korrekturet. Mer information finns i [Granska korrektur i Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) och [Granska korrektur i Desktop Proofing Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)

1. **Ny version** - projektledaren skapar en ny version (eller en kopia) av beviset och delar det med kunden. Se [Kopierar korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) och [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

1. **Nytt korrekturmeddelande** - klienten får ett e-postmeddelande med ett nytt korrektur med [!UICONTROL Go to proof] länk. Mer information finns i [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **[!UICONTROL Review proof]** - kunden granskar korrekturet, lägger till kommentarer och fattar ett beslut.
1. Kunden kan endast se den version av beviset som uttryckligen har delats med kunden. de inte kan se den interna versionen.
1. **[!UICONTROL Email alert]** - projektledaren får ett e-postmeddelande med en sammanfattning av kundens granskning (beroende på inställningarna för korrekturet).
1. **Ändringsbegäran** - projektledaren låter designern få information om ändringsbegäranden. Detta kan du göra med funktionen Skriv ut kommentarer. Mer information finns i [Skriv ut och exportera kommentarer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Ny version** (om det behövs) - designern ändrar filen och överför den till [!DNL Workfront Proof] som en ny version. Mer information finns i .

Du kan upprepa den här processen tills korrekturet har godkänts.
