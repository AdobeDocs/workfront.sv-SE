---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Konfigurera korrekturinställningar i [!DNL Workfront Proof]
description: Du kan konfigurera ett korrektur som du skapar eller redigerar i korrektur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 0%

---

# Konfigurera korrekturinställningar i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan konfigurera ett korrektur som du skapar eller redigerar på något av följande sätt:

>[!NOTE]
>
>Du kan konfigurera de här inställningarna för alla nya korrektur som du skapar. Mer information finns i .

## Lås korrekturet när det senaste beslutet har fattats

Du kan ställa in ett korrekturläge så att det låses när den slutliga godkännaren fattar sitt beslut. Detta är användbart om du vill vara säker på att granskarna inte kan gå tillbaka till korrekturet och lägga till ytterligare kommentarer eller ändra sina beslut.

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Proof settings]**, markera **[!UICONTROL Lock proof when all required decisions are made]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Lock the proof when all decisions are made]**.

Information om beslut finns i [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Kräv inloggning för alla användare som granskar korrekturet

En av de stora sakerna med [!DNL Workfront Proof] är att vem som helst kan granska ett bevis, du behöver inte ha ett eget [!DNL Workfront Proof] att göra det. Mottagarna får ett e-postmeddelande med en personlig URL som tar dem direkt till korrektursidan, utan att de behöver logga in [!DNL Workfront Proof].

Men om du behöver högre säkerhetsnivå för din granskning och godkännandeprocess kan du använda kräv inloggning till korrekturet. Detta innebär att endast [!DNL Workfront Proof] -användare kan läggas till i korrekturet. Och de måste ange sina e-postadresser och lösenord innan de kan komma åt dem.

>[!NOTE]
>
>* *För att någon ska kunna logga in på beviset (när inloggning krävs har aktiverats) måste de ha lagts till i beviset.*
>* *Om inloggning krävs är aktiverad går det inte att aktivera prenumerationer.*

Så här kräver du inloggning för alla användare som granskar korrekturet:

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Proof settings]**, markera **[!UICONTROL Require login]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Login required]**.

## Kräv endast ett beslut för korrektur

Den här inställningen är användbar när du bara behöver en person från en grupp, avdelning eller företag för att fatta ett beslut om beviset.

Även om du tilldelar flera personer rollen som godkännare eller granskare och godkännare uppdateras korrekturens status när en person fattar ett beslut om ett bevis (enligt det beslut som fattats). Mer information om korrekturstatus finns i [Visa förlopp och status för ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Workflow]**, markera **[!UICONTROL Require only one decision for this stage]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Only one decision required]**.

Information om beslut finns i [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Kräv att beslut signeras elektroniskt

Du kan kräva en elektronisk signatur från alla granskare som fattar beslut om beviset för att kunna tillhandahålla sina e-postadresser och lösenord. När en granskare fattar ett beslut visas en uppmaning om att ange e-postadress och lösenord och bekräfta sitt beslut. Mer information finns i [Elektroniska signaturer i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Proof settings]**, markera **[!UICONTROL Require decisions to be electronically signed]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Require decisions to be electronically signed]**.

Information om beslut finns i [Konfigurera alternativ för godkännandebeslut i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Tillåt inte användare att hämta originalfilen

Du kan hålla granskarna på ett korrektur genom att inte hämta originalfilen som korrekturet skapades från.

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Proof settings]**, avmarkera **[!UICONTROL Download original file]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Download of original file]**.

## Tillåt andra användare att prenumerera på korrektur

Prenumerationen är en avancerad inställning som fungerar med Korrektur-URL och Mini-korrektur.

Som standard kan personer som inte har lagts till specifikt i korrekturet och som använder Korrekturens URL eller Mini-korrekturet bara visa korrekturet i skrivskyddat läge. Personer som redan är granskare av beviset kan logga in med sin e-postadress. Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Om du aktiverar prenumeration på korrekturet kan personer som inte har lagts till explicit i beviset prenumerera på själva beviset (d.v.s. lägga till sig själva till beviset). De tilldelas sedan den roll och e-postavisering som du väljer för dem i prenumerationsinställningarna.

Om Prenumeration har aktiverats för ett korrektur aktiveras fälten nedan:

* **[!UICONTROL Subscriber validation required]** - Prenumeranten måste klicka på en länk i ett e-postmeddelande för att få tillgång till ett korrektur\
   Om du väljer det här alternativet får den som prenumererar inte omedelbar åtkomst till korrekturet, utan en länk till korrekturet i ett e-postmeddelande. Syftet med prenumerantvalidering är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till.

* **[!UICONTROL Default role for new subscribers]** - Det här är standardkorrekturrollen som tilldelas alla granskare som abonnerar på korrekturet.
* **[!UICONTROL Default email alert for new subscribers]** - Det här standardmeddelandet som tilldelas alla granskare som abonnerar på korrekturet.

Se även [Prenumerera på ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

Så här tillåter du att andra användare prenumererar på ett korrektur:

1. Skapa ett nytt korrektur enligt beskrivningen i [Generera korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   eller\
   Öppna sidan med korrekturinformation för ett befintligt korrektur enligt beskrivningen i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. För ett nytt bevis, under **[!UICONTROL Proof settings]**, avmarkera **[!UICONTROL Subscribe to proof via public URL or embed code]**.\
   eller\
   För ett befintligt bevis, under **[!UICONTROL Settings]**, markera **[!UICONTROL Subscription]**.
