---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta Final Release Activity
description: Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i Beta Final-utgåvan 2018.2. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 20 juni 2018. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 2018.2 Beta Final Release Activity

Den här sidan beskriver alla ändringar som senast fanns i förhandsvisningsmiljön i Beta Final-utgåvan 2018.2. Funktionerna gjordes tillgängliga i förhandsvisningsmiljön den 20 juni 2018. Den kommer att göras tillgänglig i produktionsmiljön i juli 2018.

>[!IMPORTANT]
>
> Funktionerna som beskrivs på den här sidan kan ändras innan de är tillgängliga i produktionsmiljön.

En lista över alla ändringar som gjorts under 2018.2 finns på  [Aktivitetsöversikt för version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Följande nya funktioner lanseras i samband med 18.2-utgåvan:

* [Ange e-postleveranstjänster för svar på Workfront e-postmeddelanden](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [Ta emot e-postmeddelanden för kommentarer om dokument](#receive-email-notifications-for-comments-on-documents)
* [Systemspårade uppdateringar innehåller inte längre en ikon](#system-tracked-updates-no-longer-contain-an-icon)
* [Alternativet att konvertera en kommentar till en aktivitet har tagits bort](#option-to-convert-a-comment-to-a-task-was-removed)
* [Workfront för Salesforce](#workfront-for-salesforce)
* [Förbättringar för Workfront för Slack](#workfront-for-slack-improvements)
* [Mobilförbättringar](#mobile-improvements)

## Ange e-postleveranstjänster för svar på Workfront e-postmeddelanden {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

Workfront-administratörer kan nu välja mellan olika e-postleveranstjänster när de konfigurerar Workfront så att användare kan kommentera objekt via e-postsvar. Workfront kan konfigureras att använda antingen standardtjänsten för e-post eller ett POP-e-postkonto.

Före den här uppdateringen måste Workfront-administratörer skapa ett POP-konto för varje användare. 

Mer information om hur du konfigurerar ett POP-e-postkonto finns i .

Mer information om standardtjänsten för e-post finns i .

## Ta emot e-postmeddelanden för kommentarer om dokument {#receive-email-notifications-for-comments-on-documents}

Du får nu ett e-postmeddelande när någon kommenterar ett dokument som du äger. Det här alternativet är aktiverat som standard. Du kan använda inställningen&quot;En kommentar läggs till i mitt dokument&quot; för att inaktivera alternativet för e-postmeddelanden.

Före den här ändringen fick du inga meddelanden när någon kommenterade ett dokument som du äger. 

Mer information finns i [Ändra dina egna e-postmeddelanden](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>När den här funktionen ursprungligen släpptes får användarna ett meddelande i appen utöver ett e-postmeddelande. Du får inte längre något meddelande i appen när någon kommenterar ett dokument som du äger. 

## Systemspårade uppdateringar innehåller inte längre en ikon {#system-tracked-updates-no-longer-contain-an-icon}

Varje gång en uppdatering skapas i uppdateringsområdet för ett objekt (t.ex. i ett projekt) innehåller uppdateringen inte längre någon motsvarande ikon.

Före den här ändringen innehöll alla systemuppdateringar också en ikon som representerade den uppdatering som gjordes.

Mer information om systemuppdateringar finns i [Systemspårade uppdateringar](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Alternativ för att konvertera en kommentar till en uppgift har tagits bort {#option-to-convert-a-comment-to-a-task-was-removed}

Alternativet att konvertera en kommentar till en uppgift har tagits bort.

Tidigare kunde du konvertera en kommentar till en uppgift medan du var i uppdateringsområdet för ett objekt.

## Workfront för Salesforce {#workfront-for-salesforce}

Vi lanserar en ny körklar integrering mellan Salesforce och Workfront. Du kan göra följande:

* Skapa automatiskt nya Workfront-projekt när en Salesforce-möjlighet når en viss fas, när en ny produkt läggs till i en säljprojekt eller när typen av konto uppdateras.
* Skapa Workfront-förfrågningar från en Salesforce-möjlighet eller ett konto.

Den här integreringen är tillgänglig för alla kunder som har en Workfront Pro-utgåva eller en senare, och den blir kostnadsfri.

Mer information om Workfront för Salesforce finns i  [Adobe Workfront för Salesforce](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md).

## Förbättringar av Workfront för Slack {#workfront-for-slack-improvements}

Du kan konfigurera så att du får Workfront-meddelanden i din Slack Workfront-kanal.

Följande Workfront-meddelanden kan även konfigureras för att levereras i Slack:

* När någon taggar dig i en kommentar eller uppdatering.
* När du tilldelas en ny uppgift eller ett nytt ärende.
* När du ombeds godkänna ett objekt.

Innan den här förbättringen kunde du inte få Workfront-meddelanden i Slack.

Mer information om Workfront-meddelanden i Slack finns i [Ta emot Adobe Workfront-meddelanden i Slack](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Mobilförbättringar {#mobile-improvements}

Följande nya funktioner kommer att lanseras i mobilbutikerna i samband med produktionsutgåvan 18.2:

* Inline-redigering för objektnamn 

  Nu kan du infoga redigeringsfält som namnet på ett projekt, en uppgift eller ett problem i mobilappen.

* Överför dokument 

  Nu kan du överföra dokument till objekt i Workfront mobilapp.

* Överföra en profilbild 

  Nu kan du överföra ett profilfoto till din iOS-mobilapp.

  Den här funktionen är bara tillgänglig för iOS mobilapp.

Följande funktioner har redan släppts till Android Beta-versionen av Workfront-mobilappen och de släpps också till Android och iOS mobilappar. Upplevelsen för iOS-plattformen innehåller följande skillnader jämfört med den Android-upplevelse som redan släppts:

* Nytt navigeringsfält längst ned för iOS 

* Ny självstudiekurs för iOS 

Mer information om de här funktionerna och om du vill se videoklipp som visar dem finns i [2018.2 släppningsaktivitet för Beta 4](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md) och [2018.2 släppningsaktivitet för Beta 5](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md).
