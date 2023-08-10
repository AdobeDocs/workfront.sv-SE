---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Systemspårade uppdateringar
description: Adobe Workfront fångar upp aktiviteten som äger rum på vissa objekt genom att logga statusinformation i objektets [!UICONTROL Updates] område.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 207a8c8a642f3204a2d007789eb7ee8cd9379f1b
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Systemspårade uppdateringar

[!DNL Adobe Workfront] hämtar aktiviteten för vissa objekt genom att logga statusinformation i objektets [!UICONTROL Updates] område.

The [!UICONTROL Updates] omfattar följande typer av uppdateringar:

* **Användaruppdateringar:** Anges manuellt av användare. Kallas även kommentarer, svar och anteckningar.

  Mer information om hur du konfigurerar användaruppdateringar finns i [Konfigurera inställningar för användaruppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systemuppdateringar:** Automatiskt skapat av systemet. En systemuppdatering innehåller en kort anteckning som beskriver vilken typ av ändring som har gjorts för objektet.

  Mer information om systemuppdateringsflöden och hur du aktiverar dem finns i [Konfigurera systemuppdateringar](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Överväganden om systemspårade uppdateringar

* Systemspårade uppdateringar är inte tillgängliga för alla objekt som har uppdateringsområdet. The [!UICONTROL Updates] -området är tillgängligt för följande objekt:

   * [!UICONTROL Project]
   * [!UICONTROL Task]
   * [!UICONTROL Issue]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Program]
   * [!UICONTROL User]
   * [!UICONTROL Template]
   * [!UICONTROL Template Task]
   * [!UICONTROL Team]
   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Story]

     I [!DNL Workfront], en artikel är en uppgift.
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]

     Du måste ha ytterligare en licens för att ha tillgång till [!UICONTROL Goals] område. Mer information finns i [Krav för att använda Workfront-mål](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Card] ombord

     Mer information om uppdateringar av kort finns i [Använd anslutna kort på ritytor](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] spårar inte några systemuppdateringar för följande objekt:

   * [!UICONTROL Team]
   * [!UICONTROL Template]
   * [!UICONTROL Template Task]
   * Ad hoc [!UICONTROL Card]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Användare kan visa systemuppdateringar som standard eller välja att inte visa dem.

  Mer information om hur du inaktiverar visning av systemuppdateringar finns i avsnittet [Aktivera eller inaktivera systemuppdateringar](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) i artikeln [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >Vi håller just nu på att omarbeta kommentarupplevelsen och [!UICONTROL Updates] område i [!DNL Workfront].
  >
  > Du kan inte dölja systemuppdateringar när du använder den nya kommentarsfunktionen.
  > 
  >Mer information om de nya kommentarfunktionerna finns i [Ny kommentarsfunktion](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Workfront registrerar systemspårade uppdateringar för följande objekt, men det finns inget alternativ för att inaktivera visning av dem:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Program]
   * [!UICONTROL Iteration]

* [!DNL Workfront] administratörer kan definiera vilken typ av ändringar som systemet ska spåra i [!UICONTROL Updates] område. Inte alla objekt som har [!UICONTROL Updates] området har också konfigurerats [!UICONTROL update] feeds. Följande objekt har en [!UICONTROL Updates] Område som hämtar systemspårade uppdateringsfeeds, men som inte har konfigurerbara uppdateringsflöden:

   * [!UICONTROL Document]
   * [!UICONTROL Timesheet]
   * [!UICONTROL Iteration]
   * [!UICONTROL Goal]


