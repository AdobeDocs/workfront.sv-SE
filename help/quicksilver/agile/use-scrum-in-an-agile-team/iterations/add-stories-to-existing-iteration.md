---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Lägga till artiklar i en befintlig upprepning
description: Du kan lägga till artiklar i en iteration på flera olika sätt.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Lägga till artiklar i en befintlig upprepning

Du kan lägga till artiklar i en iteration på något av följande sätt:

* Från eftersläpningen efter att upprepningen har skapats, enligt beskrivningen i avsnittet [Flytta artiklar från eftersläpningen till en iteration eller [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) i [Hantera den flexibla eftersläpningen](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Från sidan [!UICONTROL Details] för den enskilda aktiviteten eller problemet
* Från en uppgift eller en utleveranslista
* Från en rapport
* Från en kontrollpanel

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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Worker] eller högre</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL Manage] åtkomst till det projekt som artikeln är på</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

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

Du kan konfigurera enskilda Scrum-team så att de använder projektdatum som standard, i stället för upprepningsdatum. Mer information finns i avsnittet [Konfigurera hur datum ska användas när arbetsobjekt läggs till i en iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) i artikeln [Konfigurera repet](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Lägga till en artikel i en befintlig iteration

Så här lägger du till artiklar i en iteration direkt från uppgiften eller utgåvan:

>[!IMPORTANT]
>
>När aktiviteten har flyttats till upprepningen kan du inte uppdatera [!UICONTROL Duration Type] eller [!UICONTROL Task Constraint]. [!UICONTROL Duration Type] är inställt på [!UICONTROL Simple] och [!UICONTROL Task Constraint] är inställt på [!UICONTROL Fixed Dates] så att tidslinjen för aktiviteten hålls konsekvent med tidslinjen för iterationen.

### Från fliken Åtgärder eller Problem

Du kan lägga till vilken uppgift eller vilket problem som helst i en iteration om du har Hantera-åtkomst till projektet. Tänk på följande när du flyttar en uppgift eller ett problem till en iteration:

* Om du lägger till flera team kan uppgiften eller utgåvan bara visas på en grupps upprepning. Det här är den iteration du väljer i steg 3 nedan.
* Om uppgiften eller utgåvan tilldelas ett smidigt team och flyttas till ett annat teams iteration ändras inte teamuppdraget.
* Om uppgiften eller utgåvan inte har tilldelats ett team tilldelas uppgiften eller utgåvan till det team som äger den.
* Du kan inte lägga till överordnade uppgifter i iterationen. Om du lägger till några underordnade uppgifter visas den överordnade aktiviteten på Samlingstavlan som en simbana.

1. Gå till det projekt, den rapport eller den kontrollpanel som innehåller uppgiften eller problemet som du vill lägga till i en iteration.
1. Markera en eller flera uppgifter eller problem.
1. Klicka på **[!UICONTROL More]** ![](assets/more-icon.png) > **[!UICONTROL Add to Iteration]**.\
   Du kan inte tilldela uppgifter eller ärenden som tilldelats icke-flexibla team.

1. Skriv namnet på iterationen i rutan **[!UICONTROL Add Stories]**.

   >[!NOTE]
   >
   >Du kan flytta en artikel från en befintlig iteration till en ny iteration.

1. Om du lägger till uppgifter klickar du på **[!UICONTROL Add Stories]**.\
   eller\
   Om du lägger till problem klickar du på **[!UICONTROL Add Issues]**.
