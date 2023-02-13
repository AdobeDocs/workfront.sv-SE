---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Systemspårade uppdateringar
description: Adobe Workfront fångar upp aktiviteten som äger rum på vissa objekt genom att logga statusinformation i objektets [!UICONTROL Updates] område.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Systemspårade uppdateringar

[!DNL Adobe Workfront] hämtar aktiviteten för vissa objekt genom att logga statusinformation i objektets [!UICONTROL Updates] område.

The [!UICONTROL Updates] omfattar följande typer av uppdateringar:

* **Användaruppdateringar:** Anges manuellt av användare. Kallas även kommentarer, svar och anteckningar.

   ![](assets/updates-qs-350x125.png)

* **Systemuppdateringar:** Automatiskt skapat av systemet. En systemuppdatering innehåller en kort anteckning som beskriver vilken typ av ändring som har gjorts för objektet.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Följande objekt kan ha uppdateringar:

* Projekt
* Uppgift
* Problem
* Portfolio
* Program
* Användare
* Mallar
* Malluppgifter
* Dokument
* Tidrapporter

Dina [!DNL Workfront] licenser avgör om systemuppdateringar visas som standard i [!UICONTROL Updates] objektområde. [!DNL Workfront] användare med [!UICONTROL Plan] licensen innehåller systemuppdateringar som visas i [!UICONTROL Updates] som standard. Användarna kan dock filtrera bort systemuppdateringar enligt beskrivningen i [[!UICONTROL Enable] eller inaktivera systemuppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) avsnitt i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Alla andra [!DNL Workfront] Filtersystemuppdateringar för licenser som standard.

[!DNL Workfront] administratörer kan definiera vilken typ av ändringar som systemet ska spåra i [!UICONTROL Updates] område. Alla objekt har inte konfigurerats [!UICONTROL update] statusflöden. Följande objekt har en [!UICONTROL Updates] Område som hämtar systemspårade uppdateringsfeeds, men som inte har konfigurerbara statusflöden för uppdateringar:

* Mallar
* Malluppgifter
* Dokument
* Tidrapporter

Mer information om systemuppdateringsflöden och hur du aktiverar dem finns i [Konfigurera systemuppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Mer information om hur du konfigurerar användaruppdateringar finns i [Konfigurera inställningar för användaruppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
