---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Konfigurera visningsinställningar för hemkalendern
description: Du kan konfigurera inställningarna för hemkalendern så att de integreras med en webbaserad version av Outlook och hjälpa dig att spåra arbetsbelastningen utifrån de tillgängliga arbetstiderna.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Konfigurera [!UICONTROL Home Calendar] visningsinställningar

<!--Audited: 01/2024-->

Du kan konfigurera [!UICONTROL Home Calendar] inställningar för att göra följande:

* Integrera med en webbaserad version av [!DNL Outlook] i molnet [!DNL Office 365] eller [!DNL Outlook Live]. Du kan visa alla händelser i Outlook-kalendern och alla associerade kalendrar som du väljer i [!UICONTROL Home Calendar] i Adobe Workfront.
* Hjälper dig att spåra din arbetsbelastning mot dina tillgängliga arbetstider på [!UICONTROL Allocation] bar.

Mer information om hemkalendern finns i [[!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

I den här artikeln beskrivs hur du konfigurerar inställningarna för hemkalendern och integrerar hemkalendern med den externa Outlook-kalendern.

## Åtkomstkrav

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

*Om du vill veta vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Om integrering [!DNL Microsoft Outlook] kalendrar

Tänk på följande när du konfigurerar din hemkalender med [!DNL Microsoft Outlook] kalender:

* Du kan bara integrera en webbaserad version av [!DNL Outlook] i molnet [!DNL Office 365] eller [!DNL Outlook Live].

  Lokalt [!DNL Outlook] och [!DNL Outlook] på ett molnbaserat företag [!DNL Exchange] servern stöds inte.

  Om din organisation använder enkel inloggning behöver du [!DNL Microsoft 365 E3] eller [!DNL E5].

* Bifogade filer som är kopplade till din [!DNL Outlook] händelser är inte kopplade till [!DNL Outlook] händelser i din hemkalender.
* Integration med en [!DNL Outlook] kalendern måste fyllas i för varje enskild användare.
* Händelser som visas i [!UICONTROL Due] -fältet visas inte på [!DNL Microsoft] om du inte har dragit dem från [!UICONTROL Work List] till [!DNL Adobe Workfront] Kalender. Mer information finns i [[!UICONTROL Due] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) och [Arbetslista på [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* När du aktiverar integreringen med [!DNL Outlook], arbetar bara objekt som dras till [!UICONTROL Home Calendar] från och med den tidpunkten synkroniseras. Objekt som fanns på hemkalendern innan integreringen aktiverades visas inte, och du måste dra dem till hemkalendern igen om du vill att de ska visas i [!DNL Outlook].
* När du delar (eller tar bort delning) ett [!DNL Outlook] kalendern med andra personer, eller när du ändrar behörighetsnivån för en kalender som du delar med andra, påverkar den här ändringen inte deras kalendrar i cirka 30 minuter. Mer information finns i [!DNL Microsoft Outlook] dokumentation.\
   När du integrerar [!DNL Workfront] Kalender med en [!DNL Outlook] som du delar med andra användare, kommer de inte att se din [!DNL Workfront] Kalenderobjekt i cirka 30 minuter.

>[!NOTE]
>
>The [!DNL Outlook] kalenderkonfigurationen är helt separat från [!DNL Outlook] Tillägg ([!UICONTROL [!DNL Outlook] Integration] eller [!DNL Workfront Outlook]). Det krävs ingen installation för att konfigurera kalendern, men det krävs en installation för [!DNL Outlook] Tillägg. Mer information om [!DNL Outlook] Se tillägg [Konfigurera [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Konfigurera [!UICONTROL Home Calendar] visa inställningar och integrera dem med Outlook-kalendrar

1. I [!UICONTROL Home Calendar] visa klickar du på **[!UICONTROL Settings]** kugghjulsikon ![Calendar_Settings_istället_icon.png](assets/calendar-settings-gear-icon.png) i det övre högra hörnet för att öppna **[!UICONTROL Calendar settings]** till höger.

   Om du behöver information om hur du använder [!UICONTROL Home Calendar] se [Visa [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Valfritt) För att integrera [!DNL Microsoft Outlook] kalender, klicka på **[!UICONTROL Add account]** i det övre högra hörnet av **[!UICONTROL Calendar settings]** -panelen. Om du blir ombedd att göra det anger du [!DNL Microsoft Outlook] inloggningsinformation. Du kan upprepa det här steget om du vill lägga till flera [!DNL Outlook] konton.

   >[!NOTE]
   >
   >Du måste ge [!DNL Workfront] behörighet att komma åt [!DNL Outlook] kalender. Beviljande av tillstånd tillåter [!DNL Workfront] om du vill ha tillgång till kalenderdata, läs [!DNL outlook] och läsa och uppdatera [!DNL Microsoft] kalender.

1. Uppdatera webbläsarfönstret för att se information från din [!DNL Outlook] kontot i kalendern och i [!UICONTROL Calendar settings] -panelen.
1. Klicka på **[!UICONTROL Settings]** kugghjulsikonen igen i det övre högra hörnet för att öppna **[!UICONTROL Calendar settings]** -panelen. ![Calendar_Settings_istället_icon.png](assets/calendar-settings-gear-icon.png)

1. (Valfritt) Under varje [!DNL Microsoft] konto som du har lagt till i föregående steg, välj **[!UICONTROL View]** eller **[!UICONTROL Sync]**:

   * **[!UICONTROL View]**: Det här är ett skrivskyddat alternativ som visas [!DNL Microsoft] kalenderhändelser på [!UICONTROL Home Calendar].
   * **[!UICONTROL Sync]**: Det här alternativet tillåter en tvåvägssynkronisering mellan [!DNL Microsoft] och [!UICONTROL Home] kalendrar. Med andra ord: [!DNL Workfront] [!UICONTROL Home Calendar] objekt exporteras till [!DNL Microsoft] kalender och [!DNL Microsoft] kalenderobjekt som importeras till din Workfront [!UICONTROL Home Calendar] i realtid.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Valfritt) Under [!DNL Workfront] eller ett integrerat konto väljer du de associerade kalendrar som du vill visa på din [!UICONTROL Home Calendar] (till exempel din PTO-, Birthdays- eller Holidays-kalender) och klicka sedan på webbläsarens [!UICONTROL Refresh] eller [!UICONTROL Reload] för att se ändringarna.

1. (Valfritt) I dialogrutan **[!UICONTROL General]** avsnitt under **[!UICONTROL Start Week On]** väljer du den dag du vill visa som första dag i arbetsveckan i hemkalendern.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Konfigurera följande alternativ:

   * **[!UICONTROL My Work Days]:** Välj vilka dagar du ska arbeta.
   * **[!UICONTROL My Usual Start Time]:** Välj den tidpunkt då du börjar din arbetsdag.
   * **[!UICONTROL My Usual End Time]:** Välj den tid du vill avsluta din arbetsdag.

   [!DNL Workfront] använder de här tre inställningarna för att beräkna hur många timmar du arbetar under en vecka. Det här numret påverkar [!UICONTROL Allocation] bar, som hjälper dig att spåra arbetsbelastningen mot dina tillgängliga arbetstimmar. Mer information finns i [[!UICONTROL Allocation] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) i artikeln [[!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Klicka utanför **[!UICONTROL Calendar settings]** för att stänga den.

   [!DNL Workfront] sparar ändringarna automatiskt.

Mer information om hur du använder [!UICONTROL Calendar] för att hantera dina arbetsuppgifter och inbyggda kalenderhändelser, se [Använd [!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
