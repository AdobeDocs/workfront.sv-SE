---
product-area: projects
navigation-topic: convert-issues
title: Bryt länken till problem från deras lösta objekt
description: När du skapar ett projekt eller en uppgift genom att konvertera en utgåva till projektet eller uppgiften kan du välja att behålla den ursprungliga utgåvan. Din Adobe Workfront-administratör måste aktivera den här inställningen för att du ska kunna använda det här alternativet när du konverterar utgåvan. Mer information om hur du konverterar problem till projekt och uppgifter finns i Översikt över hur du konverterar problem i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Bryt länken till problem från deras lösta objekt

När du skapar ett projekt eller en uppgift genom att konvertera en utgåva till projektet eller uppgiften kan du välja att behålla den ursprungliga utgåvan. Din Adobe Workfront-administratör måste aktivera den här inställningen för att du ska kunna använda det här alternativet när du konverterar utgåvan.\
Mer information om hur du konverterar problem till projekt och uppgifter finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

När du bestämmer dig för att behålla det problem som konverterades till projektet eller uppgiften är problemlösningen knuten till projektet eller uppgiften. Problemet blir ett objekt som kan lösas i projektet eller uppgiften. Projektet eller aktiviteten är problemlösarens objekt.

Du kan också manuellt länka ett problem till ett annat problem. Den andra utgåvan blir det upplösta objektet för den första utgåvan, i det här fallet.\
Mer information om hur du löser objekt finns i [Översikt över upplösta och upplösta objekt](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Det går inte att ändra utgivningsstatusen eftersom den ändras automatiskt med statusen för det upplösta objektet.

Du kan bryta länken mellan en problemlösning och en fråga i ett projekt, en uppgift eller ett ärende genom att ta bort projektet, uppgiften eller problemet.

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
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Visa åtkomst till aktiviteter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för problemet</p> <p>Visa behörigheter för aktiviteten eller projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Bryta länken för ett problem från ett projekt, en uppgift eller ett ärende

1. Gå till problemet som är länkat till ett projekt, en uppgift eller ett problem.
1. Klicka på **Ärendeinformation** -avsnitt.
1. Gå till **Översikt** området på **Ärendeinformation** -avsnitt.
1. I **Löst av** tar du bort den lösta objekttypen.\
   Ett problem kan lösas av ett projekt, en uppgift eller ett problem.

   Detta tar bort det matchande objektet från problemet.

1. Klicka **Spara** **Ändringar**.\
   Problemet är inte längre kopplat till ett projekt, en uppgift eller ett problem, och du kan nu lösa problemet separat.
