---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Ersätta knappen Work On It (Arbeta på) med en Start-knapp
description: Adobe Workfront standardkonfiguration innehåller knappen Arbeta med för uppgifter och utgåvor som visas för objekt som du har tilldelats.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Ersätt knappen [!UICONTROL Work On It] med en [!UICONTROL Start]-knapp

Standardkonfigurationen för [!DNL Adobe Workfront] innehåller en [!UICONTROL Work On It]-knapp för uppgifter och ärenden som visas för objekt som du har tilldelats. När du klickar på [!UICONTROL Work On It] för objekt som du har tilldelats, signalerar du till andra användare att du har tagit emot arbetet och bekräftar att du kommer att arbeta med det. Knappen [!DNL Work On It] uppdaterar dock inte aktiviteten eller utgivningsstatusen till en signal om att arbetet faktiskt har startats.

Du kan ersätta knappen [!DNL Work On It] med en [!UICONTROL Start]-knapp för ett team som du tillhör. I det här fallet klickar du på knappen [!UICONTROL Start] i stället för [!UICONTROL Work On It], som automatiskt uppdaterar status och [!UICONTROL Actual Start Date] för arbetsposten och signalerar att du har påbörjat arbetet. Mer information om vilka inställningar som teamet kan påverka dina ändringar i knappen [!UICONTROL Work On It] finns i avsnittet [Konfigurera knappen [!UICONTROL Start]](#configure-the-uicontrol-start-button) i den här artikeln.

>[!IMPORTANT]
>
>Om du klickar på knappen [!UICONTROL Start] ändras objektets status och [!UICONTROL Actual Start Date]. Om någon annan har börjat arbeta med en aktivitet eller ett problem (som ändrade statusen till [!UICONTROL In Progress] och fyllde i [!UICONTROL Actual Start Date]) visas knappen för objektet som [!UICONTROL Work On It] även om ett team du tillhör har fått knappen ersatt med en [!UICONTROL Start]-knapp.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan eller licenstyp du har.

## Konfigurera knappen [!UICONTROL Start]

Om du har en [!UICONTROL Plan]-licens kan du konfigurera knappen [!UICONTROL Start] för ett team i [!UICONTROL Edit]-teamfönstret. Så här fungerar knappen när den har aktiverats för ett team:

* **Teamet har tilldelats en arbetsuppgift**: Om ett team har tilldelats arbetsuppgifterna kan teamets medlemmar se knappen [!UICONTROL Start] och de statusar som har konfigurerats för teamet.
* **Användaren tillhör ett Hem-team**: Om inget team har tilldelats arbetsobjektet men användaren har tilldelats ett Hem-team i sin profil, ser användaren knappen [!UICONTROL Start] och de statusar som har konfigurerats för det teamet. Detta är ett scenario som vi rekommenderar om du vill att användarna ska använda knappen [!UICONTROL Start] ofta.
* **Användaren tilldelas till en arbetsuppgift**: Om det inte finns något team tilldelat arbetsuppgifterna och ingen Hem-grupp tilldelad användaren, men användaren tilldelas arbetsuppgiften, ser användaren knappen [!UICONTROL Start] och den kombinerade statusen som konfigurerats för alla team som de har tilldelats.
* **Användaren har inte tilldelats några team:** Om det inte finns något team tilldelat arbetsuppgifterna och inget team tilldelats användaren, inklusive hemteamet, och objektet tilldelas användaren, visas knappen [!UICONTROL Work On It].

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i
>
>* Mobilappen [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] e-postmeddelanden
>

Så här konfigurerar du knappen Start:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Teams]**.

1. Välj ett team i listrutan **[!UICONTROL Teams]**.\
   eller\
   Klicka på **[!UICONTROL Create Team]**.

1. Klicka på ikonen **[!UICONTROL More]** ![](assets/more-icon.png) och sedan på **[!UICONTROL Edit]**.

1. Hitta knappavsnittet **[!UICONTROL Work On It]** längst ned på sidan [!UICONTROL Edit Teams].
1. Markera kryssrutan **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]**.
1. Välj en eller flera statusvärden för varje arbetsuppgiftstyp. Om du väljer mer än en status visas en listruta när du klickar på [!UICONTROL Start] där du kan välja önskad status.
1. Klicka på **[!UICONTROL Save changes]**. Användarna ser nu en [!UICONTROL Start Task]- eller en [!UICONTROL Start Issue]-knapp i stället för knappen [!UICONTROL Work On It] när de tilldelas en arbetsuppgift.

   >[!NOTE]
   >
   >Vi rekommenderar att du ställer in teamet som en användares hemteam så att startknappen visas på alla deras tilldelade arbetsuppgifter. Se [Associera användare med ett hemteam](#associate-users-with-a-home-team) nedan.

## Associera användare med ett hemteam

Så här associerar du användare med ett hemteam:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka på **[!UICONTROL Users]** och välj sedan den eller de användare som du vill associera med ett hemteam.
1. Klicka på menyn **[!UICONTROL More]** och välj sedan **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Markera fältet **[!UICONTROL Home Team]** i avsnittet **[!UICONTROL Organization]**. Börja skriva namnet på det team vars inställningar du vill associera med användarna. Klicka på teamets namn när du ser det i listan.

1. Klicka på **[!UICONTROL Save Changes]**.\
   De användare du har valt är nu associerade med ett hemteam.

   Alla gruppinställningar, inklusive statusvärdena som är kopplade till knappen [!UICONTROL Done], visas nu för dessa användare.

