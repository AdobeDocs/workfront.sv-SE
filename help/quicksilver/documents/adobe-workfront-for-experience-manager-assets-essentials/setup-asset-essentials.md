---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurera integreringen av Experience Manager Assets Essentials
description: Koppla samman ditt material med ditt i Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 9965ec9f436724e438fbbc5977f22761cc673878
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Konfigurera integreringen av Experience Manager Assets Essentials

Koppla samman materialet med innehållet i Experience Manager Assets Essentials &#x200B;:

* Skicka material och metadata från Adobe Workfront till Experience Manager Assets Essentials-&#x200B;
* Länka material från Experience Manager Assets Essentials till projekt och uppgifter i Workfront &#x200B;
* Underlätta versionshantering för resurser som skickas till Experience Manager Assets Essentials

Du kan också ansluta flera Experience Manager Assets-databaser till en Workfront-miljö eller flera Workfront-miljöer till en Experience Manager Assets-databas över olika företags-ID:n. Följ konfigurationsinstruktionerna i den här artikeln för varje integrering som du vill konfigurera.

## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>Adobe Workfront-plan*</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager licens</strong>
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Du måste ha Experience Manager Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationer på åtkomstnivå</strong>
   </td>
   <td>Du måste vara Workfront-administratör. Mer information om Workfront-administratörer finns i <strong>Bevilja användaren fullständig administrativ åtkomst</strong>.
   </td>
  </tr>
</table>


*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Konfigurera integreringen

1. Klicka på **Huvudmeny** ikonen i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar**.
1. Välj  **Dokument** ![dokument, ikon](assets/document-icon.png) i den vänstra panelen väljer **Integrering med Experience Manager**.
1. Välj **Lägg till integrering med Experience Manager**.
1. Ange följande:

   <table>
   <tr>
      <td><strong>Namn</strong>
      </td>
      <td>Ange det namn som du vill att användarna ska se på knappen Lägg till nytt i området Dokument.
      </td>
   </tr>
   <tr>
      <td><strong>Navigerings-URL</strong>
      </td>
      <td>Navigerings-URL:en fylls i automatiskt. Den här URL:en används för att länka till din organisations Assets Essentials-instans från huvudmenyn för snabb åtkomst.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets</strong>
      </td>
      <td>
      Systemet fyller automatiskt i den Experience Manager-databas som är kopplad till ditt organisations-ID.
      </td>
   </tr>
   </table>

1. Klicka **Spara** eller gå vidare till [Konfigurera metadata (valfritt)](#set-up-metadata-optional) i den här artikeln.


## Konfigurera metadata (valfritt)

Mappa Workfront-objektdata till mediefält i Experience Manager Assets. Metadata mappas när en resurs överförs från Workfront för första gången.


### Förutsättningar

Innan du börjar måste du

* Konfigurera ett metadataschema i Experience Manager Assets Essentials enligt anvisningarna i [Konfigurera metadatamappning mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Valfritt) Konfigurera anpassade formulärfält i Workfront. Workfront har många inbyggda anpassade fält som du kan använda. Du kan dock även skapa egna anpassade fält. Mer information finns i [Skapa eller redigera ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Workfront- och Experience Manager Assets-fält som stöds**

**AEM nyckelord**

Du kan mappa ett fält som stöds av Workfront till ett nyckelord i Experience Manager Assets Essentials.

Om du vill länka ett fält till ett nyckelord väljer du `dc:subject` i listrutan för Experience Manager Assets i metadatamappningsområdet.

Om du vill mappa flera enkelradiga textfält till nyckelord anger du en kommaseparerad lista över nyckelordsvärden på Workfront-sidan av metadatamappningen. `dc:subject` på Experience Manager Assets sida. Varje fältvärde kopplas till ett separat nyckelord. Du kan använda ett beräkningsfält för att kombinera flera Workfront-fält till ett enda kommaseparerat textfält.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Resurser

Metadata mappas när en resurs överförs från Workfront för första gången. Dokument med inbyggda eller anpassade fält mappas automatiskt till de angivna fälten första gången en resurs skickas till Experience Manager Assets Essentials.

1. I **Workfront** väljer du ett inbyggt eller anpassat Workfront-fält.
   >[!NOTE]
   >
   >Du kan mappa ett enstaka Workfront-fält till flera Experience Manager Assets-fält. Du kan inte mappa flera Workfront-fält till ett enda Experience Manager Assets-fält.
1. I **Experience Manager** väljer du ett Experience Manager Assets-fält.

   Om du vill mappa ett Workfront-fält till en Experience Manager Assets-tagg väljer du `dc:subject`.
1. Upprepa steg 1 och 2 efter behov.
   ![aktivera metadata](assets/metadata-assets-essentials.png)
1. Klicka **Spara** eller gå vidare till [Konfigurera länkade mappar (valfritt)](#set-up-linked-folders-optional) i den här artikeln.


## Konfigurera länkade mappar (valfritt)

{{setup-linked-folder}}
