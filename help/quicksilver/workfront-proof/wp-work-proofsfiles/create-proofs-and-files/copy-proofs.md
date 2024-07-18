---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Kopierar korrektur i  [!DNL Workfront Proof]
description: Granskare med redigeringsbehörighet för ett korrektur kan skapa en kopia av korrekturet, antingen som en ny version av det befintliga korrekturet eller som ett nytt korrektur. (Mer information finns i . Mer information om redigeringsrättigheter finns i Korrekturbehörighetsprofiler i Workfront Proof.)
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7d2db918-ebf0-4c52-9039-54c3eb5515f0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Kopierar korrektur i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Granskare med redigeringsbehörighet för ett korrektur kan skapa en kopia av korrekturet, antingen som en ny version av det befintliga korrekturet eller som ett nytt korrektur. (Mer information finns i . Mer information om redigeringsrättigheter finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Granskarna som fanns på det ursprungliga korrekturet visas automatiskt i avsnittet [!UICONTROL Share] på sidan [!UICONTROL Copy proof], men de kan tas bort. Om en granskare tas bort, kvarstår deras kommentarer.

>[!NOTE]
>
>En kopia av ett korrektur räknas mot din månadsgräns för korrektur. Om kopian skapas som en ny version inkluderas den i antalet versionsuppsättningar. Mer information finns i [Hantera korrekturversioner i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-versions.md).

## Kopiera ett korrektur

1. Gå till någon av **[!UICONTROL Views]**-sidorna enligt beskrivningen i [Hantera objekt på vysidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Öppna **[!UICONTROL More]**-menyn för korrekturet.\
   ![](assets/more-button-small.png)

1. Välj **[!UICONTROL Copy]** i listrutan.
1. På sidan **[!UICONTROL Copy proof]** som visas anger du om du vill skapa kopian som en ny version av det befintliga korrekturet eller som ett nytt korrektur.\
   Som standard är namnet på din kopia&quot;Kopia av [det ursprungliga korrekturnamnet]&quot;.

1. (Valfritt) Om du vill byta namn på ditt kopieringskorrektur skriver du en ny **[!UICONTROL Proof name]**.
1. (Valfritt) Gör något av följande i avsnittet **[!DNL Share]**:

   * Lägg till granskare i korrekturet. Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md). Mer information om hur du lägger till grupper i ett korrektur finns i [Lägg till grupper i ett korrektur](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md).

   * Tilldela en granskare en korrekturroll. Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
   * Ange e-postaviseringar för granskare. Mer information finns i [Konfigurera inställningar för e-postmeddelanden i [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).
   * Ange en deadline.
   * Ange om du vill skicka ett e-postmeddelande. Mer information finns i [Korrekturmeddelanden och påminnelser.](https://support.workfront.com/hc/en-us/sections/115000920788-Proof-notifications-and-reminders)
   * Inkludera ett anpassat ämne och meddelande i e-postmeddelandet.

1. Gör något av följande i avsnittet **[!UICONTROL Organize]**:

   * Lägg till korrekturet i en mapp. Mer information finns i [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).
   * Om mappen delas kontrollerar du listan med personer som mappen delas med. Mer information finns i [Dela mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).
   * Använd en eller flera taggar på korrekturet. Mer information finns i [Skapa och hantera taggar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).

1. I avsnittet **[!UICONTROL More]**-inställningar väljer du [Konfigurera korrekturinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md). Mer information finns i [Konfigurera korrekturinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md)De val som görs i det här avsnittet visas på sidan Korrekturinformation (där vissa fält kan redigeras). Mer information finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Observera att du även kan skapa en kopia av ett korrektur på följande platser (om du har den nödvändiga kontobehörighetsprofilen):

* **Språkvisningsprogrammet**. Mer information om korrekturläsare finns i [Granska korrektur i Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) (för statiska korrektur) och [Granska korrektur i Desktop Proofing Viewer](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer) (för interaktiva korrektur).

* **Sidan med korrekturinformation**. Mer information finns i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

* **Sidan Mappinformation**. Mer information finns i [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

* **Valfri listvysida**. Mer information finns i [Hantera objekt på vysidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Kopiera befintliga korrekturinställningar för ett nytt korrektur

Istället för att behöva välja granskare, arbetsflöden, taggar och mappar om och om igen när du skapar ett nytt korrektur kan du skapa det med inställningar för ett befintligt korrektur. Om det behövs kan du justera inställningarna.

Så här kopierar du befintliga korrekturinställningar för ett nytt korrektur:

1. Gå till någon av **[!UICONTROL Views]**-sidorna enligt beskrivningen i [Hantera objekt på vysidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Öppna **[!UICONTROL More]**-menyn för korrekturet.\
   ![](assets/more-button-small.png)

1. Välj **[!UICONTROL View proof details]** i listrutan.
1. Klicka på **[!UICONTROL More]**.\
   ![More_button_text_version.png](assets/more-button-text-version.png)

1. Klicka på **[!UICONTROL Copy with new file]** i listrutan.
1. På sidan **[!UICONTROL New proof]** som visas överför du en ny fil och klickar sedan på **[!UICONTROL Create]**.
