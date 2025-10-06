---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Behörighetsnivåer för  [!DNL Workfront] Outlook
description: Tillägget  [!DNL Workfront for Outlook] kräver åtkomst till läs-/skrivpostlådan. Integreringen av  [!DNL Workfront for Outlook] kräver behörigheter på högsta nivå eftersom den har funktioner för att hämta e-postbilagor från Outlook Exchange-servern och överföra dem till  [!DNL Workfront] när användaren skickar en begäran från ett e-postmeddelande som innehåller bilagor.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Behörighetsnivåer för [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft har inaktiverat stöd för äldre Exchange-onlinetoken](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) som användes av Workfront Outlook-tillägget för autentisering. Denna ändring av Microsoft har stegvis genomförts och är klar den 1 oktober 2025.
>
>**Eftersom Microsoft har inaktiverat dessa token fungerar inte längre integreringen i Workfront för Microsoft Outlook.**

[!DNL Workfront for Outlook] kräver den högsta av de fyra behörighetsnivåerna som tillåts i [!DNL Outlook] tillägg.

Mer information om behörigheter i [!DNL Outlook]-tillägg finns i [Sekretess, behörigheter och säkerhet för [!DNL Outlook] tillägg](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) i [!DNL Microsoft]-dokumentationen.

Tillägget [!DNL Workfront for Outlook] kräver läs-/skrivpostlådeåtkomst (`ReadWriteMailbox`), som är det högsta behörighetsområdet.
Integreringen av [!DNL Workfront for Outlook] kräver behörigheter på högsta nivå eftersom den har funktioner för att hämta e-postbilagor från Exchange-servern [!DNL Outlook] och överföra dem till [!DNL Workfront] när användaren skickar en begäran från ett e-postmeddelande som innehåller bilagor. För att den här funktionen ska fungera använder [!DNL Workfront for Outlook] funktionen `mailbox.getCallbackTokenAsync()` från JavaScript-API:t för tillägget [!DNL Office] för att hämta token och använda den för att hämta e-postbilagor från Exchange-servern. Den enda behörighet som tillåter användning av den funktionen är `ReadWriteMailbox`. Mer information finns i [Sekretess, behörigheter och säkerhet för Outlook-tillägg](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) i Microsoft-dokumentationen.

Tillägget [!DNL Workfront for Outlook] kräver även behörighet `ReadWriteItem` (ingår i `ReadWriteMailbox`), som används för att läsa e-postbrödtexten och läsa/uppdatera e-postmetadata:

* Läs e-postbrödtext:

  [!DNL Workfront for Outlook] läser e-posttexten när en användare skickar begäran eller skickar e-postbrödtexten som en uppdatering till [!DNL Adobe Workfront] Object.
* Läs/uppdatera e-postmetadata:

  [!DNL Workfront for Outlook] uppdaterar e-posthuvuden när en användare skickar en begäran från ett e-postmeddelande. Detta görs för att lagra information om det skickade [!DNL Adobe Workfront]-objektet, så nästa gång användaren öppnar tillägget för samma e-postmeddelande visas information om tidigare åtgärder med det e-postmeddelandet.

[!DNL Workfront for Outlook] har bara åtkomst till en användares postlåda när användaren utför en åtgärd i tillägget. Den har ingen bakgrundsfunktion. Workfront för Outlook har endast åtkomst till användarens postlåda i följande scenario:

* Användaren försöker skicka en begäran, skapa en uppgift eller skicka ett e-postmeddelande som en uppdatering från [!DNL Workfront for Outlook] (Öppnar tillägget och väljer en åtgärd)
   * [!DNL Workfront for Outlook] läser e-posttexten som ska fyllas i i formuläret inuti tillägget.
   * [!DNL Workfront for Outlook] läser e-postmetadata för att visa information om tillägget om de tidigare åtgärderna som utförts i tillägget med samma e-postadress.
* När en användare skickar en begäran skapar en uppgift eller skickar ett e-postmeddelande som en uppdatering från [!DNL Workfront for Outlook] (klicka på knappen [!UICONTROL submit] i tillägget):
   * [!DNL Workfront for Outlook] läser e-postmeddelandet för att skicka det till Workfront som en begärandebeskrivning eller kommentar.
   * [!DNL Workfront for Outlook] uppdaterar e-postmetadata för att lagra information om skickade begäranden eller uppdaterade objekt.
   * [!DNL Workfront for Outlook] hämtar e-postbilagor från Exchange-servern för att överföra dem till skickade begäranden, skapade uppgifter eller uppdaterade objekt.
