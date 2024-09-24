---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Lägg till en inmatningskolumn i en anslagstavla
description: Du kan också lägga till en inloppskolumn på din anslagstavla som automatiskt hämtar in uppgifter och ärenden som anslutna kort när de läggs till i Workfront, baserat på filter som du anger.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 0c0c1f538cfd12e18c504fcb42ee424789d1cde8
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---

# Lägga till en inloppskolumn på en anslagstavla

Du kan också lägga till en inloppskolumn på din anslagstavla som automatiskt hämtar in uppgifter och utleveranser som anslutna kort när de läggs till i [!DNL Workfront], baserat på filter som du definierar. Inloppskolumnen kan fungera som en eftersläpningskolumn för ett Kanban-team, en plats där ett supportteam kan se problem när de läggs till i en begärandekö eller i andra syften som du behöver.

Endast en inloppskolumn får finnas på en rityta, och den visas alltid som kolumnen längst till vänster.

Inloppskolumnen är inte tillgänglig på ett dynamiskt bord. Du kan dock uppdatera filtren som definierar vilka kort som ska föras in på en dynamisk anslagstavla. När du ändrar de här filtren på ett dynamiskt ritbord återställs kortinställningar som inte ingår i Workfront-aktiviteten eller -problemet (till exempel taggar).

>[!NOTE]
>
>Av säkerhetsskäl är det bara ägaren av en anslagstavla som kan ändra ritytans filter på panelen Konfigurera.

Intagskolumnen är begränsad till 300 uppgifter och 300 problem. Standardordningen för objekten i inloppskolumnen är följande:

Uppgifter:

* Primär order: Projektnamn
* Sekundär ordning: Arbetsfördelningsstruktur

Problem:

* Primär order: Projektnamn
* Sekundärordning: Referensnummer

>[!IMPORTANT]
>
>Vi rekommenderar att du uppdaterar styrelsen ofta om flera användare arbetar på samma gång. Om du uppdaterar sidan är det lättare att hålla de visuella ändringarna på ritytan uppdaterade och det går inte att flytta dubblettkort till ritytan från inmatningskolumnen.
>
>Om du vill synkronisera med Workfront och ta med dig nya uppgifter och problem till styrelsen eller inloppskolumnen klickar du på **[!UICONTROL More]**-menyn ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) bredvid styrelsens namn och väljer **[!UICONTROL Sync connected items]**.

Mer information om kolumner finns i [Hantera bockkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Mer information om anslutna kort finns i [Använda anslutna kort på kort](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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

## Skapa en inloppskolumn med enkla filter

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Configure]** till höger om kortet för att öppna konfigurationspanelen.
1. Expandera **[!UICONTROL Board]**.
1. Aktivera **[!UICONTROL Dynamically intake items to board]**.

   ![Alternativ för enkla filter för inloppskolumner](assets/intake-column-simple-filters.png)

   Inloppskolumnen läggs till till vänster om ritytan. Den är tom tills du tillämpar filter på den.

1. (Valfritt) Sök efter och välj [!DNL Workfront] [!UICONTROL **Projekt**].
1. (Valfritt) Sök efter och välj användare eller team [!UICONTROL **Uppdrag**].
1. Välj [!UICONTROL **Inkludera slutfört arbete**] om du vill visa uppgifter och problem med statusen Fullständigt i inloppskolumnen.

   >[!NOTE]
   >
   >Om det här alternativet inte är markerat kommer kort i andra statusar att&quot;ramla av&quot; och inte längre visas.

1. Klicka på [!UICONTROL **Använd**].

   Alla objekt visas som anslutna kort i brädans inloppskolumn.

   ![Intagskolumn](assets/intake-column-added3.png)

## Skapa en inloppskolumn med avancerade filter

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Configure]** till höger om kortet för att öppna konfigurationspanelen.
1. Expandera **[!UICONTROL Board]**.
1. Aktivera **[!UICONTROL Dynamically intake items to board]**.

   Inloppskolumnen läggs till till vänster om ritytan. Den är tom tills du tillämpar filter på den.

