---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrera [!DNL Workfront Proof] med [!DNL Basecamp]
description: Om du använder  [!DNL Basecamp] för projekthantering kan du erbjuda dina projektteam mer gransknings- och godkännandeverktyg med  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Integrera [!DNL Workfront Proof] med [!DNL Basecamp]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du använder [!DNL Basecamp] för projekthantering kan du erbjuda ditt projektteam mer omfattande gransknings- och godkännandeverktyg med [!DNL Workfront Proof].

## Förstå integreringen av [!DNL Basecamp] med [!DNL Workfront]

Genom att integrera med [!DNL Basecamp] kan användare visa, granska och godkänna korrektur i [!DNL Basecamp]. Användare kan skicka in korrektur till ditt [!DNL Workfront Proof]-konto och ansluta dem till ditt [!DNL Basecamp]-projekt. Dina granskare kan kommentera och fatta beslut via [!DNL Basecamp] med hjälp av det minikorrektur som är inbäddat i ditt Basecamp-meddelande.

När [!DNL Workfront Proof] är integrerat har [!DNL Basecamp] följande korrekturfunktioner:

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

* Konfigurera [!DNL Basecamp] i [Kontoinställningar:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Detta aktiverar Basecamp-integreringen för hela organisationen. Mer information finns i [Aktivera basstämpelintegrering med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Konfigurera [!DNL Basecamp] i [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Detta gör att konstruktörer och ägare av bevis kan ansluta till sitt personliga Basecamp-konto och auktorisera [!DNL Workfront Proof]-åtkomst. Mer information finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

Du kan integrera [!DNL Workfront] med antingen [!DNL Basecamp] eller [!DNL Basecamp Classic]. För varje version av [!DNL Basecamp] används ett annat API och olika konfigurationsprocedurer krävs därför.

Mer information om hur du konfigurerar [!DNL Basecamp Classic] finns i [Integrera [!DNL Workfront Proof] med [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Aktiverar integreringen av [!DNL Basecamp] med [!DNL Workfront Proof]

Som [behörighetsprofiler för korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) eller [behörighetsprofiler för korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) kan du konfigurera [!DNL Basecamp]-integreringen för hela kontot i dina [kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Samla in följande information i [!UICONTROL Basecamp]:

   * URL:en för ditt [!DNL Basecamp]-konto
   * URL:en som hittades i avsnittet [!UICONTROL My info]

1. Logga ut från [!DNL Basecamp].
1. Klicka på **[!UICONTROL Account settings]** i det övre högra hörnet.
1. Klicka på fliken **[!UICONTROL Integrations]**.
1. Klicka på **[!UICONTROL Enable]** i avsnittet **[!UICONTROL [!DNL Basecamp]]** till höger om **[!UICONTROL [!DNL Basecamp] integration]**.

1. Bredvid **[!UICONTROL [!DNL Basecamp] version]** kontrollerar du att **[!UICONTROL Classic version]** är den version du integrerar med.

1. (Villkorligt) Om ingen [!DNL Basecamp]-URL visas klickar du på **[!UICONTROL Edit]**, skriver in URL:en för ditt [!DNL Basecamp]-konto, utan &quot;http://&quot; och klickar sedan på **[!UICONTROL Save]**.

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]** i fönstrets övre högra hörn.

1. Klicka på fliken **[!UICONTROL Integrations]**.
1. Under **[!DNL Basecamp]**, till höger om **[!UICONTROL Basecamp integration]**, klickar du på **[!UICONTROL Enable]**.

1. Klicka på **[!UICONTROL Edit]** till höger om **[!UICONTROL [!DNL Basecamp] API Token]** i alternativen som visas.

1. I rutan som visas skriver du den URL som finns i avsnittet [!UICONTROL My info] i [!DNL Basecamp] och klickar sedan på **[!UICONTROL Save]**.\
   När du har integrerat [!DNL Workfront Proof] med [!DNL Basecamp] kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings)

1. Om du inte kan aktivera integreringen av [!DNL Basecamp] kanske ditt [!DNL Workfront Proof]-konto-ID inte är samma som det konto-ID du använder i [!DNL Basecamp].
1. När du har integrerat [!DNL Workfront Proof] med [!DNL Basecamp] kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

## Konfigurera personliga inställningar

När du har konfigurerat [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) för din organisation bör var och en av de författare som skapar/skickar korrektur ange sina [personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Gå till **[!UICONTROL Personal**&#x200B;**settings]**.

1. Öppna fliken **[!UICONTROL Integrations]** (1).
1. Om du vill aktivera integreringen av [!DNL Basecamp] klickar du på **[!UICONTROL Enable]** (2).
1. Klicka på **[!UICONTROL Connect to your [!DNL Basecamp] account]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Logga in på ditt [!DNL Basecamp]-konto (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Klicka på **[!UICONTROL Yes, I'll allow access]** för att auktorisera [!DNL Workfront Proof]-åtkomst till ditt konto (2).\
   ![Basecamp_authentication_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Valfritt) När din personliga integrering är aktiv (3) kan du enkelt växla mellan dina [!DNL Basecamp]-konton.

   1. Klicka på **[!UICONTROL Switch [!DNL Basecamp] account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      [!UICONTROL Switch Basecamp Account] tar dig till sidan [!UICONTROL Personal Settings] där du kan välja vilket av dina [!DNL Basecamp]-konton du vill integrera med ditt [!DNL Workfront Proof]-konto.

   1. Klicka på **[!UICONTROL Re-Integrate with [!DNL Basecamp]]** (5) innan du väljer [!DNL Basecamp]-kontot\

      Sidan [!UICONTROL Personal Settings] uppdateras och din senaste lista över [!DNL Basecamp]-konton visas.

   1. Klicka på **[!UICONTROL Integrate with this account]** för att ansluta den till [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Du kan nu lägga till korrektur i [!DNL Basecamp] projekt.
