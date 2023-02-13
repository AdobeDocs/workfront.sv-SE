---
product-area: projects
navigation-topic: create-projects
title: Importera ett projekt från Microsoft Project
description: Du kan importera projekt från Microsoft Project till Adobe Workfront och hantera alla projekt i ett och samma program. Varje gång du importerar ett projekt från Microsoft Project skapas ett nytt projekt i Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Importera ett projekt från Microsoft Project

Du kan importera projekt från Microsoft Project till Adobe Workfront och hantera alla projekt i ett och samma program. Varje gång du importerar ett projekt från Microsoft Project skapas ett nytt projekt i Workfront.

>[!IMPORTANT]
>
>Alla Microsoft Project-fält överförs inte till Workfront.
>
>Mer information om kompatibilitet för fält mellan Workfront och Microsoft Project finns i [Mappa Microsoft Project-fält till Adobe Workfront-projekt](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Åtkomstkrav

framtagen för P&amp;P:

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
   <td> <p>Aktuell licens: Standard </p> 
   eller
   <p>Äldre licens: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till projekt finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Bevilja åtkomst till projekt</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du skapar ett projekt får du automatiskt behörigheten Hantera i projektet </p> <p> Mer information om projektbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till projekt finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Bevilja åtkomst till projekt</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du skapar ett projekt får du automatiskt behörigheten Hantera i projektet </p> <p> Mer information om projektbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa ett projekt från ett MS-projekt

Du kan skapa ett projekt från området Projekt på huvudmenyn eller från området Projekt i en portfölj eller ett program.

1. Gå till Microsoft Project och öppna ett projekt som du vill importera från i Workfront.
1. Klicka **Fil** sedan **Spara som** för att spara projektet som en XML-fil.

1. Logga in på Workfront.
1. Gör något av följande:

   * Klicka på **Huvudmeny** ![](assets/main-menu-icon.png), klicka **Projekt** och sedan expandera **Nytt projekt**.
   * Gå till en portfölj och expandera sedan **Nytt projekt**.
   * Gå till ett program och expandera **Nytt projekt**.
   * Om du är gruppadministratör kan du även skapa ett projekt i avsnittet Projekt i en grupp som du hanterar. Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Välj **Importera MS-projekt** alternativ.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Klicka **Välj fil** bläddrar du sedan efter XML-filen på datorn som du exporterade från Microsoft Project.
1. Importera den markerade filen.

   Workfront påbörjar importprocessen och skapar ett nytt projekt baserat på den fil som exporteras från Microsoft Project.

   När importen är klar dirigeras du till den nya projektsidan som visar en bekräftelse på att importen har slutförts.

   >[!NOTE]
   >
   >Workfront har 15 minuters tidsbegränsning för filöverföringar. Om filöverföringen tar längre tid än så rekommenderar vi att du delar upp ditt projekt i mindre projekt och importerar dem separat. När du har importerat dem till Workfront flyttar du arbetsmomenten från ett projekt till ett annat. Mer information om hur du flyttar uppgifter finns i [Flytta uppgifter](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Valfritt) Fortsätt redigera projektet i Workfront. Mer information om hur du redigerar projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

   Statusen för ett nytt projekt som skapats från en mall motsvarar den status som definieras av Workfront-administratören i området Projektinställningar eller av en gruppadministratör i området Gruppprojektinställningar. Mer information om hur du konfigurerar projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
