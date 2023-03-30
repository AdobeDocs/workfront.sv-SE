---
product-area: projects;templates
navigation-topic: create-projects
title: Skapa ett projekt med en mall
description: Du kan använda mallar som ett ramverk för att skapa projekt. Om du har projekt som upprepas ofta kan du spara tid genom att använda mallar för den allmänna tidslinjen i det nya projektet.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: e38411056b3f9be6d0241ee18e71984ef2a678a0
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# Skapa ett projekt med en mall

Du kan använda mallar som ett ramverk för att skapa projekt. Om du har projekt som upprepas ofta kan du spara tid genom att använda mallar för den allmänna tidslinjen i det nya projektet.

Med mallar kan du hämta upprepningsbara processer, information och inställningar som är kopplade till dina projekt. Informationen som är kopplad till en mall överförs till projektet. Detta inkluderar uppgifter, uppdrag, varaktighet, dokument, ekonomisk information, risker och anpassade formulär.

>[!TIP]
>
>Workfront definierar det nya projektets grupp och status enligt följande:
>
>* Standardstatusen för ett nytt projekt som skapats från en mall motsvarar den status som definieras av Workfront-administratören i området Projektinställningar eller av en gruppadministratör (eller Workfront-administratör) i området Projektinställningar för en grupp. Mer information om hur du konfigurerar projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) eller [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Det nya projektets grupp är mallgruppen. Om mallen inte är associerad med en grupp är projektgruppen hemgruppen för den användare som skapar projektet.
>
>* Statuserna som är tillgängliga för ett nytt projekt matchar statusvärdena för den grupp av projektet som är antingen mallgruppen eller hemgruppen för användaren som skapar projektet.


Du har följande alternativ för att skapa ett projekt från en mall:

* Skapa ett projekt från en mall i området Projekt
* Skapa ett projekt från en mall på mallnivå
* Koppla en mall till ett befintligt projekt

   Mer information finns i [Bifoga en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Skapa ett projekt från en mall i området Grupper

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront licensöversikt*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och mallar</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om åtkomst till projekt finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Bevilja åtkomst till projekt</a>. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till en mall</p> <p>När du skapar ett projekt får du automatiskt behörigheten Hantera i projektet </p> <p> Mer information om projektbehörigheter finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa ett projekt från en mall i området Projekt

Du kan skapa ett projekt från området Projekt på huvudmenyn eller från området Projekt i en portfölj eller ett program.

1. Gör något av följande:

   * Klicka på **Huvudmeny** ![](assets/main-menu-icon.png), klicka **Projekt** och sedan expandera **Nytt projekt**.
   * Gå till en portfölj och expandera sedan **Nytt projekt**.

      >[!TIP]
      >
      >När du skapar ett projekt med hjälp av en mall från en portfölj uppdateras fältet Portfolio i det nya projektet till att visa den portfölj som du valde att skapa projektet från. Detta skriver över Portfolio-fältet i mallen, om det har angetts.

   * Gå till ett program och expandera **Nytt projekt**.

      >[!TIP]
      >
      >När du skapar ett projekt med hjälp av en mall från ett program uppdateras fältet Program för de nya projekten så att det program du valde att skapa projektet från visas. Fältet Portfolio i mallen uppdateras för att visa portföljen för det program du valde att skapa projektet från. Fälten Program och Portfolio i mallen skrivs över, om de har angetts.

   * Om du är gruppadministratör kan du även skapa ett projekt i avsnittet Projekt i en grupp som du hanterar. Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >När du skapar ett projekt med en mall från en grupp, visas den grupp du skapar projektet från i fältet Grupp i det nya projektet endast när fältet Grupp i mallen inte har angetts. Om mallgruppsfältet anges är gruppfältet för det nya projektet mallfältet.
   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Klicka på namnet på en mall i dialogrutan **Favoritmallar** list

   ![](assets/new-project-from-template-dropdown-with-template-favorites-nwe-350x235.png)

   eller

   Gör följande:

   1. Välj **Nytt projekt från mall**.
   1. I **Sökmallar** börjar du skriva namnet på en mall och klickar på den när den visas i listan.
   1. Granska mallinformation till höger.

      Mallinformationen innehåller följande:

      * Mallvaraktighet
      * Mallägare
      * Antalet uppgifter på den översta nivån som innehåller namnen på de tre viktigaste uppgifterna
      * Antalet uppgifter i mallen
      * Namnen på de anpassade mallformulären
   1. (Valfritt) Håll muspekaren över namnet på en mall och klicka på **Favoriter** **icon** ![](assets/favorites-icon-small.png) för att markera den som en favorit för framtida bruk.

      eller

      Expandera **Favoritmallar** och välj en mall i listrutan.

      >[!TIP]
      >
      >Du kan ha upp till 40 Workfront-objekt markerade som favoriter. Detta inkluderar mallar och andra objekt.

   1. Klicka **Använd mall** när du har valt en mall.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!NOTE]
   >
   >Om du har använt vyn Milstolpe på projektlistan klickar du på namnet på en mall i **Nytt från mallavsnittet**.
   >
   >
   >![](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)   >

1. The **Nytt projekt** öppnas.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

1. Om ett fält redan är ifyllt i mallen fylls fältet i automatiskt i **Nytt projekt** box. Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Klicka **Skapa projekt**.

   All information som definieras i mallen kopplas automatiskt till det nya projektet om du inte ändrade dem i det föregående steget.

## Skapa ett projekt från en mall i området Mallar

I stället för att börja i området Projekt kan du skapa ett projekt från en mall genom att börja med mallen.

 

1. Från **Huvudmeny**, klicka **Mallar**.

1. Klicka på namnet på en mall som du vill använda.
1. Klicka på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Skapa projekt.**

   ![Skapa projekt från mall](assets/project-sharing-on-template-nwe-2022-350x172.png)

   The **Nytt projekt** öppnas.

1. Ange ett namn för projektet, granska varje avsnitt och gör nödvändiga ändringar.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

   Om ett fält redan är ifyllt i mallen fylls fältet i automatiskt i **Nytt projekt** box. Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicka **Skapa projekt.**

   All information som definieras i mallen kopplas automatiskt till det nya projektet om du inte ändrade dem i det föregående steget.
