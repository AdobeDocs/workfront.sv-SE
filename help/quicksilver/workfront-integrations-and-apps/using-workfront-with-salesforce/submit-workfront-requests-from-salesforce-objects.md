---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt
description: Efter installation [!DNL Adobe Workfront] for [!DNL Salesforce], you can submit [!DNL Workfront] förfrågningar från [!DNL Salesforce] Affärsmöjligheter och konton. Den här funktionen finns både i Classic och i Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt

Efter installation [!DNL Adobe Workfront for Salesforce]kan du skicka in [!DNL Workfront] förfrågningar från [!DNL Salesforce] Affärsmöjligheter och konton. Den här funktionen finns i båda [!DNL Classic] och [!DNL Lightning Experience] ramverk.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda de funktioner som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan*</p></td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licens*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Att skicka in [!DNL Workfront] begäran från en [!DNL Salesforce] Möjligheter eller konto säkerställer att du har följande i din miljö:

* Dina [!DNL Workfront] administratören har installerat [!DNL Workfront for Salesforce].\
   Mer information om installation [!DNL Workfront for Salesforce], se [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Dina [!DNL Workfront] administratören har lagt till [!DNL Workfront] till [!UICONTROL Opportunity] och [!UICONTROL Account] sidlayouter.\
   Mer information om hur du lägger till [!DNL Workfront] till en sidlayout, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Du har en [!DNL Workfront] kontot och du kan logga in på det från [!DNL Workfront] i ditt säljprojekt eller konto.\
   När du har loggat in kan du se [!UICONTROL New Requests] där du kan börja skriva begäranden.

## Skicka [!DNL Workfront] förfrågningar från [!DNL Salesforce]

1. Gå till ett säljprojekt eller konto i Salesforce.
1. Gå till [!DNL Workfront] -avsnitt.
1. I **[!UICONTROL New Requests]** väljer du en begärandetyp på fliken **[!UICONTROL Select a Request Type]** nedrullningsbar meny.

   Du kan se samma begärandeköer som du har åtkomst till i Workfront.

1. Börja fylla i de tillgängliga fälten för din begäran.

   Skicka en begäran från [!DNL Salesforce] är identiskt med att skicka en begäran i [!DNL Workfront] webbprogram.

   >[!NOTE]
   >
   >Överföra ett dokument med [!DNL Workfront] plugin in [!DNL Salesforce] är inte tillgängligt för tillfället.

   Fortsätt följa stegen som beskrivs i [Skapa och skicka [!DNL Adobe Workfront] förfrågningar](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Klicka på **[!UICONTROL Submit]**.

## Visa [!DNL Workfront] förfrågningar

1. Gå till ett säljprojekt eller konto i [!DNL Salesforce].
1. Gå till **[!DNL Workfront]** -avsnitt.

   >[!NOTE]
   >
   >Beroende på hur [!DNL Workfront] administratören konfigurerade det här avsnittet. Det kan ha ett annat namn.

1. Välj **[!UICONTROL Submitted Requests]** -fliken.

   Du kan visa alla förfrågningar som du eller andra har skickat från det här säljprojektet eller kontot på den här fliken.Förfrågningar som skickas till den här begärandekön i webbprogrammet visas inte i den här listan i [!DNL Salesforce].

   >[!NOTE]
   >
   >Begäranden som skickas till den här begärandekön i webbprogrammet visas inte i den här listan i Salesforce.

   ![salesforce_skickad_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Du kan visa följande information om de skickade förfrågningarna:

   * Namn på begäran (i [!UICONTROL Subject] kolumn)
   * Referensnummer
   * Typ av begäran
   * Status
   * Skickat den
   * Begärd av namn
   * Tilldelad till namn\

      När den här informationen uppdateras i [!DNL Workfront], uppdateras den också i den här listan.

1. (Valfritt) Klicka på namnet på begäran för att öppna den i [!DNL Workfront].

1. (Valfritt) Klicka på **[!UICONTROL Go to [!DNL Salesforce]]** för att få tillgång till det säljprojekt eller konto där emissionen har sitt ursprung i följande områden i Workfront:

   * I [!UICONTROL Details] problemsektion
   * På panelen Sammanfattning när du markerar problemet i en lista, efter att du klickat [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) i listans verktygsfält.
   * I utgåvans rubrik, när [!UICONTROL Integrations] fältet är tillgängligt. Systemadministratören eller gruppadministratören måste lägga till [!UICONTROL Integrations] till layoutmallen för att visa länken Gå till Salesforce i utgåvans rubrik. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >The [!UICONTROL Go to Salesforce] länk är synlig för alla [!DNL Workfront] användare som kan se problemet. Du måste ha en [!DNL Salesforce] för att kunna gå till [!DNL Salesforce] Affärsmöjlighet eller konto där problemet loggades.
