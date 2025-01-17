---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administrera Adobe Workfront Fusion Templates
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Administrering av [!DNL Adobe Workfront Fusion] mallar

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artiklarna:
>
>* [Godkänn eller avböj mallar för fliken Offentligt](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [Redigera mallar](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Om du är administratör har du behörighet att visa, ändra, byta namn på, publicera, godkänna och ta bort mallar som skapats av andra. Du kan utföra dessa åtgärder från sidan [!UICONTROL Templates] i området [!DNL Adobe Workfront Fusion Administration].

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
  <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront Fusion-administratör för din organisation.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Visa [!DNL Workfront Fusion]-mallar som en [!DNL Workfront Fusion]-administratör

Så här visar du en tabell över alla mallar som skapats och deras status:

1. Klicka på **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna området [!UICONTROL Administration].

   >[!NOTE]
   >
   >Administrationsområdet visas bara för Workfront Fusion-administratörer.

1. Klicka på **[!UICONTROL Templates]** i den vänstra navigeringspanelen.

Det finns tre kolumner som är relaterade till mallens publiceringsstatus. En bock i en kolumn anger följande:

* **[!UICONTROL Published]**: Dessa mallar visas för närvarande på fliken [!UICONTROL Team templates] i användargränssnittet.
* **[!UICONTROL Requested approval]**: De här mallarna väntar på ditt godkännande. De visas för närvarande på fliken [!UICONTROL Team templates] i användargränssnittet.
* **[!UICONTROL Approved]**: Dessa mallar har godkänts. De visas för närvarande på fliken [!UICONTROL Public templates] i standardanvändargränssnittet.

>[!NOTE]
>
>Mallar med bockmarkeringen i både kolumnen [!UICONTROL Requested approval] och kolumnen [!UICONTROL Approved] har redan godkänts och publicerats, men det finns en nyare version av dem som väntar på ditt godkännande.

## Redigera [!DNL Workfront Fusion]-mallar som administratör

1. Klicka på **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna området [!UICONTROL Administration].
1. Klicka på **[!UICONTROL Templates]** i den vänstra navigeringspanelen.
1. Klicka på **[!UICONTROL Detail]** till höger om mallen som du vill redigera.

Du kan nu redigera mallen på liknande sätt som när du redigerar en mall som en icke-adminanvändare. I [!UICONTROL Options] i det övre högra hörnet finns det dock ytterligare ett alternativ - SVG-diagrammet som innehåller SVG-koden. Publiceringsprocessen är densamma som för en standardanvändare. Mer information finns i avsnittet Publicerings- och delningsmallar.

Mer information om särskilda mallalternativ som du kan redigera finns i [Skapa nya mallar i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Mer information om publiceringsmallar finns i [Publish och dela [!DNL Adobe Workfront Fusion] mallar](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Godkänn eller avgodkänn [!DNL Workfront Fusion] mallar

Om du godkänner en mall blir den synlig på fliken [!UICONTROL Public templates] och tillgänglig för alla användare. Om du avvisar en mall tas den bort från fliken [!UICONTROL Public templates] och blir bara tillgänglig för det team som skapade den.

1. Klicka på **[!UICONTROL Administration]** i den vänstra navigeringspanelen för att öppna området [!UICONTROL Administration].
1. Klicka på **[!UICONTROL Templates]** i den vänstra navigeringspanelen.
1. Om du vill godkänna en mall klickar du på **[!UICONTROL Approve]** till höger om mallen.
1. Om du inte vill godkänna en mall klickar du på **[!UICONTROL Disapprove]** till höger om mallen.

>[!NOTE]
>
>Om du godkänner mallen som tidigare godkänts och sedan redigerats, kommer ditt andra godkännande att skriva över den ursprungliga mallen.

## Klona ett scenario som en mall

Som administratör kan du klona ett scenario som en mall.

Instruktioner om hur du klonar ett scenario som en mall finns i [Skapa en mall från ett scenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) i [Skapa nya mallar i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
