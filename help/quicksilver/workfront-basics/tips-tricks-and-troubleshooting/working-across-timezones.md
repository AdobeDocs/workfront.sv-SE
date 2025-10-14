---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Arbeta över tidszoner
description: Det kan vara praktiskt att förstå hur  [!DNL Adobe Workfront]  använder tidszoner för att beräkna tidsfält för objekt och tider i andra områden, som e-postmeddelanden.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 7697bb68e2042291e5290048cfc2f626145979af
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Arbeta över tidszoner

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Det kan vara praktiskt att förstå hur [!DNL Adobe Workfront] använder tidszoner för att beräkna följande:

* Tidsfält för objekt
* Antal gånger i andra [!DNL Workfront] områden, t.ex. automatiska Workfront-e-postmeddelanden

>[!WARNING]
>
>Om du inte hittar din exakta tidszon i listan som vi anger, söker du efter den tidszon som är närmast din och uppdaterar den för din instans.
>
>Tänk också på att en liknande tidszon kanske inte matchar din perfekt.
>
>En del länder eller territorier kan till exempel observera sommartid, men det är inte säkert att ditt land gör det. Om det behövs kan du behöva justera datorns tidszoner efter dessa ändringar.


## Tidszoner i [!DNL Workfront]

De tider du ser i [!DNL Workfront] baseras på tidszonskonfigurationer för din organisations [!DNL Workfront]-instans och för din användarprofil. Om de här två tidszonerna är olika kan du se tidsskillnader i olika områden och funktioner som du använder i [!DNL Workfront].

>[!NOTE]
>
>I ett anpassat formulär som bifogas till ett objekt beräknas och sparas datum- och tidssatser i beräknade anpassade fält med UTC (Coordinated Universal Time), inte med de tidszonskonfigurationer som angetts för organisationens instans och din användarprofil. Beräkningar i ett anpassat formulär genereras och visas baserat på varje användares enskilda tidszoner.

