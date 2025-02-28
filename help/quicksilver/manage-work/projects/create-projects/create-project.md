---
product-area: projects
navigation-topic: create-projects
title: Skapa ett projekt
description: Ett projekt är en stor arbetsenhet i Adobe Workfront. Du kan skapa projekt från grunden, använda en mall eller konvertera utgåvor eller uppgifter till projekt.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Skapa ett projekt

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Projekt representerar en stor mängd arbete som behöver utföras i Adobe Workfront.

## Åtkomstkrav

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p>
        <p>eller</p>
        <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>När du skapar ett projekt får du automatiskt behörigheten Hantera för projektet.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Olika sätt att skapa projekt

Du kan skapa ett projekt i Workfront på något av följande sätt:

* Skapa ett projekt från grunden utan att använda en mall. I den här artikeln beskrivs hur du skapar ett projekt från grunden.

* Kopiera ett befintligt projekt.\
  Mer information om att kopiera projekt finns i [Kopiera ett projekt](../../../manage-work/projects/manage-projects/copy-project.md).

* Använd en mall.\
  Mer information om hur du använder en mall för att skapa ett nytt projekt finns i [Skapa ett projekt med en mall](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importera ett projekt från Microsoft Project.\
  Mer information om hur du importerar ett projekt från MS Project finns i [Importera ett projekt från Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importera ett projekt med snabbstart.

  Som Workfront-administratör kan du importera projekt med en snabbstart.

  Mer information om hur du importerar data med hjälp av snabbstartsfunktioner i Workfront finns i [Importera data till Adobe Workfront med en snabbstartsmall](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Mer information om hur du importerar projekt med hjälp av snabbstartsfunktioner finns i [Snabbstartscenario: enkla projekt- och uppgiftsimportförberedelser](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publicera ett projekt från ett scenario i Adobe Workfront Scenario Planner.

  Scenarioplaneraren kräver något av följande:

   * En ytterligare licens för den nuvarande Workfront-licensstrukturen.
   * En Ultimate-licens för den nya Workfront License-strukturen.

  Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md). Mer information om hur du skapar projekt från publiceringsinitiativ finns i [Uppdatera eller skapa projekt genom att publicera projekt i scenarioplanen](../../../scenario-planner/publish-scenarios-update-projects.md).

* Lägg till projekt när du kopplar dem från en posttyp i Workfront Planning. I produktionsmiljön kan du bara skapa projekt utan mallar från Workfront Planning. <span class="preview">Du kan skapa projekt med hjälp av en mall i förhandsvisningsmiljön.</span>

  Du måste ha en ny Workfront-licens och en extra Workfront Planning-licens för Workfront Planning.

  Mer information om åtkomst till Workfront Planning finns i [Åtkomstöversikt](/help/quicksilver/planning/access/access-overview.md).

  Mer information om hur du skapar projekt genom att lägga till dem i poster finns i avsnittet Skapa projekt när du ansluter dem med poster från Workfront Planning i artikeln [Skapa Workfront-objekt från Workfront Planning när du ansluter dem till poster](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## Förutsättningar

Innan du börjar måste du se till att:

* Din system- eller gruppadministratör har aktiverat inställningen&quot;Tillåt användare att skapa projekt utan att använda en mall&quot; under Konfigurera.

  Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nya standardinställningar för projekt

När du skapar ett projekt använder Workfront en uppsättning standardinställningar. Status, Grupp och Schemaläge är till exempel förinställda när du skapar ett projekt.

Tänk på följande:

* Som Workfront-administratör eller gruppadministratör kan du konfigurera standardinställningarna för ett nytt projekt när du konfigurerar projektinställningar för hela Workfront-instansen eller för en grupp.
* Workfront tillämpar inställningarna för gruppen, om det finns några, innan den tillämpar inställningarna som angetts av Workfront-administratören.
* Standardstatusen för ett nytt projekt motsvarar den status som definieras av Workfront-administratören i området Projektinställningar eller av en gruppadministratör (eller Workfront-administratör) i området Projektinställningar för en grupp.

  >[!NOTE]
  >
  >Vi rekommenderar att standardstatusen för ett nytt projekt är Planering. När du gör ändringar i det nya projektet ser det till att inga meddelanden skickas till användarna som är tilldelade projektet.
  >
  >Mer information om hur du ställer in standardstatus och andra standardinställningar för ett nytt projekt finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) eller [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Följande scenarier gäller för hur Workfront definierar gruppen och statusen för ett nytt projekt:

   * Om du skapar ett projekt från grunden är projektgruppen din hemgrupp.

     Projektets status är standardstatus i Projektinställningar i din hemgrupp, om det finns någon, eller i din Workfront-instans. Du kan ändra standardstatus när du skapar projektet till vilken status som helst som är tillgänglig för Projektgruppen.

   * Om du skapar ett projekt med hjälp av en mall har inställningarna från mallen företräde framför de inställningar som har angetts av Workfront- eller gruppadministratören.

     Det nya projektets grupp är mallgruppen. Om mallen inte är associerad med en grupp är projektgruppen hemgruppen för den användare som skapar projektet.

     Standardstatusen för ett nytt projekt som skapats från en mall motsvarar den status som definieras av Workfront-administratören i området Projektinställningar eller av en gruppadministratör (eller Workfront-administratör) i området Projektinställningar för gruppen. Du kan ändra standardstatus när du skapar ett projekt från en mall, till någon av statusvärdena för den grupp av projektet som är antingen mallgruppen eller hemgruppen för den användare som skapar projektet.

   * Om du skapar ett projekt genom att konvertera ett problem, är gruppen för ett nytt projekt gruppen för problemets befintliga projekt. Om den användare som konverterar problemet inte har tillgång till problemets projekt eller om problemets projekt inte har någon grupp, är gruppen för det nya projektet hemgruppen för den användare som konverterar problemet.

     Det nya projektets status matchar gruppstatusarna för gruppen som är associerad med projektet, som antingen är gruppen för det ursprungliga projektet eller hemgruppen för användaren som konverterar problemet.

     Om du använder en mall när du skapar projektet genom att konvertera problemet, se det andra scenariot ovan för att ta reda på vilken grupp och vilken status Workfront gäller för det nya projektet.

## Skapa ett projekt från grunden

>[!NOTE]
>
>Om du skapar ett projekt med hjälp av en mall rekommenderar vi att du också ser artikeln [Skapa ett projekt med hjälp av en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Gör något av följande:

   * Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet. Klicka på **Projekt** och expandera sedan **Nytt projekt**.
   * Gå till en portfölj och expandera sedan **Nytt projekt**.
   * Gå till ett program och expandera sedan **Nytt projekt**.
   * Om du är gruppadministratör kan du även skapa ett projekt i avsnittet Projekt i en grupp som du hanterar. Mer information finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Ny projektmeny](assets/new-project-dropdown-nwe-350x358.png)

1. Klicka på **Nytt projekt** på menyn om du vill skapa ett projekt från grunden.
1. Ange ett namn för projektet. Tryck på Retur för att spara namnet.

   ![Ange ett namn för projektet](assets/rename-untitled-project.png)

   Projektsidans sidhuvud innehåller en snabb översikt över aktuell hälsa och förloppet för ett projekt. Informationen i projekthuvudet ändras allt eftersom projektinformationen uppdateras.

1. Klicka på **Börja lägga till aktiviteter**.

   eller

   Klicka på **Ny aktivitet** om du vill lägga till aktiviteter i projektet och tilldela resurser till dem.

   Mer information om hur du lägger till uppgifter i ett projekt finns i [Skapa uppgifter i ett projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Redigera projektinformationen genom att klicka på menyn **Mer** och sedan på **Redigera** ![Redigera-ikonen](assets/qs-edit-icon.png) bredvid namnet på projektet.

   Dialogrutan **Redigera projekt** öppnas.

   Mer information om hur du redigerar ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Valfritt) När du har konfigurerat projektinställningarna och lagt till uppgifterna kan du ändra projektets status till **Aktuell**.

   Detta anger att projektet nu är klart att starta och att användare som är tilldelade till uppgifterna nu kan börja arbeta med dem.

   Mer information om projektstatus finns i [Åtkomst till listan över systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
