---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visa: Procentandel av tillgängligheten för heltidsekvivalenter för användare"
description: Du kan lägga till en kolumn i vyn för en användarlista för att visa en lista över de jobbroller som användaren är associerad med samt procentandelen FTE som är tillgänglig för varje jobbroll, enligt definitionen i användarprofilen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Visa: användarroll i procent av FTE-tillgänglighet

Du kan lägga till en kolumn i vyn över en användarlista för att visa en lista över de jobbroller användaren är kopplad till samt procentandelen FTE-tillgänglighet för varje jobbroll, enligt definitionen i användarprofilen.

Mer information om hur du definierar procentandelen FTE-tillgänglighet för användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Krav för åtkomst

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Någon</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licens för Adobe Workfront*</td> 
   <td> <p>Begära att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>NOT</b>

Om du fortfarande inte har åtkomst kan du fråga Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Behörigheter för objekt</td> 
   <td> <p>Hantera behörigheter till en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilket abonnemang, vilken licenstyp eller vilken åtkomst du har kontaktar du Workfront-administratören.

## Visa procentandel för användarjobbroll för FTE-tillgänglighet

1. Gå till en lista över användare.
1. Välj **Ny vy** i listrutan **Visa**.

1. Klicka på **Lägg till kolumn** i området **Förhandsvisa kolumn**.

1. Klicka på rubriken för den nya kolumnen och klicka sedan på **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka på **Klicka för att redigera text**.
1. Ta bort texten som du hittar i **rutan Textläge** och ersätt den med följande kod:
   <pre>displayname=Roller Tid Procent<br>listDelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Klicka på Spara **och sedan** på **Spara vy**.

1. (Valfritt) Ange ett namn för vyn och klicka sedan på **Spara vy**.
