---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt
description: Efter installation av [!DNL Adobe Workfront] för [!DNL Salesforce], you can submit [!DNL Workfront] förfrågningar från [!DNL Salesforce] säljprojekt och konton. Den här funktionaliteten finns både i Classic och Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---

# Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Integreringen av Workfront för Salesforce kommer inte att vara tillgänglig efter den **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Salesforce.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Salesforce finns i [Salesforce-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

När du har installerat [!DNL Adobe Workfront for Salesforce] kan du skicka [!DNL Workfront] förfrågningar från [!DNL Salesforce] säljprojekt och konton. Den här funktionaliteten finns i både [!DNL Classic]- och [!DNL Lightning Experience]-ramverket.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Om du vill skicka en [!DNL Workfront]-begäran från en [!DNL Salesforce]-affärsmöjlighet eller ett -konto måste du ha följande i din miljö:

* [!DNL Workfront]-administratören har installerat [!DNL Workfront for Salesforce].\
   Mer information om att installera [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* [!DNL Workfront]-administratören har lagt till avsnittet [!DNL Workfront] i sidlayouterna [!UICONTROL Opportunity] och [!UICONTROL Account].\
   Mer information om hur du lägger till avsnittet [!DNL Workfront] i en sidlayout finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Du har ett [!DNL Workfront]-konto och du kan logga in på det från avsnittet [!DNL Workfront] i ditt säljprojekt eller konto.\
   När du har loggat in kan du se fliken [!UICONTROL New Requests] där du kan börja skriva in begäranden.

## Skicka [!DNL Workfront] förfrågningar från [!DNL Salesforce]

1. Gå till ett säljprojekt eller konto i Salesforce.
1. Gå till avsnittet [!DNL Workfront].
1. På fliken **[!UICONTROL New Requests]** väljer du en begärandetyp i listrutan **[!UICONTROL Select a Request Type]**.

   Du kan se samma begärandeköer som du har åtkomst till i Workfront.

1. Börja fylla i de tillgängliga fälten för din begäran.

   Att skicka en begäran från [!DNL Salesforce] är identiskt med att skicka en begäran i webbprogrammet [!DNL Workfront].

   >[!NOTE]
   >
   >Överföring av ett dokument med plugin-programmet [!DNL Workfront] i [!DNL Salesforce] är inte tillgängligt för tillfället.

   Fortsätt att följa stegen som beskrivs i [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Klicka på **[!UICONTROL Submit]**.

## Visa [!DNL Workfront] förfrågningar

1. Gå till ett säljprojekt eller konto i [!DNL Salesforce].
1. Gå till avsnittet **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Beroende på hur administratören för [!DNL Workfront] konfigurerade det här avsnittet kan det ha ett annat namn.

1. Klicka på fliken **[!UICONTROL Submitted Requests]**.  

   Du kan visa alla förfrågningar som du eller andra har skickat från det här säljprojektet eller kontot på den här fliken.Förfrågningar som skickas till den här begärandekön i webbprogrammet visas inte i den här listan i [!DNL Salesforce].

   >[!NOTE]
   >
   >Begäranden som skickas till den här begärandekön i webbprogrammet visas inte i listan i Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Du kan visa följande information om de skickade förfrågningarna:

   * Begäransnamn (i kolumnen [!UICONTROL Subject])
   * Referensnummer
   * Typ av begäran
   * Status
   * Skickat den
   * Begärd av namn
   * Tilldelad till namn\

     När den här informationen uppdateras i [!DNL Workfront] uppdateras den också i den här listan.

1. (Valfritt) Klicka på namnet på begäran för att öppna den i [!DNL Workfront].

1. (Valfritt) Klicka på **[!UICONTROL Go to [!DNL Salesforce]]** om du vill komma åt affärsmöjligheten eller kontot där utgåvan kom från följande områden i Workfront:

   * I avsnittet [!UICONTROL Details] av problemet
   * När du markerar problemet i en lista på panelen Sammanfattning ska du klicka på [!UICONTROL Open Summary] ![ikonen för panelen Sammanfattning](assets/summary-panel-icon.png) i listans verktygsfält.
   * I utgåvans rubrik, när fältet [!UICONTROL Integrations] är tillgängligt. Systemet eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna visa länken Gå till Salesforce i utgåvans huvud. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Länken [!UICONTROL Go to Salesforce] är synlig för alla [!DNL Workfront]-användare som kan visa problemet. Du måste ha ett [!DNL Salesforce]-konto för att kunna gå till det [!DNL Salesforce]-säljprojekt eller konto där problemet loggades.
