---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Översikt över enkel inloggning i Adobe Workfront
description: Workfront har en centralt hanterad konfiguration för enkel inloggning (SSO) som enkelt kan integrera Workfront med företagets befintliga SSO-lösning. Den här konfigurationen är enkel att konfigurera och hantera och är tillgänglig för både OnDemand- och OnPremise Enterprise-kunder.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Översikt över enkel inloggning i Adobe Workfront

{{important-admin-console-onboard}}


Workfront har en centralt hanterad konfiguration för enkel inloggning (SSO) som enkelt kan integrera Workfront med företagets befintliga SSO-lösning. Den här konfigurationen är enkel att konfigurera och hantera och är tillgänglig för både OnDemand- och OnPremise Enterprise-kunder.

För att du ska kunna använda SSO-funktionerna i Workfront måste din organisation konfigurera ett SSO-program. Sedan kan du konfigurera Workfront så att det kan kommunicera med din SSO-lösning.

Med federerade lösningar kan användarna logga in på alla sina program genom att ange sitt användarnamn och lösenord i en central inloggningsportal.

![](assets/overview-sso-wf.png)


## Konfigurera brandväggen

När du använder en SSO-lösning initierar Workfront en anslutning till servern på den angivna porten.

Om du prenumererar på Workfront on-demand och om du har konfigurerat brandväggen eller e-postservern så att endast vissa leverantörer tillåts åtkomst till den, måste du lägga till vissa IP-adresser för Workfront i brandväggens tillåtelselista. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurera enkel inloggning

Workfront kan integreras med följande SSO-lösningar:

* Samordnade lösningar som stöder SAML 2.0

   Mer information om hur du integrerar Workfront med SAML 2.0 finns i [Konfigurera Adobe Workfront med SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Samordnade lösningar som stöder SAML 2.0 med hjälp av ADFS

   Mer information om hur du integrerar Workfront med SAML 2.0 med ADFS finns i [Konfigurera Adobe Workfront med SAML 2.0 med ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
