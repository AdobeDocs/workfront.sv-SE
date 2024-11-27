---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler-inställningar kan ge sämre prestanda
description: När användaren har skapats kan du redigera användaren och aktivera"Tillåt endast SAML 2.0-autentisering" så att användaren och lösenordet styrs av SAML-systemet. När det här alternativet är aktiverat kan användaren bara logga in via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: ZScaler-inställningar kan ge sämre prestanda

>[!NOTE]
>
>Detta är ett problem med ZScaler och kommer inte att åtgärdas av Workfront.

ZScalers webbtjänst använder `http/1.1` som standard, vilket kan ge sämre prestanda i Workfront.

Konfigurera ZScaler-programmet så att `http/2` används för att kontrollera och lösa problemet. Detta kan inte konfigureras i Workfront.

Du hittar information om `http/2` i dokumentationen för ZScaler.
