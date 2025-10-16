---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Redigera artikelinformation
description: När du visar en artikelruta på Kanban-tavlan kan du redigera textbunden information direkt från artikelrutan.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Redigera artikelinformation

## Förstå vilken information som kan visas och redigeras {#understand-what-information-can-be-viewed-and-edited}

När du visar en artikelruta på [!UICONTROL Kanban]-panelen är informationen i följande tabell tillgänglig. Du kan redigera de flesta textbundna uppgifterna direkt från artikelrutan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Information</strong> </th> 
   <th><strong>Synlig</strong> </th> 
   <th><strong>Redigerbar textbunden</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Artikelnamnet med en länk direkt till uppgiften eller utgåvan</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektnamnet med en länk direkt till projektet</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Antalet punkter eller timmar som fyllts i i artikeln och antalet punkter eller timmar som tilldelats artikeln<br>Dessa siffror används för att beräkna och visa Procent färdigt för varje artikel.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percent Complete] för varje artikel och utgåva.<br>[!UICONTROL The Percent Complete] för iterationen beräknas baserat på [!UICONTROL Percent Complete] för varje artikel.<br></p> <p>När du uppdaterar [!UICONTROL Percent Complete] för en artikel eller ett problem kan du välja valfritt nummer mellan 0 och 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Vem artikeln är tilldelad till</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Färgen eller kategorin för rutan</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Eventuella ytterligare fält (inklusive anpassade fält) som kan ha lagts till i den flexibla vyn genom att ändra den flexibla vyn enligt beskrivningen i"Skapa och anpassa en flexibel vy" i <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Vyöversikt i [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och redigera information i en artikelruta

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Kanban-team i listrutan eller sök efter ett team i sökfältet.

1. Gå till anslagstavlan för [!UICONTROL Kanban].
1. Expandera artikelrutan om du vill visa alla fält som är kopplade till artikeln.

   ![Artikelkort](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Valfritt) Om du vill redigera ett fält klickar du på fältet och gör sedan eventuella ändringar.
Du måste ha [!UICONTROL Edit] rättigheter till aktiviteten eller utgåvan för att kunna redigera artikelrutan.
Mer information om varje fält och om det kan redigeras finns i [Förstå vilken information som kan visas och redigeras](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Om du vill ändra [!UICONTROL Percent Complete] måste du ange ett tal mellan 0 och 100. Fältet är inte ett reglage som du kan flytta.
