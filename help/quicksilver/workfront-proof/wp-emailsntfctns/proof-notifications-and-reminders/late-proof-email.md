---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Sena korrekturrundor via e-post
description: E-postadressen för det senaste korrekturet skickas till mottagarna när ett korrektur närmar sig deadline eller når deadline. Den här typen av e-postmeddelanden kan inte inaktiveras på korrekturnivå, men kan konfigureras på konto- och användarnivå.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# [!UICONTROL Late proof] e-post

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

The [!UICONTROL Late Proof] e-post skickas till mottagarna när ett korrektur närmar sig deadline eller når deadline. Den här typen av e-postmeddelanden kan inte inaktiveras på korrekturnivå, men kan konfigureras på konto- och användarnivå.

* [!UICONTROL Late proof] e-postmeddelanden skickas automatiskt till granskarna när ett bevis når sin deadline och inte alla granskningar eller beslut har fattats.

   Dessa e-postmeddelanden är aktiverade som standard och kan inte justeras för hela konton, men användare kan inaktivera dem i standardinställningarna för korrektur.

* I riskzonen skickas e-post till granskarna när ett bevis är nära deadline. De är inaktiverade som standard och kan aktiveras i [!UICONTROL Account Settings]. När de är aktiverade kan de även justeras i [!UICONTROL Proofing defaults].

Dessa meddelanden kan inte anpassas.

De personer som kommer att meddelas är:

* Ägaren, endast när [!UICONTROL Email] när korrektur är försenade markeras i [!UICONTROL Owner's Proofing defaults].
* Alla godkännare som ännu inte har fattat sitt beslut om beviset. Information om beslut finns i [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Om e-postmeddelanden är inaktiverade som standard i [!UICONTROL Account settings], nej [!UICONTROL Late proof] e-post skickas även om granskarna och godkännarna ännu inte har lämnat in sina kommentarer och beslut. Du kan även inaktivera [!UICONTROL Late proof] e-postmeddelanden i standardinställningarna för korrektur.

Tänk på följande när det gäller korrekturmeddelanden:

* Dina [!DNL Workfront] administratör eller [!DNL Workfront Proof] kan administratören inkludera organisationens logotyp i dina e-postmeddelanden, vilket förklaras i [Varumärken [!DNL Workfront Proof] webbplats](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Om du behöver dela flera korrektur med samma granskare och du inte vill att de ska få flera e-postmeddelanden, kan du överföra dem samtidigt. Alla granskare får ett mejl med information om alla korrektur och en personlig URL för varje korrektur.

   >[!NOTE]
   >
   >Skaparen av korrekturet får ett separat [!UICONTROL Proof made] e-post för varje korrektur som skapas. Mer information finns i [The [!UICONTROL Proof Made] e-post](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Om du eller dina granskare inte får ett förväntat e-postmeddelande läser du  [Konfigurera [!DNL Workfront Proof] e-postmeddelanden för att undvika skräppostfilter](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
