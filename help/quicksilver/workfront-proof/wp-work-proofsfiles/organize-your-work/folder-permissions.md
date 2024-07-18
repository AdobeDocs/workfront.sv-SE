---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Förstå mappbehörigheter i  [!DNL Workfront Proof]
description: Om en person har behörighet att se ett objekt i en mapp kan han eller hon även se själva mappen. De kan dock bara se de objekt i mappen som har delats med dem.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Förstå mappbehörigheter i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om en person har behörighet att se ett objekt i en mapp kan han eller hon även se själva mappen. De kan dock bara se de objekt i mappen som har delats med dem.

## Gemensamma mappar

Om en mapp är offentlig kan användare på kontot (förutom observatörer och ljusanvändare) se mappnamnet i den vänstra sidofältet.

Din behörighetsprofil påverkar även de behörigheter du har över gemensamma mappar:

| **Profil/åtgärd** | **Visa alla objekt i mappen** | **Visa objekt som delas med dem** | **Lägg till objekt** | **Ta bort objekt** | **Lägg till undermappar** | **Ta bort undermappar** | **Redigera mappinformation** |
|---|---|---|---|---|---|---|---|
| **Skapare** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Faktureringsadministratör** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administratör** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Ansvarig** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Hanteraren** | Nej | Ja | Ja | Nej | Ja | Nej | Ja |
| **Observer** | Nej | Ja | Nej | Nej | Nej | Nej | Nej |

{style="table-layout:auto"}

Om den gemensamma mappen ägs av en hanterare kan han eller hon ta bort rotmappen och alla undermappar.

Mer information finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Privata mappar

Om en mapp är privat kommer andra användare på samma konto inte att kunna se namnet på mappen i det vänstra sidofältet såvida inte mappen eller objekten i mappen uttryckligen har delats med dem eller de har en profil som Supervisor, Administratör eller Faktureringsadministratör:

| **Profil/åtgärd** | **Visa alla objekt i mappen** | **Visa objekt som delas med dem** | **Lägg till objekt** | **Ta bort objekt** | **Lägg till undermappar** | **Ta bort undermappar** | **Redigera mappinformation** |
|---|---|---|---|---|---|---|---|
| **Skapare** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Faktureringsadministratör** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administratör** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Ansvarig** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Hanteraren** | Nej | Ja | Nej | Nej | Nej | Nej | Nej |
| **Observer** | Nej | Ja | Nej | Nej | Nej | Nej | Nej |

{style="table-layout:auto"}

Om du t.ex. vill att projektledaren och deras team bara ska se specifika mappar, kan projektledaren konfigurera en privat mapp och sedan dela mappen med specifika användare.

När du delar en privat mapp kan du bestämma om du vill att hanterare ska kunna skapa, redigera och ta bort mappobjekt.

Du kan ange detta för varje person separat på sidan Ny mapp och ändra det i avsnittet [!UICONTROL Shared with] på sidan Mappinformation. Mer information finns i [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) och [Hantera mappar och deras innehåll i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Om en privat mapp delas med en observatör eller en observatör får de skrivskyddad åtkomst till alla objekt i mappen. Mer information finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Dela mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Om en överordnad mapp är privat kommer alla undermappar också att vara privata. Du kan inte ha en offentlig undermapp under en privat överordnad mapp. Du kan dock ha en privat undermapp under en offentlig överordnad mapp.
>* Mappens skapare och ägare har alltid åtkomst till den och kan inte tas bort.
>* Det är bara skaparen och ägaren av den privata mappen som kan ta bort mappen.

