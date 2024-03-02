---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrera från den gamla eller förbättrade anslutningen till Workfront för Adobe Experience Manager as a Cloud Service-integrering
description: Informationen på den här sidan förklarar de bästa sätten att gå från Workfront för Experience Cloud förbättrade eller äldre anslutningar till den senaste inbyggda integreringen som ansluter Workfront och Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migrera från den gamla eller förbättrade anslutningen till Workfront för Adobe Experience Manager as a Cloud Service-integrering

Informationen på den här sidan förklarar de bästa sätten att gå från Workfront för Experience Cloud förbättrade eller äldre anslutningar till den senaste inbyggda integreringen som ansluter Workfront och Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Denna information gäller inte kunder som använder Adobe Experience Manager Assets On-Premise eller Managed Services.

## Flytta din Workfront-instans till Admin Console

Kunder som tänker använda den nya inbyggda integreringen mellan Workfront och Adobe Experience Manager Assets as a Cloud Service måste se till att deras Workfront-miljö är knuten till en Adobe Admin Console. För befintliga Workfront-miljöer kommer detta sannolikt att kräva en migrering av miljön till en ansluten Adobe Admin Console. Mer information om migreringen och den associerade checklistan finns i [Förbered er på att anställa Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe måste hjälpa till att genomföra migreringen. Gör något av följande om du vill ha hjälp:

* Om du har åtkomst till Workfront Hub skickar du din begäran till [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Om du inte har Workfront Hub-åtkomst kan du skicka din begäran till [Begärandekö för tidig migrering från Workfront till Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Konfigurera din nya integrering av Workfront för Adobe Experience Manager-resurser as a Cloud Service

När Workfront-miljön har migrerats till en Adobe Admin Console kan Workfront-administratörer konfigurera den nya inbyggda integreringen. Konfigurationshjälp finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Flytta befintligt material till Workfront för Adobe Experience Manager as a Cloud Service integrering

När du har konfigurerat din miljö kan du flytta befintliga länkade resurser och mappar till Adobe Experience Manager. Detta är ett valfritt steg men säkerställer att tidigare länkade mappar och resurser via den äldre eller förbättrade kopplingen fortfarande är tillgängliga när dessa anslutningar avinstalleras.

Mer information om hur du flyttar resurser finns i [Migrera länkade mappar och dokument](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validera alla viktiga användningsfall som ska användas

Det är viktigt att validera alla kritiska användningsfall som är avsedda att användas via den inbyggda integreringen innan du avinstallerar den gamla eller förbättrade kopplingen.

## Avinstallera den gamla eller förbättrade anslutningen

Slutligen måste du avinstallera den gamla eller förbättrade anslutningen. Den inbyggda integreringen är inte avsedd att köras parallellt med någon av anslutarna.

Information om hur du avinstallerar finns i

* Avinstallationsanvisningar för äldre anslutning: [Avinstallera Workfront med Adobe Experience Manager äldre anslutning](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Avinstallationsinstruktioner för utökad anslutning: [Avinstallera Workfront med Adobe Experience Manager förbättrad anslutning](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
