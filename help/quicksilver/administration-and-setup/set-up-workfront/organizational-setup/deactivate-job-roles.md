---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Inaktivera jobbroller
description: Som  [!DNL Adobe Workfront] administratör eller en användare med administrativ åtkomst till jobbroller kan du inaktivera jobbroller som blir föråldrade i systemet. När du inaktiverar en jobbroll i stället för att ta bort den, kan du behålla all associerad historikinformation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Inaktivera jobbroller

Som administratör för [!DNL Adobe Workfront] eller användare med administrativ åtkomst till jobbroller kan du inaktivera jobbroller som blir föråldrade i systemet. När du inaktiverar en jobbroll i stället för att ta bort den, kan du behålla all associerad historikinformation.

Du kan även återaktivera jobbroller som tidigare har inaktiverats.

## Åtkomstkrav

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till jobbroller</td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Effekten av att inaktivera jobbroller

Om du inaktiverar en jobbroll visas den inte längre i följande områden:

* Typhuvudfältet [!UICONTROL Assignments] (för uppgifter, malluppgifter, utgåvor, godkännanden och routningsregler)
* Fälten [!UICONTROL Assignments] i listor och rapporter
* Användarprofiler

  >[!NOTE]
  >
  >När du lägger till en ny roll för en användare visas ingen inaktiverad jobbroll. Men den visas fortfarande i fälten [!UICONTROL Primary Role] och [!UICONTROL Other Roles] om användaren var associerad med jobbrollen innan den inaktiverades.

* Dialogrutan [!UICONTROL Sharing] för objekt, inklusive tilldelning av layoutmallar
* Typsnittsfält i anpassade formulär
* Fältet [!UICONTROL Pool Members] i [!UICONTROL Resource Pools]
* Fältet [!UICONTROL Job Role] i en [!UICONTROL Billing Rate]-redigeringsskärm när en användare åsidosätter faktureringstaxor för projekt
* [!UICONTROL Add assignment to Kanban board]-dialogrutan i ett projekt
* Fältet [!UICONTROL Job Role] för en plan eller ett initiativ när någon använder [!DNL Adobe Workfront Scenario Planner].

  [!DNL Scenario Planner] är bara tillgängligt i den nya [!DNL Adobe Workfront]-upplevelsen och kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i [Översikt [!DNL Scenario Planner] Översikt](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Inaktiverade roller visas alltid i filter i listor, rapporter och andra verktyg som [!UICONTROL Workload Balancer].

## Överväganden innan en jobbroll inaktiveras

Det är bättre att inaktivera i stället för att ta bort jobbroller som blir föråldrade så att du kan behålla all historik som är kopplad till roller som du har använt tidigare.

>[!NOTE]
>
>Allt arbete som tilldelats jobbrollen före inaktiveringen förblir tilldelat.

Vi rekommenderar att du gör följande innan du inaktiverar en oanvänd jobbroll:

* Skapa rapporter för alla objekt som har tilldelats den roll du tänker inaktivera och tilldela om dem till en aktiv jobbroll. Mer information om hur du skapar rapporter finns i [Skapa en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Du kan skapa en rapport för att filtrera efter uppgifter eller ärenden där den inaktiverade rollen har tilldelats. Använd sedan rapporten för att tilldela om utestående uppgifter eller ärenden till en aktiv roll.

* Ta en inventering av alla godkännandeprocesser, aktuella godkännandesökvägar och routningsregler eller andra objekt som har tilldelats den jobbroll som du planerar att inaktivera och tilldela om dem till en aktiv roll.

  >[!TIP]
  >
  >Om du inaktiverar en jobbroll som tilldelats som standardtilldelad i en routningsregel när du använder begärandeköer, kvarstår rollen och begäranden dirigeras fortfarande till den inaktiverade rollen. Vi rekommenderar att du uppdaterar routningsregler med aktiva roller innan du inaktiverar teamet.

  Mer information om hur du skapar godkännandeprocesser och routningsregler finns i följande artiklar:

   * [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Inaktivera en jobbroll

{{step-1-to-setup}}

1. Klicka på &#x200B; **[!UICONTROL Job Roles]i den vänstra panelen.**
1. (Valfritt) I listrutan **[!UICONTROL Filter]** väljer du **[!UICONTROL Active]** om du bara vill visa aktiva jobbroller.
1. Klicka på namnet på den jobbroll som du vill inaktivera.
1. Välj **[!UICONTROL Is Active]** i listrutan **[!UICONTROL No]**.

   ![Inaktivera jobbroll](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klicka på **[!UICONTROL Save Changes]**.

   Jobbrollen är inaktiverad och kan inte längre tilldelas till arbete, associeras med layoutmallar och så vidare. Mer information om all användning av jobbroller i [!DNL Workfront] finns i [Översikt över jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
