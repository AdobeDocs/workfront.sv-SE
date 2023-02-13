---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: Konfigurera ett satellitkonto i [!DNL Workfront Proof]
description: Satellitkonton är betalda konton som du konfigurerar och hanterar inifrån dina egna konton [!DNL Workfront] Korrekturkonto. Mer information finns i"Satellitkonton" i [!DNL Workfront] Korrektur.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Konfigurera ett satellitkonto i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Satellitkonton är betalda konton som du konfigurerar och hanterar inifrån dina egna konton [!DNL Workfront Proof] konto. Mer information finns i [Satellitkonton i [!DNL Workfront] Korrektur](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md).

Alla faktureringsadministratörer kan skapa ett satellitkonto. Mer information om faktureringsadministratörer finns i [[!UICONTROL Proof Permissions Profiles] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
> Satellitkonton måste anges på en av våra [!UICONTROL Standard] eller högre planer.

## Skapa ett satellitkonto {#creating-a-satellite-account}

Så här skapar du ett satellitkonto:

1. Gå till [!UICONTROL Billing] sida.\
   Mer information om faktureringssidan finns i  [The [!DNL Workfront Proof] [!UICONTROL Billing] Sida](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Klicka på **[!UICONTROL New Satellite]** kontoknappen. (1)

   Ett popup-fönster visas.

   ![New_Satellite_Account.png](assets/new-satellite-account-350x156.png)

1. Ange kundens information, inklusive eventuella relevanta kampanjkoder.
1. Klicka på **[!UICONTROL Save]**. Satellitkontot visas automatiskt i [!UICONTROL Accounts] nedrullningsbar meny högst upp i [!UICONTROL Billing] sida.
1. Välj det nya satellitkontot i listrutan.
1. Fortsätt med [Välja en plan för ditt satellitkonto](#selecting-a-plan-for-your-satellite-account) för att uppgradera ditt satellitkonto.

## Välja en plan för ditt satellitkonto {#selecting-a-plan-for-your-satellite-account}

När du har konfigurerat satellitkontot enligt beskrivningen i [Skapa ett satellitkonto](#creating-a-satellite-account)måste du uppgradera till önskad plan.

1. Gå till [!UICONTROL Billing] sida.\
   Mer information om faktureringssidan finns i  [The [!DNL Workfront Proof] [!UICONTROL Billing] Sida](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. I **[!UICONTROL Your accounts]** den nedrullningsbara menyn längst upp på sidan (1), välj det relevanta satellitkontot.

   Faktureringssidan för satellitkontot visas och faktureringskontaktuppgifterna från ditt konto replikeras automatiskt.

   ![Satellite_account_change_plan.png](assets/satellite-account-change-plan-350x156.png)

1. Klicka på **[!UICONTROL Change Plan]** längst upp till höger på sidan. (2)\
   eller\
   Öppna popup-fönstret genom att klicka på namnet på ditt aktuella eller nästa plan. (3)

1. Uppgradera eller nedgradera din plan.

## Lägga till användare i ditt satellitkonto

När du har uppgraderat satellitkontot till den plan du valt måste du lägga till användare i kontot.

1. Logga in på [!DNL Workfront Proof] som [!DNL Workfront Proof] administratör.
1. Klicka på **[!UICONTROL Account Settings]**.
1. Välj det relevanta satellitkontot i listrutan högst upp på sidan. (1)\
   Sidan med kontoinställningar för satellitkontot visas.
1. Klicka på **[!UICONTROL New user]** längst upp till höger på sidan. (2)\
   The [!DNL New User] visas.

1. Ange användarens information och klicka sedan på **[!UICONTROL Save]**.\
   Användaren får ett e-postmeddelande som ger dem åtkomst till kontot.

Användare som läggs till i satellitkontot visas som medlemmar i kontaktlistan för navkontot.

På samma sätt visas användare i navkontot som medlemmar i kontakterna för satellitkontot.

Om du vill visa en fullständig lista över alla användare i satellitkontot klickar du på **[!UICONTROL Users]** -fliken.

![SA_New_User.png](assets/sa-new-user-350x156.png)

## Länka befintliga separata konton till ditt navkonto

Om du tidigare har skapat andra separata konton för dina kunder kan dessa konverteras till satellitkonton.

Vi ska ta hand om det här åt dig genom att länka dem till [!DNL Workfront Proof] konto (vilket gör det till ett navkonto).

Allt du behöver göra är att ge oss följande information:

* Namnet på [!DNL Workfront Proof] konto och e-postadress som du använde för att konfigurera
* Namnen på de separata konton som du vill länka till ditt konto och e-postadresserna som används för att konfigurera separata konton.
