---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Tilldela arbete gruppvis med hjälp av arbetsbelastningsutjämnaren
description: Du kan tilldela resurser till flera uppgifter och flera problem samtidigt med Adobe Workfront Workload Balancer.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---

# Tilldela flera arbeten med hjälp av belastningsutjämnaren

<!--Audited: 07/2024-->

Du kan tilldela resurser till flera uppgifter och flera problem samtidigt med Adobe Workfront Workload Balancer.

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

## Att tänka på när du gör masstilldelningar i arbetsbelastningsutjämnaren

* Du kan snabbt hantera användartilldelningar för flera uppgifter och problem i ett eller flera projekt. Ändringar i tilldelningar visas omedelbart i Utjämning av arbetsbelastning.
* Du kan inte tilldela resurser till arbetsobjekt som är slutförda eller till objekt i ett slutfört projekt.
* Du kan göra följande när du tilldelar flera användare samtidigt:

   * Tilldela en användare till alla arbetsobjekt som för närvarande är tilldelade till en jobbroll.
   * Ersätt användartilldelningar mellan användare.
   * Ta bort tilldelningen för en användare från alla arbetsobjekt.

**EXEMPEL**

* Du ansvarar för att göra användartilldelningar i flera nya projekt. Projekten skapades ursprungligen från mallar och jobbroller är redan tilldelade till de olika aktiviteterna i projekten. Du vill tilldela en specifik användare, Jackie Simms, till alla uppgifter som för närvarande är tilldelade till en jobbroll. Du kan använda funktionen Tilldela för att tilldela dessa uppgifter till Jackie Simms.
* 45 uppgifter i tre olika projekt tilldelas Jackie Simms. Jackie lämnar organisationen och nu måste du omfördela hennes uppgifter till en annan användare. Du kan använda funktionen Ersätt för att tilldela dessa uppgifter till den nya personen.
* Tio uppgifter i två olika projekt tilldelas en annan användare, Rick Kuvec. Du inser att Rick tilldelades dessa uppgifter av misstag, men du vet inte vem de behöver tilldelas just nu. Du måste frigöra Rick för alla uppgifter samtidigt. Du kan använda funktionen Ta bort tilldelning för att ta bort Rick från dessa uppgifter.

## Tilldela flera arbeten samtidigt i belastningsutjämnaren

