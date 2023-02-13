---
content-type: reference
navigation-topic: announcements
title: Ändringar som krävs för att lägga till korrektur i tillåtelselista
description: Korrekturdomänen ändras från proofhq.com till workfront.com.
author: Luke
feature: Product Announcements
exl-id: 05a1fd37-224b-4a0b-abef-4d9a015de524
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Ändringar som krävs för att lägga till korrektur i tillåtelselista

Korrekturdomänen ändras från proofhq.com till workfront.com.

Om din brandvägg eller e-postserver är konfigurerad att endast tillåta åtkomst till vissa leverantörer, måste du lägga till följande extra URL-adress i din tillåtelselista för att se till att användare i din organisation kan visa korrektur i Adobe Workfront både i webbläsarvisningsprogrammet och i skrivbordsvisningsprogrammet:

&#42;.workfront.com

The &#42;proofhq.com URL krävs också.

Mer information om hur du uppdaterar tillåtelselista finns i [Konfigurera brandväggens tillåtelselista](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Denna uppdatering gäller endast korrektur inom Workfront; gäller inte när du använder det fristående Workfront Proof-programmet.
