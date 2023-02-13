---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Testmiljö för förhandsgranskning av sandlådor - [!DNL Workfront Proof]
description: Sandlådan Preview är en testmiljö som fungerar som en kopia av din aktiva miljö och uppdateras varje helg av [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Testmiljö för förhandsgranskning av sandlådor - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Sandlådan Preview är en testmiljö som fungerar som en kopia av din aktiva miljö och uppdateras varje helg av [!DNL Workfront Proof].

## Förstå förhandsvisningssandlådan

Sandlådan för förhandsgranskning fungerar som en miljö där användare i organisationen kan testa och arbeta med data från produktionsmiljön utan att påverka produktionsmiljön. Det är idealiskt för att genomföra utbildningstillfällen, testa nya funktioner och fastställa installationsfunktioner.

Dessutom överförs nya produktfunktioner till förhandsgranskningssandlådan innan de levereras till produktionsmiljön. Dina användare kan testa nya funktioner där utan att det påverkar deras vanliga arbetsflöde i produktionsmiljön.

Sandlådan för förhandsgranskning innehåller dina faktiska produktionsdata. Data flödar från produktion till förhandsgranskning, inte tvärtom. Den uppdateras varje helg så att data kan ligga upp till en vecka bakom produktionsmiljön. Objekt som har skapats sedan den senaste uppdateringstiden finns i förhandsvisningens sandlådemiljö tills nästa uppdatering.

## Åtkomst till sandlådan Förhandsgranska

Som standard har du som systemadministratör tillgång till sandlådemiljön för förhandsgranskning. Kontakta din [!DNL Workfront] eller vårt supportteam.

* [Åtkomst till förhandsvisningssandlådan som fristående [!DNL Workfront Proof] Kund](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Åtkomst till förhandsvisningssandlådan som en [!DNL Workfront]+[!DNL Workfront Proof] Kund](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Åtkomst till förhandsvisningssandlådan som fristående [!DNL Workfront Proof] Kund

1. Navigera till denna URL:  `https://preview.proofhq.com`.
1. Logga in med dina autentiseringsuppgifter för förhandsgranskning.\
   Dina autentiseringsuppgifter för förhandsgranskning bör vara desamma som dina produktionsuppgifter om du inte har ändrat dem i Produktion efter att uppdateringen av förhandsvisningen har utförts. Inloggningarna synkroniseras bara när en uppdatering görs, vilket sker varje helg. De synkroniseras inte automatiskt.

### Åtkomst till förhandsvisningssandlådan som en [!DNL Workfront+Workfront] Korrektur för kund

Som systemadministratör har du åtkomst till [!DNL Workfront Proof] Förhandsgranska sandlåda via [!DNL Workfront] gränssnitt.

Så här öppnar du [!DNL Workfront Proof] Sandlåda för förhandsgranskning:

1. Logga in på [!DNL Workfront] miljö.
1. Klicka **[!UICONTROL Setup]** i fältet Global navigering.
1. Klicka på **[!UICONTROL System]** >**[!UICONTROL Preferences]**.

1. I **[!UICONTROL Test Environments]** avsnitt, klicka **[!UICONTROL Sandbox Preview]**.

1. Logga in med dina autentiseringsuppgifter för förhandsgranskning.\
   Dina autentiseringsuppgifter för förhandsgranskning bör vara desamma som dina produktionsuppgifter såvida du inte har ändrat dem i Produktion efter att uppdateringen av förhandsgranskningen har utförts. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.
1. Klicka på [!DNL Workfront Proof] -ikonen i det globala navigeringsfältet.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   The [!DNL Workfront Proof] Förhandsvisningsmiljön visas.

## Ta emot e-postmeddelanden från sandlådan Förhandsgranska

E-postmeddelanden utlöses aldrig från [!DNL Workfront Proof] Förhandsvisningsmiljö.
