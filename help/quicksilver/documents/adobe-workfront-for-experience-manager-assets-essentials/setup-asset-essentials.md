---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurera integreringen av Experience Manager Assets Essentials
description: Koppla samman materialet med innehållet i Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Konfigurera integreringen av Experience Manager Assets Essentials

Koppla samman materialet med innehållet i Experience Manager Assets Essentials &#x200B;:

* Överför material och metadata från Adobe Workfront till Experience Manager Assets Essentials-&#x200B;
* Länka material från Experience Manager Assets Essentials till projekt och uppgifter i Workfront &#x200B;
* Underlätta versionshantering för resurser som skickas till Experience Manager Assets Essentials

>[!NOTE]
>
>Du kan också ansluta flera Experience Manager Assets-databaser till en Workfront-miljö eller flera Workfront-miljöer till en Experience Manager Assets-databas över olika företags-ID:n. Följ konfigurationsinstruktionerna i den här artikeln för varje integrering som du vill konfigurera.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licens
   </td>
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>Nytt: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] licens
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Produkt
   </td>
   <td>Du måste ha Experience Manager Assets Essentials och du måste läggas till som användare i Admin Console.
   </td>
  </tr>
  <tr>
   <td>Konfigurationer på åtkomstnivå
   </td>
   <td>Du måste vara en [!DNL Workfront]-administratör.
   </td>
  </tr>
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera integreringen

{{step-1-to-setup}}

1. Välj ikonen **Dokument** ![dokument](assets/document-icon.png) i den vänstra panelen och välj sedan **Experience Manager-integrering**.
1. Välj **Lägg till Experience Manager-integrering**.
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
      <td>Navigerings-URL:en fylls i automatiskt. Den här URL:en används för att länka till instansen Resurser Essentials från huvudmenyn för snabb åtkomst.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets-databas</strong>
      </td>
      <td>
      Systemet fyller automatiskt i den Experience Manager-databas som är kopplad till ditt företags-ID.
      </td>
   </tr>
   </table>

1. Klicka på **Spara** eller gå vidare till avsnittet [Konfigurera metadata (valfritt)](#set-up-metadata-optional) i den här artikeln.


## Konfigurera metadata (valfritt)

Mappa Workfront-objektdata till mediefält i Experience Manager Assets. Metadata mappas när en resurs överförs från Workfront för första gången.


### Förutsättningar

Innan du börjar måste du

* Konfigurera ett metadataschema i Experience Manager Assets Essentials enligt beskrivningen i [Konfigurera mappning av metadata för resurser mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
* (Valfritt) Konfigurera anpassade formulärfält i Workfront. Workfront har många anpassade fält som du kan använda. Du kan dock även skapa egna anpassade fält. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Workfront- och Experience Manager Assets-fält som stöds

### AEM-nyckelord

Du kan mappa ett fält som stöds av Workfront till ett nyckelord i Experience Manager Assets Essentials.

Om du vill länka ett fält till ett nyckelord väljer du `xcm:keywords` i listrutan Experience Manager Assets i metadatamappningsområdet.

Om du vill mappa flera enkelradiga textfält till nyckelord anger du en kommaseparerad lista över nyckelordsvärden i Workfront-sidan av metadatamappningen och `xcm:keywords` på Experience Manager Assets-sidan. Varje fältvärde kopplas till ett separat nyckelord. Du kan använda ett beräkningsfält för att kombinera flera Workfront-fält till ett enda kommaseparerat textfält.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Assets

Metadata mappas när en resurs överförs från Workfront för första gången. Dokument med inbyggda eller anpassade fält mappas automatiskt till de angivna fälten första gången en resurs skickas till Experience Manager Assets Essentials.

1. I kolumnen **Workfront fält** väljer du ett inbyggt eller anpassat Workfront-fält.

   >[!NOTE]
   >
   >Du kan mappa ett enstaka Workfront-fält till flera Experience Manager Assets-fält. Du kan inte mappa flera Workfront-fält till ett enda Experience Manager Assets-fält.

1. I fältet **Experience Manager** väljer du ett Experience Manager Assets-fält.

   Om du vill mappa ett Workfront-fält till en Experience Manager Assets-tagg väljer du `xcm:keywords`.

1. Upprepa steg 1 och 2 efter behov.
   ![aktivera metadata](assets/metadata-assets-essentials.png)
1. Klicka på **Spara** eller gå vidare till avsnittet [Konfigurera länkade mappar (valfritt)](#set-up-linked-folders-optional) i den här artikeln.


## Konfigurera länkade mappar (valfritt)

{{setup-linked-folder}}
