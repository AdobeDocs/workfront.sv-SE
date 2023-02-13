---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Visa och redigera artikelinformation på Scrum board
description: När du visar en artikelruta på Kanban-tavlan kan du redigera textbunden information direkt från artikelrutan.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Visa och redigera artikelinformation på [!UICONTROL Scrum] board

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
   <td> <p>Projektnamnet med en länk direkt till projektet<br>Den här länken visas endast i artiklar (överordnade uppgifter, inte underuppgifter) när den flexibla vyn används på en iteration. den inte visas när du använder en flexibel vy i ett projekt.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Antalet punkter eller timmar som fyllts i artikeln och antalet punkter eller timmar som tilldelats artikeln<br>Dessa tal används för att beräkna och visa [!UICONTROL Percent Complete] för varje artikel.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>The [!UICONTROL Percent Complete] för varje artikel och utgåva.<br>The [!UICONTROL Percent Complete] för iteration beräknas baserat på [!UICONTROL Percent Complete] för varje artikel.</p> <p>Vid uppdatering [!UICONTROL Percent Complete] för en artikel eller ett problem kan du välja ett valfritt nummer mellan 0 och 100.</p> </td> 
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
   <td> <p>Eventuella ytterligare fält (inklusive anpassade fält) som kan ha lagts till i den flexibla vyn genom att ändra den flexibla vyn enligt beskrivningen i"Skapa och anpassa en [!UICONTROL Agile] Visa" i <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Översikt över vyer i [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Redigera åtkomst till uppgiften eller problemet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa och redigera information i en artikelruta

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Scrum-team i listrutan eller söker efter ett team i sökfältet.

1. Välj **[!UICONTROL Iterations]** om du vill välja en viss upprepning, eller markera **[!UICONTROL Current Iteration]**.

1. Gå till [!UICONTROL Scrum] flexibel artikelpanel.
1. Expandera [!UICONTROL story] om du vill visa alla fält som är kopplade till artikeln.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Valfritt) Om du vill redigera ett fält klickar du på fältet och gör sedan eventuella ändringar.

   Du måste ha [!UICONTROL Edit] behörighet till uppgiften eller utgåvan för att redigera artikelrutan.

>[!NOTE]
>
>Ändra [!UICONTROL Percent Complete]måste du ange ett tal mellan 0 och 100. Fältet är inte ett reglage som du kan flytta.
