---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Tilldela arbete manuellt med hjälp av arbetsbelastningsutjämnaren
description: Du kan tilldela arbetsobjekt till användare manuellt med hjälp av Adobe Workfront Workload Balancer.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Tilldela arbete manuellt med hjälp av Utjämning av arbetsbelastning

Du kan tilldela arbetsobjekt till användare manuellt med hjälp av Adobe Workfront Workload Balancer.

Allmän information om hur du tilldelar arbete till användare med hjälp av arbetsbelastningsutjämnaren finns i [Översikt över hur du tilldelar arbete i belastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Contribute behörigheter eller högre till projekt, uppgifter och ärenden som innehåller Skapa uppdrag</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tilldela arbete manuellt i arbetsbelastningsutjämnaren

Du kan tilldela arbetsobjekt som ännu inte har tilldelats en användare eller tilldela om artiklar som har tilldelats användare i Utjämning för arbetsbelastning.

1. Gå till den arbetsbelastningsutjämnare där du vill tilldela arbete.

   Du kan tilldela användare arbete med hjälp av belastningsutjämnaren i resursområdet, i projektet eller på teamnivå. Mer information om var arbetsbelastningsutjämnaren finns i Workfront finns i [Hitta arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Valfritt) Gå till området **Ej tilldelat arbete** och använd ett filter för att visa uppgifter eller problem

   eller

   Gå till området **Tilldelad arbetsplats** och expandera namnet på en användare för att visa de arbetsobjekt som har tilldelats dem, om du vill tilldela om deras objekt.

1. Klicka på menyn **Mer** ![](assets/qs-more-menu.png) till vänster om namnet på ett arbetsobjekt och klicka sedan på **Tilldela det här till**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Du kan även använda följande kortkommandon för att tilldela uppgifter eller ärenden:
   >
   >* I Windows: CTRL-klicka på aktivitets- eller problemfältet.
   >* I Mac: CMD-klicka på aktivitets- eller problemfältet.

1. Gör något av följande:

   * Börja skriva namnet på en användare, en jobbroll eller ett team som du vill tilldela objektet i fältet **Sök efter personer, roller eller team**, markera det när det visas i listan och klicka sedan på **Spara**.

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
   > Om din Workfront- eller gruppadministratör har aktiverat delegeringar i din miljö använder du fliken Uppdrag för att tilldela användare till uppgiften eller problemet. Använd fliken Delegeringar för att visa användare som har delegerats till arbetsposten. Mer information om hur du delegerar arbete finns i [Delegera uppgifter och problem](../../manage-work/delegate-work/how-to-delegate-work.md).


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

   * Klicka på **Avancerat** för att komma åt avancerade tilldelningar.

     Mer information om hur du gör avancerade uppdrag finns i [Skapa avancerade uppdrag](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Valfritt) Klicka på ikonen **Visa allokeringar** ![](assets/show-allocations-icon-small.png) och sedan på menyn **Mer** ![](assets/qs-more-menu.png) > **Redigera allokeringar**.

   eller

   Dubbelklicka på en daglig eller veckovis allokering för att ändra den tid som användaren tilldelas arbetsuppgiften.

   Mer information om hur du ändrar användartilldelningar i arbetsbelastningsutjämnaren finns i avsnittet &quot;Ändra användartilldelningar&quot; i artikeln [Hantera användartilldelningar i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Mer information om hur du tar bort tilldelningar från ett arbetsobjekt med hjälp av arbetsbelastningsutjämnaren finns i [Ta bort tilldelning av arbete i arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
