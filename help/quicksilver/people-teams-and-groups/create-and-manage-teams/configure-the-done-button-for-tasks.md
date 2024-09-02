---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurera Klar-knappen för uppgifter
description: Knappen Klar kan automatiskt ange status för en uppgift eller ett problem. Som standard markeras en uppgift som Slutfört när en tilldelad klickar på Klar på sin arbetsuppgift.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Konfigurera knappen [!UICONTROL Done] för uppgifter

Knappen [!UICONTROL Done] kan automatiskt ange status för en aktivitet eller ett problem. Som standard markeras en uppgift som [!UICONTROL Completed] när en tilldelad klickar på Klar på sin arbetsuppgift.[!UICONTROL Adobe Workfront]

## Ökning

Användare med vissa behörigheter kan konfigurera knappen [!UICONTROL Done] så att den återspeglar vissa statusvärden i systemet. Det finns två olika sätt att använda knappen [!UICONTROL Done] för åtgärder i [!UICONTROL Workfront]:

* Om användaren har ett tilldelat Home Team kan en [!DNL Workfront]-administratör eller en användare med en [!UICONTROL Plan]-licens konfigurera knappen [!UICONTROL Done] så att den återspeglar vissa statusvärden för teammedlemmar. Se [Konfigurera knappen [!UICONTROL Done] för ett team](#configure-the-uicontrol-done-button-for-a-team) i den här artikeln.
* Om användaren inte har någon [!UICONTROL Home Team], men har [!UICONTROL Other Teams] i sin profil, söker Workfront efter inställningen för knappen [!UICONTROL Done] i något av de team som är kopplade till användaren. Markeringen är slumpmässig och statusen som är associerad med någon av grupperna används för uppgiften.
* Om användaren inte har tilldelats något hemteam är knappen [!UICONTROL Done] för uppgifter knuten till en fullständig status. Det finns inga konfigurationsalternativ tillgängliga i det här scenariot. Knappen [!UICONTROL Done] får automatiskt den här statusen som standard.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera knappen [!UICONTROL Done] för ett team

Du kan ändra vilken status som ska användas för arbetsobjektet med knappen [!UICONTROL Done]. Du kan också ange flera statusvärden och låta användaren välja vilken status som passar bäst.

{{step1-to-team}}

1. Klicka på ikonen **[!UICONTROL Switch team]** och välj sedan ett nytt team i listrutan eller sök efter ett team i sökfältet.
1. Klicka på menyn **[!UICONTROL More]** och sedan på **[!UICONTROL Edit]**.
1. Hitta avsnittet **[!UICONTROL Done Button]** längst ned på sidan **[!UICONTROL Team Settings]**.

1. Välj en status eller mer än en status för varje arbetsuppgiftstyp.

   >[!NOTE]
   >
   >Tänk på följande när du väljer status för uppgifter eller problem:
   >
   >* När du väljer en status för varje typ av arbetsuppgift, ställs uppgiften eller utleveransstatusen in på den statusen när en användare klickar på [!UICONTROL Done] på sitt objekt. Om du anger flera statusvärden för varje typ av arbetsobjekt läggs en nedrullningsbar meny till i knappen [!UICONTROL Done] och användaren måste välja en status för att kunna ändra statusen för arbetsobjektet.
   >* Du kan bara associera statusvärden på systemnivå med knappen [!UICONTROL Done]. Du kan inte associera gruppspecifika statusvärden med arbetsartikelstatusvärden.
   >* När en användare som är tilldelad objektet placerar objektet i den status som är associerad med knappen [!UICONTROL Done], visas objektet som [!UICONTROL Done] för den användaren oavsett om den status du väljer är en [!UICONTROL Completed] - eller [!UICONTROL Closed] -status eller en arbetsstatus.
   >   
   >   
   >  Om du till exempel associerar knappen [!UICONTROL Done] med [!UICONTROL In Progress] visas arbetsposten som [!UICONTROL Done] för användaren som ändrar statusen från [!UICONTROL New] till [!UICONTROL In progress].
   >   
   >* Problemtyperna är anpassningsbara och kan ha andra namn än de som visas nedan i din miljö.\
   >  Följande är standardåtgärder och problemtyper:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   Om aktiviteten eller utgåvan har tilldelats flera användare visas ett [!UICONTROL Done with my part]-alternativ i listrutan, utöver de statusvärden som har valts för ditt team.

1. Klicka på **[!UICONTROL Save Changes]**.

## Associera användare med ett hemteam

Om du vill göra ändringarna av [!UICONTROL Done]-knappfunktionen synliga för användarna kan du göra gruppen vars inställningar du har ändrat hemgruppen för användarna.

Så här associerar du användare med ett hemteam:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka på **[!UICONTROL Users]** och välj sedan den eller de användare som du vill associera med ett hemteam.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Markera fältet **[!UICONTROL Home Team]** i avsnittet **[!UICONTROL Organization]**. Börja skriva namnet på det team vars inställningar du vill associera med användarna. Klicka på teamets namn när du ser det i listan.

1. Klicka på **[!UICONTROL Save Changes]**.\
   De användare du har valt är nu associerade med ett hemteam.
Alla gruppinställningar, inklusive statusvärdena som är kopplade till knappen [!UICONTROL Done], visas nu för dessa användare.
