---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Lås eller lås upp en grupptidrapport och timinställning
description: Om du är gruppadministratör kan du konfigurera och sedan låsa en tidrapport och timinställning för gruppen efter att en Workfront-administratör har låst upp den på systemnivå.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Lås eller lås upp en grupptidrapport och timinställning

Om du är gruppadministratör kan du konfigurera och sedan låsa en tidrapport och timinställning för gruppen efter att en Workfront-administratör har låst upp den på systemnivå.

Genom att låsa en Adobe Workfront-inställning kan du vara säker på att alla i gruppen och dess undergrupper använder samma inställning för den inställningen. Även om du fortfarande kan konfigurera om en inställning som du låser kan gruppadministratörer inte göra det för lägre undergrupper.

Om du däremot låser upp en inställning på gruppnivå blir undergruppsadministratörer mer flexibla när det gäller att hantera hur deras grupper arbetar med dessa objekt. När en inställning är olåst kan gruppadministratörer konfigurera om den för dessa undergrupper.

Detta är parallellt med möjligheten för en Workfront-administratör att låsa eller låsa upp en inställning för alla i systemet.

Mer information om hur en Workfront-administratör kan låsa eller låsa upp en tidrapport och timinställning för alla grupper i systemet finns i [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Mer information om hur du konfigurerar en tidrapport och timinställningar för en grupp finns i [Konfigurera tidrapport- och timinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Om du konfigurerar en olåst inställning för en grupp påverkas inte den inställningen för undergrupper under gruppen.
>
>  När en ny undergrupp skapas ärver den dock inställningarna och det låsta eller olåsta läget för gruppen direkt ovanför den.
>
>* Om du flyttar en grupp under en grupp som har en låst inställning, ärver den flyttade gruppen den inställningen och den låses för den flyttade gruppen.
>* Om du flyttar en grupp under en grupp som har en olåst inställning påverkas inte den flyttade gruppen av den inställningen.
>
>  Om inställningen i den flyttade gruppen är låst när den flyttas förblir den låst, men gruppadministratören kan låsa upp den nu eftersom den är olåst för den överordnade gruppen.
>

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Lås eller lås upp en grupptidrapport och timinställning

>[!TIP]
>
>Om du är Workfront-administratör kan du kringgå steg 1-4 genom att gå till Inställningar > Tidrapport och timmar > Inställningar och sedan söka efter gruppens namn i rutan längst upp på sidan.

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **Grupper** i den vänstra panelen.
1. Klicka på namnet på gruppen där du vill låsa eller låsa upp en tidrapport och timinställning.
1. Klicka på **Inställningar för tidrapporter och timmar** i den vänstra panelen.

1. Gör något av följande på sidan som visas:

   * Om du vill att administratörer för grupper under gruppen ska kunna konfigurera en inställning för sina grupper, låser du upp den ![](assets/unlock-toggle-button.png).
   * Om du vill att alla grupper under din konfiguration ska använda din inställning, måste du se till att den är låst ![](assets/lock-toggle-button.png) (detta är standardinställningen).

     >[!IMPORTANT]
     >
     >Det är viktigt att kommunicera med administratörer och användare i grupper under din egen för att säkerställa att alla behov beaktas när du konfigurerar en låst inställning. När du låser den ärvs konfigurationen för den av alla undergrupper nedan. Om inställningen har låsts upp under en viss tid ersätter konfigurationen de som gruppadministratörer i lägre undergrupper kan ha gjort.

1. Klicka på **Spara**.
