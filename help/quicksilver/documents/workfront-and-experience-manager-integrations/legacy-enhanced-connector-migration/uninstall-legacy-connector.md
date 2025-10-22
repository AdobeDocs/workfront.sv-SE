---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Avinstallera den gamla kopplingen
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Avinstallera Workfront med Adobe Experience Manager äldre anslutning

Du måste avinstallera Workfront med Adobe Experience Manager äldre anslutning till den senaste inbyggda integreringen som ansluter Workfront och Adobe Experience Manager Assets as a Cloud Service.

## Avbeställ Workfront

1. Öppna Adobe Experience Manager.
1. Gå till **Verktyg** > **Molntjänster** > **Workfront integreringskonfiguration** i Experience Manager.
1. Välj din konfiguration (global-workfront som standard) och klicka på **Egenskaper**.

   ![avsluta prenumeration från arbetsytan](assets/unsubscribe-from-workfront.png)

1. Inaktivera synk av dokument, kommentarer och metadata. Etiketten ska vara dag inaktiverad.
Detta tar bort prenumerationerna i Workfront och gör att användaren kan skapa en ny prenumeration med samma URL som definieras i Day CQ Link Externalizer.

## Ta bort integreringskonfigurationen för Workfront

När du har tagit bort prenumerationen är det nu säkert att ta bort integreringskonfigurationen för Workfront.

1. Öppna konfigurationen och välj **Ta bort**.

   ![ta bort konfiguration](assets/delete-wf-configuration.png)

## Ta bort mappning

Därefter måste du ta bort Workfront Property Mapping.

1. Gå till **Verktyg** > **Assets** > **Workfront-egenskapsmappning** i Experience Manager.

1. Markera alla mappningar och klicka på **Ta bort**.

## Användarbehörigheter

Alla användare som använder AEM Dam från Workfront fick läsbehörighet till `/content/dam`. Om en användare inte längre behöver det kan du ta bort de behörigheter som tilldelats dessa användare.

Kopplingen fungerar med systemets Workfront-tjänst för användare. Detta avinstalleras när anslutningen avinstalleras.

>[!NOTE]
>
>Om du använder Connecter version 2.0.3 och lade till gruppen `workfront-aem-connector-group`, måste även detta tas bort genom att gå till **Verktyg** > **Dokumentskydd** > **Grupper**.

## Day CQ Link Externalizer

Om du inte behöver Dag CQ Link Externalizer kan du återställa den till `localhost:4502` genom att gå till `/system/console/configMgr` och leta efter Dag CQ Link Externalizer.

>[!NOTE]
>
>Om du använder Adobe Experience Manager as a Cloud Service kan du ändra detta genom att undersöka ditt projekt och hitta filen _com.day.cq.commons.impl.ExternalizerImpl.xml_ inuti _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Dagens CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## Avinstallera anslutningsprogram

Vilka steg som krävs för att avinstallera anslutningspaketet varierar beroende på vilken Adobe Experience Manager-version du har.

### Adobe Experience Manager lokal

Om du använder Adobe Experience Manager lokalt går du till _crx/packmgr/index.jsp_ och letar efter `workfront-aem-connector.all-<version>.zip`, klickar på **Mer** och sedan på **Avinstallera**.

Kontrollera under `/conf` för att se till att alla filer som skapats av Workfront har tagits bort.

### Adobe Experience Manager as a Cloud Service

För Adobe Experience Manager as a Cloud Service kan du ta bort beroenden för kopplingen från projektets pom.files.

## Brandvägg och Dispatcher

Glöm inte att ta bort dina vitlistade Workfront-URL:er om kommunikation inte längre behövs. Dessutom använder kopplingen sidhuvudena apiKey och användarnamn som angetts för dispatchern. Dessa kan också tas bort.
