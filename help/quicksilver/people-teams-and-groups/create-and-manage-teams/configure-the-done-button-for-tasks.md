---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurera Klar-knappen för uppgifter
description: Knappen Klar kan automatiskt ange status för en uppgift eller ett problem. Som standard markeras en uppgift som Slutfört när en tilldelad klickar på Klar på sin arbetsuppgift.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Done] knapp för uppgifter

The [!UICONTROL Done] kan automatiskt ange status för en uppgift eller ett problem. Som standard [!UICONTROL Adobe Workfront] markerar en uppgift som [!UICONTROL Completed] när en tilldelad klickar på Klar på sin arbetsuppgift.

## Översikt

Användare med vissa behörigheter kan konfigurera [!UICONTROL Done] om du vill visa vissa statusvärden i systemet. Det finns två olika sätt [!UICONTROL Done] fungerar för uppgifter i [!UICONTROL Workfront]:

* Om användaren har ett tilldelat Home Team, [!DNL Workfront] administratör eller en användare med [!UICONTROL Plan] licensen kan konfigurera [!UICONTROL Done] för att visa vissa statusvärden för teammedlemmar. Se [Konfigurera [!UICONTROL Done] knapp för ett team](#configure-the-uicontrol-done-button-for-a-team) i den här artikeln.
* Om användaren inte har en [!UICONTROL Home Team], men de har [!UICONTROL Other Teams] i sin profil söker Workfront efter inställningen för [!UICONTROL Done] på något av de team som är kopplade till användaren. Markeringen är slumpmässig och statusen som är associerad med någon av grupperna används för uppgiften.
* Om användaren inte har tilldelats något hemteam [!UICONTROL Done] knappen för uppgifter är kopplad till en fullständig status. Det finns inga konfigurationsalternativ tillgängliga i det här scenariot. The [!UICONTROL Done] anges automatiskt som standard för denna knapp.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] plan*</strong></p></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licens*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Konfigurera [!UICONTROL Done] knapp för ett team

Du kan ändra vilken status som ska användas för arbetsuppgiften med [!UICONTROL Done] -knappen. Du kan också ange flera statusvärden och låta användaren välja vilken status som passar bäst.

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Teams]**.

1. Klicka på **[!UICONTROL Switch team]** väljer du sedan ett nytt team i listrutan eller söker efter ett team i sökfältet.
1. Klicka på **[!UICONTROL More]** menyn och klicka sedan på **[!UICONTROL Edit]**.
1. Hitta **[!UICONTROL Done Button]** längst ned i **[!UICONTROL Team Settings]** sida.

1. Välj en status eller mer än en status för varje arbetsuppgiftstyp.

   >[!NOTE]
   >
   >Tänk på följande när du väljer status för uppgifter eller problem:
   >
   >* När du väljer en status för varje typ av arbetsuppgift, ställs uppgiften eller utleveransstatusen in på den statusen när en användare klickar på [!UICONTROL Done] på deras objekt. Om du anger flera statusvärden för varje typ av arbetsuppgift läggs en listruta till i [!UICONTROL Done] och användaren måste välja en status för att kunna ändra status för arbetsuppgiften.
   >* Du kan bara associera statusvärden på systemnivå med [!UICONTROL Done] -knappen. Du kan inte associera gruppspecifika statusvärden med arbetsartikelstatusvärden.
   >* När en användare som är tilldelad objektet placerar objektet i den status som är associerad med [!UICONTROL Done] -knapp, objektet visas som [!UICONTROL Done] för den användaren oavsett om den valda statusen är en [!UICONTROL Completed] eller [!UICONTROL Closed] status eller en arbetsstatus.
   >   
   >   
   >  Du kan till exempel associera [!UICONTROL Done] knapp med [!UICONTROL In Progress] gör att arbetsuppgiften visas som [!UICONTROL Done] för användaren som ändrar status från [!UICONTROL New] till [!UICONTROL In progress].
   >   
   >* Problemtyperna är anpassningsbara och kan ha andra namn än de som visas nedan i din miljö.\
   >  Följande är standardåtgärder och problemtyper:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   Om uppgiften eller utgåvan har tilldelats flera användare visas en[!UICONTROL Done with my part]&quot; i den nedrullningsbara menyn, förutom de olika statusar som valts för ditt team.

1. Klicka på **[!UICONTROL Save Changes]**.

## Associera användare med ett hemteam

Så här gör du ändringar i [!UICONTROL Done] för användarna kan du göra de inställningar som du har ändrat i hemgruppen för användarna synliga.

Så här associerar du användare med ett hemteam:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka **[!UICONTROL Users]** väljer du sedan den eller de användare som du vill associera med ett hemteam.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. I **[!UICONTROL Organization]** väljer du **[!UICONTROL Home Team]** fält. Börja skriva namnet på det team vars inställningar du vill associera med användarna. Klicka på teamets namn när du ser det i listan.

1. Klicka på **[!UICONTROL Save Changes]**.\
   De användare du har valt är nu associerade med ett hemteam.
Alla gruppinställningar, inklusive statusvärdena som är kopplade till [!UICONTROL Done] knappen visas nu för dessa användare.
