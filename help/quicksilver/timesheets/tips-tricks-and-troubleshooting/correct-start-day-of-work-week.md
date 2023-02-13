---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Korrigera arbetsveckans startdag för tidrapporter
description: Veckodagens startdag på min tidrapport matchar inte veckodagens startdag som har konfigurerats på min tidrapportprofil.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Korrigera arbetsveckans startdag för tidrapporter

## Problem

Veckodagens startdag på min tidrapport matchar inte veckodagens startdag som är konfigurerad på min tidrapportprofil (enligt beskrivningen i [Skapa, redigera och tilldela tidrapportprofiler](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Lösning

Startdagen i veckan för en tidrapport i Adobe Workfront använder språk- och språkinställningarna i webbläsaren för att bestämma veckodagen. På grund av detta måste du uppdatera språk- och språkinställningarna för webbläsaren. 

Om webbläsarspråket till exempel är Engelska och språkinställningen är USA, startar veckan på söndag. Alternativt kan webbläsarspråket anges till engelska och språkinställningen till Storbritannien är startdagen måndag.

Den här inställningen påverkar även veckostartdagen i popup-kalendrar i systemet.

Ändringen av språkinställningen påverkar inte veckostartdagen i resursstödrastret (eller resurstödrastervyn). Veckan börjar alltid på söndag.

Här följer anvisningar om hur du ändrar språk- och språkinställningar för olika webbläsare som stöds av Workfront.

* **Krom:** Kopiera och klistra in följande länk i webbläsaren Chrome: `chrome://settings/languages` sedan till Språk.
* **Firefox:**Kopiera och klistra in följande länk i din Firefox-webbläsare: `about:preferences#content` sedan till Språk.
* **IE 11:** Verktyg -> Internetalternativ -> Allmänt -> Språk
* **Safari:** Tyvärr tillåter inte Safari att du byter webbläsarspråk utan att ändra hela operativsystemets språk. Det är antagligen enklare att installera en annan webbläsare, som Chrome eller Firefox.

 
