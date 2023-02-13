---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: The [!DNL Workfront] Korrekturfaktureringssida
description: Så här öppnar du [!UICONTROL Billing] öppnar du inställningsmenyn längst upp till höger på skärmen och väljer Fakturering i listrutan.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# The [!DNL Workfront Proof] Faktureringssida

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Faktureringssidan

Så här öppnar du [!UICONTROL Billing] sida, öppna **[!UICONTROL Settings]** menyn längst upp till höger på skärmen och väljer **[!UICONTROL Billing]** i listrutan.

The [!UICONTROL Billing] sidan innehåller följande:

* Kontonamn (1)
* Kontolista (t.ex. om du har satellitkonton)(2)
* Ändra plan (3)
* Ändra betalningsinformation (4)
* Nytt satellitkonto (5)
* Stäng konto (6)
* Aktuell planinformation (7)
* Faktureringskontakt och adress (8)
* Användningsstatistik (9)
* Faktureringshistorik (10)
* Faktureringsaktivitet (11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Current Plan]

I detta avsnitt (7) visas information om din nuvarande plan, inklusive följande:

* Namnet på planen
* Aktuell betalningsmetod
* Aktuella start- och slutdatum för plan
* Nästa plantyp
* Betalningsmetod för nästa plan

   Mer information finns i [Välj betalningsmetod i [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Billing Contact and Address]

I detta avsnitt (8) visas de viktigaste faktureringskontakterna och adressinformationen för ditt konto.

Faktureringskontakten kan bara väljas bland de användare som har konfigurerats som faktureringsadministratörer för ditt konto. På satellitkonton kan endast faktureringsadministratörer från huvudkontot anges i det här fältet.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Du kan ha flera faktureringsadministratörer på ditt konto, men bara en av dem, markerad i [!UICONTROL Billing contact] kommer att få alla faktureringsmeddelanden och kontoanvändningsmeddelanden.

Detta inkluderar följande e-postmeddelanden:

* Bevis på användning
* Fakturor
* Nedgradera
* Meddelande om senarelagd betalning/tillfälligt upphörande av konto
* Kreditkortsfel

   ![Billin_CC.png](assets/billin-cc-350x103.png)

The [!UICONTROL Billing CC] kan du också lägga till en e-postadress som ska kopieras på alla faktureringsrelaterade e-postmeddelanden. Klicka på fältet för att aktivera inlineredigering och ange en e-postadress som du väljer (detta kan också vara en befintlig användares e-postadress).

## [!UICONTROL Billing Address]

I det här avsnittet används infogad redigering, så klicka bara på fälten för att ange/redigera texten.

>[!NOTE]
>
> Vi inkluderar den här adressen på dina prenumerationsfakturor, så se till att dessa data alltid är aktuella.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL Usage Statistics]

I det här avsnittet visas användningsstatistik för ditt konto under den aktuella faktureringsperioden, inklusive följande:

* Lagring används
* Använda korrektur
* Användningsgräns

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Usage Warnings]

The [[!UICONTROL Proof Permissions Profiles] in [!DNL Workfront] Korrektur](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) inställd som faktureringskontakt (1) på ditt konto meddelas via e-post när ditt konto når:

* 75 % och sedan 98 % av din lagringskapacitet
* 75 % och sedan 100 % av din korrekturgräns

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

När korrekturet eller lagringsgränsen är nådd visas även varningarna högst upp i [!UICONTROL Billing] sida:

* Gränsen för antalet korrektur har nåtts

   ![Korrektur_gräns_nådd.png](assets/proofs-limit-reached-350x65.png)

* Lagringsgränsen har nåtts

![Storage_limit_found.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Ditt korrekturantal används när korrektur skapas i ditt konto och kan inte återställas genom att ta bort korrektur.

Du kan frigöra lagringsutrymme genom att ta bort korrektur och filer och tömma [!UICONTROL Trash] efteråt.

Kom ihåg att om du behöver fler korrektur, lagring eller användare kan du uppgradera ditt konto när som helst; och det får omedelbar effekt.

## [!UICONTROL Billing History]

I det här avsnittet visas aktiviteten för de senaste faktureringsperioderna. Du kan även hämta dina fakturor från det här avsnittet.

Mer information finns i &quot; [Laddar ned [!DNL Workfront Proof] Faktura](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL Billing Activity]

I det här avsnittet visas de senaste ändringarna av faktureringsinställningarna, t.ex. prenumerationer, uppgraderingar, nedgraderingar och förnyelser av dina [!DNL Workfront Proof] Planera.

Om du ändrar din plan till en som har en lägre användargräns (1) inaktiveras användare som överskrider den nya gränsen automatiskt när den nya planen börjar. Den här aktiviteten registreras också i dina kontologgar (2).

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
