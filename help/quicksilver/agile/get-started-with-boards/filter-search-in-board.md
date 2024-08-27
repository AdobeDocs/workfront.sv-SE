---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrera och söka på en anslagstavla
description: Du kan filtrera en anslagstavla så att endast vissa kort visas.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Filtrera och söka på en anslagstavla

Du kan filtrera en anslagstavla så att den visas:

* Kort som tilldelats vissa personer
* Kort med vissa taggar
* Kort med en viss status
* Kort som förfaller inom en viss tidsram
* Arkiverade kort
* Kort som är kopplade till ett visst projekt

När du sorterar på anslagstavlan sorteras alla kort i kolumnerna. Det går inte att sortera en enstaka kolumn, och eftersläpningen eller inloppskolumnen sorteras inte.

Genom att söka kan du även hitta ett visst kort på kortet.

När filter används visas en indikator på ![ritytan ](assets/boards-filterapplied-30x30.png). Klicka på **[!UICONTROL Clear All]** för att ta bort alla filter från ritytan och klicka på komprimeringsikonen för att stänga filterpanelen.

![Panelen Filter](assets/boards-all-filters-collapsed-0823.png)

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

## Filtrera en anslagstavla efter tilldelningar

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Members] och markera den eller de personer vars kort du vill se. Du kan även visa kort som inte har tilldelats.

   ![Filtrera efter medlem](assets/boards-filter-by-assignees-0822.png)

## Filtrera en anslagstavla efter taggar

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Tags] och markera de taggar du vill se.

   ![Filtrera efter tagg](assets/boards-filter-by-tags-0822.png)

## Filtrera en anslagstavla efter status

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Statuses] och välj de statustyper som du vill se.

   Du kan även dölja färdiga kort.

   ![Filtrera efter status](assets/boards-filter-by-status-0822.png)

## Filtrera en anslagstavla efter förfallodatum

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Due Date] och välj datumalternativen som du vill se.

   Endast kort i de valda datumintervallen visas.

   ![Filtrera efter förfallodatum](assets/boards-filter-by-due-date-0822.png)

## Filtrera en anslagstavla för att visa arkiverade kort

Som standard visas bara aktiva kort på en anslagstavla. Du kan filtrera anslagstavlan så att även arkiverade kort visas.

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Konfigurera**] till höger på kortet för att öppna konfigurationspanelen.
1. Expandera [!UICONTROL **kort**].
1. Aktivera [!UICONTROL **Visa arkiverade kort på anslagstavlan**].
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Archived Cards] och välj **[!UICONTROL Archived cards]** om du vill visa arkiverade kort.

   Filtret visar antalet arkiverade kort.

   ![Filtrera arkiverade kort](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Avsnittet [!UICONTROL Archived Cards] är inte tillgängligt i filtret om du inte har aktiverat konfigurationsinställningen för att visa arkiverade kort. Mer information finns i [Anpassa vilka fält som ska visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Välj **[!UICONTROL Archived cards]** igen om du vill ta bort alternativet och bara visa aktiva kort.

## Filtrera en anslagstavla efter anslutning

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Filter**], expandera avsnittet [!UICONTROL Connection] och välj [!DNL Workfront] -projekten för de anslutna kort som du vill se.

   Du kan även visa kort som inte är anslutna till ett projekt.

   ![Filtrera efter anslutning](assets/boards-filter-by-connection.png)

## Sortera på en bräda

När du väljer ett alternativ att sortera efter sorteras alla kolumner. Det går inte att sortera en enstaka kolumn, och eftersläpningen eller inloppskolumnen sorteras inte.

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Sortera efter**] och välj [!UICONTROL **Namn**], [!UICONTROL **Förfallodatum**], [!UICONTROL **Uppskattning**], [!UICONTROL **Status**] eller [!UICONTROL **Anslutning**].

   Anslutning (projektnamn) gäller endast anslutna kort, och de andra alternativen sorterar både anslutna kort och ad hoc-kort i kolumnerna.

   Alternativet &quot;användarordning&quot; returnerar korten i den ordning de ställdes in manuellt, innan några andra sorteringsalternativ tillämpades. Det här är standardsorteringen för kolumnerna.

1. Välj [!UICONTROL **Omvänd ordning**] om du vill sortera kolumnerna i omvänd ordning för sorteringsalternativet.

   Pilen på sorteringsikonen anger om kolumnerna är sorterade i stigande eller fallande ordning.

   När en annan sortering än standardsorteringen används visas en indikator på sorteringsikonen ![Sortera använd](assets/sort-applied-boards.png).

   ![Sortera efter kolumner på en rityta](assets/sort-by-columns-in-board.png)

## Sök på en anslagstavla

1. Gå till styrelsen.
1. Klicka på [!UICONTROL **Sök**] och skriv en sökterm. Tryck sedan på Enter.

   Alla kort som innehåller söktermen visas.

   Klicka på X för att rensa sökningen.

   ![Sök efter kort på en anslagstavla](assets/boards-searchbox.png)
