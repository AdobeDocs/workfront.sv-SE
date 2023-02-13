---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: The [!DNL Adobe Workfront] Förhandsgranska sandlådemiljö
description: Sandlådan för förhandsgranskning är en testmiljö som fungerar som en kopia av din livemiljö. Den uppdateras varje helg av Workfront. Data som läggs till i din livemiljö på fredag visas i din förhandsvisningssandlåda senast följande måndag. Alla supportpaket har åtkomst till den här sandlådan.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---

# The [!DNL Adobe Workfront] Förhandsgranska sandlådemiljö

Det finns två testmiljöer för [!DNL Workfront] som är kopior av [!DNL Workfront] produktionsmiljö:

* Sandlådan Förhandsgranska

   Sandlådan Preview är en testmiljö som fungerar som en kopia av din aktiva miljö och uppdateras varje helg av [!DNL Workfront]. Data som läggs till i din livemiljö på fredag visas i din förhandsvisningssandlåda senast följande måndag.

   Alla supportpaket har tillgång till förhandsvisnings-sandlådan.

* Sandlådan Anpassad uppdatering

   Sandlådan för anpassad uppdatering är en separat testmiljö som uppdateras manuellt av dig. Det finns en extra kostnad för att hämta den anpassade uppdateringssandlådan. Mer information om den här miljön finns i [The [!DNL Adobe Workfront] Anpassad miljö för uppdatering av sandlådan](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Supportpaket</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred]och [!UICONTROL Enterprise] Supportpaket</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Förhandsgranska sandlåda</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Anpassad uppdateringssandlåda</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förhandsgranska sandlåda

Sandlådan Preview fungerar som en miljö där användare i organisationen kan testa och arbeta med data från produktionsmiljön utan att påverka produktionsmiljön.

Sandlådan Preview innehåller dina faktiska produktionsdata; Men den uppdateras varje helg så att data kan ligga upp till en vecka bakom produktionsmiljön. Objekt som har skapats sedan den senaste uppdateringstiden finns i förhandsvisningens sandlådemiljö tills nästa uppdatering.

