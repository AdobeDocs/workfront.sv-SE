---
content-type: reference
navigation-topic: announcements
title: Sofing av e-post och borttagning av POP-svar
description: Vi gör två ändringar av det sätt på vilket Adobe Workfront skickar och tar emot e-post med version 20.3 (riktad mot augusti 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Spoofing &amp; POP Reply

Vi gör två ändringar av det sätt på vilket Adobe Workfront skickar och tar emot e-post med version 20.3 (riktad mot augusti 2020).

## Utgående e-post från Workfront

I ett försök att öka den framgångsrika leveransen av e-postmeddelanden kommer vi att eliminera förfalskning av e-postmeddelanden, som ofta taggas som skräppost (se Spefofing av e-post). Alla e-postmeddelanden från Workfront skickas från `notifications@my.workfront.com`, både automatiska varningar och kommunikation mellan användare. Ett exempelmejl från Joan Harris kommer att se ut så här i ditt mejlområde:

![Exempel på e-post](assets/noreply.png)

*Vi rekommenderar att du kontaktar IT-teamet* för att se till att e-post från `notifications@my.workfront.com` inte blockeras för inkommande e-post till ditt system. Du kan också referera till [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) för information om vilka IP-adresser som vår trafik och e-post kommer från.

## Inkommande e-postsvar till meddelanden (POP-svar)

I vissa e-postmeddelanden kan användare svara via e-post och få svaret kopierat till Workfront som ett kommentarsvar i Workfront-systemet. Systemadministratörer i Workfront har traditionellt kunnat välja mellan att tillhandahålla en egen POP-e-postserver för att ta emot svaren eller att använda det inbyggda svarssystemet i Workfront. Det anpassade alternativet för POP-e-postserver tas bort i version 20.3. Alla konton som har konfigurerats för att använda en anpassad server kommer automatiskt att överflyttas för att använda Workfront inbyggda e-postsvarssystem. Ingen åtgärd krävs för systemadministratörer eller andra Workfront-användare.

E-post som kommer direkt från Workfront Proof ändras inte. Du kommer att fortsätta få dessa e-postmeddelanden som du har gjort tidigare.

Om du har frågor eller funderingar kan du kontakta [Workfront Support Team](https://experienceleague.adobe.com/?support-tab=home#support).
