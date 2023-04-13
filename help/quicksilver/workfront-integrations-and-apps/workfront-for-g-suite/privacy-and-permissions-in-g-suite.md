---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Sekretess och behörigheter i Workfront för G Suite
description: Sekretess och behörigheter i Workfront för G Suite
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 0862af846ca77c33132ec631cf1e3eae253d3cd8
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Sekretess och behörigheter i Workfront för G Suite

Eftersom kundens integritet är viktig lagrar eller samlar Adobe Workfront inte in några identifierande kunddata som följer av auktorisering från tredje part av en plugin-app från Google.

Vi behöver följande behörigheter för att plugin-programmet för Workfront for G Suite ska kunna leverera maximalt värde:

* **Visa e-postmeddelanden när tillägget körs**: Workfront for G Suite kan spara massor av timmar genom att konvertera e-post till nya uppgifter i Workfront och automatiskt fylla i uppgiftens titel och beskrivning med e-postens ämne och brödtext. Med plugin-programmet kan du även skicka e-postmeddelanden till Workfront som nya kommentarer. Plugin-programmet måste visa dina e-postmeddelanden när tillägget körs för att leverera det här värdet.
* **Kör som Gmail-tillägg/icke-känslig**: Behörigheter krävs för att Workfront for G Suite-tillägget ska fungera i Gmail-miljön. Plugin-programmet kräver en Gmail-miljö för att fungera, så det kräver `Run as a Gmail add-on / non-sensitive` behörighet.
* **Visa metadata för e-postmeddelanden när tillägget körs**: För att förbättra arbetsflödena bekräftar Workfront for G Suite-pluginen om ett e-postmeddelande är ett Workfront-meddelande och identifierar typen av Workfront-meddelanden (ny arbetsbegäran, godkännandebegäran, ny kommentar osv.). Plugin-programmet kräver `View your email message metadata when the add-on is running` behörighet att leverera det här värdet.
* **Plugin-programmet måste köras som ett kalendertillägg eller som inte är känsligt**: Workfront for G Suite-pluginen kan anslutas till din kalender så att du kan visualisera hur uppgifter påverkar tidsplaner. Plugin-programmet behöver `Run as a Calendar add-on / non-sensitive` behörighet att göra detta.
* **Anslut till en extern tjänstbehörighet:** I slutändan måste plugin-programmet ansluta till Workfront API, som är ryggraden i plugin-värdet. Workfront API är en extern tjänst för Google, så plugin-programmet kräver `Connect to an external service permission` för att få plugin-programmet att fungera.

Mer information om Adobe Workfront engagemang för kundintegritet finns i [Workfront sekretesspolicy](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