1. Klicka på [!UICONTROL **Använd avancerade filter**].
1. Klicka på **[!UICONTROL Add filter sources]** och välj **[!UICONTROL Tasks]** eller **[!UICONTROL Issues]**.

   ![Avancerade filteralternativ för inmatningskolumn](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Du kan filtrera inloppskolumnen så att den innehåller både uppgifter och problem, men du måste konfigurera filtren separat för varje objekttyp.
   >
   >Du kan också välja sparade filter och systemstandardfilter.

1. Klicka på **[!UICONTROL New filter]** på filterpanelen för att komma igång.

   ![Klicka på Nytt filter](assets/intake-filter-dialog5.png)

1. Skapa filtret och klicka på **[!UICONTROL Save as new]**.

   ![Filterverktyget](assets/intake-filter-dialog6.png)

   I det här exemplet visas ett filter för aktiviteter från ett specifikt projekt som har statusen [!UICONTROL New] eller [!UICONTROL In Progress].

   >[!NOTE]
   >
   >Vi rekommenderar att du inte använder jokertecknet&quot;Me&quot; (inloggad användare) i ett kortfilter eftersom det inte alltid är säkert att uppgifter eller problem visas för den inloggade användaren. När styrelsen har konfigurerats med rätt uppgifter och ärenden kan du filtrera ritytan så att den visar objekt för en viss tilldelad person. Mer information finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Mer information om hur du skapar ett filter finns i avsnittet&quot;Skapa eller redigera ett filter i standardverktyget&quot; i artikeln [Skapa eller redigera filter i [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Namnge filtret och klicka på **[!UICONTROL Save]**.

   ![Ange ett namn för filtret](assets/intake-filter-dialog7.png)

   Om du ger filtret ett unikt namn kan du söka efter det senare.

1. Filtret visas i listan med sparade filter och används automatiskt i inloppskolumnen. Klicka på krysset högst upp på filterpanelen för att stänga det.

   ![Sparat filter](assets/intake-filter-dialog8.png)

1. (Valfritt) Om du vill dela filtret med andra håller du pekaren över det sparade filtret, klickar på **[!UICONTROL More]**-menyn ![Mer-menyikonen](assets/more-icon-spectrum.png) och väljer **[!UICONTROL Share]**. Välj de användare eller team du vill dela med i rutan Filterdelning. Mer information finns i [Dela ett filter, en vy eller en gruppering](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Valfritt) Om du vill ta med både uppgifter och problem i inloppskolumnen klickar du på **[!UICONTROL Filter sources]** och väljer det andra objektet för att skapa ett annat filter.
1. När du är klar med att lägga till filter kontrollerar du att rätt uppgifter och problem visas i intag-kolumnen.

   ![Intagskolumn](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Du kan uppdatera filtren när som helst genom att öppna konfigurationspanelen, klicka på **[!UICONTROL Filter sources]** och välja **[!UICONTROL Tasks]** eller **[!UICONTROL Issues]**.

## Använda inloppskolumnen

Kort i inloppskolumnen går inte att redigera förrän du flyttar dem till andra kortkolumner. Du kan klicka på kortet för att öppna det i en skrivskyddad vy eller klicka på ![Öppna uppgift eller utgåva](assets/boards-launch-icon.png) för att öppna uppgiften eller utgåvan på en ny flik i webbläsaren.

Du kan ändra ordning på objekten i inloppskolumnen manuellt.

Ikonerna längst upp till höger i kolumnen visar hur många kort som finns i kolumnen och hur många filter som används.

1. (Valfritt) Om du vill söka efter ett objekt i kolumnen för intag klickar du på ![ikonen Sök](assets/search-icon.png) i kolumnen.
1. (Valfritt) Om du vill flytta ett kort från infusionskolumnen till en annan kolumn drar och släpper du kortet där du vill att det ska visas.

   eller

   Klicka på **[!UICONTROL More]**-menyn ![Mer menyikon](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Move]**. Välj sedan en annan kolumn i rutan **[!UICONTROL Move Item]** och välj **[!UICONTROL Move]**.

1. (Valfritt) Om du vill ta bort inloppskolumnen klickar du på **[!UICONTROL More]**-menyn ![Mer-menyikonen](assets/more-icon-spectrum.png) och väljer **[!UICONTROL Delete]**.
