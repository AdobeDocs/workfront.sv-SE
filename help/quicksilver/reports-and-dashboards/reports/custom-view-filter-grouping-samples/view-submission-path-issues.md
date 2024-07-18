---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: överföringssökväg för utgåvor'
description: Du kan visa den sökväg genom vilken ett problem har skickats in i en problemrapport. Sökvägen anger kön, ämnesgrupp och köämne där problemet ursprungligen skickades.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Visa: överföringssökväg för problem

Du kan visa den sökväg genom vilken ett problem har skickats in i en problemrapport. Sökvägen anger kön, ämnesgrupp och köämne där problemet ursprungligen skickades.

![issue_submit_path.png](assets/issue-submission-path-350x66.png)

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

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa överföringssökvägen för utgåvor

1. Gå till en lista med problem.
1. Välj **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** i området **Förhandsvisa kolumn**.

1. Klicka på den nya kolumnens rubrik och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du söker i rutan **Textläge** och ersätt den med följande kod:
   <pre>displayname= Issue Path<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valueField=displayQueueBreadcrumb <br>valueFormat=HTML<br></pre>

1. Klicka på **Spara vy**.
