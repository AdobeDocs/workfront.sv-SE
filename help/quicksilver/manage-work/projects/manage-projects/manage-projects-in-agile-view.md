---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Hantera ett projekt i flexibel vy
description: Obligatoriska planer, licenstyper och åtkomst till Adobe Workfront Plan Team, Pro, Business eller Enterprise Workfront License Type Review, Work eller Plan Behörigheter i åtkomstmodellen Redigera åtkomst och möjlighet att skapa rapporter, instrumentpaneler och kalendrar
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 070bc906d7ca0729697cf9def08416b00e691fc8
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Hantera ett projekt i flexibel vy

{{preview-and-fast-release}}

<!--
Required plans, license types, and access

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront Plan</a> </p> </td> 
   <td> <p>Team, Pro, Business, or Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront License Type</p> </td> 
   <td> <p>Review, Work, or Plan </p> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
 </tbody> 
</table>
-->

Du kan använda smidiga funktioner i ditt projekt utan de administrativa utmaningar som vanligtvis följer med flexibla rutiner (som att hantera en eftersläpning i teamet eller skapa iterationer).

Om du vill arbeta i en flexibel miljö som använder en eftersläpning i team och där du kan skapa iterationer från uppgifter i eftersläpningen följer du instruktionerna i [Arbeta i en flexibel miljö](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till följande områden:</p> 
    <ul> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Rapporter, instrumentpaneler, kalendrar</p> </li> 
     <li> <p>Filter, vyer, grupperingar</p> </li> 
    </ul> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förstå Agile-projekt

>[!NOTE]
>
>Det här avsnittet gäller endast för den äldre Agile-vyn, inte för styrelsevyn för ett projekt.

* [Flexibla funktioner i ett projekt](#agile-functionality-in-a-project)
* [Skillnader när du använder Agile-vyn i ett projekt jämfört med en iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Flexibla funktioner i ett projekt {#agile-functionality-in-a-project}

Följande smidiga funktioner är tillgängliga när du hanterar ett projekt i en flexibel vy:

* Slutförandestatus\
  Mer information om slutförandestatus finns i [Statusöversikt för Iteration-slutförande](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Story board\
  Mer information om artikelpanelen finns i [Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) -avsnitt.

Det finns vissa skillnader mellan att använda rörliga vyer i ett projekt och att arbeta i en rent flexibel miljö (med eftersläpningar och iterationer). Mer information finns i [Skillnader när du använder Agile-vyn i ett projekt jämfört med en iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) i den här artikeln.

### Skillnader när du använder Agile-vyn i ett projekt jämfört med en iteration {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Uppgifter och underuppgifter följer olika visningsregler på artikelstyrelsen](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Backloggar och iterationer används inte](#backlogs-and-iterations-are-not-used)
* [Uppgiftsordningen bibehålls i vyn Agile och kan inte ordnas om](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Aktiviteter mäts endast i planerade timmar](#tasks-are-measured-only-in-planned-hours)
* [Agile Team används inte](#the-agile-team-is-not-used)
* [Varje användare i projektet kan visa projektet i en annan Agile-vy](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Uppgifter och underuppgifter följer olika visningsregler på artikelstyrelsen {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Uppgifter som varken har en överordnad uppgift eller en underuppgift visas alltid som ett artikelkort på artikelpanelen.\
  Följande uppgifter visas till exempel i projektlistvyn:

  ![Flexibel projektlista - aktiviteter utan överordnade eller underordnade uppgifter](assets/agile-project-single-list-nwe.png) Följande uppgifter visas i projektvyn:

  ![Projektflexibel vy - aktiviteter utan överordnade eller underordnade uppgifter](assets/agile-project-singlecard-nwe.png)

* Överordnade aktiviteter som har underaktiviteter visas alltid i **Artiklar** artikelpanelens kolumn. Underaktiviteter visas i den överordnade uppgiftens simfält.\
  Följande uppgifter visas till exempel i projektlistvyn:

  ![Flexibel projektlista - aktiviteter med överordnade och underaktiviteter](assets/agile-project-parent-list-nwe.png)\
  Följande uppgifter visas i projektvyn:

  ![Flexibel projektvy - aktiviteter med överordnade och underordnade uppgifter](assets/agile-project-parent-nwe.png)

* Underuppgifter på andra nivån (underuppgifter till underaktiviteter) visas som ett hängande grått kort från den överordnade aktiviteten.
* Underuppgifter på tredje nivån (underuppgifter till underuppgifter till underuppgifter) visas aldrig på artikelpanelen.

#### Backloggar och iterationer används inte {#backlogs-and-iterations-are-not-used}

När du visar ett projekt i en flexibel vy används inte följande flexibla komponenter:

* **Eftersläpning:** Ingen eftersläpning används eftersom alla uppgifter i projektet automatiskt visas som artiklar.
* **Iterationer:** I stället för att skapa iterationer för att definiera datum när arbetet ska utföras, blir de dagar som för närvarande anges på projekttidslinjen arbetsdagar.

#### Uppgiftsordningen bibehålls i vyn Agile och kan inte ordnas om {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

Den ordning i vilken uppgifter visas i ett projekt bevaras när du visar projektet på en flexibel artikelpanel.

Du kan inte ändra ordning på uppgifter i projektet när du visar projektet i en flexibel vy. Eftersom ändringar av uppgiftsordningen kan påverka andra uppgifter som kan ha beroenden måste du visa projektet i en standardvy för att kunna ändra uppgiftsordningen.

#### Aktiviteter mäts endast i planerade timmar {#tasks-are-measured-only-in-planned-hours}

Uppgifter i ett projekt mäts alltid i Planerade timmar.

I en iteration kan uppgifter (artiklar) mätas i timmar eller punkter.

#### Agile Team används inte {#the-agile-team-is-not-used}

Eftersom rörliga team slutför arbetet med iterationer som de tilldelats, används inte rörliga team när de visar ett projekt i en flexibel vy.

I stället blir alla användare i projektet i stort sett de smidiga teamen för det projektet.

#### Varje användare i projektet kan visa projektet i en annan Agile-vy {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Till skillnad från en smidig upprepning kan användare i ett projekt anpassa den flexibla vyn för sig själva, medan andra användare använder en annan flexibel vy.

I en smidig upprepning bestäms den information som finns tillgänglig på den flexibla artikelpanelen (t.ex. tillgängliga statuskolumner) på teamnivån.

Mer information om hur du anpassar en flexibel vy finns i [Skapa eller anpassa en Agile-vy](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Visa ett projekt i Agile-vyn

1. Gå till projektet som du vill visa i en flexibel vy, antingen i uppgiftslistan <span class="preview">eller listan över utgåvor</span>.
1. Klicka på **Styrelse** icon ![Ikon för anslagstavla](assets/board-icon-for-agile-view.png).

   Vyn i projektvyn visas som standard.

   ![Vy över projekt](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Valfritt) Klicka på **Konfigurera** för att ange alternativ för kolumner och kort.

   Mer information finns i [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) och [Anpassa vilka fält som visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Observera att du inte kan definiera kolumnprinciper i en projektvy.

1. (Valfritt) Klicka på **Använd äldre flexibilitet** om du vill använda den gamla, flexibla vyn i stället för den vanliga vyn.

1. (Valfritt - endast äldre flexibel vy) Om du har skapat en anpassad flexibel vy, eller om en annan användare har skapat en anpassad flexibel vy och delat den med dig, kan du visa den i stället för standardvyn för flexibel visning.

   Klicka på **Visa** och klicka sedan på den anpassade flexibla vy som du vill visa.

   Den anpassade flexibla vyn används nästa gång du klickar på **Agile** -ikon.

   Mer information om hur du skapar en ny flexibel vy finns i [Skapa och anpassa Agile-vyer](#create-and-customize-agile-views).

   Projektet visas i en anpassad, flexibel vy.

1. (Villkorligt - endast äldre, flexibel vy) Om uppgifter i projektet använder andra statusvärden än &quot;Nytt&quot;, &quot;Pågår&quot; eller &quot;Fullständigt&quot; (standardstatusvärdena för Agilvyn), måste du lägga till ytterligare statusvärden i den flexibla vyn för att uppgifter i dessa statusar ska kunna visas.

   Om aktiviteterna har en status som inte visas på den mobila artikelpanelen visas inte själva uppgiften på den mobila artikelpanelen (procentandelen slutfört av dessa uppgifter bidrar dock fortfarande till procentandelen slutfört för överordnade uppgifter och procentandelen slutfört för det övergripande projektet).

   Om du vill lägga till statusvärden i den flexibla vyn skapar du en ny flexibel vy eller anpassar en befintlig flexibel vy enligt beskrivningen i avsnittet&quot;Skapa eller anpassa en flexibel vy&quot; i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Valfritt) Om du vill återgå till listvyn klickar du på **Lista** -ikon.

## Skapa och anpassa Agile-vyer {#create-and-customize-agile-views}

>[!NOTE]
>
>Det här avsnittet gäller endast för den äldre Agile-vyn, inte för styrelsevyn för ett projekt.

Precis som med standardvyer i Workfront kan du anpassa befintliga flexibla vyer eller skapa nya flexibla vyer från grunden. Till skillnad från standardvyer kan du inte skapa nya flexibla vyer som baseras på befintliga flexibla vyer.

Mer information om hur du skapar och anpassar flexibla vyer finns i avsnittet&quot;Skapa eller anpassa en flexibel vy&quot; i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Dela en befintlig Agile-vy

>[!NOTE]
>
>Det här avsnittet gäller endast för den äldre Agile-vyn, inte för styrelsevyn för ett projekt.

Mer information om hur du delar en flexibel vy finns i [Dela ett filter, en vy eller en grupp](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Ta bort en befintlig Agile-vy

>[!NOTE]
>
>Det här avsnittet gäller endast för den äldre Agile-vyn, inte för styrelsevyn för ett projekt.

Mer information om hur du tar bort en vy finns i avsnittet Ta bort en vy i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
