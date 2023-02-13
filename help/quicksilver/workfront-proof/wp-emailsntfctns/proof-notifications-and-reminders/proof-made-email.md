---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: E-postmeddelande om korrekturet
description: Ett e-postmeddelande om korrekturutskrift skickas till den som skapat beviset endast när han eller hon har skapat ett bevis. Om en person har skapat ett bevis och gjort en annan person till ägare, är det bara den nya ägaren som får det korrekturutskick som har gjorts via e-post. Skaparen och/eller ägaren får ingen; får de bara e-postmeddelandet"Proof Made". Mer information om e-postmeddelandet Nytt korrektur finns i Nytt korrekturmeddelande.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a6bfe471-2032-4b74-8316-584f923e8651
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# The [!UICONTROL Proof Made] e-post

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

A [!UICONTROL Proof Made] e-post skickas till den som skapat beviset endast när han eller hon har skapat ett bevis. Om en person har skapat ett bevis och gjort en annan person till ägare, är det bara den nya ägaren som får [!UICONTROL Proof made] e-post. Skaparen och/eller ägaren får ingen; får de bara [!UICONTROL Proof Made] e-post. Mer information om [!UICONTROL New Proof] e-post, se [[!UICONTROL New proof] e-post](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

Användare kan inaktivera [!UICONTROL Proof Made] e-postmeddelanden i deras profilinställningar enligt nedan.

>[!NOTE]
>
> Om korrekturets skapare eller ägare har [!UICONTROL Proof Made] e-postmeddelanden som är inaktiverade som standard i deras personliga inställningar, de får inga [!UICONTROL Proof Made] eller [!UICONTROL New Proof] e-post, även om [!UICONTROL Notify people by email] kryssrutan är markerad på [!UICONTROL New proof] sida.

![Korrektur_gjort_e-post.png](assets/proof-made-email-350x214.png)

A [!UICONTROL Proof Made] e-postmeddelandet innehåller ditt personliga meddelande (om du inkluderar ett) och följande korrekturinformation:

* Korrekturnamn
* Personlig länk till beviset
* Versionsnummer
* Miniatyrbild av korrekturet
* Förlopp
* En länk för att dela korrekturet med någon annan
* På så sätt kan du dela korrektur-URL:en och/eller hämtningslänken för originalfilen.

>[!NOTE]
>
> Genom att dela korrekturlänkar kan du inte uttryckligen lägga till granskare i korrekturet, du delar bara det offentliga korrektur-URL:en och mottagaren får skrivskyddad åtkomst till korrekturet.

Se [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) för mer information.

Om du inte vill att den här länken ska visas i mottagarens e-post bör du inaktivera [!UICONTROL Public sharing] korrekturinställningar ([!UICONTROL Download original file] och [!UICONTROL Public URL]).

## Inaktiverar [!UICONTROL Proof Made] E-post

1. Klicka **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**&#x200B;öppnar du **[!UICONTROL Proofing defaults]** tabbtangenten och sedan klicka **[!UICONTROL Disable]** nästa **[!UICONTROL Email confirmation when proofs are ready]**.

1. ![Korrektur_Skapad_av_Korofing_defaults.png](assets/proof-made---proofing-defaults-350x103.png)

1. Se [Konfigurera e-postmeddelandeinställningar i Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) för mer detaljerade instruktioner.
1. Om e-postmeddelanden är inaktiverade som standard i [!UICONTROL Account settings], får den som skapade eller äger beviset inte något [!UICONTROL Proof Made] eller [!UICONTROL New Proof] e-post, även om detta är aktiverat i deras personliga inställningar och [!UICONTROL Notify people by email] kryssrutan är markerad på [!UICONTROL New proof] sida.
