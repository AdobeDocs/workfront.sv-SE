---
product-area: projects;templates
navigation-topic: create-projects
title: Skapa ett projekt med en mall
description: Du kan använda mallar som ett ramverk för att skapa projekt i Adobe Workfront. Om du har projekt som upprepas ofta kan du spara tid genom att använda mallar för det nya projektet.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---

# Skapa ett projekt med en mall

<!-- Audited: 01/2024 -->

Du kan använda mallar som ett ramverk för att skapa projekt i Adobe Workfront. Om du har projekt som upprepas ofta kan du spara tid genom att använda mallar för den allmänna tidslinjen i det nya projektet.

Med mallar kan du hämta upprepningsbara processer, information och inställningar som är kopplade till dina projekt. Informationen som är kopplad till en mall överförs till projektet. Detta inkluderar uppgifter, uppdrag, varaktighet, dokument, ekonomisk information, risker och anpassade formulär.

>[!TIP]
>
>Workfront definierar det nya projektets grupp och status enligt följande:
>
>* Standardstatusen för ett nytt projekt som skapats från en mall motsvarar den status som definieras av Workfront-administratören i området Projektinställningar, eller av en gruppadministratör (eller Workfront-administratör) i området Projektinställningar för en grupp. Information om hur du konfigurerar projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) eller [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Det nya projektets grupp är mallgruppen. Om mallen inte är associerad med en grupp är projektgruppen hemgruppen för den användare som skapar projektet.
>
>* Statuserna som är tillgängliga för ett nytt projekt matchar statusvärdena för gruppen för projektet, som är antingen gruppen för mallen, eller hemgruppen för användaren som skapar projektet.

Du har följande alternativ för att skapa ett projekt från en mall:

* Skapa ett projekt från en mall i området Projekt
* Skapa ett projekt från en mall på mallnivå
* Koppla en mall till ett befintligt projekt

  Mer information finns i [Koppla en mall till ett projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Skapa ett projekt från en mall i området Grupper

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-licens</td> 
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till projekt och mallar</p>
   <p>Redigera åtkomst till portföljer och program om mallen du använder innehåller en Portfolio och ett program</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till en mall</p> 
  <p>Om mallen du använder innehåller en Portfolio och ett program måste du ha behörigheten Hantera för portföljen och programmet för att skapa projektet </p> 
   <p>När du skapar ett projekt får du automatiskt behörigheten Hantera för projektet.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Skapa ett projekt från en mall i området Projekt

Du kan skapa ett projekt från området Projekt på huvudmenyn eller från området Projekt i en portfölj eller ett program.

>[!NOTE]
>
>Systemet eller gruppadministratören kan ändra gränssnittet med hjälp av en layoutmall. I det här fallet kan vissa av namnen på de avsnitt och områden som avses i följande steg vara olika i din instans av Workfront.

1. Gör något av följande:

   * Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet. Klicka på **Projekt** och expandera sedan **Nytt projekt**.
   * Gå till en portfölj och expandera sedan **Nytt projekt**.

     >[!TIP]
     >
     >När du skapar ett projekt med hjälp av en mall från en portfölj uppdateras fältet Portfolio för det nya projektet till att visa den portfölj som du valde att skapa projektet från. Detta skriver över Portfolio-fältet i mallen, om det har angetts.

   * Gå till ett program och expandera sedan **Nytt projekt**.

     >[!TIP]
     >
     >När du skapar ett projekt med hjälp av en mall från ett program uppdateras fältet Program för de nya projekten så att det program du valde att skapa projektet från visas. Portfolio-fältet i mallen uppdateras för att visa portföljen för det program du valde att skapa projektet från. Detta skriver över fälten Program och Portfolio i mallen, om de anges.

   * Om du är gruppadministratör kan du även skapa ett projekt i avsnittet Projekt i en grupp som du hanterar. Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >När du skapar ett projekt med en mall från en grupp, visas den grupp du skapar projektet från i fältet Grupp i det nya projektet endast när fältet Grupp i mallen inte har angetts. Om mallgruppsfältet anges är gruppfältet för det nya projektet mallfältet.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nya projektalternativ](assets/new-project-dropdown.png)

1. Klicka på namnet på en mall i listan **Favoritmallar**.

   ![Välj en favoritmall](assets/new-project-from-template-dropdown-with-template-favorites.png)

   eller

   Gör följande:

   1. Välj **Nytt projekt från mall**.
   1. I fältet **Sökmallar** börjar du skriva namnet på en mall och klickar på den när den visas i listan.
   1. Granska mallinformationen till höger.

      Mallinformationen innehåller följande:

      * Mallvaraktighet
      * Mallägare
      * Antalet uppgifter på den översta nivån, som innehåller namnen på de tre viktigaste uppgifterna
      * Antalet uppgifter i mallen
      * Namnen på de anpassade mallformulären

   1. (Valfritt) Hovra över namnet på en mall i den vänstra rutan och klicka på ikonen **Favoriter** **&#x200B;**&#x200B;![Favoriter](assets/favorites-icon-small.png) för att markera den som en favorit för framtida bruk.

      eller

      Expandera listan **Favoritmallar** och välj en mall i listrutan.

      >[!TIP]
      >
      >Du kan ha upp till 40 Workfront-objekt markerade som favoriter. Detta inkluderar mallar och andra objekt.

   1. Klicka på **Använd mall** när du har valt en mall.

      ![Mallinformation](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Om du har använt milstolpevyn på listan med projekt klickar du på namnet på en mall i avsnittet **Nytt från mall**.
      >
      >
      >![Milstolpevy för att skapa ett projekt från en mall](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   Rutan **Nytt projekt** öppnas.

   ![Ny projektruta](assets/new-project-from-template-box.png)

1. Om ett fält redan har fyllts i i mallen fylls fältet i automatiskt i rutan **Nytt projekt** . Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Klicka på **Skapa projekt**.

   All information som definieras i mallen kopplas automatiskt till det nya projektet om du inte ändrade dem i det föregående steget.

## Skapa ett projekt från en mall i området Mallar

I stället för att börja i området Projekt kan du skapa ett projekt från en mall genom att börja med mallen.

{{step1-to-templates}}

1. Klicka på namnet på en mall som du vill använda.
1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png) och sedan på **Skapa projekt**.

   ![Skapa projekt från mall](assets/project-sharing-on-template.png)

   Rutan **Nytt projekt** öppnas.

1. Ange ett namn för projektet, granska varje avsnitt och gör eventuella ändringar.

   ![Ny projektruta](assets/new-project-from-template-box.png)

   Om ett fält redan har fyllts i i mallen fylls fältet i automatiskt i rutan **Nytt projekt** . Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicka på **Skapa projekt**.

   All information som definieras i mallen kopplas automatiskt till det nya projektet om du inte ändrade dem i det föregående steget.
