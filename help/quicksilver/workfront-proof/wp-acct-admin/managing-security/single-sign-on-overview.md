---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Enkel inloggning [!DNL Workfront Proof]
description: Med enkel inloggning (SSO) kan dina användare logga in [!DNL Workfront Proof] med organisationens befintliga användarnamn och lösenord.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Enkel inloggning [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

An [!UICONTROL Enterprise] [!DNL Workfront] Planering krävs för att använda den här funktionen. Mer information om olika planer finns i [Workfront-planer](https://www.workfront.com/plans).

Med enkel inloggning (SSO) kan dina användare logga in [!DNL Workfront Proof] med organisationens befintliga användarnamn och lösenord.

För att tillhandahålla den här funktionen använder vi [!DNL Security Assertion Markup Language] (SAML) 2.0, ett XML-baserat protokoll som gör att du kan auktorisera data och utbyta autentisering mellan en identitetsleverantör och en webbtjänst.

Det innebär att du autentiserar mot ditt eget inloggningssystem, inte mot [!DNL Workfront Proof]Inloggningssida.

Du måste ha konfigurerat anpassade underdomäner eller domäner på din [!DNL Workfront] Korrekturkonto för att aktivera SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Du kan läsa mer om fullt anpassade domäner i  [Varumärken [!DNL Workfront Proof] webbplats - avancerad](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Se [Konfigurera enkel inloggning för [!DNL Workfront Proof] användare](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) om du vill ha information om hur du konfigurerar enkel inloggning för ditt konto.
