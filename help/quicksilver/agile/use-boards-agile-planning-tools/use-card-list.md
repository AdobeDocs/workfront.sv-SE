---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Använda kortlistan
description: Du kan skapa en kortlista i en arbetsström och lägga till korten i iterationer.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Använda kortlistan

>[!IMPORTANT]
>
>Arbetsströmmar är inte tillgängliga för alla kunder.

Du kan skapa en kortlista i en arbetsström och lägga till korten i iterationer.

Kortlistan kan fungera som en eftersläpning av arbete för arbetsflödet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> 
   <p>Nytt: [!UICONTROL Contributor] eller senare</p> 
   <p>eller</p>
   <p>Aktuell: [!UICONTROL Request] eller högre</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till kort i kortlistan

{{step1-to-boards}}

1. Om du vill öppna ett arbetsflöde klickar du på [!UICONTROL **Visa arbetsflöde**].
1. Klicka på fliken [!UICONTROL **Kortlista**].
1. Klicka på [!UICONTROL **Lägg till kort**].
1. Lägg till följande information i dialogrutan [!UICONTROL **Skapa/redigera kort**]:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Kortets namn.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>En beskrivning av kortet.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Det uppskattade antalet timmar som kortet ska fyllas i. Det här är bara en manuell inmatning.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Välj en status för kortet.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Välj en iteration som kortet ska tilldelas.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>Om du vill tilldela kortet börjar du skriva ett namn i sökfältet och markerar det sedan när det visas i listan. Du kan lägga till både enskilda personer och team, och du kan tilldela flera personer eller team till ett kort.</p><p>Tilldelningar måste vara medlemmar i arbetsflödet, annars visas de inte i urvalslistan.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Klicka på [!UICONTROL **Spara**].
1. Fortsätt lägga till kort tills du har skapat kortlistan.

## Visa kort

Om du vill visa alla kort för arbetsflödet i en enda lista klickar du på [!UICONTROL **listvyn**] på fliken Kortlista.

Om du vill visa alla kort för arbetsflödet grupperade efter upprepning klickar du på [!UICONTROL **Iterationsvyn**]. Oplanerade kort visas i sin egen grupp.

Om du vill redigera ett befintligt kort markerar du det i listan och klickar på [!UICONTROL **Redigera**].

Om du vill ta bort ett kort markerar du det i listan och klickar på [!UICONTROL **Ta bort**].

### Filterkort

Kort kan bara arkiveras från iterationspanelen. När ett kort arkiveras visas det inte i kortlistan om du inte filtrerar för att visa arkiverade kort. Mer information om att arkivera ett kort finns i [Ta bort eller arkivera ett kort från en anslagstavla](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Åtkomst till kortlistan för arbetsflödet.
1. Klicka på [!UICONTROL **Filter**] och välj [!UICONTROL **Alla**], [!UICONTROL **Aktiva kort**] eller [!UICONTROL **Arkiverade kort**].

   När ett annat filter än standardfiltret används i kortlistan visas en indikator på filterikonen ![Filter använt](assets/boards-filterapplied-30x30.png).

### Sök i kortlistan

1. Åtkomst till kortlistan för arbetsflödet.
1. Klicka på [!UICONTROL **Sök**] och skriv en sökterm. Tryck sedan på Enter.

   Alla kort som innehåller söktermen visas.
Klicka på X för att rensa sökningen.

   ![Sök efter kort på en anslagstavla](assets/boards-searchbox.png)

## Lägga till kort i en iteration

>[!NOTE]
>
>Du måste skapa en iteration innan du kan lägga till kort i den. Mer information finns i [Skapa en iteration i ett arbetsflöde](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Åtkomst till kortlistan för arbetsflödet.
1. Välj [!UICONTROL **iterationsvyn**] för att se vilka kort som har tilldelats en iteration och vilka som är oplanerade.
1. Välj ett oplanerat kort i listan och klicka på [!UICONTROL **Redigera**].
1. Välj en iteration i fältet [!UICONTROL **Iterations**].
1. Om du använder artikelpunkter anger du ett värde i fältet [!UICONTROL **Beräkning**].
1. Klicka på [!UICONTROL **Spara**].

   Kortet flyttas till iteration och iterationsmåtten visar antalet kort och punkter.

   Du kan också dra och släppa ett kort från gruppen Oplanerade kort i iteration eller klicka på [!UICONTROL **Lägg till kort**] för att lägga till ett nytt kort i iteration.

>[!TIP]
>
>Om du har skapat en upprepningsprocessboard visas alla oplanerade kort i kortlistan i kolumnen [!UICONTROL Backlog]. När ett kort flyttas till en annan kolumn blir det en del av den aktiva iterationen. Kort som du lägger till i listan läggs till i en kolumn baserat på deras status.
