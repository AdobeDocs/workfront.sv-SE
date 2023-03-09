---
title: Inaktivera eller återaktivera ett anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan återaktivera eller inaktivera ett anpassat formulär. Vi rekommenderar att du inaktiverar anpassade formulär i stället för att ta bort formulär som du inte längre använder för att bevara historiska data.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Inaktivera eller återaktivera ett anpassat formulär

Du kan återaktivera eller inaktivera ett anpassat formulär. Vi rekommenderar att du inaktiverar anpassade formulär i stället för att ta bort formulär som du inte längre använder för att bevara historiska data.

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
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Inaktivera ett anpassat formulär

Du kan inaktivera anpassade formulär som du inte längre använder utan att förlora tillhörande historiska data. Användare kan inte lägga till ett inaktivt anpassat formulär i objekt, men de kan fortfarande visa och lägga till data i fälten på objekt där det redan var bifogat.

Fält i ett inaktivt anpassat formulär kan även infogas i en vy. Om en användare lägger till ett fält från ett inaktivt anpassat formulär under en infogad redigering, bifogas formuläret automatiskt till objektet, även om det anpassade formuläret är inaktiverat.

Så här inaktiverar du ett anpassat formulär:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).
1. Välj **Anpassad Forms**.
1. På **Forms** markerar du det anpassade formulär som du vill inaktivera.
1. I kolumnen Är aktiv väljer du **Falskt** och klicka utanför kolumnen. Formuläret är inte längre aktivt.

## Återaktivera ett anpassat formulär

Om du återaktiverar ett anpassat formulär behåller det de tidigare inställningarna och användarna kan interagera med det som om det aldrig hade inaktiverats.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).
1. Välj **Anpassad Forms**.
1. På **Forms** markerar du det anpassade formulär som du vill återaktivera.
1. I kolumnen Är aktiv väljer du **True** och klicka utanför kolumnen. Formuläret är nu aktivt.