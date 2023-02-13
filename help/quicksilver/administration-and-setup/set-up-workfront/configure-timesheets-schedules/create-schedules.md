---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Skapa ett schema
description: Du kan definiera användarnas arbetsveckor med hjälp av scheman. Du kan associera ett schema med en användare eller ett projekt. Detta gör att [!DNL Workfront] för att beräkna tidslinjer och användartillgänglighet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Skapa ett schema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Som en [!DNL Adobe Workfront] kan du definiera din arbetsvecka med hjälp av scheman. Du kan associera ett schema med en användare eller ett projekt. Detta gör att [!DNL Workfront] för att beräkna tidslinjer och användartillgänglighet.

När du har användare som arbetar i olika tidszoner ser du till att deras arbete registreras i genom att skapa ett schema i varje tidszon och associera det med dessa användare [!DNL Workfront] i realtid och att deras tillgänglighet alltid är korrekt beroende på när de arbetar.

Mer information om hur du associerar scheman med användare och projekt finns i följande artiklar:

* [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md)

Gruppadministratörer kan också skapa scheman som är kopplade till de grupper som de hanterar. Mer information finns i [Skapa och ändra en grupps scheman](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Mer information om hur du använder scheman för att hjälpa användare att samarbeta i [!DNL Workfront] över tidszoner, se [Arbeta över tidszoner](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Skapa ett schema

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på **[!UICONTROL Schedules]**.
1. Klicka på **[!UICONTROL New Schedule]**.
1. Ange ett namn för schemat.
1. (Valfritt) Välj **[!UICONTROL Default Schedule]** om du vill identifiera det här schemat som standard.

   Du kan ha flera scheman i [!DNL Workfront], men du kan bara ha ett standardschema.

   Du måste ha minst ett schema i [!DNL Workfront]. Om du bara har ett är det standardschemat.

   >[!NOTE]
   >
   >Du kan inte ange ett schema som standardschema om du är gruppadministratör. Endast en [!DNL Workfront] kan administratören ange ett schema som standard för systemet.

   ![](assets/new-schedule.png)

1. I **[!UICONTROL Schedule]** väljer du ett dagligt schema genom att dra den blå konturen över timblocken för att markera dem.

   Vi rekommenderar att du väljer 8 1-timmars block under en 9-timmars tidsperiod. Det här tar plats för lunch eller andra pauser.

   ![](assets/new-schedule-with-exceptions.png)

1. På **[!UICONTROL Details]** anger du följande information:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Ange gruppen vars administratörer har behörighet att redigera schemat.</p>
     <p><b>VIKTIGT</b>:</p>
      <ul>
       <li>
       <p>Om du är gruppadministratör och skapar ett schema är det här fältet obligatoriskt.</p>
       <p>Som gruppadministratör kan du bara skapa ett schema om det är avsett för en grupp eller undergrupp som du är utsedd som administratör för.</p>
       <p>Om du bara hanterar en grupp markeras gruppen som standard i det här fältet.</p>
       <p>Om du hanterar flera grupper måste du markera en grupp i det här fältet innan du kan spara schemat.</p></li>
       <li>Om du är en [!DNL Workfront] om administratören skapar ett schema är det här fältet valfritt. När du skapar ett schema utan att associera det med en grupp, sparas det som ett schema på systemnivå och kan inte hanteras av en gruppadministratör för någon grupp.
       <p>Scheman som tilldelats konton eller projekt är synliga för alla användare som kan redigera dessa objekt. Detta gäller för scheman på både systemnivå och gruppnivå.</p>
       </li>
       <p>Om en grupp med administrationsåtkomst anges för ett schema tilldelas inte schemat användarna i gruppen. kan bara gruppadministratörer i gruppen redigera, ta bort och kopiera schemat.</p>
       <p>Gruppadministratörer kan inte redigera, ta bort eller kopiera scheman på systemnivå. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Markera grupperna med [!UICONTROL View] åtkomst som det här schemat är synligt för.</p>
     <p>Det är bara användarna i de grupper som anges här som kan hitta schemat i listrutan när de tilldelar det till användare eller projekt.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Välj tidszon för schemat.</p>
     <p>Om du associerar schemat med en användare rekommenderar vi att tidszonen för schemat matchar användarens tidszon. Mer information om användarens tidszoner finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil.
     </td>
    </tr>
   </table>


1. På **[!UICONTROL Exceptions]** anger du undantagen till schemat.

   Undantag är hela eller halva dagar som måste uteslutas från schemat, till exempel helger eller företagsevenemang.

   >[!NOTE]
   >
   >Om du redan vet vilka de återkommande schemaundantagen är kan du definiera schemaundantagen för många år i framtiden.

   Du kan undanta hela eller delar av dagar från arbetsschemat. Klicka på datumet för att markera det som ett undantag och välj sedan **[!UICONTROL All day]** för att ange om undantaget är en hel dag eller inte.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Ange start- och sluttid för undantagen för partiella dagar.

   ![partiell-day-exception-on-schedules.png](assets/partial-day-exception-on-schedules.png)

1. Klicka **[!UICONTROL Save]** och sedan klicka **[!UICONTROL Save]Ändringar**.

1. (Valfritt) Associera schemat med en användare.

   Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Valfritt) Associera schemat med ett projekt.

   Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).
