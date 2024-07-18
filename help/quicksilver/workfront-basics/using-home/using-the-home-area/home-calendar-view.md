---
content-type: overview
product-area: calendars
navigation-topic: use-the-home-area
title: Vyn Hemkalender
description: I vyn [!UICONTROL Home Calendar] i området [!UICONTROL Home] kan du visa och hantera arbetsveckan och arbetstilldelningar i en personlig arbetskalender som bara är synlig för dig. Du kan använda den för att schemalägga när du vill göra ditt arbete. Och du kan integrera det med externa kalendrar som en [!UICONTROL Microsoft Outlook]-kalender.
author: Nolan
feature: Get Started with Workfront
exl-id: 174bf68f-bbb7-4777-aeeb-53a0b3a8b1f7
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# [!UICONTROL Home Calendar]-vy

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated for QS except for section about expanding a work item in the list--this isn't working yet in QS.</p>
-->

I vyn [!UICONTROL Home Calendar] i området [!UICONTROL Home] kan du visa och hantera arbetsveckan och arbetstilldelningar i en personlig arbetskalender som bara är synlig för dig. Du kan använda den för att schemalägga när du vill göra ditt arbete. Och du kan integrera det med externa kalendrar som en [!UICONTROL Microsoft Outlook]-kalender.

>[!NOTE]
>
>Vyn [!UICONTROL Home Calendar] skiljer sig från [!UICONTROL Calendar]-rapporter. Mer information om [!UICONTROL Calendar] rapporter finns i [[!UICONTROL Calendar] rapportöversikt ](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Om du behöver instruktioner för hur du konfigurerar [!UICONTROL Home Calendar] kan du läsa [Konfigurera [!UICONTROL Home Calendar]-visningsinställningarna](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

Mer information om hur du kommer åt vyn [!UICONTROL Home Calendar] finns i [Visa [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

Mer information om hur du integrerar [!UICONTROL Home Calendar] med en extern kalender finns i [[!UICONTROL Configure your [!UICONTROL Home Calendar]] Vyinställningar ](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

De återstående avsnitten i den här artikeln förklarar avsnitt och funktioner i [!UICONTROL Home Calendar]-vyn mer ingående.

## Arbetslista på [!UICONTROL Home Calendar]

Arbetsobjekt (Uppgifter, Utgåvor, Förfrågningar och Godkännanden) som tilldelats dig, dina grupper, dina team och dina roller visas i [!UICONTROL work list] till vänster om kalendern i området [!UICONTROL Home].

![](assets/calview-qs-350x185.png)

Du kan dra dina arbetsobjekt från [!UICONTROL work list] till [!UICONTROL Home Calendar] för att schemalägga när du vill arbeta med dem. Mer information om hur du schemalägger ditt arbete finns i [Använd [!UICONTROL Home Calendar]-vyn](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

Du kan klicka på en arbetspost i listan för att visa och uppdatera förloppet.

![](assets/work-item-cl-350x126.png)

Beroende på vilket objekt du har kan följande information visas till vänster i kalendern för det objekt du väljer i arbetslistan:

* **[!UICONTROL Project name]**: Visas i det övre vänstra hörnet av arbetsobjektet. Detta är det projekt som artikeln är associerad med. I exemplet ovan är projekttiteln&quot;Fall in 2020 campaign&quot;.
* **[!UICONTROL Work item name]**: Visas under projektnamnet. I exemplet ovan är arbetsobjektets titel&quot;15 september&quot;.
* **[!UICONTROL Done]**: Klicka på den här knappen om du vill ändra status för din arbetstilldelning till [!UICONTROL Done]. Den här knappen visas bara när du har tilldelats uppgiften eller utgåvan.
* **[!UICONTROL Done with my part]**: Klicka på knappen [!UICONTROL Done with my part] om du vill ändra status för din arbetstilldelning till [!UICONTROL Done].
* **[!UICONTROL Planned]**: Visar de timmar en resurshanterare har allokerat för arbete som ska slutföras för objektet. Mer information om planerade timmar finns i [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* **[!UICONTROL Logged]**: Visar de timmar du har loggat in på arbetsobjektet i antingen en tidrapport eller på fliken [!UICONTROL Updates] för objektet. Mer information finns i [Logga in på ett arbetsobjekt i [!UICONTROL Home] området ](../../../workfront-basics/using-home/using-the-home-area/log-time-on-work-item-in-home.md)

* **[!UICONTROL Scheduled]**: Visar de timmar som du har schemalagt för arbetsobjektet i vyn [!UICONTROL Calendar]. Mer information om hur du flyttar arbetsobjekt till vyn [!UICONTROL Calendar] finns i [Schemalägg arbetsobjekt i [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md#scheduling-work-items-in-home-calendar) i [Använd vyn [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

* **[!UICONTROL Details]**: Klicka på den här knappen om du vill visa information om arbetsobjektet på den högra panelen i vyn [!UICONTROL Calendar].
* **[!UICONTROL Work On It]**: Klicka på den här knappen om du vill acceptera uppdraget att arbeta med objektet.

## Allokeringsfält

När du konfigurerar [!UICONTROL Home Calendar] anger du hur många timmar du normalt arbetar under en vecka (se [Konfigurera [!UICONTROL Home Calendar]-visningsinställningarna](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md)). [!DNL Adobe Workfront] använder det här talet för att fastställa din totala allokerbara arbetstid.

Fältet [!UICONTROL Allocation] är en visuell representation av antalet timmar i arbetsveckan och hur du använder dem.

![](assets/allocation-bar-qs-350x181.png)

Färgerna i fältet [!UICONTROL Allocation] anger följande information:

* **Grå**: Antal timmar som schemalagts för händelser från integrerade kalendrar. Mer information om hur du integrerar kalendrar finns i avsnittet [Konfigurera dina [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md#configuring-your-home-calendar-view) i [Konfigurera dina [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

* **Blå**: Antal timmar som du har schemalagt för [!DNL Workfront] arbetsobjekt som du har tilldelats. Du kan schemalägga arbete genom att dra objekt från [!UICONTROL Work List] och släppa dem i kalendern. Mer information om schemaläggning av arbete finns i avsnittet [Schemalägg arbetsobjekt i [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md#scheduling-work-items-in-home-calendar) i [Använd [!UICONTROL Home Calendar]-vyn](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

* **Ljusblå**: Antalet lediga timmar som är tillgängliga för allokering.
* **Röd** (visas inte ovan): Schemalagda händelser och arbetsobjekt som har överskridit det antal timmar som du har tillgängligt för veckan.

## [!UICONTROL Due] bar

Fältet [!UICONTROL Due] på [!UICONTROL Home Calendar] visar de objekt som förfaller för den vecka som visas enligt deras [!UICONTROL Planned Completion Date].

![](assets/duebar-qs-350x140.png)

>[!NOTE]
>
>Om du har integrerat din Microsoft-kalender med din [!DNL Workfront]-kalender visas inte objekt i [!UICONTROL Due] -fältet i din Microsoft-kalender om du inte har dragit dem från arbetslistan till din [!DNL Workfront]-kalender. Mer information finns i avsnittet [Arbetslista i [!UICONTROL Home Calendar]](#work-list-on-the-home-calendar) ovan och i artikeln [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).
