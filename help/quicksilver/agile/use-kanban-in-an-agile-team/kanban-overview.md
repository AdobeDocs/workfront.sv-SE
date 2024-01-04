---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban - översikt
description: Läs den här artikeln för att få en bättre förståelse för hur Kanban-tavlan fungerar.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Kanban - översikt

<!-- Audited: 01/2024 -->

I följande avsnitt kan du bättre förstå hur [!UICONTROL Kanban] kortfunktioner.

En beskrivning av[!UICONTROL anban] metod, se [Skapa ett smidigt team](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Om du är intresserad av att migrera från ett rörligt team [!UICONTROL Kanban] gå till [!DNL Workfront] [!UICONTROL Boards], se [Migrera smidigt team [!UICONTROL Kanban] kort till [!DNL Workfront] boards](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] styrelselayout och -funktioner

The [!UICONTROL Kanban] brädet består av följande element:

**Kolumn med eftersläpning**: Visar alla uppgifter som finns i eftersläpningen. Den här kolumnen visas inte som standard. Mer information om eftersläpningen, inklusive hur den visas på [!UICONTROL Kanban] board, se [Hantera den flexibla eftersläpningen](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Artikelstatus**: Anger hur en artikel fortskrider baserat på vilken statuskolumn artikeln finns i.

Mer information finns i [Uppdatera artikelstatus på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Du kan anpassa artikelstatus för projektet genom att ändra den flexibla vyn enligt beskrivningen i avsnittet [[!UICONTROL Create or customize an Agile view]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Skapa eller redigera vyer i [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Högst femtio kort visas som standard på Kanban-tavlan, men du kan klicka **[!UICONTROL Show More]** för att visa ytterligare kort.

## Relation mellan underaktiviteter och artiklar

Om en artikel innehåller underuppgifter kan du inte uppdatera någon information om själva den överordnade artikeln (till exempel punkter/timmar eller procent färdigt). Dessutom kan du inte flytta artikeln över [!UICONTROL Kanban] för att uppdatera sin status. I stället återspeglas alla ändringar du gör i artikelns underuppgifter i artikeln. De kombinerade artikelpunkterna eller timmarna för alla underaktiviteter avgör den överordnade artikelns punkter eller timmar.

Om en artikel t.ex. bara har en underuppgift som har ett värde på 4 punkter, har artikeln också fyra punkter. Om du ändrar värdet för underaktivitetspunkten till 3 ändras punktvärdet för den överordnade artikeln till 3. Om du skapar en annan underaktivitet i samma artikel och anger punktvärdet för den underaktiviteten till 4, ändras punktvärdet för artikeln till 7 för att återspegla det kombinerade punktvärdet för båda underaktiviteterna.

Samma logik gäller för underaktiviteter på andra nivån (underaktiviteter för underaktiviteter). Om en underaktivitet har en eller flera underaktiviteter på andra nivån beräknas underaktiviteten utifrån underaktiviteterna på andra nivån.

## Funktioner som stöds

Du kan göra följande när du använder Kanban-tavlan:

* [Lägga till en underaktivitet i en befintlig artikel på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Lägg till befintliga uppgifter eller ärenden i [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Tilldela användare till en artikel på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Lägg till artiklar och utgåvor från [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Ta bort artiklar eller utgåvor från [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Redigera artikelinformation](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrera efter användare på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Hantera PIA-gränsen på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Ändra ordning på artiklarna på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Uppdatera artikelstatus på [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Använd flaggor i artiklar på sidan [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Lägg till eftersläpningen i [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
