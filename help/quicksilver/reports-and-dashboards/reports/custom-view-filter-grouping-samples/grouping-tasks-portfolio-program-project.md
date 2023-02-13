---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: uppgifter per portfölj, program och projekt'
description: Använd den här uppgiftsgrupperingen för att gruppera uppgifter efter portföljen, efter program och sedan efter det projekt de är kopplade till.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Gruppering: uppgifter per portfölj, program och projekt

Använd den här uppgiftsgrupperingen för att gruppera uppgifter efter portföljen, efter program och sedan efter det projekt de är kopplade till.

![](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Gruppera uppgifter efter portfölj, program och projekt

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Klicka **Växla till textläge**.
1. Ta bort texten i **Gruppera din rapport** område.
1. Ersätt texten med följande kod:

   <pre>group.0.linkedname=project<br>group.0.namekey=portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valuefield=project:program:name<br>group.1.valueformat=string<br>group.2.name=Project<br>group.2.valuefield=project:name<br>group.2.valueformat=HTML<br>textmode=true<br></pre>

1. Klicka **Spara gruppering**.
