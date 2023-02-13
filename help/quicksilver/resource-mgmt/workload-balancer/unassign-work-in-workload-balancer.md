---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Ta bort tilldelning av arbete i belastningsutjämnaren
description: Du kan ta bort tilldelning av användare från arbetsobjekt på arbetsytan Tilldelad arbetsyta i Adobe Workfront Workload Balancer eller tilldela om dem till andra användare, roller eller team.
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Ta bort tilldelning av arbete i belastningsutjämnaren

Du kan ta bort tilldelning av användare från arbetsobjekt på arbetsytan Tilldelad arbetsyta i Adobe Workfront Workload Balancer eller tilldela om dem till andra användare, roller eller team.

Du kan ta bort användartilldelningar från arbetsobjekt manuellt, genom att dra och släppa eller gruppvis. I den här artikeln beskrivs hur du tar bort användartilldelningar manuellt.

Mer information om hur du frigör användare genom att dra och släppa finns i [Tilldela arbete i belastningsutjämnaren genom att dra och släppa](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Mer information om att ta bort flera användare samtidigt finns i [Tilldela flera arbeten med hjälp av belastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera, när du använder belastningsutjämnaren för ett team eller i resursområdet </p>
   <p>Arbeta, när du använder belastningsutjämnaren för ett projekt </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till följande:</p> 
    <ul> 
     <li> <p>Resurshantering</p> </li> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Uppgifter</p> </li> 
     <li> <p>Problem</p> </li> 
    </ul> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden som innehåller Skapa uppdrag</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

 

## Ta bort tilldelning av arbetsobjekt i arbetsbelastningsutjämnaren

Du kan antingen ta bort tilldelning från användare och flytta dem till arbetsytan Ej tilldelad eller tilldela om dem till andra användare.

Så här tar du bort tilldelning av arbetsobjekt från användare:

1. Gå till **Tilldelat arbete** och utöka en användare.
1. Gör något av följande:

   * Hitta det objekt som du vill ta bort tilldelning för i en användares område, klicka på det och dra och släpp det i området Ej tilldelat eller i en annan användares område.
   * Klicka på **Mer** icon ![](assets/more-icon-task-list.png) till höger om namnet på en arbetsuppgift klickar du på **Tilldela detta till** tar du sedan bort namnet på enheterna som tilldelats arbetsuppgiften eller anger ett annat namn och klickar på **Spara**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   Objektet visas i området Ej tilldelat arbete om det matchar filtervillkoren för det området och inte har tilldelats någon annan användare, eller om det har tilldelats en annan användare i användarområdet.

   Mer information om filtrering av information i Utjämning av arbetsbelastning finns i [Filtrera information i Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
