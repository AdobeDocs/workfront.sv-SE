---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Ta bort tilldelning av arbete i arbetsbelastningsutjämnaren
description: Du kan ta bort tilldelning av användare från arbetsobjekt på arbetsytan Tilldelad arbetsyta i Adobe Workfront Workload Balancer eller tilldela om dem till andra användare, roller eller team.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Ta bort tilldelning av arbete i belastningsutjämnaren

Du kan ta bort tilldelning av användare från arbetsobjekt på arbetsytan Tilldelad arbetsyta i Adobe Workfront Workload Balancer eller tilldela om dem till andra användare, roller eller team.

Du kan ta bort användartilldelningar från arbetsobjekt manuellt, genom att dra och släppa eller gruppvis. I den här artikeln beskrivs hur du tar bort användartilldelningar manuellt.

Mer information om hur du frigör användare genom att dra och släppa finns i [Tilldela arbete i belastningsutjämnaren genom att dra och släppa](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Mer information om att frigöra flera användare samtidigt finns i [Tilldela flera användare samtidigt med hjälp av belastningsutjämnaren för arbetsbelastning](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera när du använder belastningsutjämnaren för arbetsbelastning i resursområdet:</br>
       Arbeta, när du använder belastningsutjämnaren för ett team eller projekt</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till följande:</p> 
    <ul> 
     <li>Resurshantering</li> 
     <li>Projekt</li> 
     <li>Uppgifter</li> 
     <li>Problem</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden som innehåller Skapa uppdrag</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort tilldelning av arbetsobjekt i arbetsbelastningsutjämnaren

Du kan antingen ta bort tilldelning från användare och flytta dem till arbetsytan Ej tilldelad eller tilldela om dem till andra användare.

Så här tar du bort tilldelning av arbetsobjekt från användare:

1. Gå till området **Tilldelat arbete** i Utjämning av arbetsbelastning och expandera en användare.
1. Gör något av följande:

   * Hitta det objekt som du vill ta bort tilldelning för i en användares område, klicka på det och dra och släpp det i området Ej tilldelat eller i en annan användares område.
   * Klicka på ikonen **Mer** ![Mer ](assets/more-icon-task-list.png) till höger om namnet på ett arbetsobjekt, klicka på **Tilldela det här till**, ta bort namnet på enheterna som tilldelats arbetsobjektet eller ange ett annat namn och klicka sedan på **Spara**.

     ![Tilldela detta till](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   Objektet visas i området Ej tilldelat arbete om det matchar filtervillkoren för det området och inte har tilldelats någon annan användare, eller om det har tilldelats en annan användare i användarområdet.

   Mer information om filtrering av information i arbetsbelastningsutjämnaren finns i [Filtrera information i Arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
