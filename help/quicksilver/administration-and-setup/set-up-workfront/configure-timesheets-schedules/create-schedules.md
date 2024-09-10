---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Skapa ett schema
description: Du kan definiera användarnas arbetsveckor med hjälp av scheman. Du kan associera ett schema med en användare eller ett projekt. Detta gör att  [!DNL Workfront]  kan beräkna tidslinjer och användartillgänglighet.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Skapa ett schema

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Som [!DNL Adobe Workfront]-administratör kan du definiera din arbetsvecka med scheman. Du kan associera ett schema med en användare eller ett projekt. Detta gör att [!DNL Workfront] kan beräkna tidslinjer och användartillgänglighet.

När du har användare som arbetar i olika tidszoner ser det till att deras arbete registreras i [!DNL Workfront] i realtid och att deras tillgänglighet alltid är korrekt beroende på när de arbetar genom att skapa ett schema i varje tidszon och associera det med dessa användare.

Mer information om hur du associerar scheman med användare och projekt finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) och [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Gruppadministratörer kan också skapa scheman som är kopplade till de grupper som de hanterar. Mer information finns i [Skapa och ändra en grupps scheman](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Mer information om hur du använder scheman för att hjälpa användare att samarbeta i [!DNL Workfront] över tidszoner finns i [Arbeta över tidszoner](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Mer information om hur scheman används vid resursplanering finns i [Översikt över scheman](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) och [Översikt över resursplanering](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td><p>Nytt: [!UICONTROL Standard]</p>
       <p>eller</p>
       <p>Aktuell: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett schema

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Schedules]**.
1. Klicka på **[!UICONTROL New Schedule]**.
1. Ange ett namn för schemat.
1. (Valfritt) Välj **[!UICONTROL Default Schedule]** om du vill identifiera schemat som standard.

   Du måste ha minst ett schema i [!DNL Workfront]. Om du bara har ett är det standardschemat.

   Du kan ha fler än ett schema, men du kan bara ha ett standardschema.

   >[!NOTE]
   >
   >Du kan inte ange ett schema som standardschema om du är gruppadministratör. Endast en [!DNL Workfront]-administratör kan ange ett schema som standard för systemet.

   ![Nytt schema](assets/new-schedule.png)

1. Välj ett dagligt schema på fliken **[!UICONTROL Schedule]** genom att dra den blå konturen över timblocken för att markera dem.

   Vi rekommenderar att du väljer 8 1-timmars block under en 9-timmars tidsperiod. Det här tar plats för lunch eller andra pauser.

   ![Tidsblock i ett schema](assets/new-schedule-with-exceptions.png)

1. Ange följande information på fliken **[!UICONTROL Details]**:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Markera gruppen vars administratörer har behörighet att redigera schemat.</p>
     <p><b>VIKTIGT</b>:</p>
      <ul>
       <li>
       <p>Om du är gruppadministratör och skapar ett schema är det här fältet obligatoriskt.</p>
       <p>Som gruppadministratör kan du bara skapa ett schema om det är avsett för en grupp eller undergrupp som du är utsedd som administratör för.</p>
       <p>Om du bara hanterar en grupp markeras gruppen som standard i det här fältet.</p>
       <p>Om du hanterar flera grupper måste du markera en grupp i det här fältet innan du kan spara schemat.</p></li>
       <li>Om du är [!DNL Workfront]-administratör och skapar ett schema är det här fältet valfritt. När du skapar ett schema utan att associera det med en grupp, sparas det som ett schema på systemnivå och kan inte hanteras av en gruppadministratör för någon grupp.
       <p>Scheman som tilldelats konton eller projekt är synliga för alla användare som kan redigera dessa objekt. Detta gäller för scheman på både systemnivå och gruppnivå.</p>
       </li>
       <p>Om du anger en grupp med administrationsåtkomst för ett schema tilldelas inte schemat till användarna i gruppen. Det tillåter bara gruppadministratörer i gruppen att redigera, ta bort och kopiera schemat.</p>
       <p>Gruppadministratörer kan inte redigera, ta bort eller kopiera scheman på systemnivå. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Välj de grupper med [!UICONTROL View] åtkomst som kan se det här schemat.</p>
     <p>Det är bara användarna i de grupper som anges här som kan hitta schemat i listrutan när de tilldelar det till användare eller projekt.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Välj tidszon för schemat.</p>
     <p>Om du associerar schemat med en användare rekommenderar vi att tidzonen för schemat matchar användarens tidszon. Mer information om användarens tidszoner finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil.
     </td>
    </tr>
   </table>


1. Ange eventuella undantag för schemat på fliken **[!UICONTROL Exceptions]**.

   Undantag är hela eller halva dagar som måste uteslutas från schemat, t.ex. helger eller företagsevenemang.

   >[!NOTE]
   >
   >Om du redan vet vilka de återkommande schemaundantagen är kan du definiera schemaundantagen för många år i framtiden.

   Du kan undanta hela eller delar av dagar från arbetsschemat. Klicka på datumet för att markera det som ett undantag och markera sedan fältet **[!UICONTROL All day]** för att ange om undantaget är en hel dag eller inte.

   ![Undantag hela dagen](assets/schedule-adding-an-all-day-exception.png)

1. Ange start- och sluttid för undantagen för partiella dagar.

   ![Undantag för partiell dag](assets/partial-day-exception-on-schedules.png)

1. Klicka på **[!UICONTROL Save]** och sedan på **[!UICONTROL Save]Ändringar**.

1. (Valfritt) Associera schemat med en användare.

   Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Valfritt) Associera schemat med ett projekt.

   Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).
