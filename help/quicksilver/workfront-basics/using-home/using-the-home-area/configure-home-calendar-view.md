---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Konfigurera visningsinställningar för hemkalendern
description: Du kan konfigurera inställningarna för hemkalendern så att de integreras med en webbaserad version av Outlook och hjälpa dig att spåra arbetsbelastningen utifrån de tillgängliga arbetstiderna.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Konfigurera visningsinställningar för [!UICONTROL Home Calendar]

<!--Audited: 01/2024-->

Du kan konfigurera inställningarna för [!UICONTROL Home Calendar] så att du gör följande:

* Integrera med en webbaserad version av [!DNL Outlook] i molnbaserad [!DNL Office 365] eller [!DNL Outlook Live]. Du kan visa alla händelser från din Outlook-kalender och alla associerade kalendrar som du väljer i din [!UICONTROL Home Calendar] i Adobe Workfront.
* Hjälp dig att spåra din arbetsbelastning mot dina tillgängliga arbetstimmar i fältet [!UICONTROL Allocation].

Mer information om hemkalendern finns i [[!UICONTROL Home Calendar] vy](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

I den här artikeln beskrivs hur du konfigurerar inställningarna för hemkalendern och integrerar hemkalendern med den externa Outlook-kalendern.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>Aktuell: [!UICONTROL Work] eller högre</p> 
   eller
   <p>Nytt: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan eller licenstyp du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Om att integrera [!DNL Microsoft Outlook] kalendrar

Tänk på följande när du konfigurerar din hemkalender med din [!DNL Microsoft Outlook]-kalender:

* Du kan bara integrera en webbaserad version av [!DNL Outlook] i molnbaserade [!DNL Office 365] eller [!DNL Outlook Live].

  Lokal [!DNL Outlook] och [!DNL Outlook] på en molnbaserad Enterprise [!DNL Exchange]-server stöds inte.

  Om din organisation använder enkel inloggning behöver du [!DNL Microsoft 365 E3] eller [!DNL E5].

* Bifogade filer som är associerade med dina [!DNL Outlook]-händelser är inte bifogade till [!DNL Outlook]-händelserna i din hemkalender.
* Integrering med en [!DNL Outlook]-kalender måste slutföras för varje enskild användare.
* Händelser som visas i fältet [!UICONTROL Due] visas inte i din [!DNL Microsoft]-kalender om du inte har dragit dem från [!UICONTROL Work List] till din [!DNL Adobe Workfront]-kalender. Mer information finns i [[!UICONTROL Due] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) och [Arbetslista i [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) i [[!UICONTROL Home Calendar]-vyn ](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* När du aktiverar integreringen med [!DNL Outlook] synkroniseras endast arbetsobjekt som dras till [!UICONTROL Home Calendar] från den punkten framåt. Objekt som fanns på hemkalendern innan integreringen aktiverades visas inte, och du måste dra dem till hemkalendern igen om du vill att de ska visas i [!DNL Outlook].
* När du delar (eller tar bort delning) en [!DNL Outlook]-kalender med andra personer, eller när du ändrar behörighetsnivån för en kalender som du delar med andra, påverkar inte den här ändringen deras kalendrar i cirka 30 minuter. Mer information finns i dokumentationen för [!DNL Microsoft Outlook].\
   När du integrerar [!DNL Workfront]-kalendern med en [!DNL Outlook]-kalender som du delar med andra användare kommer de därför inte att se dina [!DNL Workfront]-kalenderobjekt på cirka 30 minuter.

>[!NOTE]
>
>Kalenderkonfigurationen [!DNL Outlook] är helt skild från tillägget [!DNL Outlook] ([!UICONTROL [!DNL Outlook] Integration] eller [!DNL Workfront Outlook]). Det krävs ingen installation för att konfigurera kalendern, men det krävs en installation för tillägget [!DNL Outlook]. Mer information om tillägget [!DNL Outlook] finns i [Konfigurera [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Konfigurera visningsinställningarna för [!UICONTROL Home Calendar] och integrera dem med Outlook-kalendrar

1. I vyn [!UICONTROL Home Calendar] klickar du på kugghjulsikonen **[!UICONTROL Settings]** ![Calendar_Settings_>_icon.png](assets/calendar-settings-gear-icon.png) i det övre högra hörnet för att öppna panelen **[!UICONTROL Calendar settings]** till höger.

   Om du behöver information om hur du kommer åt vyn [!UICONTROL Home Calendar] kan du läsa [Visa [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Valfritt) Om du vill integrera din [!DNL Microsoft Outlook]-kalender klickar du på **[!UICONTROL Add account]** i det övre högra hörnet på panelen **[!UICONTROL Calendar settings]**. Om du blir ombedd att göra det anger du dina inloggningsuppgifter för [!DNL Microsoft Outlook]. Du kan upprepa det här steget om du vill lägga till flera [!DNL Outlook]-konton.

   >[!NOTE]
   >
   >Du måste ge [!DNL Workfront] behörighet att komma åt din [!DNL Outlook]-kalender. Om du ger behörighet kan [!DNL Workfront] behålla åtkomst till kalenderdata, läsa din [!DNL outlook]-profil och läsa och uppdatera din [!DNL Microsoft]-kalender.

1. Uppdatera webbläsarfönstret om du vill visa information från ditt [!DNL Outlook]-konto i kalendern och på panelen [!UICONTROL Calendar settings].
1. Klicka på kugghjulsikonen **[!UICONTROL Settings]** igen i det övre högra hörnet för att öppna panelen **[!UICONTROL Calendar settings]**. ![Calendar_Settings_istället_icon.png](assets/calendar-settings-gear-icon.png)

1. (Valfritt) Välj **[!UICONTROL View]** eller **[!UICONTROL Sync]** under varje [!DNL Microsoft]-konto som du har lagt till i föregående steg:

   * **[!UICONTROL View]**: Det här är ett skrivskyddat alternativ som visar [!DNL Microsoft] kalenderhändelser på din [!UICONTROL Home Calendar].
   * **[!UICONTROL Sync]**: Det här alternativet tillåter en tvåvägssynkronisering mellan dina [!DNL Microsoft]- och [!UICONTROL Home]-kalendrar. [!DNL Workfront] [!UICONTROL Home Calendar] objekt exporteras med andra ord till din [!DNL Microsoft]-kalender och [!DNL Microsoft] kalenderobjekt importeras till din Workfront [!UICONTROL Home Calendar] i realtid.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Valfritt) Under ditt [!DNL Workfront]-konto eller ett integrerat konto väljer du de associerade kalendrar som du vill visa i din [!UICONTROL Home Calendar] (till exempel din PTO-kalender, födelsedagar eller helgkalender) och klickar sedan på webbläsarens [!UICONTROL Refresh]- eller [!UICONTROL Reload]-knapp för att se ändringarna.

1. (Valfritt) I avsnittet **[!UICONTROL General]** under **[!UICONTROL Start Week On]** väljer du den dag du vill visa som första dag i arbetsveckan i hemkalendern.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Konfigurera följande alternativ:

   * **[!UICONTROL My Work Days]:** Välj vilka dagar du arbetar.
   * **[!UICONTROL My Usual Start Time]:** Ange när du vill starta arbetsdagen.
   * **[!UICONTROL My Usual End Time]:** Välj den tid du vill avsluta din arbetsdag.

   [!DNL Workfront] använder dessa tre inställningar för att beräkna antalet timmar du arbetar under en vecka. Det här numret påverkar fältet [!UICONTROL Allocation], som hjälper dig att spåra din arbetsbelastning mot dina tillgängliga arbetstimmar. Mer information finns i [[!UICONTROL Allocation] bar ](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) i artikelvyn [[!UICONTROL Home Calendar] ](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Klicka utanför området **[!UICONTROL Calendar settings]** för att stänga det.

   [!DNL Workfront] sparar dina ändringar automatiskt.

Mer information om hur du använder vyn [!UICONTROL Calendar] för att hantera dina arbetstilldelningar och integrerade kalenderhändelser finns i [Använd vyn [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
