---
content-type: api
navigation-topic: api-navigation-topic
title: Stöd för JSONP upphör
description: Stöd för JSONP upphör
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Stöd för JSONP upphör

Eftersom JSONP (Javascript with Padding) är en gammal standard med kända säkerhetsbrister kommer Adobe Workfront inte längre att stödja JSONP från och med november 2018. Detta beslut stöder vårt större initiativ att modernisera Workfront.

JSONP är en standard som gör det möjligt att utföra förfrågningar mellan olika ursprung eller webbplatser. Många av Workfront kunder och partners använder JSONP för att få tillgång till Workfront från ett system på sin egen domän som en del av integreringen. JSONP tillåter att begäranden från andra domäner än Workfront behandlas av Workfront-programmet.

Om du använder JSONP som en del av någon av dina Workfront-integreringar måste du uppdatera integreringen så att den använder CORS-standarden (Cross-Origin Resource Sharing). Uppdateringen kräver att du gör följande:

1. Skicka en begäran till Workfront supportteam om att få domäner som används för att göra korsdomänsförfrågningar till vår tillåtelselista.

   Om du vill lägga till dina domäner i tillåtelselista för CORS kontaktar du Workfront kundsupport på 844-306-HELP(4357) eller genom att skicka ett supportärende online.

   >[!NOTE]
   >
   >Det går bara att lägga till domäner i tillåtelselista för CORS för kunder som använde JSONP före den 1 augusti 2018.


1. Gör ändringar i integreringskoden för att använda CORS.
