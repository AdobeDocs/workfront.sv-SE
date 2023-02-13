---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront för Salesforce - översikt
description: Du kan installera [!DNL Adobe Workfront] för Salesforce så att dina Salesforce-användare kan skicka [!DNL Workfront] och automatiskt skapa projekt utan att någonsin behöva lämna Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] översikt

A [!UICONTROL Pro] [!DNL Workfront] Planering krävs för att använda den här funktionen. Mer information om olika planer finns i [[!DNL Workfront] Planer.](https://www.workfront.com/plans)

Du kan installera [!DNL Adobe Workfront for Salesforce] för att [!DNL Salesforce] användare att skicka [!DNL Workfront] skapar projekt automatiskt utan att gå ur [!DNL Salesforce].

Som [!DNL Workfront] administratör kan du hämta och konfigurera [!DNL Workfront for Salesforce]. Sedan kan du dela det så att alla andra kan göra det [!DNL Salesforce] -användare.

Mer information om installation [!DNL Workfront for Salesforce], se [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Mer information om hur du konfigurerar [!DNL Workfront] avsnitt i [!DNL Salesforce] för alla användare, se [Konfigurera [!DNL Adobe Workfront] avsnitt för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

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

## [!DNL Workfront for Salesforce]

Du kan göra följande när du använder [!DNL Workfront for Salesforce]:

* Skapa nytt manuellt [!DNL Workfront] förfrågningar från [!DNL Salesforce] inom ett säljprojekt eller ett konto.

   Mer information om hur du skapar [!DNL Workfront] förfrågningar från [!DNL Salesforce], se [Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Starta automatiskt skapandet av projekt i [!DNL Workfront] när vissa kriterier är uppfyllda i [!DNL Salesforce]. Dina [!DNL Salesforce] systemadministratören måste konfigurera utlösare för att skapa projekt från [!DNL Salesforce].

   Mer information om hur du skapar [!DNL Workfront] projekt från [!DNL Salesforce], se [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tänk på följande när du arbetar med [!DNL Workfront] for [!DNL Salesforce]:

* Vi stöder båda [!DNL Salesforce Classic] och [!DNL Lightning Experience] ramverk.
* Objekt kan bara skapas från [!DNL Salesforce] in till [!DNL Workfront].
* Du kan visa viss information om [!DNL Workfront] objekt i [!DNL Salesforce].

   Den här informationen kan inte anpassas.

   För en lista med [!DNL Workfront] fält som du kan visa från [!DNL Salesforce], se  [Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  och [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Du kan komma åt objekt som är länkade till [!DNL Salesforce] genom att klicka på **[!UICONTROL Go to Salesforce]** från Workfront.

   Du kan inte visa någon information om [!DNL Salesforce] objekt i [!DNL Workfront], men du har en länk till [!UICONTROL Salesforce] objekt från [!DNL Workfront] för att granska [!DNL Salesforce].

   [!UICONTROL The **Gå till Salesforce**] visas i följande områden:

   * The [!UICONTROL Details] del av ett projekt eller en utgåva
   * Projektets huvud eller en utgåva.

      Systemadministratören eller gruppadministratören måste lägga till [!UICONTROL Integrations] till layoutmallen för att visa [!UICONTROL Go to Salesforce] i projektet eller i ärendehuvudet.
   * The [!DNL Summary] panel för ett problem när du valde ett problem i en lista, efter att du klickat [!UICONTROL Open Summary] ![](assets/summary-panel-icon.png) i listans verktygsfält.

      >[!NOTE]
      >
      >The [!UICONTROL Go to Salesforce] länk är synlig för alla [!DNL Workfront] användare som kan visa projektet eller problemet. Du måste ha en [!DNL Salesforce] för att kunna gå till [!DNL Salesforce] Affärsmöjlighet eller konto där problemet loggades.

* När du uppdaterar fält för ett objekt i ett program uppdateras ingen information om länkade objekt i det andra programmet.
