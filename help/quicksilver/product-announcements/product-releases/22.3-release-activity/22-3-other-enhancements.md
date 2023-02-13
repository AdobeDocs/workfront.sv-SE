---
title: andra uppdateringar under tidsramen för version 22.3
description: andra uppdateringar under tidsramen för version 22.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3 Andra förbättringar

Den här sidan beskriver alla andra förbättringar som gjorts i version 2.3 till förhandsvisningsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 11 juli 2022. En lista över alla ändringar som är tillgängliga i version 2.3 finns i [22.3 Versionsöversikt](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Uppdaterade tidrapporter

Vi fortsätter att förbättra och uppdatera din upplevelse när vi arbetar med tidrapporter. Nedan följer några av funktionerna som ingår i den här uppdateringen:

* Ett nytt utseende som matchar den nya Workfront-upplevelsen.

* Spara funktionalitet automatiskt för att automatiskt spara loggade timmar och timkommentarer så fort du lägger till dem.

* En mer intuitiv sidlayout som matchar andra objektsidor. Vi har t.ex. lagt till en vänsterpanel i tidrapporten. Tidrapportsuppdateringarna visas nu i uppdateringsavsnittet i den vänstra panelen. Du kan även ta bort en tidrapport från tidrapportsidan och lägga till tidrapporten i favoritlistan.

* En bättre upplevelse när du söker efter och lägger till projekt, uppgifter eller utgåvor i tidrapporten. Detta matchar upplevelsen i alla andra listor i Workfront.

* Panelen Sammanfattning är tillgänglig för uppgifter och utgåvor för att lägga till kommentarer eller uppdatera information direkt från tidrapporten.


I den aktuella uppdateringen har även följande funktioner tagits bort:

* Skapandet av en uppgift från en uppdatering har tagits bort. Den här funktionen har tagits bort sedan 2018.2-versionen från uppdateringsområdet för alla andra objekt, men den var fortfarande tillgänglig i tidrapportens uppdateringsström.

* &quot;Lägg till utgifter från en tidrapport. &quot;har tagits bort från Inställningar för tidrapport och timmar i Inställningar och du kan inte längre logga utgifter från tidrapporten. Du kan fortfarande logga utgifter från uppgifts- och projektsidorna.


Mer information finns i följande artiklar:

* [Förstå layouten för tidrapporten](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Konfigurera tidrapport och timinställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Förbättringar av den vänstra navigeringspanelen

Vi har gjort flera förbättringar av den vänstra navigeringspanelen i Adobe Workfront.

* Utseendet och känslan hos den vänstra navigeringspanelen uppdaterades till designstandarderna för Adobe, inklusive färger och teckensnitt.

* Länken&quot;Lägg till anpassat avsnitt&quot; längst ned på panelen har bytt namn till&quot;Lägg till kontrollpanel&quot; för att bättre förklara dess funktion.

## Aktivera automatisk uppdatering av tokenrotation i dina anpassade OAuth2-program

För att du ska få större kontroll över säkerheten i dina anpassade OAuth2-program har vi lagt till ett alternativ som aktiverar uppdatering av tokenrotation. När det här alternativet är aktiverat skapas och skickas en ny uppdateringstoken automatiskt varje gång en uppdateringstoken används, och den gamla inaktiveras.

Programmet måste lagra den nya uppdateringstoken efter varje uppdatering. Denna uppdateringstoken lagras inte i Workfront.

Tidigare har uppdateringstoken gått ut efter en inställd tidsmängd som konfigurerats i de anpassade OAuth2-programinställningarna.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Använd PKCE i dina anpassade OAuth2-integrationer för webbapplikationer med en sida

Nu kan du skapa enkelsidiga webbprogram i dina anpassade integreringar med PKCE. PKCE är ett säkert auktoriseringsflöde som fungerar bra med dynamiskt uppdaterade program som mobilappar, men som är värdefullt för alla OAuth2-klienter. I stället för en statisk klienthemlighet använder PKCE en dynamiskt genererad sträng, vilket eliminerar risken för en läckt klienthemlighet.

Tidigare använde de tillgängliga alternativen för anpassade OAuth2-program antingen en användares namn och lösenord eller en klienthemlighet.

Mer information finns i [Skapa OAuth2-program för Workfront-integreringar](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
