---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Hantera projektgruppen
description: Projektgruppen består av användare som är kopplade till projektet. Medlemmarna i projektgruppen visas i avsnittet Personer i projektet.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Hantera projektgruppen

Projektgruppen består av användare som är kopplade till projektet. Medlemmarna i projektgruppen visas i avsnittet Personer i projektet.

## Åtkomstkrav

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Visa eller ge användare högre åtkomst</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Lägga till användare i ett projektteam

När du lägger till användare i projektteamet får de behörigheten Visa för projektet och projektets uppgifter, utgåvor och dokument. Mer information finns i artikeln [Översikt över projektgruppen](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Användare i projektgruppen läggs inte automatiskt till i resurshanteringsverktygen för projektet.

Du kan lägga till användare i projektteamet på följande sätt:

* [Lägg till användare automatiskt i ett projektteam](#automatically-add-users-to-a-project-team)
* [Lägga till användare manuellt i ett projektteam](#manually-add-users-to-a-project-team)

### Lägg till användare automatiskt i ett projektteam {#automatically-add-users-to-a-project-team}

De användare som uppfyller följande roller i projektet läggs automatiskt till i projektteamet och visas i avsnittet Personer när projektet skapas:

* Den som har skapat projektet
* Projektägaren
* Projektsponsorn

Användare läggs också automatiskt till i projektteamet när de tilldelas följande:

* Uppgifter
* Problem

### Lägga till användare manuellt i ett projektteam {#manually-add-users-to-a-project-team}

Om användare som inte har någon roll i projektet vill få meddelanden om vissa uppdateringar eller ändringar under projektets livslängd kan du lägga till dem manuellt i projektteamet.

Mer information om vilka meddelanden som kan aktiveras för användare i projektteamet finns i [Händelsemeddelandetyper](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Gå till projektet som du vill lägga till användare i.

1. Klicka på **Personer** i den vänstra panelen.

1. Klicka på **Lägg till användare**.

   Dialogrutan Lägg till användare i projektgruppen visas.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. I rutan **Lägg till användare** börjar du skriva namnet på en aktiv Workfront-användare som du vill lägga till i projektteamet och klickar sedan på namnet när det visas i listrutan.

   Upprepa det här steget om du vill lägga till flera användare i projektteamet. Användarna måste tillhöra den grupp som är associerad med projektet.

   >[!TIP]
   >
   >* Du kan inte lägga till användare genom att lägga till deras team, grupper, företag eller jobbroller.
   >* Lägg märke till avataren, användarens primära roll och deras e-postadress för att skilja mellan användare med identiska namn när du lägger till användarna. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
   >
   >  Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Klicka på **Lägg till**.

   Användarna får behörigheten Visa i projektet och får meddelanden om projektet som en del av projektteamet.

## Ta bort användare från ett projektteam

När du tar bort användare från deras roller i projektet blir de kvar i projektteamet.

Om du tar bort en användare från projektteamet och användaren är tilldelad aktiviteter eller ärenden i projektet, tas användaren bort från de uppgifter och utgåvor som inte har slutförts. I det här fallet återgår uppgifterna och problemen till Ej tilldelat arbetsområde i Utjämning av arbetsbelastning.

Användare som är tilldelade slutförda uppgifter och ärenden förblir tilldelade även när du har tagit bort dem från projektteamet.

Mer information om hur du tar bort användare från projektteamet finns i [Ta bort användare från projekt](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
