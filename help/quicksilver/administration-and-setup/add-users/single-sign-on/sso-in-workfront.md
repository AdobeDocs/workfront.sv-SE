---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Översikt över enkel inloggning i Adobe Workfront
description: Workfront har en centralt hanterad konfiguration för enkel inloggning (SSO) som enkelt kan integrera Workfront med företagets befintliga SSO-lösning. Den här konfigurationen är enkel att konfigurera och hantera och är tillgänglig för både OnDemand- och OnPremise Enterprise-kunder.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Översikt över enkel inloggning i Adobe Workfront

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront har en centralt hanterad konfiguration för enkel inloggning (SSO) som integrerar Workfront med företagets SSO-lösning. Den här konfigurationen är tillgänglig för både OnDemand- och OnPremise Enterprise-kunder.

Om du vill använda SSO-funktionen i Workfront måste din organisation konfigurera ett SSO-program. Sedan kan du konfigurera Workfront så att det kan kommunicera med din SSO-lösning.

Med federerade lösningar kan användarna logga in på alla sina program genom att ange sitt användarnamn och lösenord i en central inloggningsportal.

![enkel inloggning (SSO) federerad](assets/overview-sso-wf-fed-only.png)


## Konfigurera brandväggen

När du använder en SSO-lösning initierar Workfront en anslutning till servern på den angivna porten.

Om brandväggen eller e-postservern är konfigurerad att endast tillåta åtkomst till vissa leverantörer måste du lägga till vissa Workfront IP-adresser i tillåtelselista för brandväggen. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurera enkel inloggning

Workfront kan integreras med följande SSO-lösningar:

* Samordnade lösningar som stöder SAML 2.0

  Information om hur du integrerar Workfront med SAML 2.0 finns i [Konfigurera Adobe Workfront med SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Samordnade lösningar som stöder SAML 2.0 med hjälp av ADFS

  Information om hur du integrerar Workfront med SAML 2.0 med ADFS finns i [Konfigurera Adobe Workfront med SAML 2.0 med ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
