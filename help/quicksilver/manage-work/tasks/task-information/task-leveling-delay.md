---
product-area: projects
navigation-topic: task-information
title: Uppdatera nivåfördröjning för aktivitet
description: Ibland kan det finnas konflikter mellan aktivitetsscheman i ett projekt. Du kan fördela resurser eller hantera resurskonflikter genom att schemalägga om resurser och aktiviteter så att alla aktiviteter kan slutföras inom ett realistiskt schema. Mer information om att jämna ut uppgifter finns i Nivåresurser i Gantt-schemat.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Uppdatera nivåfördröjning för aktivitet

Ibland kan det finnas konflikter mellan aktivitetsscheman i ett projekt. Du kan fördela resurser eller hantera resurskonflikter genom att schemalägga om resurser och aktiviteter så att alla aktiviteter kan slutföras inom ett realistiskt schema. Mer information om att jämna ut uppgifter finns i [Nivåresurser i Gantt-schemat](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Som projektledare eller tilldelad uppgift kan du även lägga till en nivåfördröjning för enskilda uppgifter för att ta hänsyn till eventuella konflikter mellan resurser och schemaläggning. Med andra ord kan en aktivitet schemaläggas med en fördröjning för att säkerställa att en mer realistisk tidsplanering täcker resurskonflikter när Adobe Workfront nivåer används.

Om du lägger till en nivåfördröjning för en aktivitet justeras aktivitetens beräknade slutförandedatum. Information om det planerade slutdatumet finns på [Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteter </p> <p>Contribute eller högre behörighet till projekt</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Lägga till en nivåfördröjning till en uppgift

1. Gå till en uppgift som du vill lägga till en nivåfördröjning för.
1. Klicka på **Mer-ikon** till höger om uppgiftsnamnet och klicka sedan på **Redigera**.

   ![](assets/qs-task-edit-icon-highlighted-350x154.png)

1. Klicka **Inställningar**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Ange **Levelingfördröjning**, i timmar, och välj sedan en tidsenhet.\
   Det här är den tidpunkt då resursen kommer att fördröjas när aktiviteten startas på grund av resurskonflikter.

   Välj bland följande alternativ för tidsenheter:

   * Minuter
   * Timmar. Detta är standardinställningen.
   * Dagar
   * Veckor
   * Månader
   * Förflutna minuter
   * Förflutna timmar
   * Förflutna dagar
   * Förflutna veckor
   * Förflutna månader

   >[!TIP]
   >
   >Förfluten tid är en tidsenhet för en uppgifts varaktighet. Det är tiden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna.

1. Klicka **Spara**. 

 
