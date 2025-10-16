---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurera Klar-knappen för problem
description: Knappen Klar kan automatiskt ange status för en uppgift eller ett problem. Som standard markerar Adobe Workfront ett problem som Löst när en tilldelad klickar på Klar på sin arbetsuppgift.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---

# Konfigurera knappen [!UICONTROL Done] för problem

Knappen [!UICONTROL Done] kan automatiskt ange status för en aktivitet eller ett problem. Som standard markerar [!DNL Adobe Workfront] ett problem som [!UICONTROL Resolved] när en tilldelad klickar på [!UICONTROL Done] på sin arbetspost.

>[!NOTE]
>
>Knappen Klar visas som Markera som färdig i alla områden av Workfront.

## Översikt

Användare med vissa behörigheter kan konfigurera knappen [!UICONTROL Done] så att den återspeglar vissa statusvärden i systemet. Det finns tre olika sätt som knappen [!UICONTROL Done] fungerar på för problem i [!DNL Workfront]:

* Om användaren har en tilldelad [!UICONTROL Home Team] kan en [!DNL Workfront]-administratör eller en användare med en [!UICONTROL Plan]-licens konfigurera knappen [!UICONTROL Done] så att den återspeglar vissa statusvärden för teammedlemmar. Se [Konfigurera knappen [!UICONTROL Done] för ett team](#configure-the-uicontrol-done-button-for-a-team) i den här artikeln.
* Om användaren inte har någon [!UICONTROL Home Team], men har [!UICONTROL Other Teams] i sin profil, söker Workfront efter inställningen för knappen [!UICONTROL Done] i något av de team som är kopplade till användaren. Urvalet är slumpmässigt och statusen som är associerad med någon av teamen används för problemet.
* Om användaren inte har tilldelats [!UICONTROL Home Team] är knappen [!UICONTROL Done] för problem kopplad till en systemgenererad [!UICONTROL Resolved]-status som har koden [!UICONTROL RLV] med tre bokstäver. Det finns inga konfigurationsalternativ tillgängliga i det här scenariot. Knappen [!UICONTROL Done] får automatiskt den här statusen som standard.
* Om statusen [!UICONTROL Resolved] ([!UICONTROL RLV]) tas bort och användaren markerar problemet som [!UICONTROL Done] har ingen [!UICONTROL Home Team], är standardutgivningsstatusen knuten till det som har angetts som standard för [!UICONTROL Closed] för gruppen som tilldelats det projekt som utleveransen tillhör. Workfront-administratören kan konfigurera en systemomfattande standardinställning för gruppen. Se [Konfigurera knappen [!UICONTROL Done] när statusen [!UICONTROL Resolved] har tagits bort](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) i den här artikeln.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront package</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Systemadministratörsåtkomst krävs för att konfigurera Klar-knappen när statusen Löst tas bort</p> </td> 
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
   >  Om du till exempel associerar knappen [!UICONTROL Done] med Pågår visas arbetsobjektet som [!UICONTROL Done] för användaren som ändrar statusen från Nytt till Pågår.
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

1. Markera fältet **[!UICONTROL Organization]** i avsnittet **[!UICONTROL Home Team]**. Börja skriva namnet på det team vars inställningar du vill associera med användarna. Klicka på teamets namn när du ser det i listan.

1. Klicka på **[!UICONTROL Save Changes]**.\
   De användare du har valt är nu associerade med ett hemteam.
Alla gruppinställningar, inklusive statusvärdena som är kopplade till knappen [!UICONTROL Done], visas nu för dessa användare.

## Konfigurera knappen [!UICONTROL Done] när statusen [!UICONTROL Resolved] har tagits bort

Om en användare inte har något hemteam och det systemomfattande standardvärdet för [!UICONTROL Resolved] ([!UICONTROL RLV]) har tagits bort, kan en [!DNL Workfront]-administratör konfigurera [!UICONTROL Closed]-statusen för gruppen på projektet. [!DNL Workfront] väljer den här statusen för ett stängt problem när användaren klickar på knappen [!DNL Done].

### Sök efter gruppen som är associerad med projektet

När en användare skapar ett projekt tilldelas hemgruppen automatiskt till projektet. Användare med [!UICONTROL Manage] åtkomst till projektet kan när som helst ändra den här gruppen i avsnittet [!UICONTROL Project Details]. För att förstå vilken status [!DNL Workfront] använder för ett slutfört problem i det här fallet måste du förstå vilken grupp som är associerad med projektet som problemet gäller och vilken standardstatus för [!UICONTROL Closed] som den här gruppen har för problem.

Så här söker du efter gruppen som är associerad med projektet:

1. Gå till ett projekt.
1. Klicka på **[!UICONTROL Project Details]** till vänster på sidan.
1. Leta reda på avsnittet **[!UICONTROL Project association]** och sök efter **[!UICONTROL Group]**.\
   Det här är gruppnamnet som du behöver använda för att kontrollera statusen i inställningsområdet. I följande avsnitt finns instruktioner om hur du uppdaterar standardstatusen för en viss grupp.

### Uppdatera standardstatus för en viss grupp

Som [!UICONTROL Workfront]-administratör kan du uppdatera statusen för en specifik grupp:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicka på **[!UICONTROL Project Preferences]** i den vänstra panelen och sedan på **[!UICONTROL Statuses]**.

1. Klicka på **[!UICONTROL Issues]** och skriv sedan namnet på gruppen i sökrutan **[!UICONTROL System Statuses]** till höger.

1. Markera gruppen.
1. Klicka på listrutan **[!UICONTROL Set Default Statuses]** och välj sedan en standardstatus för [!UICONTROL Closed]. [!DNL Workfront] använder den här statusen för ett stängt problem när en användare klickar på knappen [!UICONTROL Done].

   >[!IMPORTANT]
   >
   >Den här statusen används endast när användaren inte har tilldelats något hemteam och [!UICONTROL RLV]-statusen har tagits bort.

1. Klicka på **[!UICONTROL Save]**.
