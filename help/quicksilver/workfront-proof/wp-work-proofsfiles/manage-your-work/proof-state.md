---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Förstå korrekturstatus i Workfront Proof
description: I [!DNL Workfront Proof]finns det korrektur i olika lägen. Dessa lägen avgör vilka åtgärder du kan utföra på beviset, som att kommentera eller fatta beslut.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Förstå korrekturstatus i Workfront Proof

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

I [!DNL Workfront Proof]finns det korrektur i olika lägen. Dessa lägen avgör vilka åtgärder du kan utföra på beviset, som att kommentera eller fatta beslut.

## Förstå korrekturläge

De fyra delstaterna är följande:

* [Aktiv](#active)
* [Låst](#locked)
* [Utkast (endast Dropzone)](#draft-dropzone-only)
* [Skickat (endast Dropzone)](#submitted-dropzone-only)

### Aktiv {#active}

Korrektur som har överförts till [!DNL Workfront Proof] via sidan Nytt korrektur eller Dropzone visas som Aktiv när de har bearbetats. När ett korrektur är aktivt kan användarna granska, kommentera och fatta beslut om korrekturet.

>[!NOTE]
>
>Korrektur som överförs via Dropzone visas bara som aktiva om alternativet Aktivera korrektur vid inskickning är aktiverat. Om alternativet inte är aktiverat måste du aktivera korrekturet manuellt.

Mer information om Dropzone-inställningar finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Låst {#locked}

Du kan låsa ett korrektur när du är klar med granskningen. Att låsa ett korrektur innebär att inga fler kommentarer eller beslut kan fattas om beviset, men det kan fortfarande öppnas.

Alla användare med redigeringsbehörighet för korrekturet kan låsa upp det.

Mer information om rättigheter finns i [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>E-postmeddelanden skickas inte längre när ett korrektur är låst. Om till exempel ett korrektur är låst före dess deadline skickas inget e-postmeddelande när tidsgränsen nås.

### Utkast (endast Dropzone) {#draft-dropzone-only}

När du skickar in ett bevis via Dropzone försätts det i utkastläge innan administratören aktiverar det. När det finns i utkastzonen kan du inte vidta några åtgärder för korrekturet.

### Skickat (endast Dropzone) {#submitted-dropzone-only}

När administratören har aktiverat ett utkast visas ditt bevis som Skickat i Dropzone. När det har skickats kan du vidta åtgärder för beviset.

## Visa och ändra korrekturstatus

Mer information om hur du visar en lista med alla korrektur i ett visst läge, till exempel visa alla aktiva eller låsta korrektur, finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) i artikeln [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Få åtkomst till dina [!DNL Workfront Proof] Instrumentpanel.

   Mer information finns i [Åtkomst [!DNL Workfront Proof] från Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. På **[!UICONTROL Dashboard]** klickar du på **[!UICONTROL Expand]** pilen bredvid det korrektur som du vill visa eller ändra läget för.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   The **[!UICONTROL Workflow process]** visas.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Visa **[!UICONTROL State]** i **[!UICONTROL Workflow process]**.

1. (Valfritt) Om du vill ändra läge för muspekaren över det aktuella läget **[!UICONTROL State]** och klicka på listrutan och välj sedan ett nytt läge.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
