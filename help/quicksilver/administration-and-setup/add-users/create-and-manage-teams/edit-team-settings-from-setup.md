---
title: Redigera inställningar för ett team i inställningsområdet
description: Som Adobe Workfront-administratör kan du redigera ett teams inställningar under Konfigurera. Du kan lägga till användare i ett team, ange teamets layoutmall och ange hur status ska registreras när arbetsobjekten slutförs av ett team.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Redigera inställningar för ett team från inställningsområdet

Som Adobe Workfront-administratör kan du redigera ett teams inställningar under Konfigurera. Du kan lägga till användare i ett team, ange teamets layoutmall och ange hur status ska registreras när arbetsobjekten slutförs av ett team.

Mer information om team finns i [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* En gruppadministratör kan redigera ett teams inställningar för en grupp som de administrerar. Mer information finns i [Skapa och ändra en grupps team](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* En användare med en planlicens kan redigera ett teams inställningar från området Personer. Mer information finns i [Redigera gruppinställningar](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Redigera inställningar för ett team

{{step-1-to-setup}}

1. Klicka på **Team** i den vänstra panelen.
1. Välj ett team och klicka sedan på **Redigera** ![](assets/edit-icon.png).

1. Gör någon av följande ändringar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Teamnamn</td> 
      <td>Skriv ett namn för teamet.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Är aktiv </td> 
       <td>Det här alternativet är aktiverat som standard för nya och befintliga team. Inaktivera det för att inaktivera teamet. Mer information finns i <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Inaktivera ett team</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupp</td> 
      <td> <p>Associera teamet med en grupp. Börja skriva namnet på gruppen och markera sedan namnet när det visas.</p> <p><b>Obs!</b> När ett team tilldelas en grupp eller undergrupp kan alla gruppadministratörer i den gruppen eller undergruppen hantera teamet utan att vara medlem i gruppen. Gruppadministratörer kan gå till Teams-området från huvudmenyn och klicka på pilen Byt team <img src="assets/switch-team-icon.png" alt="Byt ikon för team"> för att lista alla team som är tilldelade de grupper som de hanterar.</p> <p>Du kan kontrollera att du associerar rätt grupp med gruppen genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ägare</td> 
      <td>Välj en ägare för teamet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Teammedlemmar</td> 
      <td> <p>Lägg till och gruppmedlemmar. Börja skriva namnet på en användare och markera sedan namnet när det visas. Upprepa den här processen om du vill lägga till flera användare i teamet.</p> 
      <p><b>TIPS</b>: Du kan lägga till valfritt antal användare i ett team. Vi rekommenderar dock att du inte lägger till ett för stort antal i ett team eftersom teamets arbetsledning kan bli alltför komplex.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv en beskrivning för teamet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Layoutmall</td> 
      <td> <p>Börja skriva namnet på layoutmallen som du vill att teamet ska använda och klicka sedan på den när den visas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Ange om det här är ett smidigt team. Mer information om flexibla team och hur du hanterar deras arbete finns i <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Skapa ett smidigt team</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Klicka på **Spara ändringar**.
