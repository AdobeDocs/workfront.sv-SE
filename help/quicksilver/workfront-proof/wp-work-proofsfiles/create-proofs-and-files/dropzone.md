---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: Om du har Enterprise-planen kan du använda Dropzone för att skicka in nya korrektur och nya versioner av korrektur till ditt konto utan att behöva logga in på ditt konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du har Enterprise-planen kan du använda Dropzone för att skicka in nya korrektur och nya versioner av korrektur till ditt konto utan att behöva logga in på ditt konto.

När du skickar ett bevis via Dropzone visas det på Dropzone-sidan i ditt [!DNL Workfront Proof]-konto. Därifrån kan du dirigera den till ditt arbetsflöde.

## Skicka in ett nytt bevis via Dropzone-URL:en

1. Gå till den unika Dropzone-URL:en i webbläsaren, enligt beskrivningen i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Ange din e-postadress.
1. Klicka på **[!UICONTROL Select a file]** eller **[!UICONTROL Capture a web page]** och välj filen eller webbsidan som du vill överföra.

1. Ange säkerhetskoden och klicka sedan på **[!UICONTROL Next]**.\
   En förloppsindikator visar hur överföringen fortskrider.\
   På nästa skärm kan du lägga till korrekturinformation.\
   Observera att det här avsnittet bara visas om det har aktiverats i Dropzone-inställningarna.

1. När du har fyllt i informationen klickar du på **[!UICONTROL Next]**.
1. Alla granskare som läggs till i korrekturet får sina e-postmeddelanden först när beviset aktiveras (se nedan).
1. Ditt bevis går igenom följande lägen när du har skickat det till Dropzone:

   * När du först överför en fil till Dropzone visas korrekturet där som ett utkast.
   * När du är klar med inlämningen visas beviset i din Dropzone som inskickat.
   * När korrekturet har aktiverats och låsts upp visas det som aktivt i Dropzone.
   * Om korrekturet är låst visas det i Dropzone som låst.

## Skicka en ny version av ett befintligt bevis via Dropzone-URL:en

1. Gå till den unika Dropzone-URL:en i webbläsaren, enligt beskrivningen i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Ange din e-postadress.
1. Markera kryssrutan för att ange att du överför en ny version av ett befintligt korrektur.\
   Mer information om hur du skapar en ny version av ett korrektur finns i .
1. Klicka på **[!UICONTROL Select a file]** eller **[!UICONTROL Capture a web page]** och välj filen eller webbsidan som du vill överföra.

1. Ange säkerhetskoden och klicka sedan på **[!UICONTROL Next]**.\
   En förloppsindikator visar hur överföringen fortskrider.\
   Workfront Proof skickar ett valideringsmejl till dig.

1. Klicka på länken i e-postmeddelandet.\
   E-postmeddelandet öppnar Dropzone-fönstret i webbläsaren. Länken i e-postmeddelandet är giltig i 24 timmar.
1. Välj den tidigare versionen av korrekturet (endast korrekturet som du skapade/skickade visas).\
   På nästa skärm kan du lägga till korrekturinformation.\
   Det här avsnittet visas bara om det har aktiverats i Dropzone-inställningarna.

1. Skriv informationen och klicka på **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >Alla granskare som läggs till i korrekturet får sina e-postmeddelanden först när beviset aktiveras (se nedan).

   Ditt bevis går igenom följande lägen när du har skickat det till Dropzone:

   * När du först överför en fil till Dropzone visas korrekturet där som ett utkast.
   * När du är klar med inlämningen visas beviset i din Dropzone som inskickat.
   * När korrekturet har aktiverats och låsts upp visas det som aktivt i Dropzone.
   * Om korrekturet är låst visas det i Dropzone som låst.

## Mejla ett korrektur till Dropzone

>[!NOTE]
>
>Det går inte längre att skicka ett bevis till dropzone via e-post.


## Slutförde ditt bidrag

Workfront skickar ett e-postmeddelande till dig (den som skickar in formuläret) som du vill bekräfta om filen är ett nytt bevis eller en ny version. Länken i e-postmeddelandet är giltig i 24 timmar.

1. Klicka på länken och följ stegen ovan, beroende på om det är ett nytt korrektur eller en ny version av ett befintligt korrektur.

## Aktivera korrektur

Dropzone-ägaren får ett e-postmeddelande som informerar om att ett nytt bevis har skickats till Dropzone:

* Korredet visas på Dropzone-sidan i ditt konto (för att komma åt Dropzone-sidan klickar du på länken i den vänstra navigeringssidlisten).
* Beviset är tillgängligt av Dropzone-ägaren (eller en användare som har minst en personuppgiftsprofil). Ägaren kan ändras i Dropzone-inställningarna (endast en faktureringsadministratör eller en administratör kan göra detta).
* Innan korrekturet kan bearbetas måste Dropzone-ägaren aktivera/låsa upp det (en användare med minst en supervisor-profil kan också göra detta). Bevisets status visas som Skickat tills det har aktiverats/låsts upp.

Så här aktiverar du korrekturet:

1. Gå till listrutan till höger om korrekturet och klicka på **[!UICONTROL Activate]**.
1. När korrekturet har aktiverats/låsts upp:

   * Korrekturstatusen ändras till Aktiv.
   * Alla som har lagts till i korrekturet får ett e-postmeddelande som talar om att de har ett nytt korrektur att granska. (Inget e-postmeddelande skickas förrän beviset har aktiverats/låsts upp.)
   * Beviset kan bearbetas som vanligt
   * Om den som skickar in dokumentet också lägger till sig själv explicit till korrekturet får de inte något nytt korrekturmeddelande. Mer information finns i [Nytt korrekturmeddelande](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Hantera din Dropzone

På Dropzone-sidan är det enkelt att hantera överföringar till Dropzone. Dropzone-sidan innehåller följande alternativ och funktioner:

* Sidlayout (1)
* Välj om du vill inkludera/exkludera arkiverade korrektur i vyn (2)
* Åtgärdsknappar (3)
* Sortera (4)
* Filter (5)
* Menyn Korrekturåtgärder (6)
* Avarkivera beviset (7)
* Visa/dölj korrektursammanfattning (8)
* Välj ett korrektur (9)

Sidlayouten, sorterings- och filtreringsalternativen är desamma som i [!DNL Views]-listorna. Mer information finns i [Hantera objekt på vysidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

![New_Dropzone_design_feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
