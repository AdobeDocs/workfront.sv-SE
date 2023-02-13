---
navigation-topic: use-lists
title: Exportera en lista
description: Du kan exportera en lista med objekt från Adobe Workfront. När objektlistan i Workfront innehåller fler än 2 000 objekt är det enda sättet att granska alla objekt i listan på en sida att exportera listan.
feature: Get Started with Workfront
author: Lisa
exl-id: 31159d6d-f03a-4f84-a454-25a232971441
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Exportera en lista

Du kan exportera en lista med objekt från [!DNL Adobe Workfront]. När listan med objekt i [!DNL Workfront] innehåller fler än 2 000 objekt. Det enda sättet att granska alla objekt i listan på en sida är att exportera listan.

Mer information om exportformat och -begränsningar finns i [Exportera data](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

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
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] behörighet till området som listan finns i</p> <p>Om du till exempel vill exportera ett projekts uppgiftslista måste du [!UICONTROL View] behörighet till projekt.</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå.<br>För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View]</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Exportera en lista

1. Gå till en lista med objekt.
1. (Valfritt) Markera de filter, vyer och grupperingar som du vill använda i listan innan du exporterar.\
   Mer information om filter, vyer och grupperingar finns i [Rapportelement: filter, vyer och grupperingar](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

1. (Valfritt) Om du bara vill exportera vissa objekt i en lista markerar du alla objekt i listan som du vill ha med i den exporterade filen.

   >[!TIP]
   >
   >Om du vill söka efter alla objekt som du vill ta med kan du:
   >
   >   
   >   
   >   * **Markera för att visa alla eller 2 000 objekt i listorna**: Mer information finns i [Ändra hur en lista visas](../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md).
   >   
   >   * **Använd snabbfiltret**: Mer information finns i [Använda snabbfiltret på en lista](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).\
      >     Snabbfiltret gäller bara för den aktuella sidan i listan.



   ![select_all_projects_with_highlight_1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

1. Klicka **[!UICONTROL Export]** ![Exportera](assets/export.png).

1. Välj bland följande format:

   * PDF
   * [!DNL Excel]
   * [!DNL Excel] (xlsx)
   * Tabbavgränsad

      En kopia av listan exporteras till något av dessa format och sparas på datorn.

1. (Valfritt) Öppna den exporterade listan med lämpligt program.\
   Alla objekt i listan visas i den exporterade filen, oavsett om de visas på skärmen i webbprogrammet eller inte.
