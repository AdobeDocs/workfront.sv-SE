---
content-type: reference
navigation-topic: get-started-with-workfront
title: HIPAA-beredskap för Workfront
description: En Workfront-kund som, enligt definitionen i HIPAA, är en Business Associate och/eller den enhet som omfattas för vars räkning Business Associate tillhandahåller Adobe Workfront, bör använda följande riktlinjer för att konfigurera Workfront för HIPAA-klar användning.
feature: Get Started with Workfront
author: Courtney
hide: true
hidefromtoc: true
source-git-commit: 779fc409d316e957a4cbec951047e41641b69863
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# HIPAA-beredskap för Workfront

En Workfront-kund som, enligt definitionen i HIPAA, är en **Business Associate** och/eller den **Enhet som omfattas** och som Business Associate tillhandahåller Adobe Workfront för, ska använda följande riktlinjer för att konfigurera Workfront för HIPAA-klar användning:


## Lösenordskrav

| **Säkerhetsinställning** | **Vad är det?** | **Krav** |
|----------------------|------------------|------------------|
| Minsta lösenordsstyrka för avtal | Vilken är den minsta styrkan för avtalslösenord? | Minst 8 tecken |
| Minsta lösenordsstyrka för användarlösenord | Vilken minsta styrka har användarens lösenord? | Tecken från tre av följande kategorier:<br>* Versaler (latinskt alfabet)<br>* Gemener (latinskt alfabet)<br>* Bas 10 siffror<br>* Icke-alfanumeriska tecken |
| Lösenordsvaraktighet | Hur länge ska lösenord tillåtas förbli oförändrade? | Lösenord bör ändras minst var 90:e dag |
| Lösenordshistorik | Hur många tidigare lösenord ska sparas och inte tillåtas? | Minst 5 |


## Inloggningskrav

| **Säkerhetsinställning** | **Vad är det?** | **Krav** |
|----------------------|------------------|------------------|
| Maximalt antal inloggningsfel | Hur många misslyckade inloggningsförsök gör att användaren låses? | Högst 5 försök inom 5 minuter; försök tillåts efter 30 minuter |
| Maximalt antal SSO-verifieringsfel | Hur många misslyckade försök till SSO-verifiering orsakar utelåsning? | Högst 5 (gäller endast kunder som använder enkel inloggning) |


## Sessionskrav

| **Säkerhetsinställning** | **Vad är det?** | **Krav** |
|----------------------|------------------|------------------|
| Tidsgräns för session | Hur många minuters inaktivitet orsakar utloggning? | Högst 15 minuter |

## Kundens ansvar

Se till att alla anställda, representanter och/eller agenter är medvetna om och förstår villkoren i det eller de licensavtal och/eller serviceavtal som ingåtts mellan parterna, beroende på vad som är tillämpligt, för användningen av data med Workfront.

Bland annat bör följande ansvarsområden och skyldigheter ses över och meddelas: 

* Kunden ansvarar för att alla användare använder Workfront Service. 

* Kunden måste uppfylla alla villkor i avtalet med Adobe som innehåller förbjudna dataelement som kan överföras till Workfront. 

* Alla känsliga data, inklusive, men inte begränsat till, ePHI överförs på kundens egen risk.  Kunden ansvarar alltid för alla kunddata. 


## Dataskydd och efterlevnad

>[!IMPORTANT]
>
>Workfront är inte avsett att användas som arkiv för elektroniska patientjournaler. ePHI får endast behandlas om Adobe uttryckligen ger sitt skriftliga tillstånd. 

* Kontrollera att **Kryptering vid vila (EAR)** är aktiverat för alla Workfront-databaser där ePHI kan vara tillgänglig.
   * Kontakta din kontoansvarige (AE) för att kontrollera att EAR ingår i ditt köp av Workfront.
   * Konfigurera system/databaser som är tillgängliga via Workfront för att uppfylla efterlevnadskrav.
* Säkerställ att ePHI inte överförs, länkas eller delas med andra Adobe-lösningar.
* Se till att patientfotografier som bearbetas via Workfront lagras säkert och inte är tillgängliga för allmänheten.