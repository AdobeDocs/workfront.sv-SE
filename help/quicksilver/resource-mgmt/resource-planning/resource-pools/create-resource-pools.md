---
product-area: resource-management
navigation-topic: resource-pools
title: Skapa resurspooler
description: Resurspooler är användarsamlingar som gör det enklare att hantera resurser i Adobe Workfront. Mer information om resurspooler finns i Översikt över resurspooler.
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Skapa resurspooler

Resurspooler är användarsamlingar som gör det enklare att hantera resurser i Adobe Workfront. Mer information om resurspooler finns i [Översikt över resurspooler](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Redigera åtkomst till användare, projekt och mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för de projekt och mallar som du vill associera resurspoolerna med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en resurspool {#create-a-resource-pool}

1. Logga in som en användare som har behörighet att redigera resurspooler.\
   Mer information finns i [Skapa en resurspool](#create-a-resource-pool).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Resurser**.
1. Klicka **Resurspooler** i den vänstra panelen.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Klicka **Ny resurspool**.
1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Namn</strong></td>
      <td>Det här är namnet på resurspoolen.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beskrivning</strong></td>
      <td>Detta är en kort beskrivning av den här resurspoolen. Du kan till exempel ange för vilket syfte den ska användas.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Poolmedlemmar</strong></td>
      <td><p> Lägg till användare i resurspoolen separat.<br>eller <br>Om du vill lägga till ett stort antal användare samtidigt i resurspoolen. Du kan lägga till någon av följande entiteter som är kopplade till användare eller användarsamlingar:
        <ul>
         <li><strong>Team</strong>: alla medlemmar i gruppen läggs till i resurspoolen.</li>
         <li><strong>Grupper</strong>: alla medlemmar i gruppen läggs till i resurspoolen.</li>
         <li><strong>Roller</strong>: alla användare som är associerade med den rollen läggs till i resurspoolen.</li>
         <li><strong>Företag</strong>: alla användare i företaget läggs till i resurspoolen.</li>
        </ul><p>Tips: Du kan bara lägga till aktiva användare, team, <span>roller,</span> eller företag.</p><p>Obs! Om en användare blir medlem i en grupp, ett team, ett företag eller är associerad med en jobbroll efter att gruppen, teamet, företaget eller jobbrollen har lagts till i resurspoolen, läggs den nya medlemmen inte automatiskt till i resurspoolen. <br>Om en användare tillhör det team, den grupp, det företag och den jobbroll som du lägger till, läggs användaren bara till en gång i resurspoolen.<br>Användare som inaktiveras efter att ha lagts till i resurspoolen visas nedtonade i listan över användare och markeras som inaktiverade.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Valfritt) Använd **Ångra** för att ta bort användare som lagts till via en grupp, ett team, ett företag eller en jobbroll.

   >[!NOTE]
   >
   >Det finns ingen gräns för hur många användare du kan ha i en resurspool. Vi rekommenderar dock att du inte lägger till för många användare i en resurspool eftersom resurshantering annars kan bli en utmaning. I listan över användare visas endast de första 2 000 användarna i resurspoolen, och de visas i bokstavsordning.

   ![Resource_pools_NEW__UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Valfritt) Klicka på X-ikonen till höger om en användares namn för att ta bort en användare. Mer information om hur du tar bort användare från en resurspool finns i [Ta bort användare från resurspooler](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Valfritt) Använd **Sök** för att hitta en användare i resurspoolen.
1. Klicka **Skapa**.
