---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce - översikt
description: Du kan installera [!DNL Adobe Workfront] för Salesforce så att dina Salesforce-användare kan skicka [!DNL Workfront] förfrågningar och automatiskt skapa projekt utan att behöva lämna Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] - översikt

En [!UICONTROL Pro] [!DNL Workfront]-plan krävs för att använda den här funktionen. Mer information om olika tillgängliga planer finns i [[!DNL Workfront] Planer.](https://business.adobe.com/products/workfront/pricing.html)

Du kan installera [!DNL Adobe Workfront for Salesforce] så att dina [!DNL Salesforce]-användare kan skicka [!DNL Workfront] förfrågningar och automatiskt skapa projekt utan att gå ur [!DNL Salesforce].

Som [!DNL Workfront]-administratör kan du hämta och konfigurera [!DNL Workfront for Salesforce]. Sedan kan du dela den med alla andra [!DNL Salesforce]-användare.

Mer information om hur du installerar [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Mer information om hur du konfigurerar avsnittet [!DNL Workfront] i [!DNL Salesforce] för alla användare finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] Konfigurera för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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

## [!DNL Workfront for Salesforce]

Du kan göra följande när du använder [!DNL Workfront for Salesforce]:

* Skapa [!DNL Workfront]-förfrågningar manuellt från [!DNL Salesforce] inom ett säljprojekt eller ett konto.

  Mer information om hur du skapar [!DNL Workfront]-begäranden från [!DNL Salesforce] finns i [Skicka [!DNL Adobe Workfront] begäranden från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Utlös automatiskt skapande av projekt i [!DNL Workfront] när vissa villkor uppfylls i [!DNL Salesforce]. Din [!DNL Salesforce]-systemadministratör måste konfigurera utlösare för att skapa projekt från [!DNL Salesforce].

  Mer information om hur du skapar [!DNL Workfront] projekt från [!DNL Salesforce] finns i [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tänk på följande när du arbetar med [!DNL Workfront] för [!DNL Salesforce]:

* Vi stöder både ramverken [!DNL Salesforce Classic] och [!DNL Lightning Experience].
* Objekt kan bara skapas från [!DNL Salesforce] till [!DNL Workfront].
* Du kan visa viss information om [!DNL Workfront] objekt i [!DNL Salesforce].

  Den här informationen kan inte anpassas.

  En lista med [!DNL Workfront] fält som du kan visa från [!DNL Salesforce] finns i [Skicka [!DNL Adobe Workfront] begäranden från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) och [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Du kan komma åt objekt som är länkade till [!DNL Salesforce] genom att klicka på länken **[!UICONTROL Go to Salesforce]** från Workfront.

  Du kan inte visa någon information om [!DNL Salesforce]-objekten i [!DNL Workfront], men du har en länk till [!UICONTROL Salesforce]-objektet från [!DNL Workfront] för att granska det i [!DNL Salesforce].

  Länken [!UICONTROL The **Gå till Salesforce**] visas i följande områden:

   * Avsnittet [!UICONTROL Details] i ett projekt eller en utgåva
   * Projektets huvud eller en utgåva.

     Systemadministratören eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna visa länken [!UICONTROL Go to Salesforce] i projektet eller utgåvans huvud.
   * Panelen [!DNL Summary] för ett problem när du markerar problemet i en lista, efter att du klickat på [!UICONTROL Open Summary] ![ikonen för panelen Sammanfattning](assets/summary-panel-icon.png) i listans verktygsfält.

     >[!NOTE]
     >
     >Länken [!UICONTROL Go to Salesforce] är synlig för alla [!DNL Workfront]-användare som kan visa projektet eller problemet. Du måste ha ett [!DNL Salesforce]-konto för att kunna gå till det [!DNL Salesforce]-säljprojekt eller konto där problemet loggades.

* När du uppdaterar fält för ett objekt i ett program uppdateras ingen information om länkade objekt i det andra programmet.
