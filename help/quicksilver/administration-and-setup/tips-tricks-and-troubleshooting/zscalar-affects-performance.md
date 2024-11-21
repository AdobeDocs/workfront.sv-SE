---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar-inställningar kan ge sämre prestanda
description: När användaren har skapats kan du redigera användaren och aktivera"Tillåt endast SAML 2.0-autentisering" så att användaren och lösenordet styrs av SAML-systemet. När det här alternativet är aktiverat kan användaren bara logga in via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScalar-inställningar kan ge sämre prestanda

>[!NOTE]
>
>Detta är ett problem med ZScalar och kommer inte att åtgärdas av Workfront.

ZScalars webbtjänst använder `http/1.1` som standard, vilket kan ge sämre prestanda i Workfront.

Konfigurera ZScalar-programmet så att `http/2` används för att kontrollera och lösa problemet. Detta kan inte konfigureras i Workfront.

Du hittar information om `http/2` i dokumentationen för ZScalar.
