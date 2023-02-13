---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrera [!DNL Workfront Proof] med Basecamp Classic
description: Om du använder [!DNL Basecamp] för projekthantering kan du ge projektteamet bättre verktyg för granskning och godkännande med [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Integrera [!DNL Workfront Proof] med [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du använder [!DNL Basecamp] för projekthantering kan du ge projektteamet bättre verktyg för granskning och godkännande med [!DNL Workfront Proof].

## Förstå [!DNL Basecamp] Integration med [!DNL Workfront]

Integrera med [!DNL Basecamp] gör att användare kan visa, granska och godkänna korrektur i [!DNL Basecamp]. Användare kan skicka in korrektur till [!DNL Workfront Proof] konto och koppla dem till [!DNL Basecamp] projekt. Dina granskare kan [Fatta ett beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], med hjälp av det minikorrektur som är inbäddat i ditt Basecamp-meddelande.

Vid integrering med [!DNL Workfront Proof], [!DNL Basecamp] gör att användarna kan göra följande med korrektur:

* Användare kan granska och godkänna korrektur i [!DNL Basecamp Classic].
* Användarna har granskningsverktyg tillgängliga.
* Projektgranskningsteam får ett meddelande i [!DNL Basecamp] med ett mini-korrektur för granskning och godkännande.
* Användare kan växla till ett fullsidigt korrektur för granskning och godkännande.
* Man kan lägga in kommentarer och markeringar i både små och stora korrektur.

   >[!NOTE]
   >
   >När en kommentar har svarats kan den inte redigeras eller tas bort.

* Granskarna kan svara på kommentarer och markeringar som gjorts av andra granskare.
* Användarna får ett meddelande när det finns en ny version av ett korrektur.
* Användare som inte [!DNL Workfront Proof] -användare kan arbeta med ett korrektur i [!DNL Basecamp].

Integreringen av [!DNL Workfront Proof] med [!DNL Basecamp] måste ställas in på två nivåer:

* Konfigurera [!DNL Basecamp] in [Kontoinställningar:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Detta möjliggör integrering av basecamp för hela organisationen.
* Mer information finns i [Aktivera [!DNL Basecamp] Integration med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Konfigurera [!DNL Basecamp] in [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Detta gör att upphovsmän och ägare kan ansluta till sina egna [!DNL Basecamp] konto och auktorisera [!DNL Workfront Proof] åtkomst. Mer information finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

Ni kan integrera [!DNL Workfront] med antingen [!DNL Basecamp] eller [!DNL Basecamp Classic]. Varje version av [!DNL Basecamp] använder ett annat API och kräver därför olika konfigurationsprocedurer.

Mer information om konfiguration [!DNL Basecamp Classic], se [Aktivera [!DNL Basecamp] Integration med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) i den här artikeln.

Mer information om konfiguration [!DNL Basecamp], se [Integrera [!DNL Workfront Proof] med [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Aktivera [!DNL Basecamp] Integration med [!DNL Workfront Proof]

Som [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) eller [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)kan du konfigurera integreringen av basecamp för hela kontot i [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Gå till [Kontoinställningar.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Öppna **[!UICONTROL Integrations]** tab (1).
1. Om du vill aktivera integreringen av basecamp klickar du på **[!UICONTROL Enable]** (2).
1. Verifiera att [!DNL Basecamp Classic] är den version du integrerar med (3).
1. (Villkorligt) Om nej [!DNL Basecamp] URL visas (4), klicka **[!UICONTROL Edit]** och ange webbadressen till [!DNL Basecamp] konto (utan http://).
1. Klicka **[!UICONTROL Save]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Valfritt) Kontrollera [!DNL Basecamp] URL:en i webbläsaren efter inloggning på [!DNL Basecamp Classic] konto (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   När ni väl har integrerat [!DNL Workfront Proof] med [!DNL Basecamp]kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

   Om du inte kan aktivera [!DNL Basecamp] integrering, [!DNL Workfront Proof] Konto-ID:t kanske inte är samma som det konto-ID som du använder i [!DNL Basecamp].

## Konfigurera personliga inställningar

När du har konfigurerat [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) för din organisation bör alla författare som skapar/skickar in korrektur ange  [personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Det är enklast att slutföra de här stegen om du har [!DNL Basecamp] öppnas i ett webbläsarfönster och [!DNL Workfront Proof] -sessionen öppnas i ett annat fönster.

* [Hämtar dina [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token)
* [Lägg till [!DNL Basecamp] API-token till dina personliga inställningar](#adding-your-basecamp-api-token-to-your-personal-settings)

### Hämtar dina [!DNL Basecamp] API-token

Att slutföra integreringen på individuell nivå i [!DNL Workfront Proof]måste användarna ha sin egen autentiseringstoken för [!DNL Basecamp] API.

Så här hämtar du [!DNL Basecamp] API-token:

1. Logga in på [!DNL Basecamp] konto.
1. Klicka **[!UICONTROL My Info]** (1) i skärmens övre högra hörn.\
   The [!UICONTROL My Info] visas.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. I [!UICONTROL Authentication tokens] avsnitt, klicka **[!UICONTROL Show your tokens]** (2) för att visa dina personliga autentiseringstoken.
1. Välj **[!UICONTROL Token for feed readers]** eller **[!UICONTROL Basecamp API]** (3) och sedan kopiera token till Urklipp.

1. Klistra in [!DNL Basecamp] API-token i [!UICONTROL Token for feed readers] eller [!UICONTROL Basecamp API] box.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Lägg till [!DNL Basecamp] API-token till dina personliga inställningar

Klistra in [!DNL Basecamp] API-token i [!DNL Workfront Proof] [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Gå till [[!UICONTROL Integrations] - Användarinställningar](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) i [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   Administratören måste först aktivera [!DNL Basecamp Classic] för att du ska kunna aktivera dina personliga inställningar. Mer information om hur du konfigurerar integreringen finns i [Aktivera [!DNL Basecamp] Integration med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) i den här artikeln.

1. I [!DNL Basecamp] API-tokenruta (2), klistra in den token som du just kopierade från din [!DNL Basecamp] [!UICONTROL My Info] sida in i fältet (3).\
   Information om hur du kopierar [!DNL Basecamp] API-token, se [Hämtar dina [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token) i den här artikeln.

1. Klicka **[!UICONTROL Save]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Dina [!DNL Workfront Proof] [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) är nu integrerade med [!DNL Basecamp Classic] konto.
