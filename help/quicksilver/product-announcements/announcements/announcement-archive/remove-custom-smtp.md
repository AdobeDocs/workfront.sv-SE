---
content-type: reference
navigation-topic: announcements
title: Ta bort anpassad SMTP som ett alternativ för utgående e-post
description: I version 20.3 (som ska lanseras i augusti 2020) går Adobe Workfront över till ett nytt e-postsystem som avsevärt förbättrar tillförlitligheten i e-postleveransen för Workfront-uppdateringar och -meddelanden. Detta innebär att kunderna inte längre kan använda sin egen SMTP-e-postserver för att skicka e-post från Workfront-plattformen till den avsedda mottagaren. Alla e-postmeddelanden skickas direkt från Workfront Mail Server.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Ta bort anpassad SMTP som ett alternativ för utgående e-post

>[!NOTE]
>
>De funktioner som beskrivs i den här artikeln är inte längre tillgängliga och artikeln kommer att tas bort inom en nära framtid.

I version 20.3 (som ska lanseras i augusti 2020) går Adobe Workfront över till ett nytt e-postsystem som avsevärt förbättrar tillförlitligheten i e-postleveransen för Workfront-uppdateringar och -meddelanden. Detta innebär att kunderna inte längre kan använda sin egen SMTP-e-postserver för att skicka e-post från Workfront-plattformen till den avsedda mottagaren. Alla e-postmeddelanden skickas direkt från Workfront Mail Server.

Du kommer åt den här funktionen genom att logga in som systemadministratör och gå till Konfigurera > E-post > Konfigurera. Här visas en skärmbild som visar funktionen:

![Inställningar för e-postserver](assets/email-server-settings-350x226.png)

Inställningen som är markerad på den här skärmbilden ändras automatiskt till att använda alternativet Workfront Mail Server i version 20.3.

Om du har konfigurerat en anpassad SMTP-e-postserver rekommenderar vi **att du kontaktar IT-teamet** för att säkerställa att e-post från notifications@my.workfront.com inte blockeras för inkommande e-post till systemet. Du kan även referera till Konfigurera brandväggen för att få information om vilka IP-adresser som vår trafik och e-post kommer från.

Kontakta [Workfront Support Team](https://experienceleague.adobe.com/sv?support-tab=home&lang=sv#support) om du har frågor eller funderingar.
