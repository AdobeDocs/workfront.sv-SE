---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Behörighetsprofiler för korrektur i Workfront Proof
description: Som Workfront-administratör eller Workfront Proof-administratör kan du tilldela en korrekturbehörighetsprofil till en användare för att ange vilka korrekturfunktioner som användaren ska ha för alla korrektur i systemet. Mer information om hur du konfigurerar en användares behörighetsprofil för korrektur finns i Konfigurera en användares behörighetsprofil för korrektur i Workfront Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1758'
ht-degree: 0%

---

# Korrektur för behörighetsprofiler i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Som administratör för [!DNL Workfront] eller administratör för [!DNL Workfront Proof] kan du tilldela en användare en behörighetsprofil för korrektur för att ange de språkfunktioner som användaren ska ha för alla korrektur i systemet. Mer information om hur du konfigurerar en användares behörighetsprofil för korrektur finns i [Konfigurera en användares behörighetsprofil för korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Du kan också göra följande:
>
>* Bevilja användarspecifika roller för enskilda korrektur. Mer information om korrekturroller finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Skapa anpassade profiler för användare i organisationen. Mer information finns i [Konfigurera anpassade profiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

I följande tabell visas de behörigheter som är tillgängliga för respektive behörighetsprofil.

| **Egna objekt** |  |  |  |  | **Andra användares objekt** |  |  | **Admin** | **Fakturering** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Lägg till** | **Visa** | **Redigera** | **Ta bort** | **Visa** | **Redigera** | **Ta bort** | **Redigera och ta bort** | **Redigera** |
| Faktureringsadministratör | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Administratör | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisor | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Manager | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Observer |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Besökare |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Tänk på följande när det gäller roller och behörigheter:

* Tilldelade profilbehörigheter gäller endast för användarna och objekten i ditt eget konto. Undantaget är när det gäller satellitkonton, där Administratör och Faktureringsadministratör för huvudkonton (navkonton) kan komma åt och hantera kontoinställningarna och faktureringen av dessa konton från navkontonivån.
* Faktureringsadministratörer och administratörer kan ta bort användare. Detta kan bara göras i kontoinställningarna.
* När faktureringsadministratörer och administratörer visar korrektur som ägs av andra användare i deras konto, visar de dem med rollen som granskare.
* Med rollen Skrivskyddad kan faktureringsadministratörer och administratörer komma åt korrektur i mappar som delas med dem eller i mappar som de skapar.

I följande avsnitt beskrivs varje profil och de behörigheter som är associerade med profilen i en standardinställning för [!DNL Workfront Proof]:

* [Faktureringsadministratör](#billing-administrator)
* [Administratör](#administrator)
* [Ansvarig](#supervisor)
* [Hanteraren](#manager)
* [Observer](#observer)
* [Besökare](#visitor)
* [Gäst](#guest)

## Faktureringsadministratör {#billing-administrator}

Faktureringsadministratörer har åtkomst till [kontoinställningarna på  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] faktureringssidan](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) och har följande behörigheter:

![](assets/cleaner2.png)Kan generera korrektur, överföra filer och skapa mappar. Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) och [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan visa, redigera och ta bort egna korrektur och filer som de skapar.

![](assets/cleaner2.png)Kan visa, redigera och ta bort korrektur och filer som skapats av alla användare i organisationen.

![](assets/cleaner2.png)Kan ta bort gemensamma mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Har redigeringsbehörighet för alla korrektur som skapats i kontot.

![](assets/cleaner2.png)Kan anges som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan komma åt faktureringssidan och redigera faktureringsinformationen. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] Faktureringssidan](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Kan komma åt sidan Kontoinställningar och redigera kontoinformationen. Mer information finns i [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kan tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kan lägga till, redigera och ta bort användare.

![](assets/cleaner2.png)Kan skapa grupper och lägga till nya kontakter.

![](assets/cleaner2.png)Kan ta bort kontakter.

![](assets/cleaner2.png)Kan redigera korrektur om det inte finns några svar på dem.

![](assets/no2.png)Det går inte att redigera korrektursvar.

![](assets/no2.png)Det går inte att ta bort privata mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Mer information om kontoinställningar finns i [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Information om fakturering finns på [Faktureringssidan [!DNL Workfront Proof] Faktureringssidan](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administratör {#administrator}

Administratörer har åtkomst till [kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)och har följande behörigheter:

![](assets/cleaner2.png)Kan skapa korrektur, överföra filer och skapa mappar. Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) och [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan visa, redigera och ta bort korrektur och filer som de har skapat.

![](assets/cleaner2.png)Kan visa, redigera och ta bort korrektur och filer som skapats av alla användare i organisationen.

![](assets/cleaner2.png)Kan ta bort gemensamma mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Har redigeringsbehörighet för alla korrektur som skapats i kontot.

![](assets/cleaner2.png)Kan anges som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan komma åt sidan Kontoinställningar och redigera kontoinformationen. Mer information finns i [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kan tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kan lägga till, redigera och ta bort användare.

![](assets/cleaner2.png)Kan skapa grupper och lägga till nya kontakter.

![](assets/cleaner2.png)Kan ta bort kontakter.

![](assets/cleaner2.png)Kan redigera korrektur om det inte finns några svar på dem.

![](assets/no2.png)Det går inte att redigera korrektursvar.

![](assets/no2.png)Det går inte att ta bort privata mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Det går inte att komma åt sidan Fakturering eller redigera faktureringsinformationen. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] Faktureringssidan](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

Tillsynsmannen har följande behörigheter:

![](assets/cleaner2.png)Kan skapa korrektur, överföra filer och skapa mappar. Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) och [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan visa, redigera och ta bort egna korrektur och filer som de har skapat.

![](assets/cleaner2.png)Kan visa, redigera och ta bort korrektur och filer som skapats av alla användare i organisationen.

![](assets/cleaner2.png)Kan ta bort gemensamma mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Har redigeringsbehörighet för alla korrektur som skapats i kontot.

![](assets/cleaner2.png)Kan anges som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kan skapa grupper och lägga till nya kontakter.

![](assets/cleaner2.png)Kan ta bort kontakter.

![](assets/cleaner2.png)Kan redigera korrektur om det inte finns några svar på dem.

![](assets/no2.png)Det går inte att redigera korrektursvar.

![](assets/no2.png)Det går inte att ta bort privata mappar för andra användare. Mer information finns i [Mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Det går inte att komma åt faktureringssidan eller kontoinställningarna. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] och ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Det går inte att lägga till, redigera eller ta bort användare.

![](assets/no2.png)Kan inte tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager {#manager}

Chefer har följande behörigheter:

![](assets/cleaner2.png)Kan skapa korrektur, överföra filer och skapa mappar. Mer information finns i [Skapa korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) och [Skapa mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kan visa, redigera och ta bort egna korrektur och filer som de skapar eller äger.

![](assets/cleaner2.png)Kan visa, granska och godkänna korrektur för andra användare som delas med dem (skrivskyddad behörighet till allt i en delad mapp). Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan skapa grupper och lägga till en ny kontakt.

![](assets/no2.png)Det går inte att visa, redigera eller ta bort korrektur och filer som skapats av andra användare i organisationen.

![](assets/no2.png)Det går inte att redigera korrektur eller svar.

![](assets/no2.png)Det går inte att ta bort privata mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Det går inte att ta bort gemensamma mappar för andra användare. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Det går inte att komma åt faktureringssidan eller kontoinställningarna. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] och ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Det går inte att ange som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan inte tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Det går inte att lägga till, redigera eller ta bort användare.

![](assets/no2.png)Det går inte att ta bort kontakter.

### Observer {#observer}

Observatörer har följande behörigheter:

![](assets/cleaner2.png)Kan visa, granska och godkänna korrektur för andra användare som delas med dem (skrivskyddad behörighet till allt i en delad mapp). Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan visa filer som delas med dem.

![](assets/cleaner2.png) Kan visa kontakter och grupper

![](assets/no2.png)Det går inte att skapa korrektur, överföra filer och skapa mappar. Mer information finns i [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Det går inte att visa, redigera eller ta bort korrektur och filer som skapats av andra användare i organisationen.

![](assets/no2.png)Det går inte att redigera korrektur eller svar.

![](assets/no2.png)Det går inte att ta bort objekt som har skapats i organisationen.

![](assets/no2.png)Det går inte att komma åt faktureringssidan eller kontoinställningarna. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] och ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Det går inte att ange som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan inte tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Det går inte att lägga till, redigera eller ta bort användare.

![](assets/no2.png)Det går inte att skapa grupper eller lägga till nya kontakter.

![](assets/no2.png)Det går inte att ta bort kontakter.

>[!NOTE]
>
>De menyer och funktioner som är tillgängliga för observatörer är begränsade.
>
>* Observatörer kan inte se rubrikmenyn eller den gröna nya menyn på sin Dashboard
>* Följande länkar visas inte i deras inställningar: Kontoinställningar, Fakturering
>

### Besökare {#visitor}

Besökarna har följande behörigheter:

![](assets/cleaner2.png)Kan visa, granska och godkänna korrektur för andra användare som delas med dem (skrivskyddad behörighet till allt i en delad mapp). Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kan visa filer som delas med dem.

![](assets/no2.png) Kan inte visa kontakter och grupper

![](assets/no2.png)Det går inte att skapa korrektur, överföra filer och skapa mappar. Mer information finns i [Överför filer och webbinnehåll till [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Det går inte att visa, redigera eller ta bort korrektur och filer som skapats av andra användare i organisationen.

![](assets/no2.png)Det går inte att redigera korrektur eller svar.

![](assets/no2.png)Det går inte att ta bort objekt som har skapats i organisationen.

![](assets/no2.png)Det går inte att komma åt faktureringssidan eller kontoinställningarna. Mer information finns i [Faktureringssidan [!DNL Workfront Proof] och ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) [Kontoinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Det går inte att ange som Dropzone-ägare. Mer information finns i [Konfigurera dropzone i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Kan inte tömma papperskorgen. Mer information finns i [Återställa och tömma papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Det går inte att lägga till, redigera eller ta bort användare.

![](assets/no2.png)Det går inte att skapa grupper eller lägga till nya kontakter.

![](assets/no2.png)Det går inte att ta bort kontakter.

>[!NOTE]
>
>De menyer och funktioner som är tillgängliga för besökare är begränsade.
>
>* Besökarna kan inte se rubrikmenyn eller den gröna nya menyn på sin kontrollpanel
>* Besökarna ser inte följande länkar i sina inställningar: Kontoinställningar, Fakturering
>

### Gäst {#guest}

Gästprofilen används för att ge åtkomst till korrektur för granskare som inte har ett eget Workfront Proof-konto. Gäster kan komma åt korrektur som delas med dem direkt via sina personliga e-postmeddelanden.

![](assets/cleaner2.png)Kan visa, granska och godkänna korrektur som delas med dem.

![](assets/cleaner2.png)Kan visa filer som delas med dem.

![](assets/no2.png)Det går inte att komma åt instrumentpanelen.

![](assets/no2.png)Det går inte att dela mappar med dem. Mer information finns i [Hantera mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Det går inte att lägga till som författare eller moderatorer till korrektur. Mer information finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Gäster är inte Workfront Proof-användare, så de kan inte se alla korrektur som delas med dem på sin egen Dashboard.

## Redigera en användares behörighetsprofil för korrektur

Administratörer och faktureringsadministratörer kan redigera behörighetsprofilerna för alla användare i kontot.

1. Gör något av följande för att hitta användaren som ska redigeras:

   * Navigera till **[!UICONTROL Account Settings]** och klicka sedan på fliken **[!UICONTROL Users]**.

   * Gå till sidan **[!UICONTROL Contacts]**.

1. Klicka på det användarnamn vars behörigheter du vill redigera. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Klicka på listrutan **[!UICONTROL Permissions profile]** och välj en ny behörighetsprofil. :

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   Behörighetsprofiler är Administratör, Ansvarig, Hanterare och Observer.

1. Klicka utanför menyn som du vill spara.

>[!NOTE]
>
>Administratörer kan inte tilldela profilen Faktureringsadministratör. Du hittar en lista över profiländringar i följande loggar:
>
>* Loggar för kontoaktivitet
>* Användarens profillogg (endast tillgänglig för den användaren)
>

Mer information om aktivitetsloggar finns i [Förstå  [!DNL Workfront Proof] Aktivitetsgranskningsspåret](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
