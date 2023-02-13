---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ta bort eller inaktivera ett anpassat formulär
description: Du kan ta bort eller inaktivera ett anpassat formulär från systemet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Ta bort eller inaktivera ett anpassat formulär

Du kan ta bort eller inaktivera ett anpassat formulär från systemet.

>[!CAUTION]
>
>Om du tar bort ett anpassat formulär tas även alla anpassade data bort från objekten som är kopplade till formuläret. Det går inte att återställa borttagna data. Överväg att inaktivera ett anpassat formulär i stället. När du inaktiverar ett anpassat formulär som du inte längre använder behåller du alla tillhörande historiska data.

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
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Ta bort ett anpassat formulär

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms.**
1. Markera det anpassade formuläret och klicka sedan på **Ta bort**.
1. Om du är säker på att du permanent vill ta bort det anpassade formuläret och alla tillhörande data på objekt där det bifogades, klickar du på **Ja, ta bort den**.

## Inaktivera ett anpassat formulär

Du kan inaktivera anpassade formulär som du inte längre använder utan att förlora tillhörande historiska data. Användare kan inte lägga till ett inaktivt anpassat formulär i objekt, men de kan fortfarande visa och lägga till data i fälten på objekt där det redan var bifogat.

Fält i ett inaktivt anpassat formulär kan även infogas i en vy. Om en användare lägger till ett fält från ett inaktivt anpassat formulär under en infogad redigering, bifogas formuläret automatiskt till objektet, även om det anpassade formuläret är inaktiverat.

Om du återaktiverar ett anpassat formulär behålls inställningarna som det hade tidigare och användarna kan interagera med det som om det aldrig hade inaktiverats.

Så här inaktiverar du ett anpassat formulär:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på namnet på det anpassade formulär som du vill inaktivera.
1. Klicka på **Formulärinställningar** -fliken.
1. Inaktivera **Är aktiv** alternativ.
1. Klicka **Spara + Stäng**.
