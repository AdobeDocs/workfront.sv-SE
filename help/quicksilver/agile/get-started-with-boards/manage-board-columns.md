---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Hantera kortkolumner
description: En ny anslagstavla innehåller som standard tre kolumner. Du kan lägga till fler kolumner, ändra ordningen på kolumnerna, byta namn på kolumner och ta bort kolumner som du inte behöver.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: ba6b5db8416e0e564b155dd040933b41fe87c286
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Hantera kortkolumner

En ny anslagstavla innehåller som standard tre kolumner. Du kan lägga till fler kolumner, ändra ordningen på kolumnerna, byta namn på kolumner och ta bort kolumner som du inte behöver.

Kolumninställningarna innehåller principer som gör att du kan definiera alternativ för vad som händer med ett kort när det flyttas till den kolumnen.

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

&#42;Kontakta [!DNL Workfront] administratör.

## Lägga till en kolumn på en anslagstavla

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en anslagstavla. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka **[!UICONTROL Add Column]** till höger om de befintliga kolumnerna.
1. Skriv ett namn i den nya kolumnen och klicka på **[!UICONTROL Add Column]**.

   ![Lägg till ny kolumn](assets/boards-add-column.png)

>[!TIP]
>
>Information om hur du lägger till en inloppskolumn finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Ändra ordning på kolumner på en anslagstavla

1. Gå till styrelsen.
1. Dra och släpp kolumnerna i rätt ordning. Se till att du markerar kolumnens övre del innan du drar den till en annan plats.

   ![Dra och släpp kolumn](assets/boards-dragdropcolumn.png)

## Byta namn på en boardkolumn

1. Gå till styrelsen.
1. Klicka på kolumnnamnet, skriv det nya namnet och tryck på Retur.

   eller

   Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och markera **[!UICONTROL Edit]**. I området Inställningar skriver du det nya namnet i **[!UICONTROL Column name]** och klicka **[!UICONTROL Close]**.

## Ta bort en boardkolumn

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och väljer **[!UICONTROL Delete]**.

   >[!NOTE]
   >
   >Det går inte att ta bort kolumner som innehåller kort, inklusive arkiverade kort. Om du försöker ta bort en kolumn som innehåller kort måste du välja en annan kolumn för dessa kort.

## Visa kortantal

Du kan använda en konfigurationsinställning för att visa antalet kort i varje kolumn.

Om du använder PIA-gränsen för en kolumn läggs ingen separat korträknare till. Mer information om PIA-begränsningar finns i [Hantera [!UICONTROL Work in Progress] (PIA) begränsning av antalet anställda](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Gå till styrelsen.
1. Klicka **[!UICONTROL Configure]** till höger om anslagstavlan för att öppna konfigurationspanelen.
1. Expandera **[!UICONTROL Column]**.
1. Aktivera **[!UICONTROL Display a column card count]**.

   ![Aktivera korträknare](assets/display-card-count.png)

   Korträknaren visas högst upp i varje kolumn.

1. Klicka **[!UICONTROL Hide configure]** för att stänga [!UICONTROL Configure] -panelen.

## Definiera kolumninställningar och -profiler

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) i kolumnen och väljer **[!UICONTROL Edit]**.

   The [!UICONTROL Settings] visas. The **[!UICONTROL Column name]** låter dig veta vilken kolumn du definierar inställningar för.

1. Aktivera **[!UICONTROL Update field values automatically]** princip för att ändra vissa fältvärden automatiskt när ett kort flyttas till den här kolumnen.

   ![Kolumninställningar och -principer](assets/boards-column-policies-enabled.png)

1. (Valfritt) Ange ett värde för kortstatus:

   1. Välj **[!UICONTROL Status]** kryssruta.

   1. Välj den status som ska gälla för ett kort när det flyttas till den här kolumnen.

      ![Status för kolumner](assets/boards-column-status.png)

      Statusöversättningsalternativen för anslutna kort visas också. (Statusöversättning gäller inte för ad hoc-kort.) Dessa alternativ avgör vilken status som används för uppgiften eller utgåvan i [!DNL Workfront] när ett anslutet kort flyttas till den här kolumnen.

   1. Klicka på knappen **[!UICONTROL Edit]** icon ![Ikonen Redigera](assets/edit-icon-spectrum.png).
   1. Om du använder tidiga funktioner: Välj en [!UICONTROL **Egen**] status som ska gälla för kortet, för både uppgifter och ärenden.

      När ett kort flyttas till den här kolumnen [!DNL Workfront] försöker först att använda den anpassade statusen (till exempel Löst). Om den anpassade statusen inte är tillgänglig för det kortet kommer Workfront att använda systemstatusen i stället (till exempel Stängt). Systemstatusen är den status du valde i steg b ovan.

      Om statusen för den anslutna aktiviteten eller utgåvan ändras till den anpassade statusen eller systemstatusen som anges i kolumnprincipen flyttas kortet automatiskt till kolumnen.

      >[!NOTE]
      >
      >Du kan bara ange en anpassad standardstatus för kolumnen via anmälan av tidig funktion. Mer information finns i [Tidig registrering av nya funktioner för Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

   1. Om du inte använder anmälan om tidig funktion: Välj en status för uppgifter och en status för ärenden. Endast standardinställningen [!DNL Workfront] statusvärden är tillgängliga, inte anpassade statusvärden.

      >[!NOTE]
      >
      >Om du använder anpassade statusvärden i [!DNL Workfront]blir du ombedd att välja status första gången du flyttar ett anslutet kort till den här kolumnen. Om det anslutna projektet till exempel har flera statustyper som alla motsvarar [!UICONTROL Completed]måste du välja vilken status du vill använda i [!DNL Workfront]. Du kan ange ditt val som standard så att du inte behöver göra urvalet varje gång du flyttar ett kort till kolumnen.
      >Mer information om status finns i [Översikt över status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

1. (Valfritt) Ange ett värde för korttilldelningarna:

   1. Välj **[!UICONTROL Assignees]** kryssruta.
   1. Välj en åtgärd.

      * **[!UICONTROL Add on assignees]:** De tilldelningar du väljer läggs till i den befintliga listan med tilldelningar på ett kort när det flyttas till den här kolumnen.
      * **[!UICONTROL Override assignees]:** De tilldelningar du väljer åsidosätter alla andra tilldelningar och blir de enda tilldelningarna på ett kort när det flyttas till den här kolumnen.
   1. Välj de tilldelade i listrutan. Endast styrelseledamöter kan välja bland. Mer information finns i [Lägga till eller ta bort medlemmar från en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

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
