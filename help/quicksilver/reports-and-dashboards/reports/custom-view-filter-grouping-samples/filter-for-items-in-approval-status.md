---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa endast objekt med godkännandestatus'
description: Du kan bara visa objekt med en viss status som är under Väntar på godkännande. Detta fungerar på samma sätt för alla andra objekt med godkännandestatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Filter: visa endast objekt med godkännandestatus

Du kan bara visa objekt med en viss status som är under Väntar på godkännande. Detta fungerar på samma sätt för alla andra objekt med godkännandestatus.

Du kan placera följande objekt i en godkännandestatus:

* Uppgifter
* Problem
* Projekt

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

## Visa endast objekt med godkännandestatus

1. Gå till det filter som du vill anpassa, t.ex. för en lista med projekt.
1. Klicka på **Lägg till en filterregel** för fältet **Status** för objektet i listan.\
   I en projektrapport lägger du till exempel till **Status som är lika med planering** om du bara vill visa projekt som har statusen **Planering - Väntar på godkännande**.

1. Klicka på **Växla till textläge**.
1. Ändra

   ```
   status
   ```

   rad genom att lägga till **:A** i statusens nyckel med tre bokstäver:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Klicka på **Klar** och sedan på **Spara filter**.

   I listan visas endast projekt som har statusen Planering - Väntar på godkännande.