* [Din organisations [!DNL Workfront] instans](#your-organization-s-workfront-instance)
* [Din användarprofil](#your-user-profile)

### Din organisations [!DNL Workfront]-instans {#your-organization-s-workfront-instance}

Tidszonen för din organisations [!DNL Workfront]-instans anges vanligtvis för huvudkontorets plats. Detta avgör följande:

* Den tid som visas i e-postmeddelanden som genereras av [!DNL Workfront]
* Tidszonen för nytillagda användare (innan administratören för [!DNL Workfront] konfigurerar en annan tidszon för dem baserat på var de arbetar)

  Mer information om de här två exemplen finns i [Konfigurera grundläggande information för systemet](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Början eller slutet av en åsidosatt faktureringstaxa för ett projekt. Mer information finns i [Åsidosätt faktureringshastigheter för jobbroller på projektnivå](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Din användarprofil {#your-user-profile}

Fältet Tidszon i användarens profil styr den tid som visas i dina utgående e-postmeddelanden.

Tidszonen påverkar även vad som visas i en PTO-kalenderrapport.

Mer information om hur du konfigurerar tidszonen i din användarprofil finns i [Konfigurera mina inställningar](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Mer information om hur en [!DNL Workfront]-administratör (eller någon med [!UICONTROL Edit]-åtkomst till användare) kan konfigurera tidszonen i en användarprofil finns i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

### Webbläsarens tidszon

Tidszonen i webbläsaren bör konfigureras för den plats där du arbetar. Detta avgör följande:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Tider för ett objekt som du arbetar med, t.ex. start- och sluttider.

  Om användare i flera tidszoner tilldelas till ett objekt, konverterar [!DNL Workfront] objekttiderna för alla inblandade med hjälp av den tidszon som är konfigurerad i varje användares webbläsare.

  **EXEMPEL**
I EST-zonen (Eastern Standard Time), där du arbetar, ställer du in en uppgift att starta vid 16.00 och tilldela den till användare som arbetar i PST-zonen (Pacific Standard Time). :00 För dessa användare visas starttiden som :00 PM. Om det skulle visas som 4:00 PM skulle de börja jobba på det tre timmar sent.

  Om objektskaparen inte känner till skillnaden mellan de tilldelade tidszonerna och inte gör de nödvändiga justeringarna när objekttiderna anges, eller om de tilldelade inte vet den skillnaden, kan det vara svårt att få rätt timing medan alla samarbetar med objektet.

  **EXEMPEL**

  Du konfigurerar en endagsuppgift så att den startar kl. 9:00 EST, och glömmer att vissa användare arbetar med uppgiften i PST-zonen. För dem, starttid 6:00 förmiddag. Eftersom de inte kommer att börja arbeta med den förrän klockan nio på dagen (mitt på dagen) börjar aktiviteten och avslutas tre timmar senare.:00

Tidszonskonfigurationen skiljer sig mellan olika webbläsare. Mer information finns i respektive webbläsares dokumentation eller hjälpinformation.

## Hur man gör det enklare för användare att arbeta över tidszoner

Du kan hjälpa användare att arbeta enklare i flera tidszoner på flera sätt:

* [Använd scheman](#use-schedules)
* [Använd beräkningstidsfält i ett anpassat formulär](#use-calculated-time-fields-in-a-custom-form)
* [Använd textfält i stället för datumfält i ett anpassat formulär](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Använd scheman {#use-schedules}

[!DNL Workfront] administratörer skapar separata scheman för varje tidszon i organisationen för att se till att arbetet schemaläggs på rätt sätt för alla, oavsett var de befinner sig. När administratören har skapat scheman kan de associeras med vissa projekt och användare:

* **[!UICONTROL Projects]**: En projektskapare kan välja ett schema för ett enskilt projekt. Detta avgör schemaläggningen av aktiviteterna i projektet, baserat på de arbetstimmar som har angetts för de tilldelades tidszoner.
* **[!UICONTROL Users]**: En [!DNL Workfront]-administratör (eller någon med [!UICONTROL Edit] åtkomst till användare) kan välja ett schema för en enskild användare i användarens profil.

  Det här schemat kan skilja sig från ett projektschema. När någon skapar en uppgift i projektet och ännu inte har tilldelat någon till den, används till exempel projektschemat. När en användare tilldelas till uppgiften används användarens schema.

  Om flera användare tilldelas till en uppgift använder systemet något av följande, enligt inställningarna för projekt på system- eller gruppnivå:

   * Tidszonen för schemat för aktivitetens primära ägare
   * Tidszonen för schemat för projektet.

  Om en användare tilldelas till en uppgift använder systemet något av följande, enligt inställningarna i projekt som omfattar hela systemet eller hela gruppen:

   * Tidszonen för schemat för uppgiftens tilldelande
   * Tidszonen för schemat för projektet.

  Detta kan få aktivitetsdatum att ändras.

>[!BEGINSHADEBOX]

**EXEMPEL:**
En EST-användare tilldelas en endagsuppgift som ska starta kl. 9.00 PST, vilket är kl. 16.00 EST. :00 Eftersom EST-användaren endast har två återstående arbetstimmar för dagen, sträcker sig slutdatumet för uppgiften med cirka 6 timmar till nästa arbetsdag.


>[!ENDSHADEBOX]

Mer information om området [!UICONTROL Project Preferences] i [!UICONTROL Setup] finns i [Konfigurera systemomfattande projektinställningar](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Instruktioner om hur du tilldelar ett schema till ett projekt eller en användare finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Mer information om hur den tidszon som har konfigurerats i schemat påverkar distributionen av [!UICONTROL Planned Hours] i [!UICONTROL Workload Balancer] finns i [Hantera användarallokeringar i [!UICONTROL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Använd beräkningstidsfält i ett anpassat formulär {#use-calculated-time-fields-in-a-custom-form}

Du kan använda en serie beräknade anpassade fält i ett anpassat formulär för att visa den aktuella tiden för användare i organisationen, som en rad med flygplatsklockor som visar tiden i flera städer. Du kan skapa ett fält för var och en av de tidszoner där dina användare arbetar, där varje fält beräknar tiden för tidszonen.

Mer information finns i [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md), samt i avsnittet [Anpassade fält för datum och tid &#x200B;](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) i artikeln [Översikt över beräknade datamängder](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Använd textfält i stället för datumfält i ett anpassat formulär {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Om du inte vill att [!DNL Workfront] ska konvertera tider som du konfigurerar för i ett objekt för användare i olika tidszoner, kan du använda ett textfält i ett anpassat formulär som du kopplar till ett objekt, i stället för ett datumfält. På det här sättet visar tiden som du anger för alla i projektet.

Om du gör detta rekommenderar vi att du påminner formulärets användare om att beräkna skillnaden mellan deras tidszon och din så att de kan avgöra när arbetet ska börja och sluta. Du kan inkludera detta i instruktionerna som du skriver för det anpassade formuläret eller i ett verktygstips för det fältet. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
