---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administrera Adobe Workfront Fusion Templates
description: Om du är administratör har du behörighet att visa, ändra, byta namn på, publicera, godkänna och ta bort mallar som skapats av andra. Du kan utföra dessa åtgärder från [!UICONTROL Templates] sidan i [!DNL Adobe Workfront Fusion Administration] område.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Malladministration

Om du är administratör har du behörighet att visa, ändra, byta namn på, publicera, godkänna och ta bort mallar som skapats av andra. Du kan utföra dessa åtgärder från [!UICONTROL Templates] sidan i [!DNL Adobe Workfront Fusion Administration] område.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront Fusion-administratör för din organisation.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Visa [!DNL Workfront Fusion] mallar som administratör

Så här visar du en tabell över alla mallar som skapats och deras status:

1. Klicka **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna [!UICONTROL Administration] område.
1. Klicka **[!UICONTROL Templates]** i den vänstra navigeringspanelen.

Det finns tre kolumner som är relaterade till mallens publiceringsstatus. En bock i en kolumn anger följande:

* **[!UICONTROL Published]**: Dessa mallar visas för närvarande i [!UICONTROL Team templates] i användargränssnittet.
* **[!UICONTROL Requested approval]**: Dessa mallar väntar på ditt godkännande. De är synliga i [!UICONTROL Team templates] i användargränssnittet.
* **[!UICONTROL Approved]**: Dessa mallar har godkänts. De är synliga i [!UICONTROL Public templates] i standardgränssnittet.

>[!NOTE]
>
>Mallar med bockmarkering i båda [!UICONTROL Requested approval] kolumn och i [!UICONTROL Approved] -kolumnen har redan godkänts och publicerats, men det finns en nyare version av dem som väntar på ditt godkännande.

## Redigera [!DNL Workfront Fusion] mallar som administratör

1. Klicka **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna [!UICONTROL Administration] område.
1. Klicka **[!UICONTROL Templates]** i den vänstra navigeringspanelen.
1. Klicka **[!UICONTROL Detail]** till höger om mallen som du vill redigera.

Du kan nu redigera mallen på liknande sätt som när du redigerar en mall som en icke-adminanvändare. I dialogrutan [!UICONTROL Options] i det övre högra hörnet finns det ytterligare ett alternativ - SVG-diagrammet som innehåller SVG-koden. Publiceringsprocessen är densamma som för en standardanvändare. Mer information finns i avsnittet Publicerings- och delningsmallar.

Mer information om särskilda mallalternativ som du kan redigera finns i [Skapa nya mallar i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Mer information om publiceringsmallar finns i [Publicera och dela [!DNL Adobe Workfront Fusion] mallar](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Godkänn eller avslå [!DNL Workfront Fusion] mallar

Om du godkänner en mall visas den i [!UICONTROL Public templates] och är tillgängliga för alla användare. Om du avvisar en mall tas den bort från [!UICONTROL Public templates] och gör den tillgänglig endast för det team som skapade den.

1. Klicka **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna [!UICONTROL Administration] område.
1. Klicka **[!UICONTROL Templates]** i den vänstra navigeringspanelen.
1. Om du vill godkänna en mall klickar du på **[!UICONTROL Approve]** till höger om mallen.
1. Om du inte vill godkänna en mall klickar du på **[!UICONTROL Disapprove]** till höger om mallen.

>[!NOTE]
>
>Om du godkänner mallen som tidigare godkänts och sedan redigerats, kommer ditt andra godkännande att skriva över den ursprungliga mallen.

## Klona ett scenario som en mall

Som administratör kan du klona ett scenario som en mall.

Instruktioner om hur du klonar ett scenario som en mall finns i [Skapa nya mallar i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create)in [Skapa nya mallar i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
