---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Tilldela arbete manuellt med hjälp av Utjämning av arbetsbelastning
description: Du kan tilldela arbetsobjekt till användare manuellt med hjälp av Adobe Workfront Workload Balancer.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Tilldela arbete manuellt med hjälp av Utjämning av arbetsbelastning

Du kan tilldela arbetsobjekt till användare manuellt med hjälp av Adobe Workfront Workload Balancer.

Allmän information om hur du tilldelar arbete till användare med hjälp av Utjämning av arbetsbelastning finns i [Översikt över tilldelning av arbete i belastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td> <p>Planera, när du använder arbetsbelastningsutjämnaren i resursområdet</p>
   <p>Arbeta, när du använder belastningsutjämnaren för ett team eller projekt</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till följande:</p> 
    <ul> 
     <li> <p>Resurshantering</p> </li> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Uppgifter</p> </li> 
     <li> <p>Problem</p> </li> 
    </ul> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre för projekt, uppgifter och ärenden som innehåller Skapa uppdrag</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Tilldela arbete manuellt i arbetsbelastningsutjämnaren

Du kan tilldela arbetsobjekt som ännu inte har tilldelats en användare eller tilldela om artiklar som har tilldelats användare i Utjämning för arbetsbelastning.

1. Gå till den arbetsbelastningsutjämnare där du vill tilldela arbete.

   Du kan tilldela användare arbete med hjälp av belastningsutjämnaren i resursområdet, i projektet eller på teamnivå. Mer information om var arbetsbelastningsutjämnaren finns i Workfront finns i [Leta reda på arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Valfritt) Gå till **Ej tilldelat arbete** och använda ett filter för att visa uppgifter eller problem

   eller

   Gå till **Tilldelat arbete** och expandera namnet på en användare för att visa arbetsobjekten som tilldelats dem, om du vill tilldela om deras poster.

1. Klicka på **Menyn Mer** ![](assets/qs-more-menu.png) till vänster om namnet på en arbetsuppgift och klicka sedan på **Tilldela detta till**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Du kan även använda följande kortkommandon för att tilldela uppgifter eller ärenden:
   >
   >* I Windows: CTRL-klicka på aktivitets- eller problemfältet.
   >* I Mac: CMD-klicka på aktivitets- eller problemfältet.

1. Gör något av följande:

   * Börja skriva namnet på en användare, en jobbroll eller ett team som du vill tilldela objektet i **Sök efter personer, roller eller team** markerar du det när det visas i listan och klickar sedan på **Spara**.

   >[!TIP]
   >
   >När du lägger till en användare ska du lägga märke till avataren, användarens primära roll och användarens e-postadress för att skilja mellan användare med identiska namn.
   >
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
   >
   > Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Om din Workfront- eller gruppadministratör har aktiverat delegeringar i din miljö använder du fliken Uppdrag för att tilldela användare till uppgiften eller problemet. Använd fliken Delegeringar för att visa användare som har delegerats till arbetsposten. Mer information om att delegera arbete finns i [Hantera delegering av uppgifter och utgåvor](../../manage-work/delegate-work/how-to-delegate-work.md).


   Detta tilldelar eller omtilldelar arbetsuppgiften till de angivna tilldelningarna.

   Om du tilldelar ett objekt till endast ett team eller en jobbroll visas objektet endast i området Ej tilldelat arbete. Du måste tilldela arbetsobjekt till användare för att kunna visa dem i området Tilldelad arbetsyta i Utjämning för arbetsbelastning.

   >[!TIP]
   >
   >Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
   >
   >
   >Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
   >
   >   
   >   
   >   * Tilldela om arbetsuppgiften till aktiva resurser.
   >   * Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.
   >   
   >

   * Klicka **Avancerat** för att få åtkomst till avancerade uppdrag.

     Mer information om avancerade uppdrag finns i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Valfritt) Klicka på **Ikonen Visa allokeringar** ![](assets/show-allocations-icon-small.png)och klickar sedan på **Menyn Mer** ![](assets/qs-more-menu.png) > **Redigera allokeringar**.

   eller

   Dubbelklicka på en daglig eller veckovis allokering för att ändra den tid som användaren tilldelas arbetsuppgiften.

   Mer information om hur du ändrar användartilldelningar i Utjämning av arbetsbelastning finns i avsnittet Ändra användartilldelningar i artikeln [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Mer information om hur du tar bort tilldelningar från ett arbetsobjekt med hjälp av arbetsbelastningsutjämnaren finns i [Ta bort tilldelning av arbete i belastningsutjämnaren](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
