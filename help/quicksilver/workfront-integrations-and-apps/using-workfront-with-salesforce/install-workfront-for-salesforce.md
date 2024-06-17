---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installera [!DNL Adobe Workfront] for [!DNL Salesforce]
description: Installera appen innan den blir tillgänglig i [!DNL Salesforce] AppExchange, se Installera [!DNL Workfront] för Salesforce innan det blir tillgängligt på AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 1%

---

# Installera [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Installera appen innan den blir tillgänglig i [!DNL Salesforce AppExchange], se [Installerar [!DNL Workfront for Salesforce] innan det blir tillgängligt i [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Som en [!DNL Salesforce] och [!DNL Adobe Workfront] administratör kan du installera [!DNL Workfront for Salesforce] för att [!DNL Salesforce] användare att skicka [!DNL Workfront] och automatiskt skapa projekt utan att någonsin behöva lämna Salesforce.

För en allmän förståelse av vad du kan förvänta dig genom att installera [!DNL Workfront for Salesforce], se [[!DNL Adobe Workfront for Salesforce] översikt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Krav för installation och användning [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installerar [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

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

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav för installation och användning [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Du måste ha en [!DNL Salesforce] -instans med åtkomst till ett systemadministratörskonto för att installera programmet.
* Du måste ha en [!DNL Workfront] -instans med åtkomst till ett systemadministratörskonto för att konfigurera integreringen.
* [!UICONTROL Salesforce] användare måste ha [!DNL Workfront] konto för att kunna

   * Skapa [!DNL Workfront] förfrågningar från [!DNL Salesforce]
   * Visa [!DNL Workfront] begäranden eller projekt i Salesforce

## Installerar [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

Du måste vara en [!DNL Salesforce] och [!DNL Workfront] systemadministratör för att installera och konfigurera [!DNL Workfront for Salesforce].

I följande underavsnitt beskrivs hur du installerar [!DNL Workfront] för [!DNL Salesforce] Produktionsmiljö. Du kan följa samma steg för att installera [!DNL Workfront] för [!DNL Salesforce] Sandlådemiljö.

* [Installerar [!DNL Workfront for Salesforce] innan det blir tillgängligt i [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installerar [!DNL Workfront for Salesforce] i [!DNL Salesforce Classic] Ramverk](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installerar [!DNL Workfront for Salesforce] i [!DNL Salesforce Lightning Experience] Ramverk](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installerar [!DNL Workfront for Salesforce] innan det blir tillgängligt i [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] kommer att vara tillgängligt i [!DNL Salesforce AppExchange] snart.

Så här installerar du appen innan den blir tillgänglig:

1. I produktionsmiljön går du till

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   I sandlådemiljön går du till

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >Du måste vara inloggad i Salesforce för att få tillgång till dessa sidor.

1. Kontrollera **[!UICONTROL Yes, grant access to these third-party web sites]** box.

   En inläsningsskärm visas. Installationen kan ta en stund.

1. Klicka **[!UICONTROL Done]** när installationen är klar.

1. Navigera till **[!UICONTROL Setup]** > **[!UICONTROL Security]Kontroller** > **[!UICONTROL Remote Site Settings]**.
1. (Villkorligt) Välj Workfront i listan.

   eller

   Om du inte ser [!DNL Workfront] URL-adressen som anges i **[!UICONTROL All Remote Sites]** lista, klicka på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.

   Till exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.

   Till exempel: *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.

   The [!DNL Workfront] är nu installerat på din [!DNL Salesforce] -instans och **[!UICONTROL WorkfrontOpportunities]** och **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Sidorna har skapats i din miljö.

   [!DNL Salesforce] -användare kan använda appen när du har lagt till [!DNL Workfront] till sina [!UICONTROL Opportunity] eller [!UICONTROL Account] sidlayouter.\
   Mer information om hur du konfigurerar Workfront-avsnittet för användare finns i [Konfigurera Adobe Workfront-avsnittet för Salesforce-användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installerar [!DNL Workfront] for [!DNL Salesforce] i [!DNL Salesforce Classic] Ramverk

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Gå till **Inställningar.**
1. I **Bygge** avsnitt, klicka **AppExchange Marketplace**.

1. I **Sök i AppExchange Apps** ruta, typ **Workfront**.

1. Klicka på Workfront när du hittar det och klicka sedan på **Hämta nu**.
1. Klicka **[!UICONTROL Install in Production]** för att installera [!DNL Workfront] i din [!DNL Salesforce] Produktionsmiljö. (rekommenderas)
1. När du har läst och godkänt villkoren aktiverar du **[!UICONTROL I have read and agree to the terms and conditions]** fält.
1. Klicka på **[!UICONTROL Confirm and Install]**.
1. Välj **[!UICONTROL Install for All Users]** (rekommenderas), klicka sedan på **[!UICONTROL Install]**.

1. (Villkorligt) Om du tillfrågas om du vill godkänna åtkomst från en tredje part måste du välja **[!UICONTROL Yes, grant access to these third-party web sites]** och sedan klicka **[!UICONTROL Continue]**.

1. Klicka **[!UICONTROL Done]** när installationen är klar.

   The [!DNL Workfront] app listas under **[!UICONTROL Installed Packages]**.


1. Navigera till **[!UICONTROL Setup>Security Controls>Remote Site Settings]**.
1. (Villkorligt) Om du inte ser ditt [!DNL Workfront] URL-adressen som anges i **[!UICONTROL All Remote Sites]** lista, klicka på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.
Till exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.
Till exempel: *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.\
   The [!DNL Workfront] är nu installerat på din [!DNL Salesforce] -instans. The **[!UICONTROL WorkfrontOpportunities]** och **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] sidor har skapats i din miljö.\
   [!DNL Salesforce] -användare kan inte använda appen förrän du lägger till [!DNL Workfront] till sina [!UICONTROL Opportunity] eller [!UICONTROL Account] sidlayouter.\
   Mer information om hur du konfigurerar [!DNL Workfront] för användare, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installerar [!DNL Workfront for Salesforce] i [!DNL Salesforce Lightning Experience] Ramverk

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Klicka på **[!UICONTROL Setup]icon** och sedan klicka **[!UICONTROL Setup]**.

1. I **[!UICONTROL PLATFORM TOOLS]** sektion, expandera **[!UICONTROL Apps].**

1. Klicka på **[!DNL AppExchange Marketplace]**.
1. I **[!UICONTROL Search [!DNL AppExchange] Apps]** ruta, typ **[!DNL Workfront]**.

1. Klicka på Workfront när du hittar det och klicka sedan på **Hämta nu**.
1. Klicka på **[!UICONTROL Open Login Screen]**.\
   Du måste logga in med [!DNL Workfront] administratörskonto för [!DNL Salesforce].

1. Klicka på **[!UICONTROL Allow]**.
1. I **[!UICONTROL Install in This Org]** ruta, klicka **[!UICONTROL Install Here]** för installation [!DNL Workfront] i [!DNL Salesforce] Produktionsmiljö. (rekommenderas)

1. När du har läst och godkänt villkoren aktiverar du **[!UICONTROL I have read and agree to the terms and conditions]** fält.
1. Klicka på **[!UICONTROL Confirm and Install]**.
1. Välj **[!UICONTROL Install for All Users]** (rekommenderas), klicka sedan på **[!UICONTROL Install]**.

1. (Villkorligt) Om du tillfrågas om du vill godkänna åtkomst från en tredje part måste du välja **[!UICONTROL Yes, grant access to these third-party web sites]** och sedan klicka **[!UICONTROL Continue]**.

1. Klicka **[!UICONTROL Done]** när installationen är klar.

   The [!DNL Workfront] app listas under **[!UICONTROL Installed Packages]**.

1. Navigera till **[!UICONTROL Setup].**
1. I **[!UICONTROL SETTINGS]** sektion, expandera **[!UICONTROL Security].**

1. Klicka på **[!UICONTROL Remote Site Settings]**.
1. (Villkorligt) Om du inte ser ditt [!DNL Workfront] URL-adressen som anges i **[!UICONTROL All Remote Sites]** lista, klicka på **[!UICONTROL New Remote Site]**.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site Name]**.
Till exempel: *[!DNL Workfront]*.

1. (Villkorligt) Om du lägger till platsen anger du **[!UICONTROL Remote Site URL]**.
Till exempel: *yourDomain.my.workfront.com*.

1. Klicka på **[!UICONTROL Save]**.

   The [!DNL Workfront] är nu installerat på din [!DNL Salesforce] -instans och **[!DNL Workfront]** har nu lagts till i din miljö.

   [!UICONTROL Salesforce] användare kan använda [!DNL Workfront] när du har lagt till [!DNL Workfront] till sina [!UICONTROL Opportunity] eller [!UICONTROL Account] sidlayouter.\
   Mer information om hur du konfigurerar [!DNL Workfront] för användare, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
