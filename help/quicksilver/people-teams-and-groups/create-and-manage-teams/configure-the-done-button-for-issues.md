---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurera Klar-knappen för problem
description: Knappen Klar kan automatiskt ange status för en uppgift eller ett problem. Som standard markerar Adobe Workfront ett problem som Löst när en tilldelad klickar på Klar på sin arbetsuppgift.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Done] knapp för problem

The [!UICONTROL Done] kan automatiskt ange status för en uppgift eller ett problem. Som standard [!DNL Adobe Workfront] markerar ett problem som [!UICONTROL Resolved] när en tilldelad klickar [!UICONTROL Done] på deras arbetsuppgift.

## Översikt

Användare med vissa behörigheter kan konfigurera [!UICONTROL Done] om du vill visa vissa statusvärden i systemet. Det finns tre olika sätt [!UICONTROL Done] fungerar för problem i [!DNL Workfront]:

* Om användaren har en tilldelad [!UICONTROL Home Team], a [!DNL Workfront] administratör eller en användare med [!UICONTROL Plan] licensen kan konfigurera [!UICONTROL Done] för att visa vissa statusvärden för teammedlemmar. Se [Konfigurera [!UICONTROL Done] knapp för ett team](#configure-the-uicontrol-done-button-for-a-team) i den här artikeln.
* Om användaren inte har en [!UICONTROL Home Team] tilldelade, [!UICONTROL Done] knapp för problem är kopplad till ett systemgenererat [!UICONTROL Resolved] status som har kod med tre bokstäver [!UICONTROL RLV]. Det finns inga konfigurationsalternativ tillgängliga i det här scenariot. The [!UICONTROL Done] anges automatiskt som standard för denna knapp.
* Om [!UICONTROL Resolved] ([!UICONTROL RLV]) tas bort och användaren markerar problemet som [!UICONTROL Done] har inte [!UICONTROL Home Team]är standardutgivningsstatusen knuten till det som är inställt som standard för [!UICONTROL Closed] för gruppen som är tilldelad projektet som utleveransen tillhör. Workfront-administratören kan konfigurera en systemomfattande standardinställning för gruppen. Se [Konfigurera [!UICONTROL Done] när [!UICONTROL Resolved] status har tagits bort](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) i den här artikeln.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td>Systemadministratörsåtkomst krävs för att konfigurera [!UICONTROL Done] när [!UICONTROL Resolved] status har tagits bort</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

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
   >  Du kan till exempel associera [!UICONTROL Done] knappen Pågår gör att arbetsposten visas som [!UICONTROL Done] för den användare som ändrar status från Nytt till Pågår.
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
Alla gruppinställningar, inklusive statusvärdena som är kopplade till [!UICONTROL Done] är nu synliga för dessa användare.

## Konfigurera [!UICONTROL Done] när [!UICONTROL Resolved] status har tagits bort

Om en användare inte har något hemteam och det systemomfattande standardvärdet för [!UICONTROL Resolved] ([!UICONTROL RLV]) har tagits bort, en [!DNL Workfront] administratören kan konfigurera [!UICONTROL Closed] status för gruppen på projektet. [!DNL Workfront] väljer den här statusen för ett stängt problem när användaren klickar på [!DNL Done] -knappen.

### Hitta gruppen som är associerad med projektet

När en användare skapar ett projekt tilldelas hemgruppen automatiskt till projektet. Användare med [!UICONTROL Manage] åtkomst till projektet kan ändra gruppen i [!UICONTROL Project Details] när som helst. För att förstå vilken status [!DNL Workfront] används för ett slutfört problem i det här fallet måste du förstå vilken grupp som är associerad med projektet som problemet gäller och vilken standardstatus för [!UICONTROL Closed] den här gruppen har för problem.

Så här hittar du gruppen som är associerad med projektet:

1. Gå till ett projekt.
1. Klicka på till vänster på sidan **[!UICONTROL Project Details]**.
1. Leta reda på **[!UICONTROL Project association]** avsnitt, hitta **[!UICONTROL Group]**.\
   Det här är gruppnamnet som du behöver använda för att kontrollera statusen i inställningsområdet. I följande avsnitt finns instruktioner om hur du uppdaterar standardstatusen för en viss grupp.

### Uppdatera standardstatus för en viss grupp

Som [!UICONTROL Workfront] kan du uppdatera status för en viss grupp:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på i den vänstra panelen **[!UICONTROL Project Preferences]** sedan **[!UICONTROL Statuses]**.

1. Klicka **[!UICONTROL Issues]** och skriv sedan namnet på gruppen i **[!UICONTROL System Statuses]** sökruta till höger.

1. Markera gruppen.
1. Klicka på **[!UICONTROL Set Default Statuses]** nedrullningsbar meny och välj sedan en standardstatus för [!UICONTROL Closed]. [!DNL Workfront] använder den här statusen för ett stängt problem när en användare klickar på [!UICONTROL Done] -knappen.

   >[!IMPORTANT]
   >
   >Den här statusen används endast när användaren inte har tilldelats något Home Team och [!UICONTROL RLV] status har tagits bort.

1. Klicka på **[!UICONTROL Save]**.