1. Gå till den arbetsbelastningsutjämnare där du vill tilldela arbete.

   Du kan tilldela användare arbete med hjälp av belastningsutjämnaren i resursområdet, i projektet eller på teamnivå. Mer information om var arbetsbelastningsutjämnaren finns i Workfront finns i [Hitta arbetsbelastningsutjämnaren](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Klicka på **Masstilldelningar** ![](assets/bulk-assignments-wb.png) överst i arbetsbelastningsutjämnaren.

   Panelen Grupptilldelning öppnas till höger om Utjämning av arbetsbelastning.

1. (Villkorligt) Om du använder Utjämning av arbetsbelastning från området Resurser eller för ett team expanderar du listrutan **Projekt: Namn** och använder filtermodifierarna för att välja det eller de projekt som du vill göra tilldelningar för. Du kan välja projekt efter namn (det här är standardalternativet) eller efter status.

   Mer information om Workfront filtermodifierare finns i [Filter och villkorsmodifierare](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Projektnamnet är markerat som standard när du öppnar arbetsbelastningsutjämnaren för ett projekt.

   ![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Valfritt) Klicka på **Välj projektuppgifter** för att välja den eller de uppgifter som du vill tilldela till. Välj sedan aktiviteter efter namn (standardalternativet) eller Status i listrutan **Aktivitet: Namn** och använd filtermodifierarna för att söka efter specifika uppgifter.

   Mer information om Workfront filtermodifierare finns i [Filter och villkorsmodifierare](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Du kan inte välja uppgifter med statusen Slutför.

   ![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >Lämna det här valet tomt om du vill göra grupptilldelningar för både ärenden och uppgifter.

1. (Valfritt) Klicka på ikonen **Ta bort** ![](assets/delete.png) bredvid ett av de valda villkoren

   eller

   Klicka på **Radera alla** i det övre högra hörnet av panelen Gruppera uppdrag om du vill ta bort alla markeringar.

1. Välj något av följande alternativ och fortsätt med stegen som beskrivs nedan:

   * [Tilldela användare](#assign-user)
   * [Ersätt användare](#replace-user)
   * [Ta bort användartilldelning](#unassign-user)

   >[!TIP]
   >
   >Om inga objekt matchar de valda filtren är dessa alternativ nedtonade.

### Tilldela användare {#assign-user}

När du tilldelar en användare med grupptilldelningar i arbetsbelastningsutjämnaren händer följande:

* En användare tilldelas till alla arbetsobjekt som för närvarande är tilldelade till en viss roll i de valda projekten.
* Användaren har inte tilldelats följande typer av arbetsobjekt:

   * Objekt som redan har tilldelats en användare.
   * Slutförda objekt.

* Om användaren du valde inte är associerad med den angivna rollen ersätts rollen av användaren i användarens primära roll.

Så här tilldelar du en användare till arbetsuppgifter som tidigare tilldelats till jobbroller:

1. Börja tilldela arbetsobjekt med grupptilldelningar i arbetsbelastningsutjämnaren enligt beskrivningen ovan och välj **Tilldela**.

1. Klicka på listrutepilen i fältet **Rolltilldelning** och välj en roll i en lista. Endast roller som för närvarande är tilldelade i de angivna projekten visas. Detta är ett obligatoriskt fält.

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. Klicka på listrutepilen i fältet **Användare som ska tilldelas** för att välja från en lista med föreslagna användare eller för att ange en annan användares namn.

   Välj användare bland följande områden:

   * **Föreslagna tilldelningar**: Användare som kan utföra den valda rollen och som matchar villkoren för smarta tilldelningar. Mer information finns i [Översikt över smarta uppdrag](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Andra tilldelningar**: Alla användare i systemet som kan utföra den valda rollen.

     >[!TIP]
     >
     >Endast de första 50 användarna visas i området Andra uppdrag.


   När du har valt en användare visas en anteckning i Workfront om hur många objekt den angivna användaren ska tilldelas och vilken jobbroll de ska ersätta.

   >[!TIP]
   >
   >Alla roller för användaren visas i listan, under användarens namn.


1. Klicka på **Tilldela**.

   De angivna rollerna ersätts med de användare som du har valt.

   Du får en bekräftelse på hur många arbetsobjekt som har ersatts med den valda rollen.

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Ersätt användare {#replace-user}

Du kan ersätta en användare som redan är tilldelad att arbeta med artiklar med en annan användare i de markerade projekten.

När du ersätter en användare med en annan användare med grupptilldelningar i arbetsbelastningsutjämnaren händer följande:

* Ersättningsanvändaren tilldelas alla arbetsobjekt som för närvarande är tilldelade till en ursprunglig användare i de valda projekten.

* Den nya användaren tilldelas inte till någon arbetspost som redan är markerad som Fullständig.
* Om rollen som är associerad med den första användaren inte matchar någon av rollerna för den andra användaren, tilldelas den andra användaren i sin primära roll.

Så här ersätter du en användare med en annan användare:

1. Börja tilldela arbetsobjekt i arbetsbelastningsutjämnaren enligt beskrivningen ovan och välj **Ersätt**.
1. Klicka på listrutepilen i fältet **Aktuellt tilldelad användare** och välj en användare i en lista. Endast användare som för närvarande är tilldelade till ofullständiga arbetsobjekt i de angivna projekten visas. Detta är ett obligatoriskt fält.

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. I fältet **Användare som ska tilldelas** klickar du på listrutepilen för att välja från en lista med föreslagna användare eller för att ange ett annat användarnamn. Användare som visas i listan matchar som standard villkoren för smarta uppdrag. Mer information finns i [Översikt över smarta uppdrag](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront visar en anteckning om hur många objekt den aktuella tilldelade användaren ska ersätta den andra användaren och vilka roller de ska ersätta.

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Klicka på **Ersätt**.

   Den första användaren som valts ersätts av den andra användaren i alla arbetsobjekt från det valda projektet.

   Du får en bekräftelse på hur många arbetsobjekt som har ersatts med den ursprungliga användartilldelningen.

### Ta bort användartilldelning {#unassign-user}

Du kan ta bort tilldelningen för en användare från alla arbetsobjekt som användaren har tilldelats i de valda projekten.

När du tar bort tilldelningen för en användare från alla deras uppdrag med hjälp av grupptilldelningar i Utjämning av arbetsbelastning händer följande:

* Den angivna användaren tas bort från alla arbetsobjekt som han/hon har tilldelats.
* Om den otilldelade användaren är associerad med jobbroller förblir jobbrollerna tilldelade till arbetsobjekten när användaren tas bort.

* Om den angivna användaren har tilldelats till arbetsobjekt som har slutförts, förblir användaren tilldelad dessa arbetsobjekt.

Mer information om användar- och jobbrolltilldelningar finns i [Översikt över hur du tilldelar arbete i belastningsutjämnaren](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Så här tar du bort tilldelningen för en användare från arbetsobjekt i de markerade projekten eller för de markerade uppgifter eller utgåvor där de har tilldelats:

1. Börja tilldela arbetsobjekt i arbetsbelastningsutjämnaren enligt beskrivningen ovan och välj **Ta bort tilldelning**.

1. Klicka på listrutepilen i fältet **Användare för att ta bort tilldelning** och välj en användare i en lista. Endast användare som för närvarande är tilldelade till ofullständiga arbetsobjekt i de angivna projekten visas. Detta är ett obligatoriskt fält.

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront visar en anteckning om antalet objekt där den aktuella tilldelade användaren inte kommer att tilldelas.

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Klicka på **Ta bort tilldelning**.\
   Du får en bekräftelse på antalet arbetsobjekt där den angivna användaren togs bort.


