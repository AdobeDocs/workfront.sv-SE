---
product-area: projects
navigation-topic: task-duration
title: Uppdatera planerade timmar och varaktighet för en aktivitet med enkel varaktighetstyp
description: Som standard beräknar Adobe Workfront varaktigheten för en aktivitet med en enkel varaktighetstyp baserat på antalet planerade timmar. Du kan också manuellt redigera mängden Planerade timmar och Längd för en enkel varaktighet-uppgift i vissa delar av Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Uppdatera planerade timmar och varaktighet för en aktivitet med enkel varaktighetstyp

Som standard beräknar Adobe Workfront varaktigheten för en aktivitet med en enkel varaktighetstyp baserat på antalet planerade timmar. Du kan också manuellt redigera mängden Planerade timmar och Längd för en enkel varaktighet-uppgift i vissa delar av Workfront.

Du kan antingen redigera Planerade timmar och Varaktighet för en uppgift med en enkel varaktighetstyp infogad eller på aktivitetsnivå i uppdragsområdet.

Mer information om redigering av information finns i [Redigera objekt i en lista i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

I den här artikeln beskrivs hur du kan uppdatera Planerade timmar och Varaktighet för en uppgift med en enkel varaktighetstyp på aktivitetsnivån i uppdragsområdet.

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
   <td> <p>Redigera åtkomst till uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgiften</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Uppdatera planerade timmar och varaktighet för en aktivitet med enkel varaktighetstyp

>[!IMPORTANT]
>
>När du har uppdaterat varaktigheten manuellt för en enkel varaktighetsåtgärd, slutar Workfront att beräkna den baserat på de planerade timmarna.

Så här redigerar du de planerade timmarna och varaktigheten för en aktivitet med en enkel varaktighetstyp i rutan Avancerade tilldelningar:

1. I en uppgiftslista klickar du på namnet på den uppgift som du vill ändra varaktighetstypen för.
1. Gör något av följande:

   * Klicka på ikonen **Mer** ![](assets/qs-more-icon-on-an-object.png) bredvid namnet på uppgiften, klicka på **Redigera** och sedan på **Uppdrag**.
   * Klicka på **Tilldelad till** eller namnet på tilldelningarna i uppdragsområdet i uppgiftshuvudet och klicka sedan på **Avancerat**.

1. Ange ett totalt värde för **Planerade timmar** för alla tilldelningar, till exempel 10 timmar. Det totala antalet planerade timmar fördelas jämnt mellan alla resurser som tilldelats aktiviteten.
1. (Valfritt) Justera manuellt de planerade timmarna för varje resurs som tilldelats till aktiviteten. Det totala antalet planerade timmar för aktivitetsuppdateringarna för att återspegla de nya timmarna som är individuellt tilldelade till dina resurser.
1. Ange ett värde för aktiviteten **Varaktighet**, till exempel 2 dagar.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicka på **Spara**.
