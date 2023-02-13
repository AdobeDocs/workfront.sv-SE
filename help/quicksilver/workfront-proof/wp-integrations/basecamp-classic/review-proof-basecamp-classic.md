---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Granska ett korrektur i Classic
description: Basecamp är ett projekthanteringsverktyg som utvecklats av 37 signaler. Om du använder Basecamp för projekthantering kan du ge projektteamet bättre gransknings- och godkännandeverktyg med hjälp av [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b14f33dc-e059-4ee2-a429-9f1852a2b9bb
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Granska ett korrektur i [!DNL Basecamp] Klassisk

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Basecamp] är ett projekthanteringsverktyg som utvecklats av [!DNL 37signals]. Om du använder [!DNL Basecamp] för projekthantering kan du ge projektteamet bättre verktyg för granskning och godkännande med [!DNL Workfront Proof].

## Förstå korrekturgranskningar i [!DNL Basecamp Classic]

Vid integrering med [!DNL Workfront Proof], [!DNL Basecamp] gör att användarna kan göra följande med korrektur:

* Användare kan granska och godkänna korrektur i [!DNL Basecamp Classic].
* Användarna har granskningsverktyg tillgängliga.
* Projektgranskningsteam får ett meddelande i [!DNL Basecamp] med ett mini-korrektur för granskning och godkännande.
* Användare kan växla till ett fullsidigt korrektur för granskning och godkännande.
* Man kan lägga in kommentarer och markeringar i både små och stora korrektur.
* När en kommentar har svarats kan den inte redigeras/tas bort. Mer information om kommentarer finns i [Kommentera ett korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).
* Granskarna kan svara på kommentarer och markeringar som gjorts av andra granskare. Mer information om kommentarer finns i [Kommentera ett korrektur](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).
* Användarna får ett meddelande när det finns en ny version av ett korrektur.
* Användare som inte [!DNL Workfront Proof] -användare kan arbeta med ett korrektur i [!DNL Basecamp].

## Visa ett korrektur via e-postmeddelandet

Om du länkar ett korrektur till [!DNL Basecamp], [!DNL Workfront Proof] skickar ett e-postmeddelande (1) med följande information till alla granskare:

* **Korrekturinformation** (2): Visar information om korrekturet. Vilken information som visas beror på hur Workfront-administratören har konfigurerat Basecamp.
* **[!UICONTROL Go to Proof]link** (3): Beviset öppnas i Workfront.
* **[!DNL Basecamp]URL** (4): Öppnar korrekturet i Basecamp. Om granskare som inte hör till en basstämpel läggs till i korrekturet innehåller deras e-postmeddelanden inte länken för basstämpel.
* **[!UICONTROL Proof progress]** (5): Visar stadierna för godkännande och korrekturförloppsindikatorer.
* **[!UICONTROL Stage]** (6): Visar en lista över granskarna och deras individuella förlopp.

![Basecamp_ProofHQ_email_notification1__1_.png](assets/basecamp-proofhq-email-notification1--1--350x202.png)

Så här öppnar du korrekturet från e-postmeddelandet:

