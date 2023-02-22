---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare
description: Efter installationen [!DNL Adobe Workfront] för Salesforce som [!DNL Workfront] kan du göra den tillgänglig för dina användare genom att lägga till den i ett nytt avsnitt i sidlayouterna för säljprojekt och konto i Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare

A [!UICONTROL Pro] [!DNL Workfront] Planering krävs för att använda den här funktionen. Mer information om olika planer finns i [[!DNL Workfront] Planer.](https://www.workfront.com/plans)

Efter installationen [!DNL Adobe Workfront] for [!DNL Salesforce] som [!DNL Workfront] kan du göra den tillgänglig för dina användare genom att lägga till den i ett nytt avsnitt i deras [!UICONTROL Opportunity] och [!UICONTROL Account]
sidlayout i [!UICONTROL Salesforce].

Mer information om installation [!DNL Workfront for Salesforce], se [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

För användare som har [!DNL Workfront] finns i båda [!DNL Classic] och [!DNL Lightning Experience] ramverk måste du lägga till [!DNL WorkfrontOpportunities] och [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] sidor till [!UICONTROL Opportunity] och [!UICONTROL Accounts] sidlayouter.

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

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

* Du måste ha en [!DNL Salesforce] -instans med åtkomst till ett systemadministratörskonto.
* Du måste ha en [!DNL Workfront] -instans med åtkomst till ett systemadministratörskonto.

## Konfigurera [!DNL Workfront] i [!DNL Salesforce Classic] ramverk

1. Logga in på [!DNL Salesforce] som Workfront-administratör.
1. Klicka på **[!UICONTROL Setup].**
1. I **[!UICONTROL Build]** sektion, expandera **[!UICONTROL Customize].**

1. Expandera **[!UICONTROL Opportunities]** och sedan klicka **[!UICONTROL Page Layouts]** för att lägga till [!DNL Workfront] till ett säljprojekt.

   eller

   Expandera **[!UICONTROL Accounts]** och sedan klicka **[!UICONTROL Page Layouts]** för att lägga till [!DNL Workfront] till ett konto.

1. Klicka **[!UICONTROL Edit]** i en befintlig layout.

   eller

   Klicka **[!UICONTROL New]** för att lägga till en ny layout.

1. (Valfritt) Dra **[!UICONTROL Section]** till layouten och släpp den på önskad plats.\

1. (Valfritt) Ange ett namn för det nya avsnittet.

   Vi rekommenderar att du namnger det här avsnittet **[!DNL Workfront]**.

1. (Valfritt) Ange önskat **[!UICONTROL Layout]** och **[!UICONTROL Tab-key Order]** för det nya avsnittet.

   Vi rekommenderar att du väljer **[!UICONTROL 1-Column]** layout för [!DNL Workfront] -avsnitt.

1. Klicka på **[!UICONTROL OK]**.
1. I **[!UICONTROL Layout]** område, klicka **[!UICONTROL Visualforce Pages].**

1. Dra och släpp **[!UICONTROL WorkfrontOpportunities]** till det nya avsnittet i **[!UICONTROL Opportunities]** Layout.

   eller

   Dra och släpp **[!UICONTROL WorkfrontAccounts]** till det nya avsnittet i  **[!UICONTROL Account]** Layout.\

1. Klicka på **[!UICONTROL Properties]** ikonen i det övre högra hörnet av den nya komponenten.\

1. För att få en optimal visning anger du följande egenskaper för [!DNL Workfront Visualforce] sida:

   * **[!UICONTROL Width (in pixels or %)]**: 100%
   * **[!UICONTROL Height (in pixels)]**: 600
   * Välj **[!UICONTROL Show scrollbars]**.

1. Klicka på **[!UICONTROL OK]**.
1. Klicka **[!UICONTROL Save]** för att spara layouten.

   Alla användare som har den här layouten tilldelad kan nu se [!DNL Workfront] på sina [!UICONTROL Opportunities] eller [!UICONTROL Accounts] objekt.

   Användarna ser en [!DNL Workfront] inloggningsskärmen på [!DNL Workfront] -avsnitt. Om de inte har en [!DNL Workfront] kan de komprimera avsnittet, men inte ta bort det från layouten.

## Konfigurera [!DNL Workfront] i [!DNL Salesforce Lightning Experience] ramverk

Du kan lägga till [!DNL Workfront] till layouten för en [!DNL Salesforce] [!UICONTROL Opportunity] eller Konto i [!DNL Salesforce Lightning Experience] antingen genom att använda [!UICONTROL Setup] eller från ett konto eller [!UICONTROL Opportunity] -objekt.

* [Konfigurera [!DNL Workfront] i [!UICONTROL Setup] nivå](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Konfigurera [!DNL Workfront] Avsnitt på säljprojekt- eller kontonivå](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Konfigurera [!DNL Workfront] i [!UICONTROL Setup] nivå {#configure-the-workfront-section-at-the-setup-level}

1. Logga in [!DNL Salesforce] som systemadministratör.
1. Klicka på **[!UICONTROL Setup]** ikonen och klicka sedan på **[!UICONTROL Setup]**.

1. Expandera **[!UICONTROL Object and Fields]** och sedan klicka **[!UICONTROL Object Manager]**.

1. Klicka **[!UICONTROL Opportunity]** för att anpassa layouten för ett säljprojekt.

   eller

   Klicka **[!UICONTROL Account]** för att anpassa layouten för ett konto.

1. Klicka på **[!UICONTROL Page Layouts]**.
1. Klicka på namnet på en befintlig sidlayout för att redigera den.

   eller

   Klicka **[!UICONTROL New]** för att skapa en ny sidlayout.

1. Fortsätt med [Konfigurera [!DNL Workfront] Avsnitt på säljprojekt- eller kontonivå](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) nedan.

### Konfigurera [!DNL Workfront] Avsnitt på säljprojekt- eller kontonivå {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Gå till en **[!UICONTROL Opportunity]** eller **[!UICONTROL Account]**.

1. Klicka på **[!UICONTROL Setup]** ikonen och klicka sedan på **[!UICONTROL Edit Page]**.\

1. Expandera avsnittet **[!UICONTROL Custom-Managed]**.
1. Dra och släpp **[!DNL Workfront]** -komponenten på [!UICONTROL Opportunity] eller sidan Konto.

   Vi rekommenderar att du använder hela sidbredden för [!DNL Workfront] i stället för en av spalterna i layouten.

1. Klicka på **[!UICONTROL Save]**.

   Alla användare som har den här layouten tilldelad kan nu se [!DNL Workfront] på sina [!UICONTROL Opportunities] eller [!UICONTROL Accounts] objekt.

   >[!NOTE]
   >
   >Användarna ser en [!DNL Workfront] inloggningsskärmen på [!DNL Workfront] -avsnitt. Om de inte har en [!DNL Workfront] kan de komprimera avsnittet, men inte ta bort det från layouten. Användarna kan logga in med den autentiseringsmetod som du har aktiverat: Förbättrad autentisering eller din SAML-URL (Security Assertion Markup Language).

