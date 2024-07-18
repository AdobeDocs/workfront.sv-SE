---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Åtkomst till  [!DNL Adobe Workfront] objekt från en delad länk i [!DNL Slack]
description: När länkar till [!DNL Adobe Workfront] -objekt delas med dig i en Slack-kanal kan du visa ytterligare information om dem i Slack efter att du har installerat och konfigurerat  [!DNL Workfront]  för Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 587c6ac7-cc56-480f-852d-f0bd36b3f3cf
source-git-commit: eeb90d8f80b1680d880d07f41e9d80c0658495fa
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 0%

---

# Åtkomst till [!DNL Adobe Workfront]-objekt från en delad länk i [!DNL Slack]

När länkar till [!DNL Adobe Workfront]-objekt delas med dig i en [!DNL Slack]-kanal kan du visa ytterligare information om dem i [!DNL Slack] efter att du har installerat och konfigurerat [!DNL Workfront for Slack].

Mer information om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Du måste vara inloggad på [!DNL Workfront] på en separat webbläsarflik för att kunna öppna länken eller utföra ytterligare åtgärder på dessa objekt från [!DNL Slack].

När en användare delar en länk till ett objekt i [!DNL Workfront] med dig, kan ytterligare information om objektet också visas tillsammans med länken. Användaren som skickar länken måste ha minst [!UICONTROL View] behörigheter till objektet för att ytterligare information ska kunna visas i [!DNL Slack].

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda de funktioner som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan komma åt dina favoriter och senaste objekt från [!DNL Slack] måste du

