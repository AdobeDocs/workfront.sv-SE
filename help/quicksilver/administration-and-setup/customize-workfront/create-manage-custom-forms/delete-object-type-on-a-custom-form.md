---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ta bort objekttyper i ett anpassat formulär
description: I ett befintligt anpassat formulär kan du ta bort objekttyper som är kopplade till formuläret. När du har gjort det kan användare inte längre bifoga formuläret till objekt av den typen.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Ta bort objekttyper i ett anpassat formulär

I ett befintligt anpassat formulär kan du ta bort objekttyper som är kopplade till formuläret. När du har gjort det kan användare inte längre bifoga formuläret till objekt av den typen.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Ta bort objekttyper i ett anpassat formulär

Du kan ta bort objekttyper från ett befintligt anpassat formulär.

Ett anpassat formulär måste ha minst en objekttyp.

>[!CAUTION]
>
>Om någon redan har kopplat det anpassade formuläret till objekt av den typ som du vill ta bort och lagt till data i det, tas dessa data bort permanent när du tar bort den objekttypen i formuläret. Det kan innehålla historisk information som användarna behöver senare.
>
>I allmänhet rekommenderar vi att du minimerar antalet gånger som du redigerar ett anpassat formulär som redan används. Det finns inget meddelandesystem för att varna personer som använder det anpassade formuläret om dina ändringar.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** till vänster.
1. Markera det anpassade formulär som du vill redigera och klicka sedan på **Redigera**.
1. Klicka på krysset på någon av **Objekttyper** som du vill ta bort från formuläret, och sedan klicka på **Ta bort** på det varningsmeddelande som visas.

   ![](assets/click-x-object-types.jpg)

1. (Valfritt) Upprepa föregående steg för andra objekttyper som du vill ta bort från formuläret.
1. Klicka **Klar** och sedan klicka **Stäng och spara**.
