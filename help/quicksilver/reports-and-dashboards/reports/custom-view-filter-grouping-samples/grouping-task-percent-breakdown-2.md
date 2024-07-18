---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppering: aktivitetsprocentuell uppdelning 2'
description: 'I den här anpassade uppgiftsgrupperingen kan du visa uppgifter grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar procentandelen komplett i steg om 10 procent: 1-10 %, 11-20 % osv.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Gruppering: aktivitetsprocentuell uppdelning 2

I den här anpassade uppgiftsgrupperingen kan du visa uppgifter grupperade efter ett intervall av deras procentvärden för slutförande. Uppdelningarna visar procentandelen komplett i steg om 10 procent: 1-10 %, 11-20 % osv.

I följande gruppering ordnas projekt efter procentvärdet färdigt i en av dessa grupperingar:

* 0 %
* 1-10 %
* 11-20 %
* 21-30 %
* 31-40 %
* 41-50 %
* 51-60 %
* 61-70 %
* 71-80 %
* 81-90 %
* 91-99 %
* 100 %

![task_10_break_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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
   <td> <p>Begäran om att ändra en gruppering </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en gruppering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
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
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Klicka på **Växla till textläge**.
1. Ta bort texten i området **Gruppera din rapport**.
1. Ersätt texten med följande kod:
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %" IF({percentComplete}&lt;=31,"21-30 %",IF({percentComplete}&lt;41,"31-40 %",IF({percentComplete}&lt;51,"41-50 %",IF({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71,"6 1-70 %",IF({percentComplete}&lt;81,"71-80 %",IF({percentComplete}&lt;91,"81-90 %",IF({percentComplete}&lt;100,"91-99 %","100 %"))))<br>) textmode=true</pre>

1. Klicka på **Spara gruppering**.
