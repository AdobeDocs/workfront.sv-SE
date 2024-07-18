---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Visa mappade metadata för Experience Manager Assets eller Assets Essentials
description: Du kan se en realtidsvy över mappade metadata i panelen Dokumentinformation och Sammanfattning för dokument.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Visa mappade metadata för Experience Manager Assets eller Assets Essentials

Du kan se en realtidsvy över mappade metadata i panelen Dokumentinformation och Sammanfattning för dokument. Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets eller Assets Essentials. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.

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
   <td>Begäran eller senare
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials, och du måste läggas till som användare i Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Åtkomstnivåkonfigurationer*</strong>
   </td>
   <td>Redigera åtkomst till dokument
<p>
<strong>Obs! </strong>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <strong>Skapa eller ändra anpassade åtkomstnivåer</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Objektbehörigheter</strong>
   </td>
   <td>Visa åtkomst eller högre
<p>
Mer information om hur du begär ytterligare åtkomst finns i <strong>Begär åtkomst till objekt </strong>.
   </td>
  </tr>
</table>


*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.


## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en integrering med Experience Manager. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera Experience Manager Assets Essentials-integrering](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


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
