---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: visa namnet på överordnade uppgifter som versaler'
description: Du kan lägga till den här kolumnen i en uppgiftsvy om du vill visa namnet på den överordnade uppgiften med versaler.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Visa: visa namnet på överordnade uppgifter som versaler

Du kan lägga till den här kolumnen i en uppgiftsvy om du vill visa namnet på den överordnade uppgiften med versaler.

![](assets/column-task-with-all-caps-parent-350x112.png)

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

## Visa namnet på den överordnade aktiviteten som versaler

Så här skapar du den här kolumnen i en uppgiftsvy:

1. Gå till en lista med uppgifter.
1. Från **Visa** nedrullningsbar meny, välja **Anpassa vy**.\
   eller\
   Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. I **Förhandsgranska kolumn** klickar du på rubriken för den kolumn som visar aktivitetsnamnet i listan.
1. Klicka **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod: <pre>descriptionkey=name<br>displayName=Aktivitetsnamn<br>textmode=true<br>valueExpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueFormat=HTML<br>width=150<br></pre>

1. Klicka **Spara vy**.
