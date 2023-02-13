---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Redigera artikelinformation
description: När du visar en artikelruta på Kanban-tavlan kan du redigera textbunden information direkt från artikelrutan.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Redigera artikelinformation

## Förstå vilken information som kan visas och redigeras {#understand-what-information-can-be-viewed-and-edited}

När du visar en artikelruta på [!UICONTROL Kanban] finns informationen i följande tabell. Du kan redigera de flesta textbundna uppgifterna direkt från artikelrutan.

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
   <td> <p>Antalet punkter eller timmar som fyllts i artikeln och antalet punkter eller timmar som tilldelats artikeln<br>De här siffrorna används för att beräkna och visa Procent färdigt för varje artikel.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>The [!UICONTROL Percent Complete] för varje artikel och utgåva.<br>[!UICONTROL The Percent Complete] för iteration beräknas baserat på [!UICONTROL Percent Complete] för varje artikel.<br></p> <p>Vid uppdatering [!UICONTROL Percent Complete] för en artikel eller ett problem kan du välja ett valfritt nummer mellan 0 och 100.</p> </td> 
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
   <td> <p>Eventuella ytterligare fält (inklusive anpassade fält) som kan ha lagts till i den flexibla vyn genom att den flexibla vyn ändras, vilket beskrivs i"Skapa och anpassa en flexibel vy" i <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Översikt över vyer i [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa och redigera information i en artikelruta

1. Klicka på *[!UICONTROL *Main Menu]** ikon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Teams]**.

1. (Valfritt) Klicka på **[!UICONTROL Switch team]** icon ![Byt ikon för team](assets/switch-team-icon.png)väljer du sedan ett nytt Kanban-team i listrutan eller söker efter ett team i sökfältet.

1. Gå till [!UICONTROL Kanban] bräda.
1. Expandera artikelrutan om du vill visa alla fält som är kopplade till artikeln.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Valfritt) Om du vill redigera ett fält klickar du på fältet och gör sedan eventuella ändringar.\
   Du måste ha [!UICONTROL Edit] behörighet till uppgiften eller utgåvan för att redigera artikelrutan.\
   Mer information om varje fält och om det kan redigeras finns i [Förstå vilken information som kan visas och redigeras](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Ändra [!UICONTROL Percent Complete]måste du ange ett tal mellan 0 och 100. Fältet är inte ett reglage som du kan flytta.
