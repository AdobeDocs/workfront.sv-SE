---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Korrigera startdagen i arbetsveckan för tidrapporter
description: Veckodagens startdag på min tidrapport matchar inte min förväntade veckostartdag.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Korrigera arbetsveckans startdag för tidrapporter

<!--Audited: 5/2025-->

## Problem

Veckodagens startdag på min tidrapport matchar inte min förväntade veckostartdag.

Detta inträffar vanligtvis när du inte har tilldelats någon tidrapportprofil och tidrapporten har skapats manuellt.


## Lösning

Din Workfront-administratör bör skapa tidrapportprofiler och tilldela alla till en profil, enligt beskrivningen i [Skapa, redigera och tilldela tidrapportprofiler](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Din Workfront-administratör kan definiera startdatumet för en tidrapport på en annan dag än det förväntade veckostartdatumet. Kontakta dem för att ta reda på vilket startdatum en tidrapportprofil är för din tidrapport.

Om din tidrapport skapades manuellt använder startdagen i veckan i tidrapporten inställningarna för Språk för e-post i användarens profil, enligt beskrivningen i artikeln [Konfigurera mina inställningar](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Om Språket för e-post till exempel är engelska (USA), startar veckan i tidrapporten på söndag. Alternativt, med inställningen Engelska (Storbritannien) som e-postspråk, startar veckan i tidrapporten på en måndag.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


