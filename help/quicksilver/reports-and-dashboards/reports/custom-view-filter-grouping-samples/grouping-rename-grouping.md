---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Gruppering: redigera visningsnamnet i en gruppering'
description: Du kan byta namn på grupperingar till något som är mer bekant för användarna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Gruppering: redigera visningsnamnet i en gruppering

Du kan byta namn på grupperingar till något som är mer bekant för användarna.

Om du t.ex. använder standardgrupperingen Portfolio namn i en lista med projekt visas grupperingens namn som *Portfolio: Namn:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Du kan ändra den här grupperingen i textläge om du vill visa ett namn som är enklare att läsa.

![](assets/grouping-edited-name-350x160.png)

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

## Redigera visningsnamnet i en gruppering

Så här ändrar du visningsnamnet i en projektgruppering:

1. Gå till en lista med projekt.
1. Från **Gruppering** nedrullningsbar meny, välja **Ny gruppering**.

1. Klicka **Lägg till gruppering** och börja skriva &quot;Portfolio Name&quot; i dialogrutan **Först av:** markerar du det när det visas i listan.

1. Klicka **Växla till textläge**.
1. Gör något av följande:

   * Lägg till följande kod i den befintliga texten i **Gruppera din rapport** box:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      Eller i det här fallet:

      ```
      group.0.displayname=Portfolio
      ```

   * Ta bort alla rader i grupperingens textlägesgränssnitt som innehåller ordet &quot;name&quot; och lägg sedan till raden:

      ```
      group.0.name=Your Value
      ```

      Eller i det här fallet:

      ```
      group.0.name=Portfolio
      ```

      Du kan också lämna

      ```
      group.0.name
      ```

      en tom rad, i vilket fall grupperingen visar namnet på värdet som du grupperar efter.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Klicka **Klar** sedan **Spara gruppering**.
