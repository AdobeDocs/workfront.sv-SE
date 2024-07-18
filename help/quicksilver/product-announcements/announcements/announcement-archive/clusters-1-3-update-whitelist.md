---
content-type: reference
navigation-topic: announcements
title: Kunder som använder kluster 1, 2 och 3 måste uppdatera alla IP-block i tillåtelselista för att förhindra blockering av Adobe Workfront tjänster
description: För att förbättra och förbättra vår kärninfrastruktur migrerar vi snart Adobe Workfront-kunder på Clusters 01, 02 och 03 till AWS publika moln.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Kunder som använder kluster 1, 2 och 3 måste uppdatera alla IP-block i tillåtelselista för att förhindra blockering av Adobe Workfront tjänster

För att förbättra och förbättra vår kärninfrastruktur migrerar vi snart Adobe Workfront-kunder på Clusters 01, 02 och 03 till AWS publika moln.

Som en del av den här ändringen måste du lägga till följande IP-adresser till dina IP-block i tillåtelselista för att förhindra blockering av Workfront tjänster:

För enkel inloggning och POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

För e-post:

* 54.240.60.174
* 54.240.60.175

Se till att IP-blocken för ditt tillåtelselista uppdateras senast 13 maj 2019. Mer information finns i [Konfigurera brandväggens tillåtelselista](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Tack för ditt fortsatta stöd för Workfront när vi skapar en mer tillförlitlig och robust upplevelse för våra kunder.

Om du har ytterligare frågor kan du kontakta vårt supportteam på experience.workfront.com eller genom att ringa 844.306.4357 (USA) eller +44.1256.274200 (EMEA).

## Vanliga frågor

### Varför gör Workfront den här ändringen?

Workfront undersöker ständigt olika sätt att förbättra användarupplevelsen, så att våra kunder alltid får bästa möjliga service. Den här förändringen utnyttjar nya tekniker som gör att vi kan ge bästa möjliga upplevelse och förbättra vår redan robusta säkerhetsmodell.

### Vilka åtgärder krävs av mig som Workfront-administratör?

Kontakta din interna IT- eller säkerhetsavdelning om du behöver hjälp med att granska IP-blocken för tillåtelselista och lägga till IP-blocken som listas ovan.

### Vad kan min organisation förvänta sig om vi inte gör den här ändringen?

Du kan inte komma åt Workfront tjänster när vi migrerar tjänster till de nya IP-adresserna.
