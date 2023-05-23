---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Arbeta över tidszoner
description: Det kan vara till hjälp att förstå hur [!DNL Adobe Workfront] använder tidszoner för att beräkna tidsfält för objekt och tidpunkter i andra områden, t.ex. e-postmeddelanden.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Arbeta över tidszoner

Det kan vara till hjälp att förstå hur [!DNL Adobe Workfront] använder tidszoner för att beräkna följande:

* Tidsfält för objekt
* Times in other [!DNL Workfront] områden, t.ex. automatiska e-postmeddelanden från Workfront

## Tidszoner i [!DNL Workfront]

Times du ser in [!DNL Workfront] baseras på tidszonskonfigurationer för din organisations [!DNL Workfront] -instans och för din användarprofil. Om de här två tidszonerna är olika kan du se tidsskillnader i olika områden och funktioner som du använder i [!DNL Workfront].

>[!NOTE]
>
>I ett anpassat formulär som bifogas till ett objekt beräknas och sparas datum- och tidssatser i beräknade anpassade fält med UTC (Coordinated Universal Time), inte med de tidszonskonfigurationer som angetts för organisationens instans och din användarprofil. Beräkningar i ett anpassat formulär genereras och visas baserat på varje användares enskilda tidszoner.

* [Din organisations [!DNL Workfront] instance](#your-organization-s-workfront-instance)
* [Din användarprofil](#your-user-profile)

### Din organisations [!DNL Workfront] instance {#your-organization-s-workfront-instance}

Tidszonen för din organisations [!DNL Workfront] -instansen anges vanligtvis för huvudkontorets plats. Detta avgör följande:

* Den tid som visas i e-postmeddelanden som genereras av [!DNL Workfront]
* Tidszonen för nytillagda användare (före [!DNL Workfront] administratör konfigurerar en annan tidszon för dem baserat på var de arbetar)

   Mer information om de här två exemplen finns i [Konfigurera grundläggande information för ditt system](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Början eller slutet av en åsidosatt faktureringstaxa för ett projekt. Mer information finns i [Åsidosätt faktureringshastigheter för jobbroller på projektnivå](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Din användarprofil {#your-user-profile}

Tidszonen i din användarprofil bör konfigureras för den plats där du arbetar. Detta avgör följande:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Tider för ett objekt som du arbetar med, t.ex. start- och sluttider

   Om användare i flera tidszoner tilldelas till ett objekt, [!DNL Workfront] konverterar objekttiderna för alla berörda med hjälp av den tidszon som har konfigurerats i varje användarprofil.

   **Exempel:** I EST-zonen (Eastern Standard Time), där du arbetar, ställer du in en uppgift att starta vid 17:00 och tilldelar den till användare som arbetar i PST-zonen (Pacific Standard Time). För dessa användare visas starttiden som 1:00 PM. Om det skulle visas som 17:00 skulle de börja jobba på det tre timmar sent.

   Om objektskaparen inte kan se skillnaden mellan de tilldelade tidszonerna och göra nödvändiga justeringar när objekttiderna anges, eller om de tilldelade inte noterar skillnaden, kan det vara svårt att få rätt timing medan alla samarbetar med objektet.

   **Exempel:** Du konfigurerar en endagsuppgift så att den startar kl. 9.00 EST, och glömmer att vissa användare arbetar med uppgiften i PST-zonen. För dem är starttiden 06:00. Eftersom de inte kommer att börja arbeta på den förrän klockan nio (mitt på dagen) börjar uppgiften och avslutas tre timmar sen.

Mer information om hur du konfigurerar tidszonen i din användarprofil finns i [Konfigurera mina inställningar](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

För information om hur en [!DNL Workfront] administratör (eller någon med [!UICONTROL Edit] behörighet för användare) kan konfigurera tidszonen i en användarprofil, se [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Hur man gör det enklare för användare att arbeta över tidszoner

Du kan hjälpa användare att arbeta enklare i flera tidszoner på flera sätt:

* [Använd scheman](#use-schedules)
* [Använd beräkningstidsfält i ett anpassat formulär](#use-calculated-time-fields-in-a-custom-form)
* [Använd textfält i stället för datumfält i ett anpassat formulär](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Använd scheman {#use-schedules}

[!DNL Workfront] administratörer skapar separata scheman för varje tidszon i organisationen för att säkerställa att arbetet schemaläggs på rätt sätt för alla, oavsett var de befinner sig. När administratören har skapat scheman kan de associeras med vissa projekt och användare:

* **[!UICONTROL Projects]**: En projektskapare kan välja ett schema för ett enskilt projekt. Detta avgör schemaläggningen av aktiviteterna i projektet, baserat på de arbetstimmar som har angetts för de tilldelades tidszoner.
* **[!UICONTROL Users]**: A [!DNL Workfront] administratör (eller någon med [!UICONTROL Edit] åtkomst till användare) kan välja ett schema för en enskild användare i användarens profil.

   Det här schemat kan skilja sig från ett projektschema. När någon skapar en uppgift i projektet och ännu inte har tilldelat någon till den, används till exempel projektschemat. När en användare tilldelas till uppgiften används användarens schema.

   Om flera användare tilldelas till en uppgift använder systemet något av följande, som konfigurerats i projektinställningarna för hela systemet:

   * Tidszonen för schemat för aktivitetens primära ägare
   * Tidszonen för schemat för projektet.

   Detta kan få aktivitetsdatum att ändras.

   **Exempel:** En EST-användare tilldelas en endagsuppgift som schemaläggs att starta kl. 9.00 PST, vilket är kl. 19.00 EST. Eftersom EST-användaren endast har två återstående arbetstimmar för dagen, sträcker sig slutdatumet för uppgiften med cirka 6 timmar till nästa arbetsdag.

   Mer information om [!UICONTROL Project Preferences] område på [!UICONTROL Setup], se [Konfigurera systemomfattande projektinställningar](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Instruktioner om hur du tilldelar ett schema till ett projekt eller en användare finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Information om hur den tidszon som konfigurerats i schemat påverkar distributionen av [!UICONTROL Planned Hours] i [!DNL Workload Balancer], se [Hantera användarallokeringar i [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Använd beräkningstidsfält i ett anpassat formulär {#use-calculated-time-fields-in-a-custom-form}

Du kan använda en serie beräknade anpassade fält i ett anpassat formulär för att visa den aktuella tiden för användare i organisationen, som en rad med flygplatsklockor som visar tiden i flera städer. Du kan skapa ett fält för var och en av de tidszoner där dina användare arbetar, där varje fält beräknar tiden för tidszonen.

Mer information finns i [Lägga till beräknade data i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)samt avsnittet [Datum och tid för beräknade anpassade fält](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) i artikeln [Beräknade datauttryck](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Använd textfält i stället för datumfält i ett anpassat formulär {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Om du inte vill [!DNL Workfront] om du vill konvertera tider som du konfigurerar för ett objekt för användare i olika tidszoner, kan du använda ett textfält i ett anpassat formulär som du kopplar till ett objekt, i stället för ett datumfält. På så sätt visar tiden den tid du skriver för alla i projektet.

Om du gör detta rekommenderar vi att du påminner formulärets användare om att beräkna skillnaden mellan deras tidszon och din så att de kan avgöra när arbetet ska börja och sluta. Du kan inkludera detta i instruktionerna som du skriver för det anpassade formuläret eller i ett verktygstips för det fältet. Mer information finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
