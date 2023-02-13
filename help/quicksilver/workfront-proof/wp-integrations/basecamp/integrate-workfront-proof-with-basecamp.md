---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrera [!DNL Workfront Proof] med [!DNL Basecamp]
description: Om du använder [!DNL Basecamp] för projekthantering kan du ge projektteamet bättre verktyg för granskning och godkännande med [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Integrera [!DNL Workfront Proof] med [!DNL Basecamp]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du använder [!DNL Basecamp] för projekthantering kan du ge projektteamet bättre verktyg för granskning och godkännande med [!DNL Workfront Proof].

## Förstå [!DNL Basecamp] Integration med [!DNL Workfront]

Integrera med [!DNL Basecamp] gör att användare kan visa, granska och godkänna korrektur i [!DNL Basecamp]. Användare kan skicka in korrektur till [!DNL Workfront Proof] konto och koppla dem till [!DNL Basecamp] projekt. Dina granskare kan kommentera och fatta beslut via [!DNL Basecamp], med hjälp av det minikorrektur som är inbäddat i ditt Basecamp-meddelande.

Vid integrering med [!DNL Workfront Proof], [!DNL Basecamp] har följande korrekturfunktioner:

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

* Konfigurera [!DNL Basecamp] in [Kontoinställningar:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Detta möjliggör integrering av basecamp för hela organisationen. Mer information finns i [Aktivera integreringen av basecamp med [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Konfigurera [!DNL Basecamp] in [Personliga inställningar](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Detta gör att upphovspersoner och ägare kan ansluta till sina egna Basecamp-konton och auktorisera [!DNL Workfront Proof] åtkomst. Mer information finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

Ni kan integrera [!DNL Workfront] med antingen [!DNL Basecamp] eller [!DNL Basecamp Classic]. Varje version av [!DNL Basecamp] använder ett annat API och kräver därför olika konfigurationsprocedurer.

Mer information om konfiguration [!DNL Basecamp Classic], se [Integrera [!DNL Workfront Proof] med [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Aktivera [!DNL Basecamp] Integration med [!DNL Workfront Proof]

Som [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) eller [Korrektur för behörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)kan du konfigurera [!DNL Basecamp] integrering för hela kontot i [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. I [!UICONTROL Basecamp], samla in följande information:

   * URL:en för [!DNL Basecamp] konto
   * URL:en som finns i[!UICONTROL My info]&quot;

1. Logga ut från [!DNL Basecamp].
1. Klicka **[!UICONTROL Account settings]** nära det övre högra hörnet.
1. Klicka på **[!UICONTROL Integrations]** -fliken.
1. I **[!UICONTROL [!DNL Basecamp]]** till höger om **[!UICONTROL [!DNL Basecamp] integration]**, klicka **[!UICONTROL Enable]**.

1. Nästa till **[!UICONTROL [!DNL Basecamp] version]**, verifiera **[!UICONTROL Classic version]** är den version du integrerar med.

1. (Villkorligt) Om nej [!DNL Basecamp] URL visas, klicka **[!UICONTROL Edit]** skriver du URL:en till [!DNL Basecamp] utan&quot;http://&quot; och klicka sedan på **[!UICONTROL Save]**.

1. Klicka i fönstrets övre högra hörn på **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**.

1. Klicka på **[!UICONTROL Integrations]** -fliken.
1. Under **[!DNL Basecamp]**, till höger om **[!UICONTROL Basecamp integration]**, klicka **[!UICONTROL Enable]**.

1. I alternativen visas till höger om **[!UICONTROL [!DNL Basecamp] API Token]**, klicka **[!UICONTROL Edit]**.

1. I rutan som visas skriver du den URL som finns i[!UICONTROL My info]&quot; i [!DNL Basecamp]och sedan klicka **[!UICONTROL Save]**.\
   När ni väl har integrerat [!DNL Workfront Proof] med [!DNL Basecamp]kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings)

1. Om du inte kan aktivera [!DNL Basecamp] integrering, [!DNL Workfront Proof] Konto-ID:t kanske inte är samma som det konto-ID som du använder i [!DNL Basecamp].
1. När ni väl har integrerat [!DNL Workfront Proof] med [!DNL Basecamp]kan dina användare konfigurera sina personliga inställningar. Mer information om hur du konfigurerar personliga inställningar finns i [Konfigurera personliga inställningar](#configuring-personal-settings).

## Konfigurera personliga inställningar

När du har konfigurerat [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) för din organisation bör alla författare som skapar/skickar in korrektur ange sina  [personliga inställningar.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Gå till **[!UICONTROL Personal**&#x200B;**settings]**.

1. Öppna **[!UICONTROL Integrations]** tab (1).
1. Aktivera [!DNL Basecamp] integration, klicka **[!UICONTROL Enable]** (2).
1. Klicka **[!UICONTROL Connect to your [!DNL Basecamp] account]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Logga in på [!DNL Basecamp] konto (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Klicka **[!UICONTROL Yes, I'll allow access]** att godkänna [!DNL Workfront Proof] behörighet till ditt konto (2).\
   ![Basecamp_authentication_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Valfritt) När din personliga integrering är aktiv (3) kan du enkelt växla mellan [!DNL Basecamp] konton.

   1. Klicka **[!UICONTROL Switch [!DNL Basecamp] account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      The [!UICONTROL Switch Basecamp Account] tar dig till [!UICONTROL Personal Settings] sida, där du kan välja vilken av dina [!DNL Basecamp] konton som du vill integrera med [!DNL Workfront Proof] konto.

   1. Klicka **[!UICONTROL Re-Integrate with [!DNL Basecamp]]** (5) innan du väljer [!DNL Basecamp] konto\

      Det här uppdaterar [!UICONTROL Personal Settings] och visar din senaste lista över [!DNL Basecamp] konton.

   1. Klicka **[!UICONTROL Integrate with this account]** för att koppla den till [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Nu kan du lägga till korrektur i [!DNL Basecamp] projekt.
