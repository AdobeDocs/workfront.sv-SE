---
product-area: workfront-integrations
keywords: google,doc,dokument,ark,bild
navigation-topic: workfront-for-g-suite
title: Sekretess och behörigheter i Workfront för Google Workspace
description: Sekretess och behörigheter i Workfront för Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Sekretess och behörigheter i Workfront för Google Workspace

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Under den här övergångsprocessen kommer följande Workfront för Google Workspace-funktioner inte att vara tillgängliga efter **28 februari 2026**:
>
>* Åtkomst till Google Workspace-funktioner inifrån Workfront
>
>* Visa och hantera Workfront-uppgifter från Gmail eller Google Calendar-webbplatspanelen
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Google Workspace.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration-modulerna för Google Workspace finns i [Gmail-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) och [Google Calendar-moduler](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Eftersom kundens integritet är viktig lagrar eller samlar Adobe Workfront inte in några identifierande kunddata som följer av auktorisering från tredje part av en plugin-app från Google. Workfront för Google Workspace-användning och överföring av information som tas emot från Google API:er till andra program följer [Google API Services-användardataprincipen](https://developers.google.com/terms/api-services-user-data-policy), inklusive kraven för begränsad användning.

Vi behöver följande behörigheter för att Workfront för Google Workspace ska ge maximalt värde:

* **Visa dina e-postmeddelanden när tillägget körs**: Med plugin-programmet Workfront för Google Workspace kan användare spara otaliga timmar av duplicerat arbete genom att konvertera e-postmeddelanden till nya uppgifter i Workfront och automatiskt fylla i uppgiftens rubrik och beskrivning med e-postmeddelandets ämne och innehåll. Med plugin-programmet kan du även skicka e-postmeddelanden till Workfront som nya kommentarer. Plugin-programmet måste visa dina e-postmeddelanden när tillägget körs för att leverera det här värdet.
* **Kör som Gmail-tillägg/icke-känslig**: Behörigheter krävs för att Workfront för Google Workspace-tillägget ska fungera i Gmail-miljön. Plugin-programmet kräver en Gmail-miljö för att fungera, så behörigheten `Run as a Gmail add-on / non-sensitive` krävs.
* **Visa metadata för e-postmeddelanden när tillägget körs**: För att förbättra arbetsflödena bekräftar plugin-programmet Workfront för Google Workspace om ett e-postmeddelande är ett Workfront-meddelande och identifierar typen av Workfront-meddelande (ny arbetsbegäran, godkännandebegäran, ny kommentar osv.). Plugin-programmet kräver behörigheten `View your email message metadata when the add-on is running` för att kunna leverera det här värdet.
* **Plugin-programmet måste köras som ett kalendertillägg eller som inte är känsligt**: Workfront för Google Workspace-pluginprogrammet ansluter till din kalender så att du kan visualisera hur aktiviteter påverkar scheman. Plugin-programmet behöver behörighet `Run as a Calendar add-on / non-sensitive` för att kunna göra detta.
* **Anslut till en extern tjänstbehörighet:** Plugin-programmet måste slutligen ansluta till Workfront API, som är ryggraden i plugin-värdet. Workfront API är en extern tjänst för Google, så plugin-programmet kräver `Connect to an external service permission` för att plugin-programmet ska fungera.

Mer information om Adobe Workfront deltagande i kundsekretess finns i [Workfront sekretesspolicy](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Mer information finns i [Användardataprincip för Google API Services](https://developers.google.com/terms/api-services-user-data-policy).
