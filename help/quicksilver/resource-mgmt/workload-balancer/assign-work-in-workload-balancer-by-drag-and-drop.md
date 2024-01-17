---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Tilldela arbete i belastningsutjämnaren genom att dra och släppa
description: Du kan tilldela arbetsobjekt med Adobe Workfront Workload Balancer genom att dra och släppa arbetsobjekt till rätt användare.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Tilldela arbete i belastningsutjämnaren genom att dra och släppa

<!--remove production and preview preferences at release-->

Du kan tilldela arbetsobjekt med Adobe Workfront Workload Balancer genom att dra och släppa arbetsobjekt till rätt användare.

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
   <td> <p>Planera, om du vill tilldela arbete i arbetsbelastningsutjämnaren i resursområdet</p>
   <p>Arbeta, för att tilldela arbete i belastningsutjämnaren för ett team eller projekt</p>
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

## Tilldela ett objekt genom att dra och släppa

Du kan tilldela en artikel från området Ej tilldelat arbete till en användare, eller så kan du tilldela om en redan tilldelad artikel till en annan användare i området Tilldelad arbetsyta.

1. Gå till den arbetsbelastningsutjämnare där du vill tilldela arbete.

   Du kan tilldela användare arbete med hjälp av belastningsutjämnaren i resursområdet, i projektet eller på teamnivå. Mer information om var arbetsbelastningsutjämnaren finns i Workfront finns i [Leta reda på arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Valfritt) Gå till **Ej tilldelat arbete** och använda ett filter för att visa uppgifter och ärenden som inte tilldelats användare

   eller

   Gå till **Tilldelat arbete** och expandera namnet på en användare för att visa arbetsobjekten som tilldelats dem, om du vill tilldela om deras poster.

1. (Villkorligt) Klicka på knappen **Visa alla användare** icon ![](assets/show-all-users-icon-project-workload-balancer.png) för att visa alla Workfront-användare.

   Detta visar alla användare som du har åtkomst till för att visa.

   De användare som också är en del av projektteamet och redan är tilldelade till objekt i projektet har en projektikon till höger om sitt namn på den tilldelade arbetsytan.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* Alternativet Visa alla användare är bara tillgängligt i arbetsbelastningsutjämnaren för ett projekt.
   >* Använd filter om du bara vill visa de användare som är viktiga för dig. Använd till exempel ett filter om du bara vill visa användare från dina team eller grupper.



1. Klicka på fältet för en arbetsuppgift som anger den planerade eller den planerade tidslinjen och dra den över namnet på en användare i **Tilldelad** område.

   Användaren som du för pekaren över för att släppa arbetsobjektet markeras.

   >[!TIP]
   >
   >De planerade timmarna för den användare som du hovrar över uppdateras i realtid med antalet planerade timmar per dag från arbetsuppgiften, för att visa vilken effekt det kan ha om ett nytt objekt läggs till i den totala allokeringen.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. När du är klar släpper du den valda arbetsposten på samma rad som användarens namn i det tilldelade området. Artikeln tilldelas och de tilldelade planerade timmarna uppdateras för användaren med de nya timmarna från arbetsuppgiften.

   Om artikeln har tilldelats en jobbroll som användaren inte kan fylla, visas objektet under användarens namn i området Tilldelad arbetsyta och det finns även kvar i området Ej tilldelat arbete för att ange att den jobbroll som är associerad med den ännu inte har ersatts av en användare.

   >[!TIP]
   >
   >* Om du har aktiverat Gruppera efter projekt i området Inställningar visas den tilldelade uppgiften under motsvarande projekt. Om inställningen är inaktiverad visas den tilldelade uppgiften i användarområdet.
   >
   >
   >     Objektet visas enligt kriterierna för belastningsutjämnare för arbetsbelastning för sortering av arbetsobjekt. Mer information finns i [Navigera till arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Om du har aktiverat Visa alla användare i belastningsutjämnaren för ett projekt och tilldelade objekt till användare som inte tidigare har tilldelats till objekt i projektet, läggs användarna till i projektgruppen. Mer information finns i [Hantera projektteam](../../manage-work/projects/planning-a-project/manage-project-team.md).


1. (Valfritt) Klicka på fältet för ett arbetsobjekt under namnet på en användare i området Tilldelat arbete och dra det sedan över området Ej tilldelat arbete för att ta bort tilldelningen. Artikeln har inte tilldelats från användaren, men den kan fortfarande tilldelas en jobbroll. I så fall visas den i området Ej tilldelat arbete. Om objektet är tilldelat en annan användare finns det kvar i området Tilldelad arbetsyta under namnet på den användare som fortfarande är tilldelad.
1. (Valfritt) Klicka på **Ikonen Visa allokeringar** ![](assets/show-allocations-icon-small.png)och klickar sedan på **Menyn Mer** ![](assets/qs-more-menu.png) > **Redigera allokeringar**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   eller

   Dubbelklicka på en daglig eller veckovis allokering för att ändra den tid som användaren tilldelas arbetsuppgiften.

   Mer information om hur du ändrar användartilldelningar i Utjämning av arbetsbelastning finns i avsnittet Ändra användartilldelningar i artikeln [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Mer information om hur du tar bort tilldelningar från ett arbetsobjekt med hjälp av arbetsbelastningsutjämnaren finns i [Ta bort tilldelning av arbete i belastningsutjämnaren](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

