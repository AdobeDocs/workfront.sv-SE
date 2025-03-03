---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Automatiska påminnelser jämfört med påminnelser
description: I den här artikeln beskrivs skillnaderna mellan automatiska påminnelser och påminnelsemeddelanden och olika scenarier för varje.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Automatiska påminnelser jämfört med påminnelser

I den här artikeln beskrivs skillnaderna mellan automatiska påminnelser och påminnelsemeddelanden och olika scenarier för varje. Mer information om alla [!DNL Adobe Workfront]-meddelanden finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

## Automatiska påminnelser

Följande kännetecken är specifika för automatiska påminnelser:

* Kan endast aktiveras och redigeras av en [!DNL Workfront]-administratör
* Utlöses för alla uppgifter och ärenden när de förfaller, förfaller eller ligger nära det planerade slutförandedatumet
* Kan endast skickas till den som har utsetts, den som har utsetts eller till chef för den som har hand om ärendet.
* Det går inte att koppla en e-postmall till dem.

Scenario: Om du vill att påminnelser ska utlösas för alla uppgifter och problem i hela systemet konfigurerar du de automatiska påminnelseinställningarna. Mer information finns i [Konfigurera automatiska påminnelser](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Påminnelsemeddelanden

Följande egenskaper är specifika för påminnelsemeddelanden:

* Kan skapas av en administratör eller andra användare med en planlicens och administrativ åtkomst till påminnelsemeddelanden
* Kan endast kopplas manuellt till ett objekt
* Det går bara att meddela om det bifogade objektet
* Kan skickas till olika objektintressenter, till exempel ägare, skapare, godkännare eller tilldelad
* Kan antingen använda standardmeddelandet eller använda en anpassad e-postmall som bifogas

Scenario: Om du vill skapa påminnelser för projekt, tidrapporter eller vill anpassa påminnelser för uppgifter och ärenden konfigurerar du påminnelsemeddelanden. Mer information finns i [Konfigurera påminnelsemeddelanden](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
