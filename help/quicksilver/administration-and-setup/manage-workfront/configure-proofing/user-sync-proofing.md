---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Användarsynkronisering mellan Adobe Workfront och Workfront Proof
description: Användarinformationen synkroniseras från Adobe Workfront till Workfront Proof och synkroniseras inte från Workfront Proof till Workfront. På grund av detta måste du göra ändringarna i Workfront varje gång du skapar eller ändrar användare. Du kan inte göra ändringar för användare i Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Användarsynkronisering mellan Adobe Workfront och Workfront Proof

Användarinformationen synkroniseras från Adobe Workfront till Workfront Proof och synkroniseras inte från Workfront Proof till Workfront. På grund av detta måste du göra ändringarna i Workfront varje gång du skapar eller ändrar användare. Du kan inte göra ändringar för användare i Workfront Proof.

Följande avsnitt innehåller information om användarsynkronisering från Workfront till Workfront Proof:

## Synkroniserad information

Workfront synkroniserar följande användarinformation med Workfront Proof:

* Namn (användarens för- och efternamn)
* E-postadress

## När synkronisering sker

Användarinformationen synkroniseras från Workfront till Workfront Proof under följande omständigheter:

* En användares information uppdateras i Workfront
* En användare skapas i Workfront

Beroende på om det finns en användare med samma e-postadress i Workfront Proof händer något av följande:

* **Om det inte finns någon användare med ett matchande e-postmeddelande i Workfront Proof och**

   * **Språkkontroll är aktiverat för användaren:** Användaren skapas som en användare i Workfront Proof.
   * **Språkkontroll är inte aktiverat för användaren:** Användaren skapas som en kontakt i Workfront Proof.

* **Om det finns en användare med ett matchande e-postmeddelande i Workfront Proof:** Korrektur är aktiverat för den användaren i Workfront (om det inte redan har aktiverats) och informationen synkroniseras mellan de två användarna.

  Mer information finns i [Konfigurera en användares språkkontroll](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) i [Konfigurera en användares språkkontroll](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >När det finns en användare med ett matchande e-postmeddelande, i sin egen eller i någon annan korrekturmiljö, skapar Workfront en e-postadress för alias genom att lägga till användarens konto-ID som ett suffix till användarens e-postadress. Exempel: *username+accountid@domain.com*. Användarna får fortfarande korrekturmeddelanden om ett aliasmeddelande skapas.
