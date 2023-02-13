---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: användarjobbrollens procentandel av FTE-tillgänglighet'
description: Du kan lägga till en kolumn i vyn över en användarlista för att visa en lista över de jobbroller användaren är kopplad till samt procentandelen FTE-tillgänglighet för varje jobbroll, enligt definitionen i användarprofilen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Visa: procentuell andel av FTE-tillgänglighet för användarjobbroll

Du kan lägga till en kolumn i vyn över en användarlista för att visa en lista över de jobbroller användaren är kopplad till samt procentandelen FTE-tillgänglighet för varje jobbroll, enligt definitionen i användarprofilen.

Mer information om hur du definierar procentandelen FTE-tillgänglighet för användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_accessibility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## Visa användarjobbrollens procentandel av FTE-tillgänglighet

1. Gå till en lista med användare.
1. Från **Visa** nedrullningsbar meny, välja **Ny vy**.

1. I **Förhandsgranska kolumn** område, klicka **Lägg till kolumn**.

1. Klicka på den nya kolumnens rubrik och klicka sedan på **Växla till textläge**.
1. För musen över textlägesområdet och klicka **Klicka för att redigera text**.
1. Ta bort den text du hittar i **Textläge** och ersätt den med följande kod:

   <pre>displayName=Roles, tidsprocent<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueExpression=CONCAT({role},'-',{timePercentage},'%')<br>valueFormat=HTML</pre>

1. Klicka **Spara** sedan **Spara vy**.

1. (Valfritt) Ange ett namn för vyn och klicka sedan på **Spara vy**.
