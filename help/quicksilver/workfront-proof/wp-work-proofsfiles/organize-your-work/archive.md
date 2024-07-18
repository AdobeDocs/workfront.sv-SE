---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Arkivera i Workfront Proof
description: Workfront Proof arkiverar korrektur efter 60 dagars inaktivitet.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 66a15edf-8504-471a-a6be-f632760b50ed
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Arkivera i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] arkiverar korrektur efter en period på 60 dagar av inaktivitet.

Om du har redigeringsbehörighet kan du när som helst arkivera ett bevis manuellt. Mer information om redigeringsrättigheter finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

Arkiverade korrektur:

* Visas endast i vyn Arkiverade korrektur på sidan Vyer (se&quot;Hur du talar om ett korrektur är arkiverat&quot; nedan)
* Lämna ditt konto på obestämd tid (såvida de inte tas bort)
* Kan inte arkiveras av vem som helst när som helst (inklusive granskare som inte är [!DNL Workfront Proof] användare)
* Räkna med din lagringsgräns
* Lås automatiskt när de arkiveras automatiskt
* Kan låsas eller låsas upp vid manuell arkivering

Arkivering och avarkivering loggas i avsnittet Aktivitet i korrekturet. Mer information finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

>[!NOTE]
>
>Du kan inte arkivera filer och mappar.

## Arkivera korrektur manuellt

Om du har redigeringsbehörighet kan du när som helst arkivera ett bevis manuellt. Mer information om redigeringsrättigheter finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

Det kan ta upp till 24 timmar innan arkiveringsprocessen är klar.

1. Markera kryssrutan för varje korrektur som du vill arkivera på kontrollpanelen eller i en listvy (mer information om listvyer finns i [Hantera objekt på vysidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)).

1. Välj **[!UICONTROL More]** > **[!UICONTROL Archive]**.\
   Meddelanderutan [!UICONTROL Archive proofs] visas.

1. Klicka på ett alternativ för att ange om du vill att korrekturet ska vara låst eller olåst när det arkiveras.\
   [!DNL Workfront Proof] arkiverar korrekturet med det låsalternativ som du anger.

## Visar arkiverade korrektur

Ett arkiverat korrektur visas bara i **[!UICONTROL Archived proofs]**-vyn, med arkiveringsikonen till höger om korrekturnamnet.

Så här visar du den arkiverade korrekturvyn:

1. Klicka på **[!UICONTROL Views]** och sedan på **[!UICONTROL All items]** > **[!UICONTROL Archived proofs]**.

   När du klickar på namnet på ett arkiverat korrektur i den här listan visas sidan [!UICONTROL Proof details] med en **[!UICONTROL Unarchive]**-knapp högst upp på sidan.

   Om du dessutom expanderar avsnittet **[!UICONTROL Activity]** på den här sidan kan du visa en post som talar om när beviset arkiverades och vem som arkiverade det.\
   ![Archived_proof_Activity_expanded.png](assets/archived-proof-activity-expanded-350x77.png)\
   Om avsnittet **[!UICONTROL Activity]** inte visar ett namn på den användare som arkiverade beviset innebär det att beviset arkiverades automatiskt efter 60 dagars inaktivitet.\
   Om du vill visa innehållet i ett arkiverat korrektur måste du först arkivera det.

## Ej arkiverande korrektur

Vem som helst kan när som helst arkivera ett bevis. Detta inkluderar granskare som inte är [!DNL Workfront Proof] användare.

Så här avarkiverar du ett korrektur från vyn Arkiverade korrektur:

1. Klicka på **[!UICONTROL Views]** och sedan på **[!UICONTROL All items]** > **[!UICONTROL Archived proofs]**.

1. Klicka i kryssrutan bredvid de korrektur eller korrektur som du vill avarkivera.
1. Klicka på **[!UICONTROL More]** och sedan på **[!UICONTROL Unarchive]** på menyn som visas.\
   Ett meddelande visas högst upp på sidan om att ditt korrektur inte arkiveras.
