---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Enkel inloggning i  [!DNL Workfront Proof]
description: Med enkel inloggning (SSO) kan dina användare logga in på [!DNL Workfront Proof] med organisationens befintliga användarnamn och lösenord.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Enkel inloggning i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

En [!UICONTROL Enterprise] [!DNL Workfront]-plan krävs för att använda den här funktionen. Mer information om olika tillgängliga planer finns i [Workfront-planer](https://business.adobe.com/se/products/workfront/pricing.html).

Med enkel inloggning (SSO) kan dina användare logga in på [!DNL Workfront Proof] med organisationens befintliga användarnamn och lösenord.

För att tillhandahålla den här funktionen använder vi [!DNL Security Assertion Markup Language] (SAML) 2.0, ett XML-baserat protokoll som gör att du kan auktorisera data och utbyta autentisering mellan en identitetsleverantör och en webbtjänst.

Det innebär att du autentiserar dig mot ditt eget inloggningssystem, inte mot inloggningssidan för [!DNL Workfront Proof].

Du måste ha konfigurerat en anpassad underdomän eller domän på ditt [!DNL Workfront]-korrekturkonto för att kunna aktivera SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Du kan läsa mer om fullständigt anpassade domäner i [Varumärket på  [!DNL Workfront Proof] webbplatsen - avancerat](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Se [Konfigurera enkel inloggning för [!DNL Workfront Proof] användare](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) för information om hur du konfigurerar enkel inloggning för ditt konto.
