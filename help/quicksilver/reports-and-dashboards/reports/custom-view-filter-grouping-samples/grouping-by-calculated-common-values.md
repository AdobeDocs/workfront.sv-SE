---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppera: ordna listresultat med ett beräknat värde som är gemensamt för alla objekt i grupperingen'
description: Du kanske vill visa dina uppgifter grupperade efter Procent färdigt i intervallet 0-25, 26-50, 51-75, 75-99 och 100. Du kan skapa en gruppering i textläge för att göra detta.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Gruppera: ordna listresultat med ett beräknat värde som är gemensamt för alla objekt i grupperingen

Du kanske vill visa dina uppgifter grupperade efter Procent färdigt i intervallet 0-25, 26-50, 51-75, 75-99 och 100. Du kan skapa en gruppering i textläge för att göra detta.

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

## Organisera listresultat med ett beräknat värde som är gemensamt för alla objekt i grupperingen

Så här använder du den här grupperingen i en lista över uppgifter:

1. Gå till en lista med uppgifter.
1. Välj **Ny gruppering** i listrutan **Gruppering**.

1. Klicka på **Växla till textläge**.
1. Lägg till följande kod i det tillgängliga utrymmet:

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. Klicka på **Klar** och sedan på **Spara gruppering**.
