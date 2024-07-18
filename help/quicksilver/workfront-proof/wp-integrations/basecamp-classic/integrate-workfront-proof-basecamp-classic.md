---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrera [!DNL Workfront Proof] med Basecamp Classic
description: Om du använder  [!DNL Basecamp] för projekthantering kan du erbjuda dina projektteam mer gransknings- och godkännandeverktyg med  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Integrera [!DNL Workfront Proof] med [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du använder [!DNL Basecamp] för projekthantering kan du erbjuda ditt projektteam mer omfattande gransknings- och godkännandeverktyg med [!DNL Workfront Proof].

## Förstå integreringen av [!DNL Basecamp] med [!DNL Workfront]

Genom att integrera med [!DNL Basecamp] kan användare visa, granska och godkänna korrektur i [!DNL Basecamp]. Användare kan skicka in korrektur till ditt [!DNL Workfront Proof]-konto och ansluta dem till ditt [!DNL Basecamp]-projekt. Dina granskare kan och kan fatta [beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp] med hjälp av det minikorrektur som är inbäddat i ditt Basecamp-meddelande.

När [!DNL Basecamp] är integrerat med [!DNL Workfront Proof] kan användare göra följande med korrektur:

* Användare kan granska och godkänna korrektur inom [!DNL Basecamp Classic].
* Användarna har granskningsverktyg tillgängliga.
* Projektgranskningsteamen får ett meddelande i [!DNL Basecamp] med ett minikorrektur för granskning och godkännande.
* Användare kan växla till ett fullsidigt korrektur för granskning och godkännande.
* Man kan lägga in kommentarer och markeringar i både små och stora korrektur.

  >[!NOTE]
  >
  >När en kommentar har svarats kan den inte redigeras eller tas bort.

* Granskarna kan svara på kommentarer och markeringar som gjorts av andra granskare.
* Användarna får ett meddelande när det finns en ny version av ett korrektur.
* Användare som inte är [!DNL Workfront Proof]-användare kan arbeta med ett korrektur i [!DNL Basecamp].

Integrationen av [!DNL Workfront Proof] med [!DNL Basecamp] måste konfigureras på två nivåer:

* Konfigurera [!DNL Basecamp] i [Kontoinställningar:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Detta aktiverar Basecamp-integreringen för hela organisationen.
* Mer information finns i [Aktivera  [!DNL Basecamp] integreringen med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Konfigurera [!DNL Basecamp] i [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Detta gör att konstruktörer och ägare kan ansluta till sitt personliga [!DNL Basecamp]-konto och auktorisera [!DNL Workfront Proof]-åtkomst. Mer information finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

Du kan integrera [!DNL Workfront] med antingen [!DNL Basecamp] eller [!DNL Basecamp Classic]. För varje version av [!DNL Basecamp] används ett annat API och olika konfigurationsprocedurer krävs därför.

Mer information om hur du konfigurerar [!DNL Basecamp Classic] finns i [Aktivera  [!DNL Basecamp] integreringen med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) i den här artikeln.

Mer information om hur du konfigurerar [!DNL Basecamp] finns i [Integrera [!DNL Workfront Proof] med [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Aktiverar integreringen av [!DNL Basecamp] med [!DNL Workfront Proof]

Som [profiler för korrekturbehörigheter i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) eller [profiler för korrektur av behörigheter i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) kan du ställa in basstämpelintegrering för hela kontot i dina [kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Gå till [Kontoinställningar.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Öppna fliken **[!UICONTROL Integrations]** (1).
1. Klicka på **[!UICONTROL Enable]** (2) om du vill aktivera basstämpelintegreringen.
1. Kontrollera att [!DNL Basecamp Classic] är den version du integrerar med (3).
1. (Villkorligt) Om ingen [!DNL Basecamp]-URL visas (4) klickar du på **[!UICONTROL Edit]** och anger URL:en för ditt [!DNL Basecamp]-konto (utan http://).
1. Klicka på **[!UICONTROL Save]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Valfritt) Kontrollera din [!DNL Basecamp]-URL i webbläsaren efter att du loggat in på ditt [!DNL Basecamp Classic]-konto (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   När du har integrerat [!DNL Workfront Proof] med [!DNL Basecamp] kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

   Om du inte kan aktivera integreringen av [!DNL Basecamp] kanske ditt [!DNL Workfront Proof]-konto-ID inte är samma som det konto-ID du använder i [!DNL Basecamp].

## Konfigurera personliga inställningar

När du har konfigurerat [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) för din organisation bör alla författare som skapar/skickar korrektur ange sina [personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Det är enklast att slutföra de här stegen om du har [!DNL Basecamp]-sessionen öppen i ett webbläsarfönster och [!DNL Workfront Proof]-sessionen är öppen i ett annat fönster.

* [Hämtar din  [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token)
* [Lägger till din  [!DNL Basecamp] API-token i dina personliga inställningar](#adding-your-basecamp-api-token-to-your-personal-settings)

### Hämtar din [!DNL Basecamp] API-token

För att slutföra integreringen på individuell nivå i [!DNL Workfront Proof] behöver användarna sin individuella autentiseringstoken för API:t [!DNL Basecamp].

Så här hämtar du din [!DNL Basecamp] API-token:

1. Logga in på ditt [!DNL Basecamp]-konto.
1. Klicka på **[!UICONTROL My Info]** (1) i skärmens övre högra hörn.\
   Sidan [!UICONTROL My Info] visas.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. Klicka på **[!UICONTROL Show your tokens]** (2) i avsnittet [!UICONTROL Authentication tokens] för att visa dina personliga autentiseringstoken.
1. Markera **[!UICONTROL Token for feed readers]** eller **[!UICONTROL Basecamp API]** (3) och kopiera sedan token till Urklipp.

1. Klistra in din [!DNL Basecamp] API-token i rutan [!UICONTROL Token for feed readers] eller [!UICONTROL Basecamp API].\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Lägger till din [!DNL Basecamp] API-token i dina personliga inställningar

Så här klistrar du in API-token [!DNL Basecamp] i dina [!DNL Workfront Proof] [personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Gå till [[!UICONTROL Integrations] - användarinställningar](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) i dina [personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   En administratör måste först aktivera integreringen av [!DNL Basecamp Classic] för att du ska kunna aktivera dina personliga inställningar. Mer information om hur du konfigurerar integreringen finns i [Aktivera  [!DNL Basecamp] integreringen med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) i den här artikeln.

1. I rutan [!DNL Basecamp] API-token (2) klistrar du in den token som du just kopierade från [!DNL Basecamp] [!UICONTROL My Info]-sidan i fältet (3).\
   Mer information om hur du kopierar din [!DNL Basecamp] API-token finns i [Hämta din [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token) i den här artikeln.

1. Klicka på **[!UICONTROL Save]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Dina [!DNL Workfront Proof] [personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) är nu integrerade med ditt [!DNL Basecamp Classic]-konto.
