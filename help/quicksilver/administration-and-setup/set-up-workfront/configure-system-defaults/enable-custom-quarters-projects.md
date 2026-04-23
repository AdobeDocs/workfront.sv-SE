---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivera anpassade kvartal
description: I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Aktivera anpassade kvartal

<!--Audited: 03/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).

Beroende på vilka produkter ditt företag har köpt kan du konfigurera följande antal kvartal under Konfigurera för Workfront:

* Kunder som endast har köpt [!DNL Workfront] kan konfigurera upp till åtta anpassade kvartal för sitt [!DNL Adobe Workfront]-system.
* Kunder som har köpt [!DNL Workfront] och [!DNL Workfront Planning] kan konfigurera upp till 100 kvartal för sitt [!DNL Workfront]-system, som också är tillgängligt i [!DNL Planning].

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera anpassade kvartal för ditt [!DNL Workfront]-system

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Custom Quarters]**.

1. Välj **[!UICONTROL Enable Custom Quarters]**.

1. Ange ett namn för det anpassade kvartalet, till exempel&quot;Räkenskapskvot 1 2021&quot;.
1. Välj start- och slutdatum för det anpassade kvartalet.

   ![Anpassade kvartal](assets/custom-quarters-nwe.png)

1. (Valfritt) Klicka på **[!UICONTROL Add Custom Quarter]** om du vill lägga till ytterligare anpassade kvartal i systemet.

   >[!IMPORTANT]
   >
   > Om ditt företag har köpt [!DNL Workfront Planning] kan du inte spara dina anpassade kvartal om det finns luckor eller överlappningar mellan kvartalen.
   >![Anpassade kvartal med överlappningsvarning](assets/custom-quarters-with-overlap-warning.png)
   >Mellanrum och överlappningar mellan kvartalen tillåts bara för [!DNL Workfront] kunder.

1. (Valfritt och villkorligt) Om ditt företag bara har köpt [!DNL Workfront], utan [!DNL Workfront Planning], skapar du ett rapportelement som refererar till räkenskapskvartalen.

   **Exempel:** Skapa ett filter för en [!UICONTROL project]-lista och inkludera planerat slutförandedatum för ett projekt som refererar till anpassade kvartal.

   ![Projektfilter med anpassade kvartal](assets/example-of-project-filter-with-custom-quarters.png)

   Referenserna till &quot;Detta kvartal&quot;, &quot;Nästa kvartal&quot; och &quot;Sista kvartalet&quot; ersätts med nya referenser till de anpassade kvartalen.

   Mer information om rapportelement finns i [Rapportera element: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Mer information om hur du skapar filter finns i [Skapa eller redigera filter i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Valfritt och villkorligt) Om ditt företag har köpt Workfront Planning och du har tillgång till [!DNL Workfront Planning] går du till en posttypssida och öppnar en tidslinjevy. I vyn visas de nya anpassade kvartalen.
Mer information finns i [Hantera tidslinjevyn](/help/quicksilver/planning/views/manage-the-timeline-view.md).
