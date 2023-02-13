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

# Ersätt [!UICONTROL Work On It] knapp med [!UICONTROL Start] knapp

[!DNL Adobe Workfront]Standardkonfigurationen innehåller en [!UICONTROL Work On It] för uppgifter och utgåvor som visas för objekt som du har tilldelats. När du klickar [!UICONTROL Work On It] för objekt som du har tilldelats signalerar du till andra användare att du har tagit emot arbetet och bekräftar att du kommer att arbeta med det. Men [!DNL Work On It] knappen uppdaterar inte aktiviteten eller utgivningsstatusen för att signalera att arbetet faktiskt har startats.

Du kan ersätta [!DNL Work On It] knapp med [!UICONTROL Start] för ett team som du tillhör. I så fall klickar du på [!UICONTROL Start] i stället för [!UICONTROL Work On It]som automatiskt uppdaterar status och [!UICONTROL Actual Start Date] av arbetsuppgiften, vilket signalerar att du har påbörjat arbetet. Information om vilka inställningar som kan påverka dina ändringar i [!UICONTROL Work On It] finns i avsnittet [Konfigurera [!UICONTROL Start] knapp](#configure-the-uicontrol-start-button) i den här artikeln.

>[!IMPORTANT]
>
>Klicka på [!UICONTROL Start] ändras objektets status och [!UICONTROL Actual Start Date]. Om någon annan har börjat arbeta med en uppgift eller ett problem (som ändrade status till [!UICONTROL In Progress] och fyller i [!UICONTROL Actual Start Date]) visas knappen för objektet som [!UICONTROL Work On It] även när ett team du tillhör har fått knappen ersatt med en [!UICONTROL Start] -knappen.

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

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Konfigurera [!UICONTROL Start] knapp

Om du har en [!UICONTROL Plan] -licensen kan du konfigurera [!UICONTROL Start] för ett team i [!UICONTROL Edit] teamfönstret. Så här fungerar knappen när den har aktiverats för ett team:

* **Teamet har tilldelats en arbetsuppgift**: Om ett team har tilldelats arbetsuppgiften kan medlemmarna i teamet se [!UICONTROL Start] och status som konfigurerats för teamet.
* **Användaren tillhör ett hemteam**: Om inget team har tilldelats arbetsposten men användaren har tilldelats ett hemteam i sin profil, ser användaren [!UICONTROL Start] och status som konfigurerats för teamet. Detta är det scenario vi rekommenderar om du vill att användarna ska använda [!UICONTROL Start] ofta.
* **Användaren är tilldelad till en arbetsuppgift**: Om inget team har tilldelats arbetsuppgiften och inget hemteam har tilldelats användaren, men användaren har tilldelats arbetsuppgiften, ser användaren [!UICONTROL Start] och de kombinerade statusar som konfigurerats för alla team som de har tilldelats.
* **Användaren har inte tilldelats några team:** Om inget team är tilldelat arbetsuppgiften och användaren inte har något team, inklusive hemteamet, och objektet är tilldelat användaren, visas användaren som [!UICONTROL Work On It] -knappen.

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig i
>
>* The [!DNL Workfront] mobilapp
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] e-postmeddelanden
>


Så här konfigurerar du knappen Start:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Teams]**.

1. I **[!UICONTROL Teams]** väljer du ett team.\
   eller\
   Klicka på **[!UICONTROL Create Team]**.

1. Klicka på **[!UICONTROL More]** icon ![](assets/more-icon.png)och sedan klicka **[!UICONTROL Edit]**.

1. Hitta **[!UICONTROL Work On It]** knappavsnitt långt ned i [!UICONTROL Edit Teams] sida.
1. Välj **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]** kryssruta.
1. Välj en eller flera statusvärden för varje arbetsuppgiftstyp. Om du väljer mer än en status visas en listruta när du klickar på [!UICONTROL Start] där du kan välja önskad status.
1. Klicka på **[!UICONTROL Save changes]**. Användarna ser nu en [!UICONTROL Start Task] eller en [!UICONTROL Start Issue] i stället för [!UICONTROL Work On It] när de tilldelas en arbetsuppgift.

   >[!NOTE]
   >
   >Vi rekommenderar att du ställer in teamet som en användares hemteam så att startknappen visas på alla deras tilldelade arbetsuppgifter. Se [Associera användare med ett hemteam](#associate-users-with-a-home-team) nedan.

## Associera användare med ett hemteam

Så här associerar du användare med ett hemteam:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka **[!UICONTROL Users]** väljer du sedan den eller de användare som du vill associera med ett hemteam.
1. Klicka på **[!UICONTROL More]** väljer du **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. I **[!UICONTROL Organization]** väljer du **[!UICONTROL Home Team]** fält. Börja skriva namnet på det team vars inställningar du vill associera med användarna. Klicka på teamets namn när du ser det i listan.

1. Klicka på **[!UICONTROL Save Changes]**.\
   De användare du har valt är nu associerade med ett hemteam.

   Alla gruppinställningar, inklusive statusvärdena som är kopplade till [!UICONTROL Done] knappen visas nu för dessa användare.

