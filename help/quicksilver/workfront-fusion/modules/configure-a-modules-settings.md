---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Konfigurera en moduls inställningar i  [!DNL Adobe Workfront Fusion]
description: Du måste konfigurera inställningar för varje modul som du skapar.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Konfigurera en moduls inställningar i [!DNL Adobe Workfront Fusion]

Du måste konfigurera inställningar för varje modul som du skapar.

Modulerna [[!DNL Dropbox] modules](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) kräver till exempel att du anger den målmapp där du vill överföra filer. För [[!UICONTROL Email] moduler](../../workfront-fusion/apps-and-their-modules/email-modules.md) måste du ange e-postadressen dit e-postmeddelanden ska skickas.

>[!NOTE]
>
>Förutom modulinställningarna kan du även justera inställningarna för ett scenario. Du kan bland annat byta namn på ditt scenario, ändra dess schema och ange ytterligare inställningar.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr>  
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Konfigurera en moduls inställningar

1. Lägg till en ny modul i ett scenario.

   eller

   Klicka på ikonen för modulen i scenarieredigeraren, enligt beskrivningen i [Skapa ett scenario i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Om det behövs för modulen skapar du ett **[!UICONTROL Connection]** till ditt registrerade användarkonto för den aktuella tjänsten, enligt beskrivningen i [Anslutningsöversikt](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Skriv lämplig text i varje fält.

   eller

   Klicka på **[!UICONTROL Map]** om det visas till höger om fältet och mappa sedan ett objekt från en annan modul i ditt scenario.

   Folidparametrar krävs.

   Mer information om de olika objekttyperna som [!DNL Workfront Fusion] kan identifiera (till exempel datum, nummer och text) finns i [Objektdatatyper i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Villkorligt) Om modulen har avancerade alternativ som du vill visa och använda väljer du **[!UICONTROL Show advanced settings]**.
