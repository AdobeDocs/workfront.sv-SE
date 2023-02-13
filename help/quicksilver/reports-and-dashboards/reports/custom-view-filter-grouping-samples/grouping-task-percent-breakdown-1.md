---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: aktivitetsprocentuell uppdelning 1'
description: 'I den här anpassade projektgrupperingen kan du visa projekt grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar ett procentvärde på 25 procentenheter i steg om: 0-25 %, 25-50 % osv.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# Gruppering: aktivitetsprocentuell uppdelning 1

I den här anpassade projektgrupperingen kan du visa projekt grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar ett procentvärde på 25 procentenheter i steg om: 0-25 %, 25-50 % osv. 

I följande gruppering ordnas uppgifter enligt värdet för Procent färdigt i sex olika grupperingar:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25_break_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Gruppera efter procentindelning för uppgift

Så här använder du den här grupperingen:

1. Gå till en lista med uppgifter.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Klicka **Växla till textläge**.
1. Ta bort texten i **Gruppera din rapport** område.
1. Ersätt texten med följande kod:

   <pre>group.0.linkedname=direct<br>group.0.name=Procent, uppdelning<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete} &lt;100,"75-99 %","100 %")))<br>group.0.valueformat=string</pre>

1. Klicka **Spara gruppering**.
