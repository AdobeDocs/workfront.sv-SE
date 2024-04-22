---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Hantera kortkolumner
description: En ny anslagstavla innehåller som standard tre kolumner. Du kan lägga till fler kolumner, ändra ordningen på kolumnerna, byta namn på kolumner och ta bort kolumner som du inte behöver.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 99eaafe4b2143f0e29bf677904c1caa8a19d5192
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Hantera kortkolumner

En ny anslagstavla innehåller som standard tre kolumner. Du kan lägga till fler kolumner, ändra ordningen på kolumnerna, byta namn på kolumner och ta bort kolumner som du inte behöver.

Kolumninställningarna innehåller principer som gör att du kan definiera alternativ för vad som händer med ett kort när det flyttas till den kolumnen.

Mer information om hur du sorterar korten i kolumner finns i [Filtrera och söka på en anslagstavla](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

&#42;Kontakta din [!DNL Workfront] administratör.

## Lägga till en kolumn på en anslagstavla

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka **[!UICONTROL Add Column]** till höger om befintliga kolumner.
1. Skriv ett namn i den nya kolumnen och klicka på **[!UICONTROL Add Column]**.

   ![Lägg till ny kolumn](assets/boards-add-column.png)

>[!TIP]
>
>Information om hur du lägger till en inloppskolumn finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Ändra ordning på kolumner på en anslagstavla

1. Gå till styrelsen.
1. Dra och släpp kolumnerna i rätt ordning. Se till att du markerar den övre delen av kolumnen innan du drar den till en annan plats.

   ![Dra och släpp kolumn](assets/boards-dragdropcolumn.png)

## Byta namn på en boardkolumn

1. Gå till styrelsen.
1. Klicka på kolumnnamnet, skriv det nya namnet och tryck på Retur.

   eller

   Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och markera **[!UICONTROL Edit]**. I området Inställningar skriver du det nya namnet i **[!UICONTROL Column name]** och klicka **[!UICONTROL Close]**.

## Ta bort en boardkolumn

När du tar bort en kolumn från en rityta kan den inte återskapas.

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och väljer **[!UICONTROL Delete]**.

   >[!NOTE]
   >
   >Det går inte att ta bort kolumner som innehåller kort, inklusive arkiverade kort. Om du försöker ta bort en kolumn som innehåller kort måste du välja en annan kolumn för dessa kort.

## Visa kortantal

Du kan använda en konfigurationsinställning för att visa antalet kort i varje kolumn.

Om du använder PIA-gränsen för en kolumn läggs ingen separat korträknare till. Mer information om PIA-begränsningar finns i [Hantera [!UICONTROL Work in Progress] (PIA) begränsning av antalet anställda](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Gå till styrelsen.
1. Klicka **[!UICONTROL Configure]** till höger om ritytan för att öppna panelen Konfigurera.
1. Expandera **[!UICONTROL Column]**.
1. Aktivera **[!UICONTROL Display a column card count]**.

   ![Aktivera korträknaren](assets/display-card-count.png)

   Korträknaren visas högst upp i varje kolumn.

1. Klicka **[!UICONTROL Hide configure]** för att stänga [!UICONTROL Configure] -panelen.

## Definiera kolumninställningar och -profiler

Kolumnprinciper inkluderar automatisk uppdatering av fältvärden och inställning av en gräns för pågående arbete.

Principen för att uppdatera statusen fungerar automatiskt för både kortet och kolumnen:

* När ett kort flyttas till en kolumn med en profil uppdateras kortets status till den status som definierats i profilen. Detta gäller både ad hoc-kort och anslutna kort.
* När ett tillfälligt eller anslutet kort uppdateras på kortet för att matcha kolumnstatusen i profilen, eller när ett anslutet kort uppdateras någon annanstans i Workfront, flyttas kortet automatiskt till den kolumnen. Om en anpassad status på ett kort matchar systemstatusen som är tilldelad kolumnen flyttas kortet till den kolumnen.

Ett kort finns kvar i en kolumn där det är placerat om kortstatusen inte matchar någon status som angetts i någon befintlig kolumnprofil.

>[!NOTE]
>
>Dynamiska kort placerar alltid kort i kolumnen som matchar deras status, oavsett om kolumnprinciper är aktiverade eller inaktiverade. Korten återgår till sina tilldelade kolumner när du uppdaterar ritytan.
> 
>Om du flyttar ett kort från en kolumn till en annan med samma status för alla kort, återgår kortet till den ursprungliga kolumnen när du uppdaterar kortet.

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och väljer **[!UICONTROL Edit]**.

   The [!UICONTROL Settings] visas. The **[!UICONTROL Column name]** låter dig veta vilken kolumn du definierar inställningar för.

1. Aktivera **[!UICONTROL Update field values automatically]** princip för att ändra vissa fältvärden automatiskt när ett kort flyttas till den här kolumnen.

   ![Kolumninställningar och -principer](assets/boards-column-policies-enabled.png)

1. (Valfritt) Ange ett värde för kortstatus:

   1. Välj **[!UICONTROL Status]** kryssruta.

   1. Välj den status som ska gälla för ett kort när det flyttas till den här kolumnen.

      ![Status för kolumner](assets/boards-column-status.png)

      Statusöversättningsalternativen för anslutna kort visas också. (Statusöversättning gäller inte för ad hoc-kort.) Dessa alternativ avgör vilken anpassad status som används för uppgiften eller utgåvan i [!DNL Workfront] när ett anslutet kort flyttas till den här kolumnen.

   1. Välj en [!UICONTROL **Egen**] status som ska gälla för kortet för uppgifter och för utgåvor.

      När ett kort flyttas till den här kolumnen, [!DNL Workfront] försöker först att använda den anpassade statusen (till exempel Löst). Om den valda anpassade statusen inte är tillgänglig för det kortet uppmanas du att välja en annan status som motsvarar systemstatusen (från steg b ovan). Mer information om status finns i [Översikt över status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Om statusen för den anslutna aktiviteten eller utgåvan ändras till den anpassade statusen eller systemstatusen som anges i kolumnprincipen, flyttas kortet automatiskt till kolumnen.

1. (Valfritt) Ange ett värde för korttilldelningarna:

   1. Välj **[!UICONTROL Assignees]** kryssruta.
   1. Välj en åtgärd.

      * **[!UICONTROL Add on assignees]:** De tilldelningar du väljer läggs till i den befintliga listan med tilldelningar på ett kort när det flyttas till den här kolumnen.
      * **[!UICONTROL Override assignees]:** De tilldelade som du väljer åsidosätter alla andra tilldelningar och blir de enda tilldelningarna på ett kort när det flyttas till den här kolumnen.

   1. Klicka [!UICONTROL **Lägg till uppdrag**] och söka efter en användare. Välj tilldelningar från sökresultaten. Alla Workfront-användare och -team finns att välja bland.

      ![Tilldelningar för kolumn](assets/boards-column-assignees.png)

1. (Valfritt) Ange ett värde för korttaggarna:

   1. Välj **[!UICONTROL Cards]** kryssruta.
   1. Välj en åtgärd.

      * **[!UICONTROL Add on tags]:** De taggar du väljer läggs till i den befintliga listan med taggar på ett kort när det flyttas till den här kolumnen.
      * **[!UICONTROL Override tags]:** De taggar du markerar åsidosätter alla andra taggar och blir de enda taggarna på ett kort när det flyttas till den här kolumnen.

   1. Markera taggarna i listrutan. Endast taggar som redan har skapats i [!UICONTROL Tag Manager] är tillgängliga att välja mellan. Mer information om hur du lägger till nya taggar finns i [Lägg till taggar](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Taggar för kolumn](assets/boards-column-tags.png)

1. Aktivera **[!UICONTROL Work in progress limit]** princip för att begränsa antalet kort som kan läggas till i kolumnen. Ange sedan begränsningsnumret i dialogrutan **[!UICONTROL Set limit]** fält.

   ![PIA-gräns för kolumn](assets/boards-wip-limit-in-column.png)

   Mer information finns i [Hantera PIA-gränsen (Work in Progress) på en moderlista](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Klicka **[!UICONTROL Close]** för att stänga inställningsområdet och visa kolumnen och dess kort.
