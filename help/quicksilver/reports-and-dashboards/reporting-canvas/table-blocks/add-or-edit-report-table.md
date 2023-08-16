---
title: Lägga till eller redigera ett tabellblock i rapportarbetsytan
description: Lägga till eller redigera ett tabellblock i rapportarbetsytan
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: d706659c-457f-4da0-a6e7-03ea29cab700
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Lägga till eller redigera ett tabellblock i rapportarbetsytan

En tabell visar fältinformation i kolumner som kan filtreras, grupperas och sorteras.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Lägga till eller redigera ett tabellblock

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Rapportering**.
1. Klicka **Ny rapport**.

   eller

   Klicka på **Mer** icon ![](assets/more-icon-27x15.png) i rapportrubriken och klicka sedan på **Redigera**.

1. Till höger på skärmen under **Lägga till ett block**, antingen:

   Dra **Tabell** icon ![](assets/table-icon.png) till arbetsytan direkt till önskad plats.

   eller

   Dubbelklicka på **Tabell** icon ![](assets/table-icon.png) om du vill lägga till en tabell högst upp på arbetsytan.

   >[!TIP]
   >
   >Du kan ändra storleken på blocket efter att det har placerats genom att dra i hörnhandtagen.

1. Klicka **Namnlöst register** i tabellhuvudet och skriv en rubrik för tabellen.

   ![](assets/table-name-350x142.png)

1. Klicka **Redigera** mitt i tabellblocket för att konfigurera tabellen.

   >[!NOTE]
   >
   >Om tabellen redan var en del av arbetsytan (till exempel när du redigerar en befintlig rapport) visas **Redigera** knappen visas inte i mitten av blocket. Om du vill redigera tabellen klickar du på **Redigera** icon ![](assets/edit-icon.png) i tabellrubriken i stället.
   >![](assets/edit-icon-table-header-350x71.png)

1. I **Fält** till höger, leta upp ett fält som du vill lägga till som en kolumn i tabellen och dra det sedan till den plats i tabellen där du vill ha det, eller dubbelklicka på det för att lägga till det som den sista kolumnen i tabellen.

   Du kan skriva text i **Sök** för att hitta ett specifikt fält efter namn. Du kan också använda de två listrutemenyerna under den här rutan för att begränsa listan med visade fält till ett eller båda av följande:

   * Objekttypen som är associerad med fältet som du vill använda, till exempel Projekt eller Aktivitet
   * Den fälttyp du vill använda, till exempel Datum eller Valuta

   Upprepa det här steget för varje fält som du vill lägga till som en kolumn.

   >[!TIP]
   >
   >Du kan ändra kolumnordningen i en tabell genom att dra en markerad kolumn till en ny plats.

1. Gör något av följande för att konfigurera tabellen ytterligare:

   * **Lägg till ett formelfält**: Klicka **Nytt +** högst upp på **Fält** lista. Mer information om hur du skapar ett formelfält finns i [Skapa ett formelfält i Rapporteringsarbetsyta](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **Lägga till ett filter**: Dra fältet som du vill att tabellen ska filtreras efter till **Filter** ovanför tabellen. Mer information om hur du ställer in filterregler finns i [Filtrera en tabell i rapportarbetsytan](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **Gruppera rader efter specifika attribut**: Dra fältet som du vill att tabellen ska grupperas i till **Grupp** ovanför tabellen. Mer information om hur du skapar radgrupper finns i [Gruppera tabellrader i rapportarbetsytan](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).
