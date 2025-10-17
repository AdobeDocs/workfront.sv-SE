---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Visa och redigera artikelinformation på anslagstavlan
description: När du visar en artikelruta på Kanban-tavlan kan du redigera textbunden information direkt från artikelrutan.
author: Jenny
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Visa och redigera artikelinformation på [!UICONTROL Scrum]-tavlan

## Förstå vilken information som kan visas och redigeras

När du visar en artikelruta på artikelpanelen är informationen i följande tabell tillgänglig. Du kan redigera de flesta textbundna uppgifterna direkt från artikelrutan.

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
   <td> <p>Projektnamnet med en länk direkt till projektet<br>Den här länken visas bara på artiklar (överordnade aktiviteter, inte underaktiviteter) när den flexibla vyn används i en iteration. Den visas inte när du använder en flexibel vy i ett projekt.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Antalet punkter eller timmar som är fullständiga i artikeln och antalet punkter eller timmar som tilldelats artikeln<br>Dessa siffror används för att beräkna och visa [!UICONTROL Percent Complete] för varje artikel.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percent Complete] för varje artikel och utgåva.<br>Värdet [!UICONTROL Percent Complete] för iterationen beräknas baserat på [!UICONTROL Percent Complete] för varje artikel.</p> <p>När du uppdaterar [!UICONTROL Percent Complete] för en artikel eller ett problem kan du välja valfritt nummer mellan 0 och 100.</p> </td> 
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
   <td> <p>Eventuella ytterligare fält (inklusive anpassade fält) som kan ha lagts till i den flexibla vyn genom att ändra den flexibla vyn, enligt beskrivningen i"Skapa och anpassa en [!UICONTROL Agile]-vy" i <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Vyöversikt i [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p> 
   eller
   <p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>[!UICONTROL Contribute] eller [!UICONTROL Manage] åtkomst till uppgiften eller problemet</td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och redigera information i en artikelruta

{{step1-to-team}}

1. (Valfritt) Klicka på ikonen **[!UICONTROL Switch team]** ![Byt team-ikon](assets/switch-team-icon.png) och välj sedan ett nytt Scrum-team i listrutan eller sök efter ett team i sökfältet.

1. I den vänstra panelen väljer du **[!UICONTROL Iterations]** om du vill välja en viss iteration eller **[!UICONTROL Current Iteration]**.

1. Gå till den flexibla artikelpanelen för [!UICONTROL Scrum].
1. Expandera rutan [!UICONTROL story] om du vill visa alla fält som är associerade med artikeln.

   ![artikelkort](assets/agile-storycard-scrum-2021-350x333.png)

1. (Valfritt) Om du vill redigera ett fält klickar du på fältet och gör sedan eventuella ändringar.

   Du måste ha [!UICONTROL Edit] rättigheter till aktiviteten eller utgåvan för att kunna redigera artikelrutan.

>[!NOTE]
>
>Om du vill ändra [!UICONTROL Percent Complete] måste du ange ett tal mellan 0 och 100. Fältet är inte ett reglage som du kan flytta.
