---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Hantera arbetsflöden
description: Ett arbetsflöde är en konfigurerbar grupp av brädor och kort för samarbete i arbetet.
author: Lisa
feature: Agile
source-git-commit: 96819e5d81a063ad623350a0a75428629d6f7b6d
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Hantera arbetsflöden

{{highlighted-preview}}

>[!NOTE]
>
>Det finns arbetsflöden i förhandsvisningsmiljön och i produktionen via tidiga funktioner för [!UICONTROL [!DNL Workfront] Boards]. Mer information finns i [Tidig registrering av nya funktioner för Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

Ett arbetsflöde är en konfigurerbar grupp av brädor och kort för samarbete i arbetet. Arbetsströmmar kan innehålla olika typer av anslagstavlor från mallar, <span class="preview">och en kortlista med arbetsuppgifter. I ett arbetsflöde kan du spåra arbete i iterationer eller utskrifter.</span>

<span class="preview">Mer information finns i [Använda kortlistan](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) och [Skapa en iteration i ett arbetsflöde](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).</span>

Arbetsströmmar visas på kontrollpanelen tillsammans med enskilda paneler som du har åtkomst till som inte är en del av ett arbetsflöde. Mer information om panelernas kontrollpanel finns i [Använda panelkontrollpanelen](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Du kan öppna en panel genom att klicka på dess namn.

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
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

## Skapa ett arbetsflöde

{{step1-to-boards}}

1. Klicka **[!UICONTROL Add workstream]** i [!UICONTROL Workstreams] kontrollpanelens område.
1. Ange ett namn som ska ersättas **[!UICONTROL Untitled Workstream]** och tryck på Enter.

   Du kan lägga till ritytor i arbetsflödet eller klicka på [!UICONTROL **Alla anslagstavlor**] för att gå tillbaka till kontrollpanelen.

## Skapa en ny anslagstavla i ett arbetsflöde

1. Om du inte redan arbetar i ett arbetsflöde klickar du på [!UICONTROL **Visa arbetsflöde**] på kontrollpanelen för att öppna ett befintligt arbetsflöde.
1. Klicka **[!UICONTROL Add board]** på [!UICONTROL Boards] -fliken i arbetsflödet.
1. Välj en mall för styrelsen.

| Mall | Beskrivning |
|---------|----------|
| Grundläggande bräde | Tre standardkolumner finns på ritytan. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Inga kolumnprinciper används. |
| Kanban-tavla | Följande kolumner finns på styrelsen: Eftersläpning, Nytt, Pågår, Fullständigt och Väntande. Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna.<p>Om du vill använda eftersläpningen måste du ställa in filter för inloppskolumnen. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Om du vill granska standardreglerna för varje kolumn klickar du på [!UICONTROL **Mer** meny] i en kolumn och markera [!UICONTROL **Redigera**]. Du kan ändra vilken profil som helst av dessa förinställda profiler. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospektivkort | Följande kolumner finns på styrelsen: Vad gick bra? Vad kan förbättras? Vem ska vi fira? Vad kan vi göra för att gå fortare? Du kan lägga till nya kolumner och byta namn på eller ta bort standardkolumnerna. <p>Inga kolumnprinciper används. |
| <span class="preview">Upprepningsprocess</span> | <span class="preview">Detta är den anslagstavla som används för att definiera och köra en iteration. <p>Följande kolumner finns på styrelsen: Eftersläpning, Nytt, Pågår, Fullständigt och Väntande. Du kan inte lägga till några kolumner på anslagstavlan. <p>Om du vill granska standardreglerna för varje kolumn klickar du på [!UICONTROL **Mer**] meny i en kolumn och markera [!UICONTROL **Redigera**]. Du kan ändra vilken profil som helst av dessa förinställda profiler. Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

Mer information om hur du ställer in styrelsen finns i [Skapa eller redigera en anslagstavla](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrera listan med ritytor i ett arbetsflöde

När andra filter än standardvärdena används i board-listan visas en indikator på filterikonen ![Filter tillämpat](assets/boards-filterapplied-30x30.png). Klicka [!UICONTROL **Rensa alla**] för att ta bort alla filter och klicka på [!UICONTROL **Göm filter**] för att stänga filterpanelen.

{{step1-to-boards}}

1. Klicka på [!UICONTROL **Visa arbetsflöde**] för att öppna ett arbetsflöde.
1. Klicka på [!UICONTROL **Varumärkena**] om den inte redan visas.
1. Klicka [!UICONTROL **Filter**].
1. Markera de anslagstavlor som du vill se efter status (arkiverade anslagstavlor, aktiva anslagstavlor eller alla anslagstavlor).
1. Markera de ritytor som du vill visa efter mall.

## Lägga till medlemmar i ett arbetsflöde

Personer och team måste läggas till i arbetsflödet som medlemmar innan de kan visa arbetsflödet och dess innehåll. En medlem i arbetsflödet kan lägga till och ta bort medlemmar i arbetsflödet och se vilka styrelser som finns i arbetsflödet.

>[!NOTE]
>
>En medlem i ett arbetsflöde kan inte öppna en styrelse i ett arbetsflöde förrän de läggs till i den specifika styrelsen som medlem.

{{step1-to-boards}}

1. Klicka på [!UICONTROL **Visa arbetsflöde**] för att öppna ett arbetsflöde.
1. Klicka på **[!UICONTROL Add member]** icon ![Lägg till medlemmar](assets/boards-addmember-spectrum-25x25.png) för att lägga till medlemmar och team i arbetsflödet.

   Detta är samma process som att lägga till medlemmar i en styrelse. Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## Konfigurera ett arbetsflöde

{{step1-to-boards}}

1. Klicka på [!UICONTROL **Visa arbetsflöde**] för att öppna ett arbetsflöde.
1. Klicka [!UICONTROL **Konfigurera**] för att öppna [!UICONTROL Configure Workstream] -panelen.
1. (Valfritt) Skriv en beskrivning av arbetsflödet. Beskrivningen visas på kontrollpanelen.

   Det totala antalet kort, antalet spetsiga kort och antalet iterationer visas i avsnittet Kortlista. Klicka [!UICONTROL **Visa lista**] för att öppna listan och lägga till kort. Mer information finns i [Använda kortlistan](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Om en iteration har definierats visas dess startdatum, antal kort och antal punkter. Klicka [!UICONTROL **Visa upprepningsbord**] för att öppna styrelsen. Mer information finns i [Skapa en iteration i ett arbetsflöde](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Klicka [!UICONTROL **Lägg till källa**] för att definiera en källa för import av kort till arbetsflödet. För närvarande är den enda tillgängliga källan [!DNL Adobe Workfront].
1. Lägg till filter för att importera uppgifter och utgåvor från Workfront som kort.

   Att lägga till filter för arbetsflödeskällor är detsamma som att lägga till filter för en inloppskolumn på en grundbräda eller på en kanban-bräda. Mer information finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
