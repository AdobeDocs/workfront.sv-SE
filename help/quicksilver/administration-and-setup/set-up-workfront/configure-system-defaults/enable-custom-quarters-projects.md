---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivera anpassade kvartal för projekt
description: I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Aktivera anpassade kvartal för projekt

I rapporteringssyfte kan du skapa anpassade kvartal om organisationens kvartal baseras på andra specifika villkor än kalenderdatum (t.ex. arbetsdagar eller kunddagar).

Du kan konfigurera upp till åtta anpassade kvartal för [!DNL Adobe Workfront] system.

## Åtkomstkrav

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ställ in anpassade kvartal för din [!DNL Workfront] system

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. I **[!UICONTROL Timelines]** avsnitt, markera **[!UICONTROL Enable Custom Quarters]**.

1. Ange ett namn för det anpassade kvartalet, till exempel&quot;Räkenskapskvot 1 2021&quot;.
1. Välj start- och slutdatum för det anpassade kvartalet.

   ![](assets/custom-quarters-nwe.png)

1. (Valfritt) Klicka på **[!UICONTROL Add Custom Quarter]** om du vill lägga till ytterligare anpassade kvartal i systemet.
1. (Valfritt) Skapa ett rapportelement som refererar till räkenskapskvartalen.

   **Exempel:** Skapa ett filter för en [!UICONTROL project] och inkludera det planerade slutförandedatumet för ett projekt som refererar till de anpassade kvartalen.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Referenserna till &quot;Detta kvartal&quot;, &quot;Nästa kvartal&quot; och &quot;Sista kvartalet&quot; ersätts med nya referenser till de anpassade kvartalen.

   Mer information om rapportelement finns i [Rapportelement: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Mer information om hur du skapar filter finns i [Skapa eller redigera filter i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
