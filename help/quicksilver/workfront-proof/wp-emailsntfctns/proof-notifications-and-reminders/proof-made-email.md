---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: E-postmeddelande om korrekturet
description: Ett e-postmeddelande om korrekturutskrift skickas till den som skapat beviset endast när han eller hon har skapat ett bevis. Om en person har skapat ett bevis och gjort en annan person till ägare, är det bara den nya ägaren som får det korrekturutskick som har gjorts via e-post. Skaparen och/eller ägaren får ingen; de får bara e-postmeddelandet Korrektur gjort. Mer information om e-postmeddelandet Nytt korrektur finns i Nytt korrekturmeddelande.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# E-postmeddelandet [!UICONTROL Proof Made]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Ett [!UICONTROL Proof Made]-e-postmeddelande skickas endast till den som skapade korrekturet när han eller hon har skapat ett bevis. Om en person har skapat ett bevis och gjort en annan person till ägare, får endast den nya ägaren e-postmeddelandet [!UICONTROL Proof made]. Skaparen och/eller ägaren får ingen; de får bara e-postmeddelandet [!UICONTROL Proof Made]. Mer information om e-postmeddelandet [!UICONTROL New Proof] finns i [[!UICONTROL New proof] email ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Användare kan inaktivera [!UICONTROL Proof Made]-e-post i sina profilinställningar enligt nedan.

>[!NOTE]
>
> Om den som skapat eller äger korrekturet har [!UICONTROL Proof Made] e-postmeddelanden inaktiverade som standard i sina personliga inställningar, får de inga [!UICONTROL Proof Made]- eller [!UICONTROL New Proof]-e-postmeddelanden, även om kryssrutan [!UICONTROL Notify people by email] är markerad på sidan [!UICONTROL New proof] .

![Proof_Made_Email.png](assets/proof-made-email-350x214.png)

Ett [!UICONTROL Proof Made]-e-postmeddelande innehåller ditt personliga meddelande (om du inkluderar ett) och följande korrekturinformation:

* Korrekturnamn
* Personlig länk till beviset
* Versionsnummer
* Miniatyrbild av korrekturet
* Bevis förlopp
* En länk för att dela korrekturet med någon annan
* På så sätt kan du dela korrektur-URL:en och/eller hämtningslänken för originalfilen.

>[!NOTE]
>
> Genom att dela korrekturlänkar kan du inte uttryckligen lägga till granskare i korrekturet, du delar bara det offentliga korrektur-URL:en och mottagaren får skrivskyddad åtkomst till korrekturet.

Mer information finns i [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

Om du inte vill att den här länken ska visas i mottagarens e-post bör du inaktivera inställningarna för [!UICONTROL Public sharing] i korrekturet ([!UICONTROL Download original file] och [!UICONTROL Public URL]).

## Inaktiverar e-postmeddelandet [!UICONTROL Proof Made]

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**, öppna fliken **[!UICONTROL Proofing defaults]** och klicka sedan på **[!UICONTROL Disable]** bredvid **[!UICONTROL Email confirmation when proofs are ready]**.

1. ![Proof_Made_-_proofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. Mer information finns i [Konfigurera inställningar för e-postmeddelanden i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).
1. Om e-postmeddelandena är inaktiverade som standard i [!UICONTROL Account settings] får inte författaren eller ägaren av beviset några [!UICONTROL Proof Made]- eller [!UICONTROL New Proof]-e-postmeddelanden, även om detta är aktiverat i deras personliga inställningar och kryssrutan [!UICONTROL Notify people by email] är markerad på sidan [!UICONTROL New proof] .
