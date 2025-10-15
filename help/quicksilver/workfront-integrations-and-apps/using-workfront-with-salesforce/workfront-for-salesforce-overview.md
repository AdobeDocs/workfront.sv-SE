---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce - översikt
description: Du kan installera [!DNL Adobe Workfront] för Salesforce så att dina Salesforce-användare kan skicka [!DNL Workfront] förfrågningar och automatiskt skapa projekt utan att behöva lämna Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] - översikt

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Integreringen av Workfront för Salesforce kommer inte att vara tillgänglig efter den **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Salesforce.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Salesforce finns i [Salesforce-moduler](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Du kan installera [!DNL Adobe Workfront for Salesforce] så att dina [!DNL Salesforce]-användare kan skicka [!DNL Workfront] förfrågningar och automatiskt skapa projekt utan att gå ur [!DNL Salesforce].

Som [!DNL Workfront]-administratör kan du hämta och konfigurera [!DNL Workfront for Salesforce]. Sedan kan du dela den med alla andra [!DNL Salesforce]-användare.

Mer information om hur du installerar [!DNL Workfront for Salesforce] finns i [Installera [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Mer information om hur du konfigurerar avsnittet [!DNL Workfront] i [!DNL Salesforce] för alla användare finns i [Konfigurera avsnittet  [!DNL Adobe Workfront] Konfigurera för [!DNL Salesforce] användare](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

>[!NOTE]
>
>En [!UICONTROL Pro] [!DNL Workfront]-plan krävs för att använda den här funktionen. Mer information om olika tillgängliga planer finns i [[!DNL Workfront] Planer.](https://business.adobe.com/se/products/workfront/pricing.html)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda de funktioner som beskrivs i den här artikeln:

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: Standard<p>
   <p>eller</p>
   <p>Aktuell: Planera</p>


</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## [!DNL Workfront for Salesforce]

Du kan göra följande när du använder [!DNL Workfront for Salesforce]:

* Skapa [!DNL Workfront]-förfrågningar manuellt från [!DNL Salesforce] inom ett säljprojekt eller ett konto.

  Mer information finns i [Skicka [!DNL Adobe Workfront] förfrågningar från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Utlös automatiskt skapande av projekt i [!DNL Workfront] när vissa villkor uppfylls i [!DNL Salesforce]. Din [!DNL Salesforce]-systemadministratör måste konfigurera utlösare för att skapa projekt från [!DNL Salesforce].

  Mer information om hur du skapar [!DNL Workfront] projekt från [!DNL Salesforce] finns i [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tänk på följande när du arbetar med [!DNL Workfront] för [!DNL Salesforce]:

* Vi stöder både ramverken [!DNL Salesforce Classic] och [!DNL Lightning Experience].
* Objekt kan bara skapas från [!DNL Salesforce] till [!DNL Workfront].
* Du kan visa viss information om [!DNL Workfront] objekt i [!DNL Salesforce]. Den här informationen kan inte anpassas.

  En lista med [!DNL Workfront] fält som du kan visa från [!DNL Salesforce] finns i [Skicka [!DNL Adobe Workfront] begäranden från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) och [Skapa [!DNL Adobe Workfront] projekt från [!DNL Salesforce] objekt](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Du kan komma åt objekt som är länkade till [!DNL Salesforce] genom att klicka på länken [!UICONTROL Go to Salesforce] från Workfront.

  Du kan inte visa någon information om [!DNL Salesforce]-objekten i [!DNL Workfront], men det finns en länk i Workfront som tar dig till objektet i Salesforce så att du kan granska det där.

  [!UICONTROL The Go to Salesforce]-länken visas i följande områden:

   * Avsnittet [!UICONTROL Details] i ett projekt eller ett problem.
   * Projektets huvud eller en utgåva.

     Systemadministratören eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna visa länken [!UICONTROL Go to Salesforce] i projektet eller utgåvans huvud.
   * Panelen [!DNL Summary] för ett problem när du markerar problemet i en lista, efter att du klickat på [!UICONTROL Open Summary] ![ikonen för panelen Sammanfattning](assets/summary-panel-icon.png) i listans verktygsfält.

     >[!NOTE]
     >
     >Länken [!UICONTROL Go to Salesforce] är synlig för alla [!DNL Workfront]-användare som kan visa projektet eller problemet. Du måste ha ett [!DNL Salesforce]-konto för att kunna gå till det [!DNL Salesforce]-säljprojekt eller konto där problemet loggades.

* När du uppdaterar fält för ett objekt i ett program uppdateras ingen information om länkade objekt i det andra programmet.
