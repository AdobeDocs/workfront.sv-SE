---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa ofullständiga efterföljare mellan projekt'
description: Aktivitetsfiltret returnerar ofullständiga projektövergripande efterföljande.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Filter: visa ofullständiga projektövergripande efterföljande

Aktivitetsfiltret returnerar ofullständiga projektövergripande efterföljande.

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
   <td> <p>Begäran om att ändra ett filter </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Filtrera efterföljande projekt

Så här använder du det här filtret:

1. Gå till en lista med uppgifter.
1. Välj **Nytt filter** i listrutan **Filter**.

1. Klicka på **Växla till textläge**.
1. Klistra in följande kod i området **Ange filterregler för rapporten**:
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>efterföljandeMM:projectID=FIELD:projectID<br>efterföljandeMM:projectID_Mod=ne</pre>

1. Klicka på **Spara filter**.
