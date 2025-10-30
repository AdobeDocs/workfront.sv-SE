---
title: Anpassa landningssidan med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Workfront-administratör kan du använda en layoutmall för att ange det område som du vill att användarna ska se varje gång de loggar in på Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 1%

---

# Anpassa landningssidan med en layoutmall

{{preview-fast-release-general}}

Som Adobe Workfront-administratör kan du använda en layoutmall för att ange det område som du vill att användarna ska se varje gång de loggar in på Workfront.

Användare kan öppna något av följande:

* Ett särskilt Workfront-område
* En anpassad kontrollpanel.

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>När Förfrågningar anges som landningssida kan användare som har tilldelats layoutmallen som deltagare eller begärande i stället se startsidan som landningssida. Rekommenderas att välja en annan landningssida än en begäran om layoutmallar som är avsedd för medverkande eller begärande användare?

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

## Anpassa landningssidan

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på **Markera landningssida** i det övre navigeringsområdet **och markera sedan det område som du vill att användarna ska se när de loggar in.**

   Välj bland följande områden eller lägg till en anpassad kontrollpanel:

   * Kalendrar
   * Kontrollpaneler
   * Dokument
   * Mål
   * Startsida
   * Mina uppdateringar
   * Portföljer
   * Program
   * Projekt
   * Rapporter
   * Begäranden
   * Resurser
   * Scenarier
   * Team
   * Mallar
   * Tidrapporter
   * Användare
   * Utkast
   * Planering

   >[!IMPORTANT]
   >
   >För att visa områdena Scenarier, Mål och Planning krävs ytterligare licenser.
   >
   >* Mer information om Workfront-mål finns i [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).
   >
   >* Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).
   >
   >* Mer information om Workfront Planning finns i [Översikt över Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

1. <span class="preview">I förhandsvisningsmiljön: Fortsätt anpassa layoutmallen. Du kan klicka på **Använd** när som helst för att spara förloppet.</span>

   <span class="preview">eller</span>

   <span class="preview">Om du är klar med anpassningen klickar du på **Spara och stäng**.</span>

1. I produktionsmiljön: Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

   >[!TIP]
   >
   >Du kan klicka på **Spara** när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
