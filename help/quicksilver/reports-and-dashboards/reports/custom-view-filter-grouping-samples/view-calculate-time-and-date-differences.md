---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: beräkna tid- och datumskillnader'
description: Du kan beräkna skillnaden mellan följande - REDIGERA ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Visa: beräkna tid- och datumskillnader

>[!IMPORTANT]
>
>Du kan inte beräkna tid- och datumskillnaden i Adobe Workfront mellan två olika objekt av samma typ. Du kan t.ex. inte beräkna tid- och datumskillnaden mellan två datum i två olika projekt, aktiviteter eller utgåvor.

Du kan beräkna skillnaden mellan följande:

* Tid- och datumskillnaden mellan två datumfält i samma objekt
* Tid- och datumskillnaden mellan fältet i ett objekt och ett annat fält i det överordnade objektet

>[!TIP]
>
>Dessa beräkningar visar antalet dagar mellan de två datumen. Resultatet visas i dagar. Tidsstämpeln i datumfältet beaktas också, och antalet dagar kan följas av decimaler om tidsstämpeln inte matchar. Om aktiviteten slutfördes sent visas antalet dagar som ett negativt värde.

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Beräkna tiden och datumskillnaden mellan två datumfält i samma objekt

Du kan till exempel beräkna skillnaden mellan Planerat slutförandedatum och Faktiskt slutförandedatum för en aktivitet.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** och börja skriva &quot;Planerat slutförandedatum&quot; i dialogrutan **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Lägg till kolumn** och börja skriva &quot;Faktiskt slutförandedatum&quot; i dialogrutan **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Lägg till kolumn** och sedan klicka **Växla till textläge**.

1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Klicka **Spara** sedan **Spara vy**.

## Beräkna tiden och datumskillnaden mellan fältet på ett objekt och ett annat fält på ett överordnat objekt

En lista över objekt och deras överordnade objekt finns i avsnittet Förstå det inbördes beroendet och objekthierarkin i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Du kan till exempel beräkna skillnaden mellan det planerade slutförandedatumet för en aktivitet och det planerade slutförandedatumet för den överordnade aktiviteten, eller för projektet som aktiviteten är på.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** och börja skriva &quot; Project Planned Completion Date&quot; eller &quot;Parent Completion Date&quot; i **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Lägg till kolumn** och börja skriva &quot;Planerat slutförandedatum&quot; i dialogrutan **Visa i den här kolumnen** markerar du det när det visas i listan.

1. Klicka **Lägg till kolumn** och sedan klicka **Växla till textläge**.

1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med någon av följande koder:

   * Så här visar du skillnaden mellan projektets planerade slutförandedatum och aktivitetens datum:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Så här visar du skillnaden mellan planerat slutförandedatum för den överordnade aktiviteten och aktivitetens datum:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Klicka **Spara** sedan **Spara vy**.
