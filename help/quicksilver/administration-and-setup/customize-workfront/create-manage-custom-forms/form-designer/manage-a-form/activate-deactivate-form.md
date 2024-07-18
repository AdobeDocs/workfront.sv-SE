---
title: Inaktivera eller återaktivera ett anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan återaktivera eller inaktivera ett anpassat formulär. Vi rekommenderar att du inaktiverar anpassade formulär i stället för att ta bort formulär som du inte längre använder för att bevara historiska data.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Inaktivera eller återaktivera ett anpassat formulär

Du kan återaktivera eller inaktivera ett anpassat formulär. Vi rekommenderar att du inaktiverar anpassade formulär i stället för att ta bort formulär som du inte längre använder för att bevara historiska data.

>[!NOTE]
>
>Om ett anpassat formulär inaktiveras men fortfarande ingår i ett köämne eller en definition av en frågekö, bifogas det till nya begäranden. Om du inte vill att formuläret ska vara på begäran måste du ta bort det manuellt från kön.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p></td> 
  </tr>  
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Inaktivera ett anpassat formulär

Du kan inaktivera anpassade formulär som du inte längre använder utan att förlora tillhörande historiska data. Användare kan inte lägga till ett inaktivt anpassat formulär i objekt, men de kan fortfarande visa och lägga till data i fälten på objekt där det redan var bifogat.

Fält i ett inaktivt anpassat formulär kan även infogas i en vy. Om en användare lägger till ett fält från ett inaktivt anpassat formulär under en infogad redigering, bifogas formuläret automatiskt till objektet, även om det anpassade formuläret är inaktiverat.

Så här inaktiverar du ett anpassat formulär:

{{step-1-to-setup}}

1. Välj **Anpassad Forms** i den vänstra panelen.
1. I området **Forms** markerar du det anpassade formulär som du vill inaktivera.
1. I kolumnen Är aktiv väljer du **Falskt** och klickar ut ur kolumnen. Formuläret är inte längre aktivt.

## Återaktivera ett anpassat formulär

Om du återaktiverar ett anpassat formulär behåller det de tidigare inställningarna och användarna kan interagera med det som om det aldrig hade inaktiverats.

{{step-1-to-setup}}

1. Välj **Anpassad Forms** i den vänstra panelen.
1. Markera det anpassade formulär som du vill återaktivera i området **Forms**.
1. I kolumnen Är aktiv väljer du **True** och klickar utanför kolumnen. Formuläret är nu aktivt.
