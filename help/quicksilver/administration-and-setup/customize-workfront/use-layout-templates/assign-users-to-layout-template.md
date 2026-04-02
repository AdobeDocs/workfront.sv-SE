---
title: Tilldela användare till en layoutmall
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör kan du tilldela en layoutmall som du har skapat till användare, jobbroller, team eller grupper som behöver använda den.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Tilldela användare till en layoutmall

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

Du kan tilldela en layoutmall som du har skapat till alla användare, jobbroller, team eller grupper som behöver använda den.

För användare som inte har någon tilldelad layoutmall används standardlayouten. Mer information om standardlayouten finns i [Om standardlayouten för Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Användare kan också tilldela en layoutmall till sig själva enligt beskrivningen i Ändra områdena Mina arbets- och arbetsförfrågningar med layoutmallar.

Du kan tilldela flera olika layoutmallar till samma namn. Mer information om vilken layoutmall som används för en användare, roll, grupp eller team finns i [Prioritet för layoutmalltilldelning](#layout-template-assignment-priority) senare i den här artikeln.

Mer information om layoutmallar finns i [Layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

<span class="preview">Mer information om layoutmallar och affärsprofiler finns i [Översikt över affärsprofiler](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md).</span>

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
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.</p>
        <p>Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tilldela en layoutmall till användare

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >När du är nöjd med din layoutmall rekommenderar vi att du testar den enligt beskrivningen i [Testa en ny layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Klicka på **Tilldela den här till** i det övre avsnittet på sidan.
1. I rutan som visas klickar du på **Lägg till en användare, jobbroll, team, grupp <span class="preview"> eller åtkomstnivå</span>**. Börja skriva namnet på en användare, jobbroll, team, grupp <span class="preview"> eller åtkomstnivå </span> och klicka sedan på namnet när det visas i listrutan.

   Nyligen tillagda namn visas med blå bakgrund. Detta är praktiskt när du redigerar en befintlig layoutmall eftersom du kan skilja de namn du just har lagt till från de som redan finns i listan.

   En informationsikon ![Informationsikon](assets/info-icon.png) visas till höger om namnet på en användare, jobbroll, team, grupp <span class="preview"> eller åtkomstnivå </span> som redan har tilldelats en annan layoutmall. Du kan hålla muspekaren över ikonen för att se namnet på layoutmallen och bestämma om du vill åsidosätta det befintliga uppdraget.

1. Upprepa de två föregående stegen för att tilldela layoutmallen till andra användare, jobbroller, team, grupp <span class="preview">eller åtkomstnivå</span> efter behov.

   Du kan tilldela upp till 100 användare åt gången.

1. Klicka på **Klar** och sedan på **Spara och stäng** i det nedre vänstra hörnet.

   I det här steget slutförs processen att skapa och tilldela en layoutmall.

## Tilldelningsprioritet för layoutmall {#layout-template-assignment-priority}

Du och andra Workfront-administratörer kan tilldela flera olika layoutmallar till samma användare på följande fyra olika sätt:

* Till den enskilda användaren
* Till en viss jobbroll som användaren har
* För ett visst team är användaren på
* Till en viss grupp är användaren i
* <span class="preview">Till en viss åtkomstnivå tilldelas användaren till </span>

Användaren kan dock bara se en layoutmall åt gången. Mallen som är synlig avgörs av följande prioritetshierarki:

* **Individuell användare**: Layoutmallen som tilldelats personen som en enskild användare åsidosätter alla andra. Du kan åsidosätta en tidigare tilldelning som gjorts till en enskild användare genom att skapa en ny tilldelning. Den senaste tilldelningen har företräde.
* **Primär jobbroll**: Om personen inte har tilldelats en layoutmall som en enskild användare visas mallen som tilldelats för den primära jobbrollen.

  Endast layoutmallen som tilldelats en användares primära jobbroll är synlig för användaren. Mallar som tilldelats till sekundära jobbroller som innehas av användaren visas inte.

* **Hemteam**: Om personen inte har tilldelats en layoutmall som en enskild användare, eller som en användare med en primär jobbroll, ser han/hon mallen som tilldelats deras hemteam.

  Endast den mall som tilldelats en användares Hem-team är synlig för användaren. Mallar som tilldelats andra team där användaren är medlem visas inte.

* **Hemgrupp**: Om personen inte har tilldelats en layoutmall som en enskild användare, eller som en användare med en primär jobbroll, eller som medlem i ett Hem-team, ser han/hon mallen som tilldelats till hemgruppen.

  Endast den mall som tilldelats hemgruppen för en användare visas för användaren. Mallar som tilldelats någon av deras andra grupper visas inte.

* <span class="preview"> Åtkomstnivå: Om personen inte har tilldelats en layoutmall som en enskild användare, eller som en användare med en primär jobbroll, eller som medlem i ett Hem-team eller som medlem i en Hem-grupp, ser de mallen som tilldelats till deras åtkomstnivå.</span>

## Ett stort antal användare som tilldelats en layoutmall

<!--
If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
Om du har fler än 2 000 användare att tilldela till en layoutmall rekommenderar vi att du gör något av följande:

* Organisera användarna i grupper eller team och tilldela layoutmallen till dessa grupper eller team. Mer information finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) och [Skapa och hantera team](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Tilldela jobbroller till användarna och tilldela layoutmallen till deras primära jobbroll. Mer information finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
