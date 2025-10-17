---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Skapa och ändra en grupps team
description: När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med team som är kopplade till gruppen och dess undergrupper.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 0%

---

# Skapa och ändra en grupps team

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med team som är kopplade till gruppen och dess undergrupper.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Mer information om hur användare med en planlicens kan skapa ett team finns i [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Mer information om hur en Workfront-administratör kan skapa ett team finns i [Skapa ett team från inställningsområdet](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa, arbeta med och skapa team för din grupp från gruppområdet

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen som du vill skapa eller ändra team för.
1. Klicka på **Team** ![Teams](assets/teams.png) i den vänstra panelen för att lista de team som är associerade med gruppen och med eventuella undergrupper.

1. Gör något av följande:

   * **Lägg till ett team**: Klicka på **Nytt team** och använd sedan följande alternativ för att konfigurera det:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Teamnamn</td> 
       <td>Skriv ett namn för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Grupp</td> 
       <td> <p> Systemet fyller i gruppfältet för det nya teamet med gruppen som du visar. Om du vill associera teamet med en annan grupp börjar du skriva namnet på gruppen och väljer sedan namnet när den visas.</p> <p>Du kan kontrollera att du associerar rätt grupp med gruppen genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p><b>Obs!</b> När ett team tilldelas en grupp eller undergrupp kan alla gruppadministratörer i den gruppen eller undergruppen hantera teamet utan att vara medlem i gruppen. Gruppadministratörer kan gå till Teams-området från huvudmenyn och klicka på pilen Byt team <img src="assets/switch-team-icon.png" alt="Byt ikon för team"> för att lista alla team som är tilldelade de grupper som de hanterar.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Teammedlemmar</td> 
       <td> <p>Börja skriva namnet på en användare som ska vara med i teamet och markera sedan namnet när det visas i listrutan. Upprepa den här processen om du vill lägga till flera användare i teamet.</p> <p>Det finns ingen gräns för hur många användare du kan lägga till i ett team. Vi rekommenderar dock att du inte har ett alltför stort antal användare i ett team eftersom teamets hantering kan bli alltför komplex.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beskrivning</td> 
       <td>Skriv en beskrivning för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Kalender</td> 
       <td>Välj vilken kalenderflik som ska visas för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Arbeta på den</td> 
       <td>Ändra knappen Arbeta på den till en Start-knapp. När en användare klickar på Start uppdateras objektets status automatiskt.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Knappen Klar</td> 
       <td>Välj den status som du vill ange för objekt när du klickar på knappen Klar.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Redigera team**: Välj minst ett team, klicka på **ikonen** Redigera ![ikonen Redigera](assets/edit-icon.png) och använd sedan följande alternativ för att konfigurera den:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Teamnamn</td> 
       <td>Skriv ett namn för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Grupp</td> 
       <td> <p>Associera teamet med en grupp. Börja skriva namnet på gruppen och markera sedan namnet när det visas.</p> <p>Du kan kontrollera att du associerar rätt grupp med gruppen genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p><b>Obs!</b> När ett team tilldelas en grupp eller undergrupp kan alla gruppadministratörer i den gruppen eller undergruppen hantera teamet utan att vara medlem i gruppen. Gruppadministratörer kan gå till Teams-området från huvudmenyn och klicka på pilen Byt team <img src="assets/switch-team-icon.png" alt="Byt ikon för team"> för att lista alla team som är tilldelade de grupper som de hanterar.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Ägare</td> 
       <td>Välj en ägare för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Teammedlemmar</td> 
       <td> <p>Lägg till och gruppmedlemmar. Börja skriva namnet på en användare och markera sedan namnet när det visas. Upprepa den här processen om du vill lägga till flera användare i teamet.</p> <p><b>TIPS</b>: Det finns ingen gräns för hur många användare du kan lägga till i ett team. Vi rekommenderar dock att du inte har ett alltför stort antal användare i ett team eftersom teamets hantering kan bli alltför komplex.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beskrivning</td> 
       <td>Skriv en beskrivning för teamet.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Layoutmall</td> 
       <td> <p>Börja skriva namnet på layoutmallen som du vill att teamet ska använda och klicka sedan på den när den visas.</p> <p>När du utser teamet med den här layoutmallen som hemteam för användare, kommer alla användare i det här teamet att se anpassningarna i den här layoutmallen.<br>De individuella layoutmallsinställningarna åsidosätter inställningarna för startteamets layoutmall. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Ange om det här är ett smidigt team. Mer information om flexibla team och hur du hanterar deras arbete finns i <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Skapa ett smidigt team</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Arbeta på den</td> 
       <td> <p>Ändra knappen Arbeta på den till en Start-knapp. När en användare klickar på Start uppdateras objektets status automatiskt.</p> <p>Mer information om hur du konfigurerar knappen Start finns i <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersätt knappen Work On It med knappen Start</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Knappen Klar</td> 
       <td> <p>Anpassa knappen Klar. Mer information finns i:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Konfigurera Klar-knappen för uppgifter</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Konfigurera Klar-knappen för problem</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Ta bort team**: Markera minst ett team och klicka sedan på ikonen Ta bort ![Ta bort](assets/delete.png).
   * **Exportera listan med team**: Klicka på **Exportera** ![Ikonen Exportera](assets/export.png) och välj sedan det filformat som du vill använda för den exporterade listan.
