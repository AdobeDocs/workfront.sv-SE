---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrera från den gamla anslutningen till den förbättrade anslutningen
description: Följande process beskriver de bästa sätten att byta från Adobe Experience Manager äldre anslutning till den förbättrade anslutningen för integrering av Adobe Workfront med AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migrera från den gamla anslutningen till den förbättrade anslutningen

Följande process beskriver de bästa sätten att byta från Adobe Experience Manager äldre anslutning till den förbättrade anslutningen för integrering av Adobe Workfront med AEM Assets.

>[!IMPORTANT]
>
>Denna dokumentation gäller endast kunder som använder Adobe Experience Manager Assets On-Premise eller Managed Services.


För kunder som har Adobe Experience Manager Assets as a Cloud Service är migreringsvägen från den äldre kopplingen till den nya inbyggda integreringen i Workfront. Mer information om migreringsprocessen finns i [Migrera från den gamla eller förbättrade anslutningen till Workfront för Adobe Experience Manager as a Cloud Service-integrering](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementera den utökade kopplingen

>[!IMPORTANT]
>
>En certifierad partner eller Adobe konsulttjänster krävs för att implementera den förbättrade anslutningen.
>
> Partners som vill certifiera sig på den förbättrade anslutningen kan läsa följande artikel: [Workfront for Experience Manager förbättrad Connector Expert Series](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Information om hur du implementerar den förbättrade anslutningen finns i [Konfigurera Workfront för Experience Manager förbättrad anslutning](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Flytta befintliga resurser

När du har konfigurerat din miljö kan du flytta befintliga länkade resurser och mappar till Adobe Experience Manager. Detta är ett valfritt steg, men säkerställer att tidigare länkade mappar och resurser via den äldre kopplingen fortfarande är tillgängliga när den äldre anslutningen har avinstallerats.

Mer information om hur du flyttar resurser finns i [Migrera länkade mappar och dokument](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validera alla viktiga användningsfall som ska användas

Det är viktigt att validera alla kritiska användningsfall som är avsedda att användas via den förbättrade anslutningen innan den äldre anslutningen avinstalleras.

## Avinstallera den gamla kopplingen

Slutligen måste du avinstallera den äldre anslutningen. Den gamla kopplingen är inte avsedd att köras parallellt med den förbättrade anslutningen.

Information om hur du avinstallerar finns i [Avinstallera Workfront med Adobe Experience Manager äldre anslutning](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
