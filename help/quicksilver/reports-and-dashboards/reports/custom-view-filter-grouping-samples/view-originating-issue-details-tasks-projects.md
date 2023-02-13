---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: ursprungliga utgivningsdetaljer för uppgifter och projekt'
description: När ett problem konverteras till en aktivitet eller ett projekt skapas en matchande objektrelation mellan aktiviteten eller projektet och problemet. I den här vyn visas följande fält i problemet som slutförs automatiskt när aktiviteten eller projektet slutförs - REDIGERA ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Visa: ursprungliga utgivningsdetaljer för uppgifter och projekt

När ett problem konverteras till en aktivitet eller ett projekt skapas en matchande objektrelation mellan aktiviteten eller projektet och problemet. I den här vyn visas följande fält i problemet som slutförs automatiskt när aktiviteten eller projektet slutförs:

* Namn
* Anmälningsdatum
* Planerat slutförandedatum
* Faktiskt slutförandedatum
* Typ av begäran
* Originalnamn
* Tilldelad användare

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Mer information finns även i [Visa: visa information om ursprungligt problem i uppgifts- och projektlistor](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa information om ursprungligt problem för uppgifter och projekt

1. Gå till en lista med uppgifter eller en lista med projekt.
1. Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. I **Förhandsgranska kolumn** -område, ta bort alla kolumner utom en.
1. Klicka på rubriken för den återstående kolumnen och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Klicka **Spara vy**.