* Konfigurera [!DNL Workfront for Slack]\
   Instruktioner om hur du konfigurerar [!DNL Workfront for Slack] finns i [Konfigurera [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Åtkomst till projekt från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront from Slack.]

   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront from Slack] i [Åtkomst [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till ett [!DNL Workfront]-projekt.

   >[!NOTE]
   >
   >Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter till projektet för att du ska kunna se ytterligare information om det.

1. (Valfritt) Klicka på projektets namn för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
1. Titta på följande ytterligare information om projektet:

   * **[!UICONTROL Status]:** Mer information om projektstatus finns i [Öppna listan över systemprojektstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

   * **[!UICONTROL Planned Completion Date]**: Mer information om det planerade slutförandedatumet finns i [Ange projektets planerade slutförandedatum](../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

   * **[!UICONTROL Portfolio]** Namn: Mer information om portföljer finns i [Översikt över Portfolio i Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   * **[!UICONTROL Condition]**: Mer information om projektvillkor finns i [Översikt över projektvillkor och villkorstyp](../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   * **[!UICONTROL Percent Complete]**: Mer information om Procent färdigt i ett projekt finns i [Översikt över Procent färdigt](../../manage-work/tasks/task-information/project-percent-complete.md).

   * **[!UICONTROL Reference Number]**: Mer information om referensnummer för objekt finns i [Använda referensnummer för objekt](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

1. (Valfritt) Klicka på **[!UICONTROL Subscribe]** om du vill prenumerera på projektet.

   Du får en bekräftelse på att du har prenumererat på projektet.

## Åtkomst till aktiviteter från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront from Slack].

   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till en [!DNL Workfront]-aktivitet.

   >[!NOTE]
   >
   >Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter för aktiviteten för att du ska kunna se ytterligare information om den.

1. (Valfritt) Klicka på aktivitetens namn för att öppna den i [!DNL Workfront] på en ny webbläsarflik.
1. Titta på följande ytterligare information om uppgiften:

   * **[!UICONTROL Status]**

     Mer information om aktivitetsstatus finns i [Åtkomst till listan över systemaktivitetsstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md).

   * **[!UICONTROL Percent Complete]**
   * **[!UICONTROL Assigned To Name]**
   * **[!DNL Planned Completion Date]**
   * **[!UICONTROL Project Name]** eller **[!UICONTROL Parent Task Name]**
   * **[!UICONTROL Reference Number]**

     Mer information om objektreferensnummer finns i [Använda referensnummer för objekt](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

1. (Valfritt) Klicka på **[!UICONTROL Subscribe]** om du vill prenumerera på uppgiften.

   Du får en bekräftelse på att du har prenumererat på uppgiften.

1. (Valfritt) Klicka på **[!UICONTROL Assign to user]** om du vill tilldela en användare uppgiften.
1. (Villkorligt) Börja skriva namnet på en användare om du har klickat på **[!UICONTROL Assign to user]**.

   Du kan inte tilldela en uppgift till en jobbroll eller ett team från [!DNL Slack].

## Åtkomstproblem från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].

   Mer information om hur du loggar in på Workfront från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till ett [!DNL Workfront]-problem.

   >[!NOTE]
   >
   >Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter för problemet för att du ska kunna se ytterligare information om det.

1. (Valfritt) Klicka på problemets namn för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
1. Titta på följande ytterligare information om uppgiften:

   * **[!UICONTROL Status]**: Mer information om utgivningsstatus finns i [Åtkomst till listan över status för systemutleverans](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

   * **[!UICONTROL Assigned To Name]**
   * **[!UICONTROL Planned Completion Date]**
   * **[!UICONTROL Project Name]**
   * **[!UICONTROL Reference Number]**: Mer information om referensnummer för objekt finns i [Använda referensnummer för objekt](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

1. (Valfritt) Klicka på **[!UICONTROL Subscribe]** om du vill prenumerera på problemet.

   Du får en bekräftelse på att du har prenumererat på problemet.

1. (Valfritt) Klicka på **[!UICONTROL Assign to user]** för att tilldela utgåvan till en användare.
1. (Villkorligt) Börja skriva namnet på en användare om du har klickat på **[!UICONTROL Assign to user]**.

   Du kan inte tilldela en utgåva till en jobbroll eller ett team från [!DNL Slack].

## Åtkomst till portföljer från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].

   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till en [!DNL Workfront]-portfölj.

   >[!NOTE]
   >
   >Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter till portföljen för att du ska kunna se ytterligare information om den.

1. (Valfritt) Klicka på namnet på portföljen för att öppna den i [!DNL Workfront] på en ny webbläsarflik.
1. Titta på följande ytterligare information om portföljen:

   * **[!UICONTROL Portfolio Manager Name]**
   * **[!UICONTROL On Time]**
   * **[!UICONTROL ROI]**
   * **[!UICONTROL Net Value]**
   * **[!UICONTROL Status]**
   * **[!UICONTROL On Budget]**
   * **[!UICONTROL Aligned]**

     Mer information om portföljmått, inklusive [!UICONTROL ROI], [!UICONTROL Net Value], [!UICONTROL Alignment], [!UICONTROL On Time] och [!UICONTROL On Budget], finns i [Förstå [!UICONTROL Portfolio Optimizer].](../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Åtkomst till program från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].

   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till ett [!DNL Workfront]-program.

   >[!NOTE]
   >
   > Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter till programmet för att du ska kunna se ytterligare information om det.

1. (Valfritt) Klicka på namnet på programmet för att öppna det i [!DNL Workfront] på en ny webbläsarflik.
1. Titta på följande ytterligare information om programmet:

   * **[!UICONTROL Description]**
   * **[!UICONTROL Portfolio Name]**
   * **[!UICONTROL Program Manager Name]**

     Mer information om program finns i [Skapa och hantera program.](../../manage-work/portfolios/create-and-manage-programs/create-and-manage-programs.md)

## Få åtkomst till rapporter från [!DNL Slack]

1. Logga in på din [!DNL Slack]-instans och logga in på [!DNL Workfront] från [!DNL Slack].

   Mer information om hur du loggar in på [!DNL Workfront] från [!DNL Slack] finns i avsnittet Logga in på [!DNL Workfront] från [!DNL Slack] i [Åtkomst [!DNL Adobe Workfront] från [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Navigera till ett meddelande som innehåller en länk till en [!DNL Workfront]-rapport.

   >[!NOTE]
   >
   >Användaren som delar länken måste ha minst [!UICONTROL View] behörigheter till rapporten för att du ska kunna se ytterligare information om den.

1. (Valfritt) Klicka på rapportens namn för att öppna den i [!DNL Workfront] på en ny webbläsarflik.
