---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installera [!DNL Adobe Workfront] för [!DNL Salesforce]
description: Om du vill installera appen innan den blir tillgänglig på  [!DNL Salesforce] AppExchangen läser du Installera [!DNL Workfront] för Salesforce innan den blir tillgänglig på AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: c0e7340e2bf650b6f9931ae12aee07c5f7d5292b
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 1%

---

# Installera [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Information om hur du installerar appen innan den blir tillgänglig i [!DNL Salesforce AppExchange] finns i [Installera [!DNL Workfront for Salesforce] innan den blir tillgänglig på  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Som [!DNL Salesforce]- och [!DNL Adobe Workfront]-administratör kan du installera [!DNL Workfront for Salesforce] så att dina [!DNL Salesforce]-användare kan skicka [!DNL Workfront] förfrågningar och automatiskt skapa projekt utan att någonsin behöva lämna Salesforce.

En allmän förståelse för vad du kan förvänta dig genom att installera [!DNL Workfront for Salesforce] finns i [[!DNL Adobe Workfront for Salesforce] översikt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Krav för installation och användning av  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installerar  [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna använda de funktioner som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav för installation och användning av [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Du måste ha en [!DNL Salesforce]-instans med åtkomst till ett systemadministratörskonto för att kunna installera appen.
* Du måste ha en [!DNL Workfront]-instans med åtkomst till ett systemadministratörskonto för att kunna konfigurera integreringen.
* [!UICONTROL Salesforce] användare måste ha ett [!DNL Workfront]-konto för att kunna:

   * Skapa [!DNL Workfront] förfrågningar från [!DNL Salesforce]
   * Visa [!DNL Workfront] förfrågningar eller projekt i Salesforce

## Installerar [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

Du måste vara [!DNL Salesforce] och [!DNL Workfront]-systemadministratör för att kunna installera och konfigurera [!DNL Workfront for Salesforce].

I följande underavsnitt beskrivs hur du installerar [!DNL Workfront] för din [!DNL Salesforce]-produktionsmiljö. Du kan följa samma steg för att installera [!DNL Workfront] för din [!DNL Salesforce]-sandlådemiljö.

* [Installerar [!DNL Workfront for Salesforce] innan det blir tillgängligt på  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installerar [!DNL Workfront for Salesforce] i  [!DNL Salesforce Classic] ramverket](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installerar [!DNL Workfront for Salesforce] i  [!DNL Salesforce Lightning Experience] ramverket](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### [!DNL Workfront for Salesforce] installeras innan det blir tillgängligt på Marketplace i [!DNL AppExchange] {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] kommer snart att vara tillgänglig i [!DNL Salesforce AppExchange].

Så här installerar du appen innan den blir tillgänglig:

1. I produktionsmiljön går du till

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   I sandlådemiljön går du till

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Du måste vara inloggad i Salesforce för att få tillgång till dessa sidor.

1. Markera rutan **[!UICONTROL Yes, grant access to these third-party web sites]**.

   En inläsningsskärm visas. Installationen kan ta en stund.

1. Klicka på **[!UICONTROL Done]** när installationen är klar.

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Security]Kontroller** > **[!UICONTROL Remote Site Settings]**.
1. (Villkorligt) Välj Workfront i listan.

   eller

   Om du inte ser din [!DNL Workfront]-URL i listan **[!UICONTROL All Remote Sites]** klickar du på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.

   Exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.

   Till exempel *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.

   Appen [!DNL Workfront] är nu installerad på din [!DNL Salesforce]-instans och sidorna **[!UICONTROL WorkfrontOpportunities]** och **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] har skapats i din miljö.

   [!DNL Salesforce]-användare kan använda appen när du har lagt till avsnittet [!DNL Workfront] i sina [!UICONTROL Opportunity]- eller [!UICONTROL Account]-sidlayouter.\
   Mer information om hur du konfigurerar Workfront-avsnittet för användare finns i [Konfigurera Adobe Workfront-avsnittet för Salesforce-användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installerar [!DNL Workfront] för [!DNL Salesforce] i [!DNL Salesforce Classic] Framework

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Gå till **Inställningar.**
1. Klicka på **AppExchange Marketplace** i avsnittet **Build**.

1. Skriv **Workfront** i rutan **Sök i AppExchange-appar**.

1. Klicka på Workfront-appen när du hittar den och klicka sedan på **Hämta nu**.
1. Klicka på **[!UICONTROL Install in Production]** om du vill installera [!DNL Workfront]-appen i din [!DNL Salesforce] produktionsmiljö. (rekommenderas)
1. Aktivera fältet **[!UICONTROL I have read and agree to the terms and conditions]** när du har läst och godkänt villkoren.
1. Klicka på **[!UICONTROL Confirm and Install]**.
1. Välj **[!UICONTROL Install for All Users]** (rekommenderas) och klicka sedan på **[!UICONTROL Install]**.

1. (Villkorligt) Om du tillfrågas om du vill godkänna en åtkomst från tredje part måste du välja **[!UICONTROL Yes, grant access to these third-party web sites]** och sedan klicka på **[!UICONTROL Continue]**.

1. Klicka på **[!UICONTROL Done]** när installationen är klar.

   Appen [!DNL Workfront] visas under **[!UICONTROL Installed Packages]**.


1. Navigera till **[!UICONTROL Setup>Security Controls>Remote Site Settings]**.
1. (Villkorligt) Om du inte ser din [!DNL Workfront]-URL i listan **[!UICONTROL All Remote Sites]** klickar du på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.
Exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.
Till exempel *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.\
   Appen [!DNL Workfront] är nu installerad på din [!DNL Salesforce]-instans. Sidorna **[!UICONTROL WorkfrontOpportunities]** och **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] har skapats i din miljö.\
   [!DNL Salesforce] användare kan inte använda appen än förrän du lägger till avsnittet [!DNL Workfront] i deras [!UICONTROL Opportunity]- eller [!UICONTROL Account]-sidlayouter.\
   Mer information om hur du konfigurerar avsnittet [!DNL Workfront] för användare finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] Konfigurera för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### [!DNL Workfront for Salesforce] installeras i [!DNL Salesforce Lightning Experience] Framework

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Klicka på ikonen **[!UICONTROL Setup]** och sedan på **[!UICONTROL Setup]**.

1. Expandera **[!UICONTROL Apps]i avsnittet **[!UICONTROL PLATFORM TOOLS]**.**

1. Klicka på **[!DNL AppExchange Marketplace]**.
1. Skriv **[!DNL Workfront]** i rutan **[!UICONTROL Search [!DNL AppExchange] Apps]**.

1. Klicka på Workfront-appen när du hittar den och klicka sedan på **Hämta nu**.
1. Klicka på **[!UICONTROL Open Login Screen]**.\
   Du måste logga in med ditt [!DNL Workfront]-administratörskonto för [!DNL Salesforce].

1. Klicka på **[!UICONTROL Allow]**.
1. Klicka på **[!UICONTROL Install Here]** i rutan **[!UICONTROL Install in This Org]** för att installera [!DNL Workfront] i din [!DNL Salesforce] produktionsmiljö. (rekommenderas)

1. Aktivera fältet **[!UICONTROL I have read and agree to the terms and conditions]** när du har läst och godkänt villkoren.
1. Klicka på **[!UICONTROL Confirm and Install]**.
1. Välj **[!UICONTROL Install for All Users]** (rekommenderas) och klicka sedan på **[!UICONTROL Install]**.

1. (Villkorligt) Om du tillfrågas om du vill godkänna en åtkomst från tredje part måste du välja **[!UICONTROL Yes, grant access to these third-party web sites]** och sedan klicka på **[!UICONTROL Continue]**.

1. Klicka på **[!UICONTROL Done]** när installationen är klar.

   Appen [!DNL Workfront] visas under **[!UICONTROL Installed Packages]**.

1. Navigera till **[!UICONTROL Setup].**
1. Expandera **[!UICONTROL Security]i avsnittet **[!UICONTROL SETTINGS]**.**

1. Klicka på **[!UICONTROL Remote Site Settings]**.
1. (Villkorligt) Om du inte ser din [!DNL Workfront]-URL i listan **[!UICONTROL All Remote Sites]** klickar du på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.
Exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.
Till exempel *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.

   Appen [!DNL Workfront] är nu installerad på din [!DNL Salesforce]-instans och komponenten **[!DNL Workfront]** har nu lagts till i din miljö.

   [!UICONTROL Salesforce]-användare kan använda appen [!DNL Workfront] när du har lagt till avsnittet [!DNL Workfront] i sina [!UICONTROL Opportunity]- eller [!UICONTROL Account]-sidlayouter.\
   Mer information om hur du konfigurerar avsnittet [!DNL Workfront] för användare finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] Konfigurera för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
