---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Konfigurera avsnittet  [!DNL Adobe Workfront] för [!DNL Salesforce] användare
description: När du har installerat [!DNL Adobe Workfront] för Salesforce som  [!DNL Workfront] administratör kan du göra den tillgänglig för dina användare genom att lägga till den i ett nytt avsnitt i sidlayouterna för säljprojekt och konto i Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Konfigurera avsnittet [!DNL Adobe Workfront] för [!DNL Salesforce]-användare

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Integreringen av Workfront för Salesforce kommer inte att vara tillgänglig efter den **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Salesforce.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Salesforce finns i [Salesforce-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

En [!UICONTROL Pro] [!DNL Workfront]-plan krävs för att använda den här funktionen. Mer information om olika tillgängliga planer finns i [[!DNL Workfront] Planer.](https://business.adobe.com/se/products/workfront/pricing.html)

När du har installerat [!DNL Adobe Workfront] för [!DNL Salesforce] som [!DNL Workfront]-administratör kan du göra den tillgänglig för dina användare genom att lägga till den i ett nytt avsnitt i deras [!UICONTROL Opportunity] och [!UICONTROL Account]
sidlayouter i [!UICONTROL Salesforce] .

Information om hur du installerar [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

För att användare ska ha [!DNL Workfront] tillgängligt i både ramverket [!DNL Classic] och ramverket [!DNL Lightning Experience] måste du lägga till sidorna [!DNL WorkfrontOpportunities] och [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] i sidlayouterna [!UICONTROL Opportunity] respektive [!UICONTROL Accounts].

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

* Du måste ha en [!DNL Salesforce]-instans med åtkomst till ett systemadministratörskonto.
* Du måste ha en [!DNL Workfront]-instans med åtkomst till ett systemadministratörskonto.

## Konfigurera avsnittet [!DNL Workfront] i ramverket [!DNL Salesforce Classic]

1. Logga in på [!DNL Salesforce] som Workfront-administratör.
1. Klicka på **[!UICONTROL Setup].**
1. Expandera **[!UICONTROL Build]** i avsnittet **[!UICONTROL Customize].**

1. Expandera **[!UICONTROL Opportunities]** och klicka sedan på **[!UICONTROL Page Layouts]** för att lägga till avsnittet [!DNL Workfront] i ett säljprojekt.

   eller

   Expandera **[!UICONTROL Accounts]** och klicka sedan på **[!UICONTROL Page Layouts]** för att lägga till avsnittet [!DNL Workfront] i ett konto
.

1. Klicka på **[!UICONTROL Edit]** i en befintlig layout.

   eller

   Klicka på **[!UICONTROL New]** om du vill lägga till en ny layout.

1. (Valfritt) Dra komponenten **[!UICONTROL Section]** till layouten och släpp den på önskad plats.\

1. (Valfritt) Ange ett namn för det nya avsnittet.

   Vi rekommenderar att du namnger avsnittet **[!DNL Workfront]**.

1. (Valfritt) Ange önskat **[!UICONTROL Layout]** och **[!UICONTROL Tab-key Order]** för det nya avsnittet.

   Vi rekommenderar att du väljer layouten **[!UICONTROL 1-Column]** för avsnittet [!DNL Workfront].

1. Klicka på **[!UICONTROL OK]**.
1. Klicka på **[!UICONTROL Layout]** i området **[!UICONTROL Visualforce Pages].**

1. Dra och släpp komponenten **[!UICONTROL WorkfrontOpportunities]** till det nya avsnittet i layouten **[!UICONTROL Opportunities]**.

   eller

   Dra och släpp **[!UICONTROL WorkfrontAccounts]**-komponenten till det nya avsnittet i **[!UICONTROL Account]**-layouten.\

1. Klicka på ikonen **[!UICONTROL Properties]** i det övre högra hörnet i den nya komponenten.\

1. För att få en optimal visning anger du följande egenskaper för sidan [!DNL Workfront Visualforce]:

   * **[!UICONTROL Width (in pixels or %)]**: 100 %
   * **[!UICONTROL Height (in pixels)]**: 600
   * Välj **[!UICONTROL Show scrollbars]**.

1. Klicka på **[!UICONTROL OK]**.
1. Klicka på **[!UICONTROL Save]** om du vill spara layouten.

   Alla användare som har den här layouten tilldelad kan nu se avsnittet [!DNL Workfront] på sina [!UICONTROL Opportunities] - eller [!UICONTROL Accounts]-objekt.

   Användarna ser inloggningsskärmen [!DNL Workfront] i avsnittet [!DNL Workfront]. Om de inte har något [!DNL Workfront]-konto kan de komprimera avsnittet, men inte ta bort det från layouten.

## Konfigurera avsnittet [!DNL Workfront] i ramverket [!DNL Salesforce Lightning Experience]

Du kan lägga till avsnittet [!DNL Workfront] i layouten för ett [!DNL Salesforce] [!UICONTROL Opportunity] eller konto
i [!DNL Salesforce Lightning Experience] -ramverket antingen genom att gå till [!UICONTROL Setup] -området eller från ett konto
eller [!UICONTROL Opportunity] -objekt.

* [Konfigurera avsnittet  [!DNL Workfront] på nivån [!UICONTROL Setup]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Konfigurera avsnittet  [!DNL Workfront] på affärsmöjlighets- eller kontonivå](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Konfigurera avsnittet [!DNL Workfront] på nivån [!UICONTROL Setup] {#configure-the-workfront-section-at-the-setup-level}

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Klicka på ikonen **[!UICONTROL Setup]** och sedan på **[!UICONTROL Setup]**.

1. Expandera **[!UICONTROL Object and Fields]** och klicka sedan på **[!UICONTROL Object Manager]**.

1. Klicka på **[!UICONTROL Opportunity]** om du vill anpassa layouten för ett säljprojekt.

   eller

   Klicka på **[!UICONTROL Account]** om du vill anpassa layouten för ett konto.

1. Klicka på **[!UICONTROL Page Layouts]**.
1. Klicka på namnet på en befintlig sidlayout för att redigera den.

   eller

   Klicka på **[!UICONTROL New]** om du vill skapa en ny sidlayout.

1. Fortsätt med [Konfigurera  [!DNL Workfront] avsnittet på säljprojekts- eller kontonivå](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) nedan.

### Konfigurera avsnittet [!DNL Workfront] på affärsmöjlighets- eller kontonivå {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Logga in på [!DNL Salesforce] som systemadministratör.
1. Gå till en **[!UICONTROL Opportunity]** eller **[!UICONTROL Account]**.

1. Klicka på ikonen **[!UICONTROL Setup]** och sedan på **[!UICONTROL Edit Page]**.\

1. Expandera avsnittet **[!UICONTROL Custom-Managed]**.
1. Dra och släpp komponenten **[!DNL Workfront]** på ditt [!UICONTROL Opportunity] eller konto
sida.

   Vi rekommenderar att du använder sidans fulla bredd för avsnittet [!DNL Workfront] i stället för en av layoutens kolumner.

1. Klicka på **[!UICONTROL Save]**.

   Alla användare som har den här layouten tilldelad kan nu se avsnittet [!DNL Workfront] på sina [!UICONTROL Opportunities] - eller [!UICONTROL Accounts]-objekt.

   >[!NOTE]
   >
   >Användarna ser inloggningsskärmen [!DNL Workfront] i avsnittet [!DNL Workfront]. Om de inte har något [!DNL Workfront]-konto kan de komprimera avsnittet, men inte ta bort det från layouten. Användare kan logga in med den autentiseringsmetod som du har aktiverat: Förbättrad autentisering eller din SAML-URL (Security Assertion Markup Language).

