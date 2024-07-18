---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Anslutningar - översikt
description: För de flesta program är det nödvändigt att skapa en anslutning genom vilken  [!DNL Adobe Workfront Fusion] kan kommunicera med den angivna tredjepartstjänsten enligt inställningarna för det specifika scenariot.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Anslutningar - översikt

<!-- Audited: 3/2024-->

För de flesta appar kräver [!DNL Workfront Fusion] en anslutning, genom vilken den kan kommunicera med den angivna tredjepartstjänsten enligt inställningarna för det specifika scenariot.

Om du till exempel vill skapa ett scenario som hämtar information från [!DNL Workfront], måste du ge [!DNL Workfront Fusion] åtkomstbehörighet för ditt [!DNL Workfront]-konto.

En anslutning representerar den behörighet och de behörigheter som Fusion använder för att komma åt programmet. Du kan skapa en eller flera anslutningar för varje program och använda samma anslutning i flera moduler eller scenarier.

De flesta anslutningar används endast för ett enda program. En [!DNL Workfront]-anslutning kan till exempel inte användas i en [!UICONTROL Salesforce]-modul. Vissa [!DNL Adobe]-program kan dela anslutningar. Mer information finns i artiklarna för dessa program, som listas i [Appar och deras moduler](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Anslutningar hanteras på teamnivå. Alla medlemmar i ett team har tillgång till teamets anslutningar, och användare utanför ett team har inte tillgång till teamets anslutningar.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuell: Inga [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Äldre: Alla </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Planen [!DNL Workfront Fusion] ingår.</li></ul>
   <p>eller</p>
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Åtkomsträttigheter

För varje anslutning kräver [!DNL Workfront Fusion] bara de åtkomsträttigheter som krävs för att slutföra ett visst scenario. Om du till exempel skapar ett scenario för att lista dokument från [!DNL Google Docs], frågar [!DNL Workfront Fusion] inte efter behörighet att hämta dokumentens innehåll. Om du senare upptäcker att du behöver komma åt innehållet i dokumenten kan du uppdatera anslutningen eller skapa en ny som kan komma åt innehållet.

Du kan inte begränsa åtkomsten till vissa uppgifter med alla tjänster. I dessa fall måste [!DNL Workfront Fusion] kräva fullständig åtkomstbehörighet. Mer information om hur du begränsar [!DNL Workfront Fusion]-åtkomst till ditt konto som är registrerat för dessa tjänster finns i den programspecifika dokumentationen som listas i [Appar och deras moduler](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Hantera anslutningar

Du kan hantera alla anslutningar från området [!UICONTROL Connections].

>[!NOTE]
>
>Anslutningarna ägs av team. Om du inte kan hitta den anslutning du letar efter kontrollerar du att du visar rätt team.
>
>Välj ett nytt team:
>
>* Klicka på teamnamnet till vänster och välj ett nytt team.
>
>    eller
>
>* Klicka på Teamöversikt i den vänstra navigeringen och klicka sedan på listrutepilen bredvid teamnamnet uppe på sidan. Välj ett nytt team.

1. Om du vill öppna området [!UICONTROL Connections] klickar du på <b>[!UICONTROL Connections]</b> i den vänstra navigeringen.
1. (Valfritt) Ange miljö och typ av anslutning genom att klicka på listrutan Miljö och Typ och välja ett alternativ.
1. (Valfritt) Om du vill visa vilka behörigheter som tilldelats [!DNL Workfront Fusion] för en anslutning klickar du på ikonen Visa ![Visa anslutningsbehörigheter](assets/view-connection-permissions.png) för anslutningen.
1. (Valfritt) Om du vill byta namn på en anslutning markerar du anslutningsnamnet och skriver det nya namnet.
1. (Valfritt) Om du vill återauktorisera en anslutning klickar du på **Återauktorisera** för anslutningen.
1. (Valfritt) Om du vill ta bort en anslutning klickar du på **Ta bort** för den anslutningen.
1. (Valfritt) Om du vill verifiera att anslutningen till tjänsten har upprättats klickar du på **Verifiera** för anslutningen.



## Förnya en anslutning

[!DNL Workfront Fusion] får vanligtvis åtkomstbehörighet till en viss tjänst under en obegränsad tidsperiod. För vissa program krävs att åtkomstbehörigheten förnyas efter en viss tidsperiod. I dessa fall meddelar [!DNL Workfront Fusion] dig via e-post kort innan dess åtkomsträttigheter upphör att gälla.

Så här förnyar du en anslutning:

1. Klicka på knappen **[!UICONTROL Reauthorize]** i området **[!UICONTROL Connections]**.
