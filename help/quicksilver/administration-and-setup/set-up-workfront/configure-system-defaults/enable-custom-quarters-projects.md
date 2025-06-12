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
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Aktivera anpassade kvartal

<!--Audited: 11/2024-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön för alla kunder som har köpt [!DNL Adobe Workfront Planning]. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).

<div class="preview">

Beroende på vilka produkter ditt företag har köpt kan du konfigurera följande antal kvartal under Konfigurera för Workfront:

* Kunder som endast har köpt [!DNL Workfront] kan konfigurera upp till åtta anpassade kvartal för systemet [!DNL Adobe Workfront].
* Kunder som har köpt [!DNL Workfront] och [!DNL Workfront Planning] kan konfigurera upp till 100 kvartal för systemet [!DNL Workfront] som också är tillgängligt i [!DNL Planning].

</div>

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

   ![Anpassade kvartal](assets/custom-quarters-nwe.png)

1. (Valfritt) Klicka på **[!UICONTROL Add Custom Quarter]** om du vill lägga till ytterligare anpassade kvartal i systemet.

   >[!IMPORTANT]
   >
   > <span class="preview">Om ditt företag har köpt [!DNL Workfront Planning] kan du inte spara dina anpassade kvartal om det finns luckor eller överlappningar mellan kvartalen. </span>
   ><span class="preview">![Anpassade kvartal med överlappningsvarning](assets/custom-quarters-with-overlap-warning.png)</span>
   >Mellanrum och överlappningar mellan kvartalen tillåts bara för [!DNL Workfront] kunder.

1. (Valfritt och villkorligt) Om ditt företag bara har köpt [!DNL Workfront], utan [!DNL Workfront Planning], skapar du ett rapportelement som refererar till räkenskapskvartalen.


   **Exempel:** Skapa ett filter för en [!UICONTROL project]-lista och inkludera planerat slutförandedatum för ett projekt som refererar till anpassade kvartal.

   ![Projektfilter med anpassade kvartal](assets/example-of-project-filter-with-custom-quarters.png)

   Referenserna till &quot;Detta kvartal&quot;, &quot;Nästa kvartal&quot; och &quot;Sista kvartalet&quot; ersätts med nya referenser till de anpassade kvartalen.

   Mer information om rapportelement finns i [Rapportera element: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Mer information om hur du skapar filter finns i [Skapa eller redigera filter i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. <span class="preview"> (Valfritt och villkorligt) Om du har tillgång till [!DNL Workfront Planning] går du till en posttypssida och öppnar en tidslinjevy. I vyn visas de nya anpassade kvartalen. </span>
