---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Visa mappade metadata för Experience Manager Assets eller Assets Essentials
description: Du kan se en realtidsvy över mappade metadata i panelen Dokumentinformation och Sammanfattning för dokument.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Visa mappade metadata för Experience Manager Assets eller Assets Essentials

Du kan se en realtidsvy över mappade metadata i panelen Dokumentinformation och Sammanfattning för dokument. Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table>
  <tr>
   <td><strong>Adobe Workfront-paket</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser</strong>
   </td>
   <td>
   <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p>
   </td>
  </tr>
  <tr>
   <td><strong>Ytterligare produkter</strong>
   </td>
   <td>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Åtkomstnivåkonfigurationer</strong>
   </td>
   <td><p>Redigera åtkomst till dokument</p>
   </td>
  </tr>
  <tr>
   <td><strong>Objektbehörigheter</strong>
   </td>
   <td>Visa åtkomst eller högre
   </td>
  </tr>
</table>


Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en Experience Manager-integrering. Mer information finns i [Konfigurera integreringen med Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen med Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Dokumentinformation

Så här öppnar du panelen Metadata i Dokumentinformation:

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Håll muspekaren över det dokument du behöver och välj sedan **Dokumentinformation**.
1. Hitta och utöka avsnittet **Metadata**.

   >[!NOTE]
   >
   >Du kan inte redigera fält i det här avsnittet. De är skrivskyddade.

![dokumentinformationspanelen](assets/metadata-panel-doc-details.png)


## Sammanfattning av dokument

Så här öppnar du panelen Metadata på panelen Sammanfattning:

1. Gå till projektet, aktiviteten eller utgåvan som innehåller dokumentet och välj sedan **Dokument**.
1. Hitta det dokument du behöver.
1. Klicka på ikonen **Sammanfattning** ![Sammanfattning](assets/summary-panel-icon.png) och expandera sedan avsnittet **Metadata**.

   >[!NOTE]
   >
   >Du kan inte redigera fält i det här avsnittet. De är skrivskyddade.

![sammanfattning för dokument](assets/metadata-panel-summary.png)
