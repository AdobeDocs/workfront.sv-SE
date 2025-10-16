---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Lägg till artiklar i en befintlig iteration
description: Du kan lägga till artiklar i en iteration på flera olika sätt.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Lägga till artiklar i en befintlig upprepning

Du kan lägga till artiklar i en iteration på något av följande sätt:

* Från eftersläpningen efter att upprepningen har skapats, enligt beskrivningen i avsnittet [Flytta artiklar från eftersläpningen till en iteration eller [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) i [Hantera den flexibla eftersläpningen](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Från sidan [!UICONTROL Details] för den enskilda aktiviteten eller problemet
* Från en uppgift eller en utleveranslista
* Från en rapport
* Från en kontrollpanel

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera åtkomst till det projekt som artikeln är på </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förstå hur inlagda artiklar påverkar aktivitetsdatum

När du lägger till en befintlig uppgift i en iteration anges [!UICONTROL Planned Start Date] och [!UICONTROL Planned Completion Date] som standard enligt följande:

### Aktivitet [!UICONTROL Planned Start Date]

* Uppgiften använder iterationens startdatum när:

   * Projektet har ingen [!UICONTROL Planned Start Date] angiven.
   * Projektets [!UICONTROL Planned Start Date] är *före* eller *på* projektets startdatum.

* Aktiviteten använder projektets [!UICONTROL Planned Start Date] när:

   * Projektets [!UICONTROL Planned Start Date] är *efter* upprepningens startdatum.

### Aktivitet [!UICONTROL Planned Completion Date]

* Uppgiften använder iterationens slutdatum när:

   * Projektet har ingen [!UICONTROL Planned Completion Date] angiven.
   * Projektets [!UICONTROL Planned Start Date] är *före eller*, dess startdatum eller projektets [!UICONTROL Planned Completion Date] är *före eller* dess slutdatum.

* Aktiviteten använder projektets [!UICONTROL Planned Completion Date] när:

   * Projektets [!UICONTROL Planned Start Date] är *efter* iterationens startdatum och projektets [!UICONTROL Planned Completion Date] är *efter* iteration slutdatum.

Du kan konfigurera enskilda Scrum-team så att de använder projektdatum som standard, i stället för upprepningsdatum. Mer information finns i avsnittet [Konfigurera hur datum ska användas när arbetsobjekt läggs till i en iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) i artikeln [Konfigurera repet](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Lägga till en artikel i en befintlig iteration

Du kan lägga till vilken uppgift eller vilket problem som helst i en iteration om du har Hantera-åtkomst till projektet. Tänk på följande när du flyttar en uppgift eller ett problem till en iteration:

* Om du lägger till flera team kan uppgiften eller utgåvan bara visas på en grupps upprepning. Det här är den iteration du väljer i steg 3 nedan.
* Om uppgiften eller utgåvan tilldelas ett smidigt team och flyttas till ett annat teams iteration ändras inte teamuppdraget.
* Om uppgiften eller utgåvan inte har tilldelats ett team tilldelas uppgiften eller utgåvan till det team som äger den.
* Du kan inte lägga till överordnade uppgifter i iterationen. Om du lägger till några underordnade uppgifter visas den överordnade aktiviteten på Samlingstavlan som en simbana.

>[!IMPORTANT]
>
>När aktiviteten har flyttats till upprepningen kan du inte uppdatera [!UICONTROL Duration Type] eller [!UICONTROL Task Constraint]. [!UICONTROL Duration Type] är inställt på [!UICONTROL Simple] och [!UICONTROL Task Constraint] är inställt på [!UICONTROL Fixed Dates] så att tidslinjen för aktiviteten hålls konsekvent med tidslinjen för iterationen.

1. Öppna uppgiften eller problemet som du vill lägga till i en iteration.
eller
Gå till det projekt, den rapport eller den kontrollpanel som innehåller uppgiften eller problemet som du vill lägga till i en iteration. Välj sedan en eller flera uppgifter eller problem.

1. Klicka på **[!UICONTROL More]** ![Mer ikon](assets/more-icon.png) > **[!UICONTROL Add to Iteration]**.
Du kan inte tilldela uppgifter eller ärenden som tilldelats icke-flexibla team.

1. I rutan **[!UICONTROL Add To]** börjar du skriva namnet på iterationen och markerar den när den visas i listan.

   >[!NOTE]
   >
   >Du kan flytta en artikel från en befintlig iteration till en ny iteration.

1. Klicka på **[!UICONTROL Add]**.
