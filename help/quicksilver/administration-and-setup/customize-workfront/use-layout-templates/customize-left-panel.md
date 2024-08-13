---
title: Anpassa den vänstra panelen med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: I en layoutmall kan du anpassa vad användare ser i det vänstra panelområdet i hela Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Anpassa den vänstra panelen med en layoutmall

I en layoutmall kan du anpassa vad användarna ser i det vänstra panelområdet genom [!DNL Adobe Workfront].

Du kan till exempel ta reda på vilket av följande objekt som visas i den vänstra panelen när du visar en uppgift:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Ändringar som görs i ordning och synlighet återspeglas i mobilappen.

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> Om du vill utföra de här stegen på systemnivå måste du ha åtkomstnivån [!UICONTROL System Administrator].<p>Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Anpassa den vänstra panelen för ett område i [!DNL Workfront]:

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på nedpilen ![](assets/dropdown-arrow.png) under **[!UICONTROL Customize what users see]** och klicka sedan på den vänstra panelen som du vill anpassa.

   >[!NOTE]
   >
   >Mer information om alternativet [!UICONTROL Home] i den här listrutan finns i [Anpassa [!UICONTROL Home] och [!UICONTROL Summary] använda en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Mer information om alternativet Listor finns i [Anpassa filter, vyer och grupperingar med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. I listan **[!UICONTROL Left panel]** gör du något av följande för att avgöra vad som kommer att visas för det alternativ ([!DNL Workfront] område eller objekttyp) som du har valt i den vänstra panelen:

   * Visa ![](assets/add-secondary-nav-item.png) eller dölj ![](assets/delete-secondary-nav-item.png) objekt. Objekt utan ![](assets/add-secondary-nav-item.png) eller ![](assets/delete-secondary-nav-item.png) kan inte döljas.

   * Dra objekt ![](assets/move-icon---dots.png) för att ändra deras ordning på den vänstra panelen.
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Alternativ</th> 
      <th>När användare klickar på följande..</th> 
      <th>De ser de objekt i den vänstra panelen som du väljer bland följande:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>Namnet på ett projekt</td> 
      <td>[!UICONTROL Tasks], [!UICONTROL Project Details], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issues], [!UICONTROL Risks], [!UICONTROL Approvals], [!UICONTROL Baselines], [!UICONTROL Billing Rates], [!UICONTROL Billing Records], [!UICONTROL Expenses], [!UICONTROL Hours], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Namnet på en uppgift</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Predecessors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>Namnet på en utgåva</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issue Details], [!UICONTROL Hours], [!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Namnet på en portfölj</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programs], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio] [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Namnet på ett program</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Namnet på en projektmall</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>Namnet på en malluppgift</td> 
      <td>[!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>Namnet på en faktureringspost för ett projekt</td> 
      <td>[!UICONTROL Billing Record Details], [!UICONTROL Billable Hours], [!UICONTROL Billable Expenses], [!UICONTROL Fixed Revenues]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Projekt <img src="assets/projects-in-main-menu.png"> i [!UICONTROL Main menu] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>Namnet på en begäran</td> 
      <td>[!UICONTROL New Request], [!UICONTROL Submitted requests], [!UICONTROL All Requests], [!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Namnet på en instrumentpanel</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b>Obs!</b> Om du har skapat anpassade flikar för området [!UICONTROL Reports] med hjälp av en layoutmall i [!DNL Adobe Workfront Classic] visas de längst ned i listan. För användare visas de längst ned på den vänstra panelen i området [!UICONTROL Dashboards].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Namnet på ett Scrum-team</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>OBS!</strong> Objektet <strong>[!UICONTROL Current iteration]</strong> visas bara på den vänstra panelen när det finns minst en uppgift eller ett problem i iterationen.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>Namnet på ett Kanban-team</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>Namnet på ett Waterfall-team</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>Namnet på en iteration</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >De sista tre objekten i listrutan **[!UICONTROL Customize what users see]** ([!UICONTROL Lists], [!UICONTROL Home and Summary] och [!UICONTROL Branding]) används för att konfigurera andra områden än den vänstra panelen. Mer information om dem finns i följande artiklar:
>   >   
* [Anpassa filter, vyer och grupperingar med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Anpassa [!UICONTROL Home] och [!UICONTROL Summary] med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Märke Adobe [!DNL Workfront] med en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Valfritt) Om du vill lägga till ett vänsterpanelsobjekt som länkar till någon av organisationens kontrollpaneler klickar du på **[!UICONTROL Add custom section]**, skriver **[!UICONTROL Custom section title]** för objektet och lägger sedan till kontrollpanelen.

   Instrumentpanelsobjekt visas längst ned på den vänstra panelen. Användarna ser den anpassade avsnittsrubrik som du skriver bredvid instrumentpanelsobjektet när de hovrar över den vänstra panelen.

   >[!NOTE]
   >
   Användarna kan lägga till anpassade kontrollpanelsobjekt på sin egen vänstra panel. När du lägger till anpassade kontrollpanelsobjekt i en layoutmall sammanfogas objekten med deras, utan att de skrivs över eller återställs. Detta gäller även om du tilldelar användare till en ny layoutmall med anpassade instrumentpanelsobjekt. Mer information om hur användare kan anpassa den vänstra panelen finns i [Skapa anpassade flikar eller avsnitt](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Mer information om kontrollpaneler finns i [Kontrollpaneler](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **[!UICONTROL Save]**.

   >[!TIP]
   >
   Du kan klicka på [!UICONTROL Save] när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
