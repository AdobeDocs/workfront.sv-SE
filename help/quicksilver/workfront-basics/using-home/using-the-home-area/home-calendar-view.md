---
content-type: overview
product-area: calendars
navigation-topic: use-the-home-area
title: Vyn Hemkalender
description: Uppdaterat för QS förutom avsnittet om att expandera en arbetsuppgift i listan - detta fungerar ännu inte i QS.
author: Lisa
feature: Get Started with Workfront
exl-id: 174bf68f-bbb7-4777-aeeb-53a0b3a8b1f7
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# [!UICONTROL Home Calendar] visa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated for QS except for section about expanding a work item in the list--this isn't working yet in QS.</p>
-->

The [!UICONTROL Home Calendar] visa i [!UICONTROL Home] kan du visa och hantera arbetsveckan och arbetsuppgifterna i en personlig arbetskalender som bara är synlig för dig. Du kan använda den för att schemalägga när du vill göra ditt arbete. Och du kan integrera det med externa kalendrar som [!UICONTROL Microsoft Outlook] kalender.

>[!NOTE]
>
>The [!UICONTROL Home Calendar] vyn skiljer sig från [!UICONTROL Calendar] rapporter. Mer information om [!UICONTROL Calendar] rapporter, se [[!UICONTROL Calendar] rapportöversikt](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Om du behöver anvisningar om hur du konfigurerar [!UICONTROL Home Calendar], se [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

Mer information om åtkomst till [!UICONTROL Home Calendar] visa, se [Visa [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

För information som integrerar [!UICONTROL Home Calendar] med en extern kalender, se [[!UICONTROL Configure your [!UICONTROL Home Calendar]] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

De återstående avsnitten i den här artikeln förklarar avsnitt och funktioner i [!UICONTROL Home Calendar] Se mer ingående.

## Arbetslista på [!UICONTROL Home Calendar]

Arbetsobjekt (uppgifter, ärenden, förfrågningar och godkännanden) som tilldelats dig, dina grupper, dina team och dina roller visas i [!UICONTROL work list] till vänster om kalendern i [!UICONTROL Home] område.

![](assets/calview-qs-350x185.png)

Du kan dra dina arbetsobjekt från [!UICONTROL work list] till [!UICONTROL Home Calendar] för att schemalägga när du vill arbeta med dem. Mer information om schemaläggning av arbetet finns i [Använd [!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

Du kan klicka på en arbetspost i listan för att visa och uppdatera förloppet.

![](assets/work-item-cl-350x126.png)

Beroende på vilket objekt du har kan följande information visas till vänster i kalendern för det objekt du väljer i arbetslistan:

* **[!UICONTROL Project name]**: Visas längst upp till vänster på arbetsposten. Detta är det projekt som artikeln är associerad med. I exemplet ovan är projekttiteln&quot;Fall in 2020 campaign&quot;.
* **[!UICONTROL Work item name]**: Visar under projektnamnet. I exemplet ovan är arbetsobjektets titel&quot;15 september&quot;.
* **[!UICONTROL Done]**: Klicka på den här knappen om du vill ändra status för arbetstilldelningen till [!UICONTROL Done]. Den här knappen visas bara när du har tilldelats uppgiften eller utgåvan.
* **[!UICONTROL Done with my part]**: Klicka på [!UICONTROL Done with my part] om du vill ändra status för arbetsuppdraget till [!UICONTROL Done].
* **[!UICONTROL Planned]**: Visar de timmar en resurshanterare har allokerat för arbete som ska slutföras för artikeln. Mer information om planerade timmar finns i [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* **[!UICONTROL Logged]**: Visar de timmar som du har loggat in på arbetsuppgiften antingen i en tidrapport eller på [!UICONTROL Updates] -fliken för objektet. Mer information finns på [Logga tid för ett arbetsobjekt från [!UICONTROL Home] area](../../../workfront-basics/using-home/using-the-home-area/log-time-on-work-item-in-home.md)

* **[!UICONTROL Scheduled]**: Visar de timmar som du har schemalagt för arbetsuppgiften i [!UICONTROL Calendar] vy. Mer information om hur du flyttar arbetsobjekt till [!UICONTROL Calendar] visa, se [Schemalägg arbetsobjekt i [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md#scheduling-work-items-in-home-calendar) in [Använd [!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

* **[!UICONTROL Details]**: Klicka på den här knappen om du vill visa information om arbetsobjektet på den högra panelen i [!UICONTROL Calendar] vy.
* **[!UICONTROL Work On It]**: Klicka på den här knappen om du vill acceptera uppdraget att arbeta med objektet.

## Allokeringsfält

När du konfigurerar [!UICONTROL Home Calendar]anger du hur många timmar du vanligtvis arbetar under en vecka (se [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md)). [!DNL Adobe Workfront] använder det här talet för att fastställa din totala allokerbara arbetstid.

The [!UICONTROL Allocation] bar är en visuell representation av antalet timmar i arbetsveckan och hur du använder dem.

![](assets/allocation-bar-qs-350x181.png)

Färgerna i [!UICONTROL Allocation] fält:

* **Grå**: Antal schemalagda timmar för händelser från integrerade kalendrar. Mer information om hur du integrerar kalendrar finns i avsnittet [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md#configuring-your-home-calendar-view) in [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).

* **Blå**: Antal timmar som du har schemalagt för [!DNL Workfront] arbetsobjekt som du har tilldelats. Du kan schemalägga arbete genom att dra objekt från [!UICONTROL Work List] och släpper dem i din kalender. Mer information om schemaläggning av arbete finns i [Schemalägg arbetsobjekt i [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md#scheduling-work-items-in-home-calendar) avsnitt i [Använd [!UICONTROL Home Calendar] visa](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

* **Ljusblå**: Antalet lediga timmar som är tillgängliga för allokering.
* **Röd**(visas inte ovan): Schemalagda händelser och arbetsuppgifter som har överskridit det antal timmar som du har tillgängligt för veckan.

## [!UICONTROL Due] bar

The [!UICONTROL Due] på din [!UICONTROL Home Calendar] visar de objekt som förfaller för den aktuella veckan, enligt deras [!UICONTROL Planned Completion Date].

![](assets/duebar-qs-350x140.png)

>[!NOTE]
>
>Om du har integrerat din Microsoft-kalender med [!DNL Workfront] kalender, objekt i [!UICONTROL Due] fält visas inte i din Microsoft-kalender om du inte har dragit dem från arbetslistan till [!DNL Workfront] Kalender. Mer information finns i avsnittet  [Arbetslista på [!UICONTROL Home Calendar]](#work-list-on-the-home-calendar) ovan och artikeln  [Konfigurera [!UICONTROL Home Calendar] visningsinställningar](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md).
