---
title: Anpassa fästa sidor med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: I en layoutmall kan du fästa de sidor som du vill att användarna alltid ska ha tillgängliga överst i Adobe Workfront. Dessa kan antingen vara sidor som du kommer åt via huvudmenyn eller kontrollpaneler.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 0e7000597e2347bff0bc626d21aa9a6c9a839c0b
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# Anpassa fästa sidor med en layoutmall

I en layoutmall kan du fästa de sidor som du vill att användarna alltid ska ha tillgängliga överst i Adobe Workfront. Dessa kan antingen nås via huvudmenyikonen ![Huvudmeny](assets/main-menu-icon.png) eller huvudmenyikonen ![Huvudmeny](assets/main-menu-icon-left-nav.png) om den är tillgänglig, eller via kontrollpaneler.

Alla punkter som användarna har lagt till separat visas till höger om de punkter som du lägger till i layoutmallen.

Mer information om att fästa sidor finns i [Fäst sidor för att anpassa arbetsytan](../../../workfront-basics/the-new-workfront-experience/pin-pages.md).

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

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
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fästa sidor med en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Under **Övre navigeringsområdet** klickar du på **Lägg till nytt häftstift**.

1. Gör något av följande i listrutan som visas:

   * Välj bland följande områden:

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
     >För att visa mål-, scenario- och planeringsområdena krävs ytterligare licenser.
     >
     >* Mer information om Workfront-mål finns i [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).
     >
     >* Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).
     >
     >* Mer information om Workfront Planning finns i [Översikt över Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Klicka på **Lägg till en instrumentpanel**
      * Skriv ett beskrivande namn i fältet <!--**Quick link name**-->**Eget namn**
      * Välj en instrumentpanel i fältet **Lägg till en instrumentpanel** <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now -->
      * Klicka på **Lägg till**.

1. Upprepa föregående steg om du vill fästa andra sidor.

1. (Valfritt) Om du vill flytta ett häftstift håller du pekaren över stiftet och klickar på ikonen Mer ![Mer](assets/more-icon.png) bredvid nålnamnet. Klicka sedan på **Flytta åt vänster** eller **Flytta åt höger** om du vill flytta stiftet i vald riktning eller på **Flytta längst fram** om du vill flytta stiftet till den vänstra positionen.

1. (Valfritt) Om du vill byta namn på ett häftstift håller du pekaren över stiftet och klickar på ikonen Mer ![Mer](assets/more-icon.png) bredvid nålnamnet. Klicka sedan på **Byt namn på häftstiftet**. Ange ett nytt namn och klicka sedan på **Spara**.

1. (Valfritt) Om du vill ta bort ett häftstift håller du pekaren över stiftet och klickar på ikonen Mer ![Mer](assets/more-icon.png) bredvid nålnamnet. Klicka sedan på **Ta bort häftstift**.

1. Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

   >[!TIP]
   >
   >Du kan klicka på **Spara** när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
