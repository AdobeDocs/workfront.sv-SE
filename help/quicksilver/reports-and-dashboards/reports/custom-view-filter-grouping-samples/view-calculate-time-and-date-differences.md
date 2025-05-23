---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Beräkna skillnader i tid och datum'
description: Lär dig att beräkna tid- och datumskillnader.
author: Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Visa: beräkna tid- och datumskillnader

<!-- Audited: 11/2024 -->

>[!IMPORTANT]
>
>Du kan inte beräkna tid- och datumskillnaden i Adobe Workfront mellan två olika objekt av samma typ. Du kan t.ex. inte beräkna tid- och datumskillnaden mellan två datum i två olika projekt, aktiviteter eller utgåvor.

Du kan beräkna skillnaden mellan följande:

* Tid- och datumskillnaden mellan två datumfält i samma objekt
* Tid- och datumskillnaden mellan ett fält i ett objekt och ett annat fält i det överordnade objektet

>[!TIP]
>
>Dessa beräkningar visar antalet dagar mellan de två datumen. Resultatet visas i dagar. Tidsstämpeln i datumfältet beaktas också, och antalet dagar kan följas av decimaler om tidsstämpeln inte matchar. Om aktiviteten slutfördes sent visas antalet dagar som ett negativt värde.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: </p><ul><li><p>Medarbetare som ändrar en vy </p></li><li>
   <p>Standard för att ändra en rapport</p></li></ul><p>eller</p><p>Aktuell:</p><ul><li><p>Begäran om att ändra en vy </p></li><li>
   <p>Planera att ändra en rapport</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beräkna tiden och datumskillnaden mellan två datumfält i samma objekt

Du kan till exempel beräkna skillnaden mellan Planerat slutförandedatum och Faktiskt slutförandedatum för en aktivitet.

![Visa datumskillnad](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och börja skriva &quot;Planerat slutförandedatum&quot; i fältet **Visa i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Lägg till kolumn** och börja skriva&quot;Faktiskt slutförandedatum&quot; i fältet **Visa i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Lägg till kolumn** och sedan på **Växla till textläge**.

1. Hovra över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Klicka på **Spara** och sedan på **Spara vy**.

## Beräkna tiden och datumskillnaden mellan fältet på ett objekt och ett annat fält på ett överordnat objekt

En lista över objekt och deras överordnade objekt finns i avsnittet Förstå det inbördes beroendet och objekthierarkin i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Du kan till exempel beräkna skillnaden mellan det planerade slutförandedatumet för en aktivitet och det planerade slutförandedatumet för den överordnade aktiviteten, eller för projektet som aktiviteten är på.

![Visa datumskillnad för planerat slutförande](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Gå till en lista med uppgifter.
1. Klicka på **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** och börja skriva &quot; Project Planned Completion Date&quot; eller &quot;Parent Completion Date&quot; i fältet **Show i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Lägg till kolumn** och börja skriva &quot;Planerat slutförandedatum&quot; i fältet **Visa i den här kolumnen** och markera den när den visas i listan.

1. Klicka på **Lägg till kolumn** och sedan på **Växla till textläge** > **Redigera textläge**.
1. Ta bort den text du söker i rutan **Redigera textläge** och ersätt den med någon av följande koder:

   * Så här visar du skillnaden mellan projektets planerade slutförandedatum och aktivitetens datum:

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * Så här visar du skillnaden mellan planerat slutförandedatum för den överordnade aktiviteten och aktivitetens datum:

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Klicka på **Klar** och sedan på **Spara vy**.