1. Öppna korrekturet i [!DNL Workfront Proof], klicka **[!UICONTROL Go To Proof]**.\
   eller\
   Öppna korrekturet i [!DNL Basecamp]klickar du på den URL som visas i dialogrutan **[!UICONTROL [!DNL Basecamp] URL]** fält.\
   Mer information om hur du granskar ett korrektur i [!DNL Basecamp Classic], se [Granska ett korrektur i [!DNL Basecamp]](#reviewing-a-proof-in-basecamp) i den här artikeln.

## Visa korrekturet via [!DNL Basecamp Classic] Meddelande

Du kan få åtkomst till ett korrektur från en [!DNL Basecamp Classic] meddelande.

1. I [!DNL Basecamp], gå till din projektsida (1).\
   ![Basecamp_Classic_messages_1.png](assets/basecamp-classic-messages-1-350x120.png)

1. Klicka på meddelandet för det korrektur som du vill öppna. (2)\
   Meddelandet för korrekturet öppnas och ett minikorrektur visas. Namnet på korrekturet visas högst upp i meddelandefönstret (3).\
   Du kan antingen visa miniatyrbilden i [!DNL Basecamp Classic] eller in [!DNL Workfront Proof].\
   ![Basecamp_Classic_messages_2.png](assets/basecamp-classic-messages-2-350x501.png)

1. Visa korrekturet i helskärmsläge i [!DNL Workfront proof]klickar du på den URL som visas ovanför korrekturet (4).
1. (Villkorligt) Om du inte är inloggad på [!DNL Workfront Proof] i ett av webbläsarfönstren loggar du för att granska korrekturet:

   1. Klicka **[!UICONTROL Sign In]** (5) ovanför beviset.
   1. Skriv din e-postadress (6).\

      Du måste använda samma e-postadress som användes när du lades till i beviset.
   1. Klicka på **[!UICONTROL Next]**.
   1. Skriv [!DNL Workfront Proof] lösenord (7).\

      eller\
      Om du inte har en [!DNL Workfront Proof] anger du ett publikt namn som ska visas.\
      Du kan välja &quot;[!UICONTROL remember me]&quot; så att du bara behöver ange dina uppgifter en gång.

1. Om du vill granska korrekturet fortsätter du med [Granska ett korrektur i [!DNL Basecamp]](#reviewing-a-proof-in-basecamp).

>[!NOTE]
>
> Kommentarsrutan som visas under det lilla korrekturet på meddelandesidan gäller endast själva meddelandet. Om du vill skicka granskningskommentarer måste du använda kommentarsikonknappen längst upp i det lilla korrekturet eller det större [!UICONTROL Comments] längst upp i korrektur på helsida. Mer information finns i Granska en [Granska ett korrektur i [!DNL Basecamp]](#reviewing-a-proof-in-basecamp).

## Granska ett korrektur i [!DNL Basecamp]

Mini-korrektur i [!DNL Basecamp] ger dig de verktyg du behöver för att lägga till och skapa [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) på beviset. Alla användare som är tilldelade till projektet kan se dina markeringar och kommentarer och svara med sina egna kommentarer i realtid.

När du öppnar korrekturet visas korrekturet i [!UICONTROL proofing] fönstret (1) och namnet på korrektur och versionsnummer visas i det övre vänstra hörnet (2).

![Basecamp_Classic_miniproof.png](assets/basecamp-classic-miniproof-350x350.png)

Så här granskar du korrekturet:

1. Om du vill lägga till en kommentar klickar du på [!UICONTROL Comment] (3) längst upp i korrekturet och skriv in kommentaren.\
   Du behöver inte skicka något svar till [!DNL Basecamp] som kommentarer och [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) sparad till korrekturet (liknar granskning av ett korrektur i [!DNL Workfront Proof]).

1. Om du vill lägga till ett beslut klickar du på Beslut (3) längst upp på beviset och väljer ditt godkännandebeslut.\
   Mer information om hur du fattar beslut om ett bevis finns i [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

Andra funktioner i korrekturfönstret är:

* **[!UICONTROL Action menus]** (4): Gör att du kan välja inställningar för korrekturet.
* **[!UICONTROL Full-screen button]** (5): Växla mellan helskärm och minikorrektur.
* **[!UICONTROL Sidebar]** (6): Gör att du kan expandera eller krympa visningen av korrektur.
* **[!UICONTROL Username]** (7): Visar ditt användarnamn om du är inloggad på Workfront.
* **[!UICONTROL Zoom tools]** (8): Gör att du kan förstora ett område i korrekturet.
* **[!UICONTROL Page navigation tools]** (9): Bläddra till andra sidor i korrekturet.

<!--For more information on reviewing proofs, see [Legacy proofing viewer Overview](../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/legacy-proofing-viewer.md).-->
