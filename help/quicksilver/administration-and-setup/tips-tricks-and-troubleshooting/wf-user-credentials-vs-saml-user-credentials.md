---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront användarautentiseringsuppgifter jämfört med  [!DNL SAML] användarautentiseringsuppgifter
description: När användaren har skapats kan du redigera användaren och aktivera"Tillåt endast SAML 2.0-autentisering" så att användaren och lösenordet styrs av SAML-systemet. När det här alternativet är aktiverat kan användaren bara logga in via SAML. När de går till  [!DNL Workfront] URL:en omdirigeras de automatiskt till SAML-systemet och uppmanas att ange sitt SAML-användarnamn och -lösenord.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfront användaruppgifter jämfört med SAML användaruppgifter

Den här artikeln fokuserar specifikt på [!DNL Adobe Workfront] och SAML och omfattar inte andra SSO-autentiseringsmetoder.

I en databas lagrar [!DNL Workfront] varje användares e-postadress som sitt [!DNL Workfront]-användarnamn tillsammans med sitt [!DNL Workfront]-lösenord. Dessa autentiseringsuppgifter replikeras i sandlådorna för förhandsgranskning och anpassad uppdatering.

Om [!DNL Workfront] upptäcker att SAML 2.0 är konfigurerat när användaren skapas blir standardvärdet&quot;Tillåt endast SAML 2.0-autentisering&quot; för användaren. Om rutan&quot;Skicka en inbjudan via e-post till den här personen&quot; är aktiverad inaktiverar [!DNL Workfront]&quot;Tillåt endast SAML 2.0-autentisering&quot; och döljer det här alternativet. När&quot;Skicka en inbjudan via e-post till den här personen&quot; har aktiverats blir användaren en icke-SAML [!DNL Workfront]-användare.

När användaren har skapats kan du redigera användaren och aktivera **[!UICONTROL Only Allow SAML 2.0 Authentication]** så att användarens användare och lösenord styrs av SAML-systemet.

När detta är gjort kan användaren bara logga in via SAML. När de går till URL:en för [!DNL Workfront] omdirigeras de automatiskt till SAML-systemet och uppmanas att ange sitt SAML-användarnamn och -lösenord.

SAML-autentiseringsuppgifter lagras i ett externt SAML-system, till exempel Microsoft ADFS, och inte i Workfront.