Data flödar åt samma håll, från produktion till förhandsgranskning, och inte åt andra hållet. En uppdatering av förhandsvisningsmiljön schemaläggs alltid av [!DNL Workfront] varje helg. Mer information om uppdateringens specifika dag och tid finns på [status.adobe.com](https://status.adobe.com/).

Förhandsgranska sandlådan tillåter även [!DNL Workfront] för att driftsätta nya funktioner i en säker miljö, innan de är klara att driftsättas för produktion. Du kan testa de nya funktionerna och ge [!DNL Workfront] ge feedback om deras funktionalitet genom att gå till förhandsgranskningssandlådan. Därför ligger koden för förhandsvisningssandlådan alltid före produktionskoden, även om dina data uppdateras varje vecka.

Förhandsvisningsmiljön är idealisk för att köra utbildning, testa nya funktioner och fastställa installationsfunktioner.

>[!NOTE]
>
>Lägg märke till den blå banderollen högst upp på skärmen när du öppnar förhandsvisningssandlådan. Banderollen kan inte tas bort medan du arbetar i den här miljön.
>
>Namnet på miljön som du använder (förhandsversion) och den officiella versionen av koden visas på banderollen. Klicka **[!UICONTROL See what's new]** för information om den versionen.
>
>![](assets/preview-banner-nwe-350x161.png)

## Åtkomst till sandlådan Förhandsgranska

Som standard, som [!DNL Workfront] administratör, du har åtkomst till [!UICONTROL Preview] Sandlådemiljö. Om du inte har åtkomst till [!UICONTROL Preview] Sandlådemiljö enligt beskrivningen i det här avsnittet, kontakta [!DNL Workfront] eller vårt kundsupportteam.

* [Få åtkomst till sandlådan Förhandsvisa från [!DNL Workfront] Gränssnitt](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Åtkomst till förhandsvisningssandlådan med en URL](#accessing-the-preview-sandbox-using-a-url)

### Få åtkomst till sandlådan Förhandsvisa från [!DNL Workfront] Gränssnitt {#accessing-the-preview-sandbox-from-the-workfront-interface}

Som [!DNL Workfront] -administratör kan du komma åt sandlådan Preview via [!DNL Workfront] gränssnitt.

Så här kommer du åt förhandsvisningssandlådan:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. I **[!UICONTROL Test Environments]** avsnitt, klicka **[!UICONTROL Sandbox Preview]**.

1. Logga in med dina autentiseringsuppgifter för förhandsgranskning.

   Dessa bör vara samma som dina produktionsuppgifter, såvida du inte har ändrat dem i Production efter att Preview-uppdateringen har utförts. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

### Åtkomst till förhandsvisningssandlådan med en URL {#accessing-the-preview-sandbox-using-a-url}

* [Åtkomst till förhandsgranskningssandlådan för konton i kluster 1,2,3 och 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Åtkomst till sandlådan Preview för konton i kluster 4 (EMEA-konton)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Åtkomst till förhandsgranskningssandlådan för konton i kluster 1,2,3 och 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Du har tidigare använt sandlådan Preview genom att gå till [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Den här URL:en stöds inte längre och den har inte omdirigerats till vår nya URL för förhandsvisningssandlådemiljön. Den nya korrekta URL:en för förhandsvisningssandlådan är: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Om du har bokmärken som länkar till den gamla URL:en för förhandsvisningssandlådan, bör du notera den här ändringen och uppdatera URL:en i bokmärkena.

Så här loggar du in i förhandsvisningssandlådan med en URL:

1. Navigera till denna URL: [[!DNL https]/companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Om du är EMEA-kund och ditt konto finns i kluster 4, se avsnittet [Åtkomst till sandlådan Preview för konton i kluster 4 (EMEA-konton)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) i den här artikeln.

1. Logga in med dina autentiseringsuppgifter för förhandsgranskning.

   Dina autentiseringsuppgifter för förhandsgranskning bör vara desamma som dina produktionsuppgifter, såvida du inte har ändrat dem i Produktion efter att uppdateringen av förhandsvisningen har ägt rum. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

#### Åtkomst till sandlådan Preview för konton i kluster 4 (EMEA-konton) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Så här loggar du in i förhandsvisningssandlådan med en URL:

1. Navigera till denna URL: `https://companyname.preview.workfront.com/`.

   Du kan även komma åt förhandsvisningssandlådan genom att gå till [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Logga in med dina autentiseringsuppgifter för förhandsgranskning.

   Dina autentiseringsuppgifter för förhandsgranskning bör vara desamma som dina produktionsuppgifter, såvida du inte har ändrat dem i Produktion efter att uppdateringen av förhandsvisningen har ägt rum. Inloggningarna synkroniseras bara när en uppdatering görs. De synkroniseras inte automatiskt.

## Ta emot e-postmeddelanden från sandlådan Förhandsgranska

Workfront inaktiverar all e-postkommunikation från sandlådemiljön Preview. Om du vill få e-postmeddelanden från förhandsgranskningssandlådemiljön måste du aktivera den här funktionen i dina användarinställningar. Mer information om hur du aktiverar e-postmeddelanden i sandlådemiljön för förhandsgranskning finns i [Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Rapportleverans och push-meddelanden på mobilappen är alltid inaktiverade för förhandsvisningssandlådemiljön. Varken du eller [!DNL Workfront] administratören kan aktivera rapportleverans eller push-meddelanden för mobilappen när du öppnar sandlådemiljön för förhandsgranskning.
>
>Mer information om rapportleveranser för produktionsmiljön finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## enkel inloggning (SSO)

Om du använder enkel inloggning ska du samarbeta med vårt kundsupportteam för att säkerställa att den är korrekt konfigurerad så att du kan använda dina inloggningsuppgifter för att logga in på [!UICONTROL Preview] Sandbox. Om din första inloggning misslyckas kontaktar du din vanliga supportkontakt eller [!DNL Workfront] administratör för hjälp.

Mer information om enkel inloggning finns i [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Konfigurera enkel inloggning i förhandsgranskningssandlådan

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till [!DNL Adobe Admin Console]. Om din organisation har anslutit sig till [!DNL Adobe Admin Console], ingen åtgärd krävs.
>
>För en lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till [!DNL Adobe Admin Console], se [Plattformsbaserade administrationsskillnader ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Om du vill konfigurera din Preview Sandbox så att den fungerar med en enkel inloggningslösning kan du göra det genom att konfigurera den separat från din produktionsmiljö. Konfigurationen av enkel inloggning i förhandsgranskningssandlådan är oberoende av SSO-konfigurationen i produktionsmiljön.

När din förhandsvisningssandlåda uppdateras (varje helg) kopieras inte SSO-informationen från din produktionsmiljö för att skriva över konfigurationen för förhandsvisningssandlådan.

Stegen för att konfigurera enkel inloggning i förhandsgranskningssandlådan liknar de som används för att konfigurera den i produktionsmiljön.

Mer information om konfiguration [!DNL Workfront] med SSO, se [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Prestanda och tillgänglighet för förhandsvisningsmiljön

[!DNL Workfront] Förhandsgranskningsmiljöer är inte avsedda för prestanda- eller laddningstestning. Använd i stället dessa miljöer för att validera funktionaliteten med organisationens befintliga arbetsflöden.

[!DNL Workfront] Förhandsvisningsmiljöer är alltid tillgängliga.

Alla driftavbrott till en [!DNL Workfront] Förhandsgranskningsmiljön under kontorstid kommer att vara den första prioriteten omedelbart efter att eventuella produktionsproblem har lösts.

Alla driftavbrott till en [!DNL Workfront] Förhandsvisningsmiljön på helger (lördagar och söndagar) kommer att hanteras så att miljön körs under kontorstid på måndag.
