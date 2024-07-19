---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurera dropzone i [!DNL Workfront Proof]
description: Som  [!DNL Workfront Proof] administratör kan du ange, visa och redigera dina användares Dropzone-inställningar. Mer information om Dropzone finns i Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Konfigurera dropzone i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Som [!DNL Workfront Proof]-administratör kan du ange, visa och redigera dina användares Dropzone-inställningar. Mer information om Dropzone finns i [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Dropzone]**.

1. Gör någon av följande ändringar i avsnittet **[!UICONTROL Dropzone details]**:

   * **[!UICONTROL Web Dropzone]**: Aktivera eller inaktivera Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: Den URL som du måste ange i webbläsaren för att skicka in korrektur via Dropzone.
   * **[!UICONTROL Email Dropzone]**: Aktivera eller inaktivera Dropzone för e-post.

     >[!NOTE]
     >
     >E-post till dropzone stöds inte längre.

   * **[!UICONTROL Dropzone Owner]**: Ange eller redigera Dropzone-ägaren. Detta är den person som kommer att underrättas om nya ansökningar till Dropzone. För att anges som Dropzone-ägare måste användaren vara supervisor, Admin, Billing Admin eller Account Creator. Mer information finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Default role for creators]**: Alla avsändare läggs till i korrekturet med den här rollen som standard.
   * **[!UICONTROL Email notification for all creators]**: Ange e-postaviseringsinställningen för korrekturläsare (avsändare) här. Mer information om de olika varningsinställningarna finns i [Konfigurera e-postaviseringsinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   * **[!UICONTROL New version function]**: Aktivera och inaktivera funktionen Ny version i Dropzone. Detta ger eller tar bort möjligheten för människor att skicka in nya versioner av korrektur via Dropzone.
   * **[!UICONTROL Delete draft proofs after (days)]**: Ange antalet dagar efter vilka ett utkast till korrektur ska tas bort. Korrektur är i utkastläge om Dropzone-överföringen inte slutförs efter att filen har överförts till Dropzone.
   * **[!UICONTROL Hide reviewer role]**: Dölj rollfältet för granskare när personer läggs till i Dropzone.
   * **[!UICONTROL Send proof message on activation]**: Konfigurera [!DNL Workfront Proof] så att korrekturmeddelanden skickas till granskarna automatiskt när ett korrektur aktiveras.
   * **[!UICONTROL Activate proof on submission]**: Konfigurera [!DNL Workfront Proof] så att korrektur aktiveras automatiskt när de skickas in (så att de inte behöver aktiveras manuellt).

   * Om ett korrektur flyttas ut från Dropzone (till exempel till en annan mapp på ditt konto) gäller Dropzone-inställningarna inte längre för korrekturet. Detta är särskilt viktigt när det gäller e-postaviseringsinställningar.

1. Gör eventuella ändringar i avsnittet **[!UICONTROL Dropzone fields]** för att ange vilka fält som ska visas i avsnittet [!UICONTROL Proof details] på Dropzone-sändningssidan när korrektur skickas via Dropzone.
1. I avsnittet **[!UICONTROL Permitted domains]** anger du domäner som du vill ska kunna använda Dropzone.

   * Du kan klicka på **[!UICONTROL Add domain]** om du vill lägga till en domän. När du har lagt till domäninformationen klickar du på **[!UICONTROL Save]**.

   * Du kan **[!UICONTROL Edit]** och **[!UICONTROL Delete]** alla befintliga domäner som du tidigare har lagt till.

1. Under **[!UICONTROL People to notify]** anger du de personer som du vill ska meddelas tillsammans med Dropzone-ägaren när nya korrektur skickas till Dropzone [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Klicka på **[!UICONTROL Add people]**, ange mottagarens information och klicka sedan på **[!UICONTROL Save]**.

   * **[!UICONTROL Delete]** personer som du tidigare har lagt till.
