---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Avinstallera den gamla kopplingen
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Avinstallera Workfront med Adobe Experience Manager äldre anslutning

Du måste avinstallera Workfront med Adobe Experience Manager äldre anslutning till den senaste inbyggda integreringen som kopplar Workfront och Adobe Experience Manager Assets as a Cloud Service.

## Avbeställ Workfront

1. Öppna Adobe Experience Manager.
1. I Experience Manager, gå till **verktyg** > **Cloud Services** > **Konfiguration av Workfront-integrering**.
1. Välj din konfiguration (global-workfront som standard) och klicka på **Egenskaper**.
   ![avbeställa tjänsten](assets/unsubscribe-from-workfront.png)
1. Inaktivera synk av dokument, kommentarer och metadata. Etiketten ska vara dag inaktiverad.
Detta tar bort prenumerationerna i Workfront och gör att användaren kan skapa en ny prenumeration med samma URL som definieras i Day CQ Link Externalizer.

## Ta bort integreringskonfigurationen för Workfront

När du har tagit bort prenumerationen är det nu säkert att ta bort integreringskonfigurationen för Workfront.

1. Öppna konfigurationen och välj **Ta bort**.
   ![ta bort konfiguration](assets/delete-wf-configuration.png)

## Ta bort mappning

Därefter måste du ta bort Workfront Property Mapping.

1. I Experience Manager, gå till **verktyg** > **Resurser** > **Workfront Property Mapping**.

1. Markera alla mappningar och klicka på **Ta bort**.

## Användarbehörigheter

Alla användare som har åtkomst AEM Dam från Workfront fick läsbehörighet till `/content/dam`. Om en användare inte längre behöver det kan du ta bort de behörigheter som tilldelats dessa användare.

Kopplingen fungerar med systemets Workfront-tjänst för användare. Detta avinstalleras när anslutningen avinstalleras.

>[!NOTE]
>
>Om du använder Connecter version 2.0.3 och lade till gruppen `workfront-aem-connector-group`måste den också tas bort genom att **verktyg** > **Säkerhet** > **Grupper**.

## Day CQ Link Externalizer

Om du inte behöver Dag CQ Link Externalizer kan du återställa den till `localhost:4502` genom att gå till `/system/console/configMgr` och söker efter &#39;Day CQ Link Externalizer&#39;.

>[!NOTE]
>
>Om du använder Adobe Experience Manager as a Cloud Service kan du ändra detta genom att undersöka ditt projekt och hitta filen _com.day.cq.commons.impl.ExternalizerImpl.xml_ inuti _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## Avinstallera Connector-paket

Vilka steg som krävs för att avinstallera anslutningsprogrammet varierar beroende på vilken Adobe Experience Manager-version du har.

### Adobe Experience Manager On-Premise

Om du använder Adobe Experience Manager lokalt går du till _crx/packmgr/index.jsp_ och leta efter `workfront-aem-connector.all-<version>.zip`, klicka **Mer** och sedan **Avinstallera**.

Gå till `/conf` för att säkerställa att alla filer som skapats i Workfront har tagits bort.

### Adobe Experience Manager as a Cloud Service

För Adobe Experience Manager as a Cloud Service kan du ta bort beroenden för kopplingen från projektets pom.files.

## Brandvägg och Dispatcher

Glöm inte att ta bort dina vitlistade Workfront-URL:er om kommunikation inte längre behövs. Dessutom använder kopplingen sidhuvudena apiKey och användarnamn som angetts för dispatchern. Dessa kan också tas bort.
