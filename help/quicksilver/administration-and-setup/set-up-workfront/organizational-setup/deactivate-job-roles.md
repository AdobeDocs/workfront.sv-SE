---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Inaktivera jobbroller
description: Som en [!DNL Adobe Workfront] eller en användare med administrativ åtkomst till jobbroller kan du inaktivera jobbroller som blir inaktuella i systemet. När du inaktiverar en jobbroll i stället för att ta bort den, kan du behålla all associerad historikinformation.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---

# Inaktivera jobbroller

Som en [!DNL Adobe Workfront] eller en användare med administrativ åtkomst till jobbroller kan du inaktivera jobbroller som blir inaktuella i systemet. När du inaktiverar en jobbroll i stället för att ta bort den, kan du behålla all associerad historikinformation.

Du kan även återaktivera jobbroller som tidigare har inaktiverats.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] licens*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till jobbroller</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Effekten av att inaktivera jobbroller

Om du inaktiverar en jobbroll visas den inte längre i följande områden:

* The [!UICONTROL Assignments] typsnittsfält (för uppgifter, malluppgifter, utgåvor, godkännanden och routningsregler)
* The [!UICONTROL Assignments] fält i listor och rapporter
* Användarprofiler

   >[!NOTE]
   >
   >När du lägger till en ny roll för en användare visas ingen inaktiverad jobbroll. Men den visas fortfarande i [!UICONTROL Primary Role] och [!UICONTROL Other Roles] fält om användaren var associerad med jobbrollen innan den inaktiverades.

* The [!UICONTROL Sharing] dialogruta för objekt, inklusive tilldelning av layoutmall
* Typsnittsfält i anpassade formulär
* The [!UICONTROL Pool Members] fält i [!UICONTROL Resource Pools]
* The [!UICONTROL Job Role] fält i ett [!UICONTROL Billing Rate] redigeringsskärmen när en användare åsidosätter faktureringstaxor för projekt
* The [!UICONTROL Add assignment to Kanban board] i ett projekt
* The [!UICONTROL Job Role] när någon använder [!DNL Adobe Workfront Scenario Planner].

   The [!DNL Scenario Planner] är bara tillgängligt i nya [!DNL Adobe Workfront] upplevelse och kräver en extra licens. Mer information om [!DNL Workfront Scenario Planner], se [The [!DNL Scenario Planner] översikt](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Inaktiverade roller visas alltid i filter i listor, rapporter och andra verktyg som [!DNL Workload Balancer].

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

* Ta en inventering av alla godkännandeprocesser, aktuella godkännandesökvägar och routningsregler eller andra objekt som har tilldelats den jobbroll du tänker inaktivera och tilldela om dem till en aktiv roll.

   >[!TIP]
   >
   >Om du inaktiverar en jobbroll som tilldelats som standardtilldelad i en routningsregel när du använder begärandeköer, kvarstår rollen och begäranden dirigeras fortfarande till den inaktiverade rollen. Vi rekommenderar att du uppdaterar routningsregler med aktiva roller innan du inaktiverar teamet.

   Mer information om hur du skapar godkännandeprocesser och routningsregler finns i följande artiklar:

   * [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Inaktivera en jobbroll

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på &#x200B; i den vänstra panelen **[!UICONTROL Job Roles].**
1. (Valfritt) I dialogrutan **[!UICONTROL Filter]** nedrullningsbar meny, välja **[!UICONTROL Active]** om du bara vill visa aktiva jobbroller.
1. Klicka på namnet på den jobbroll som du vill inaktivera.
1. I **[!UICONTROL Is Active]** nedrullningsbar meny, välja **[!UICONTROL No]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klicka på **[!UICONTROL Save Changes]**.

   Jobbrollen är inaktiverad och kan inte längre tilldelas till arbete, associeras med layoutmallar och så vidare. Mer information om all användning av jobbroller i [!DNL Workfront], se [Översikt över jobbroll](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
