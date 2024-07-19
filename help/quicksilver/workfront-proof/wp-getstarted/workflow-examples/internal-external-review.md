---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: Intern och sedan extern granskning i  [!DNL Workfront Proof]
description: Lär dig använda Workfront Proof för granskningar utanför er organisation.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: 153951e3bba91d67bcfe5fbf22c0970743f0dc6e
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Intern och sedan extern granskning i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om din organisation slutför interna granskningar innan korrektur delas med klienter föreslår vi två sätt att du kan använda [!DNL Workfront Proof] för att förbättra ditt arbetsflöde:

## Klienter ser interna kommentarer

Det här alternativet illustrerar ett arbetsflöde där klienterna kan se alla interna kommentarer.

Designern delar korrekturet med projektledaren (och andra kollegor) först. Kollegorna granskar korrekturet och om de godkänner det kan du använda delningsfunktionen för att dela korrekturet med dina kunder. Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

![internal_external_-_option_A.png](assets/internal_external_-_option_A.png)

1. **Skapa ett nytt korrektur** - designern skapar ett nytt korrektur i [!DNL Workfront Proof] och delar det med interna granskare. Designern gör projektledaren till ägare av beviset.
1. **Intern granskning** - Projektledaren och andra kollegor granskar korrekturet.
1. **Dela korrektur** - projektledaren delar korrekturet med klienten.
1. **Nytt korrekturmeddelande** - klienten får det nya korrekturmeddelandet med länken [!UICONTROL Go to proof]. Mer information finns i [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **Granska korrektur** - kunden granskar korrekturet, lägger till kommentarer och fattar ett beslut.
1. **E-postavisering** - Project Manager får en e-postavisering (beroende på inställningarna för korrekturet). Mer information finns i [Konfigurera inställningar för e-postmeddelanden i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

1. **Ändringsbegäran** - Med Project Manager kan designern få information om ändringsbegäranden. Detta kan du göra med funktionen Skriv ut kommentarer. Mer information finns i [Skriv ut och exportera kommentarer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Ny version** (om det behövs) - designern ändrar filen och överför den till [!DNL Workfront Proof] som en ny version. Mer information finns i .

Du kan upprepa den här processen tills korrekturet har godkänts.

## Kunden ser bara sin egen version

Det här alternativet illustrerar ett arbetsflöde där korrekturläsningsprocessen hanteras av projektledaren som skapar nya versioner (efter behov) och delar korrekturet med kunden. Designern behöver inte delta i granskningsprocessen.)

![internal_external_-_option_B.png](assets/internal_external_-_option_B.png)

1. **Skapa ett nytt korrektur** - Designern skapar ett nytt korrektur i [!DNL Workfront Proof] och delar det med interna granskare. Designern gör Project Manager till ägare av beviset eller ger honom alternativt rollen [!UICONTROL Author] på korrekturet (se [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

1. **Intern granskning** - Projektledaren och andra kollegor granskar korrekturet. Mer information finns i [Granska korrektur i Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) och [Granska korrektur i Desktop Proofing Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)

1. **Ny version** - Project Manager skapar en ny version (eller en kopia) av beviset och delar det med klienten. Se [Kopiera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) och [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

1. **Nytt korrekturmeddelande** - klienten får det nya korrekturmeddelandet med en [!UICONTROL Go to proof]-länk. Mer information finns i [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **[!UICONTROL Review proof]** - kunden granskar korrekturet, lägger till kommentarer och fattar ett beslut.
1. Kunden kan bara se den version av beviset som uttryckligen har delats med dem. De kan inte se den interna versionen.
1. **[!UICONTROL Email alert]** - Project Manager får ett e-postmeddelande med en sammanfattning av klientens granskning (beroende på inställningarna för korrekturet).
1. **Ändringsbegäran** - Med Project Manager kan designern få information om ändringsbegäranden. Detta kan du göra med funktionen Skriv ut kommentarer. Mer information finns i [Skriv ut och exportera kommentarer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Ny version** (om det behövs) - designern ändrar filen och överför den till [!DNL Workfront Proof] som en ny version. Mer information finns i .

Du kan upprepa den här processen tills korrekturet har godkänts.
