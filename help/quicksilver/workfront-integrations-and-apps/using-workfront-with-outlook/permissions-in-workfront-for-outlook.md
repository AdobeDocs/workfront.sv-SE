---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Behörighetsnivåer för [!DNL Workfront] för Outlook
description: The [!DNL Workfront for Outlook] För tillägg krävs läs-/skrivbehörighet för postlådan. The [!DNL Workfront for Outlook] integreringen kräver behörigheter på högsta nivå eftersom den har funktioner för att hämta e-postbilagor från Outlook Exchange-servern och överföra dem till [!DNL Workfront], när användaren skickar en begäran från ett e-postmeddelande som innehåller bilagor.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Behörighetsnivåer för [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] kräver den högsta av de fyra behörighetsnivåerna som tillåts i [!DNL Outlook] tillägg.

Mer information om behörigheter i [!DNL Outlook] tillägg, se [Integritet, behörigheter och säkerhet för [!DNL Outlook] tillägg](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) i [!DNL Microsoft] dokumentation.

The [!DNL Workfront for Outlook] add-in kräver läs-/skrivåtkomst till postlådan (`ReadWriteMailbox`), som är det högsta behörighetsområdet.
The [!DNL Workfront for Outlook] integreringen kräver behörigheter på högsta nivå eftersom den har funktioner för att hämta e-postbilagor från [!DNL Outlook] växla server och överföra dem till [!DNL Workfront], när användaren skickar en begäran från ett e-postmeddelande som innehåller bilagor. För att denna funktionalitet ska fungera [!DNL Workfront for Outlook] använder funktionen `mailbox.getCallbackTokenAsync()` från [!DNL Office] Lägg till JavaScript API för att hämta token och använda det för att hämta e-postbilagor från Exchange-servern. Den enda behörigheten som tillåter att funktionen används är `ReadWriteMailbox`. Mer information finns i [Sekretess, behörigheter och säkerhet för Outlook-tillägg](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) i Microsoft-dokumentationen.

The [!DNL Workfront for Outlook] add-in kräver också `ReadWriteItem` behörighet (ingår i `ReadWriteMailbox`), som används för att läsa e-postbrödtexten och läsa/uppdatera e-postmetadata:

* Läs e-postbrödtext:

   [!DNL Workfront for Outlook] läser e-posttexten när en användare skickar begäran eller skickar e-postmeddelandet som en uppdatering till [!DNL Adobe Workfront] Objekt.
* Läs/uppdatera e-postmetadata:

   [!DNL Workfront for Outlook] uppdaterar e-posthuvuden när en användare skickar en begäran från ett e-postmeddelande. Detta görs för att lagra information om den inskickade [!DNL Adobe Workfront] så nästa gång användaren öppnar tillägget för samma e-post visas information om tidigare åtgärder med det e-postmeddelandet.

[!DNL Workfront for Outlook] får åtkomst till en användares postlåda endast när användaren utför en åtgärd i tillägget. Den har ingen bakgrundsfunktion. Workfront för Outlook har endast åtkomst till användarens postlåda i följande scenario:

* Användaren försöker skicka en begäran, skapa en uppgift eller skicka ett e-postmeddelande som en uppdatering från [!DNL Workfront for Outlook] (Öppna tillägget och välja en åtgärd)
   * [!DNL Workfront for Outlook] läser e-posttexten som ska fyllas i i formuläret inuti tillägget.
   * [!DNL Workfront for Outlook] läser e-postmetadata för att visa information om tillägget om de tidigare åtgärderna som utfördes i tillägget med samma e-postadress.
* När en användare skickar en begäran skapar en uppgift eller skickar ett e-postmeddelande som en uppdatering från [!DNL Workfront for Outlook] (klicka på [!UICONTROL submit] på tillägget):
   * [!DNL Workfront for Outlook] läser e-postmeddelandet för att skicka det till Workfront som en begärandebeskrivning eller kommentar.
   * [!DNL Workfront for Outlook] uppdaterar e-postmetadata för att lagra information om skickade begäranden eller uppdaterade objekt.
   * [!DNL Workfront for Outlook] hämtar e-postbilagor från Exchange-servern för att överföra dem till skickade begäranden, skapade uppgifter eller uppdaterade objekt.
