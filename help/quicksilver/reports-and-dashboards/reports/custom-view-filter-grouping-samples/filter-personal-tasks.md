---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Personliga uppgifter'
description: Aktivitetsfiltret returnerar tillfälliga arbetsbegäranden som skickas till en användare eller att göra-objekt som lagts till av användare i hemområdet. Personliga uppgifter är inte kopplade till ett projekt, men de kan flyttas till ett projekt om det behövs.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Filter: personliga uppgifter

<!--Audited: 10/2024-->

Aktivitetsfiltret returnerar tillfälliga arbetsbegäranden som skickas till en användare, eller att göra-objekt som lagts till av användare i deras Att göra-widget i hemområdet.

Ad hoc-arbetsbegäranden och att göra-objekt sparas i Adobe Workfront som personliga uppgifter.

Personliga uppgifter är inte kopplade till ett projekt, men de kan flyttas till ett projekt om det behövs. Mer information finns i [Skapa personliga uppgifter](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Rapport om personliga uppgifter](assets/personal-tasks-report.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> 
    <p>Nytt:</p>
   <ul><li><p>Medarbetare som ändrar ett filter </p></li>
   <li><p>Standard för att ändra en rapport</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Begäran om att ändra ett filter </p></li>
   <li><p>Planera att ändra en rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrera personliga uppgifter

Så här skapar du det här filtret:

1. Gå till en lista med uppgifter eller en uppgiftsrapport.
1. Klicka på **Nytt filter** i listrutan **Filter**.
1. (Villkorligt) Klicka på **Lägg till en filterregel** om du försöker få åtkomst till filtret från en rapport, eller börja välja filtervillkor i det första fältet om du får åtkomst till filtret från en lista.
1. (Villkorligt) Välj följande filtervillkor:

   * Från ett listfilter: **Aktivitet** > **Personligt** **Är sant**
   * Från ett rapportfilter: **Aktivitet** > **Personligt** > **Lika (skiftlägeskänsligt)** > **Sant**.
1. Spara filtret.

   I listan visas endast personliga uppgifter som inte finns i några projekt.
