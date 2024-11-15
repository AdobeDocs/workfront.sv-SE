---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivera anpassade kvartal för projekt
description: I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Aktivera anpassade kvartal för projekt

<!--Audited: 11/2024-->

I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).

Du kan konfigurera upp till åtta anpassade kvartal för ditt [!DNL Adobe Workfront]-system.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
   eller
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera anpassade kvartal för ditt [!DNL Workfront]-system

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. Välj **[!UICONTROL Enable Custom Quarters]** i avsnittet **[!UICONTROL Timelines]**.

1. Ange ett namn för det anpassade kvartalet, till exempel&quot;Räkenskapskvot 1 2021&quot;.
1. Välj start- och slutdatum för det anpassade kvartalet.

   ![](assets/custom-quarters-nwe.png)

1. (Valfritt) Klicka på **[!UICONTROL Add Custom Quarter]** om du vill lägga till ytterligare anpassade kvartal i systemet.
1. (Valfritt) Skapa ett rapportelement som refererar till räkenskapskvartalen.

   **Exempel:** Skapa ett filter för en [!UICONTROL project]-lista och inkludera planerat slutförandedatum för ett projekt som refererar till anpassade kvartal.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Referenserna till &quot;Detta kvartal&quot;, &quot;Nästa kvartal&quot; och &quot;Sista kvartalet&quot; ersätts med nya referenser till de anpassade kvartalen.

   Mer information om rapportelement finns i [Rapportera element: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Mer information om hur du skapar filter finns i [Skapa eller redigera filter i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
