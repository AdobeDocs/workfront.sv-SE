---
content-type: overview;reference
navigation-topic: notifications
title: Översikt över meddelanden
description: Adobe Workfront skickar e-postmeddelanden, meddelanden i appen och meddelanden till din mobila enhet.
author: Courtney
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1355'
ht-degree: 0%

---

# Översikt över meddelanden

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] skickar e-postmeddelanden, meddelanden i appen och meddelanden till din mobila enhet.

## E-postaviseringar

[!DNL Workfront] skickar e-postmeddelanden till aviseringsanvändare om aktivitet i Workfront och tillhandahåller användbar information och länkar.

Mer information om hur du ändrar inställningarna för e-postmeddelanden finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Om du vill få e-postmeddelanden från sandlådemiljön måste du aktivera e-post från din användarprofil i den miljön.

Du kan få följande e-postmeddelanden från [!DNL Workfront]:

* [Händelsemeddelanden](#event-notifications)
* [Dagliga sammandrag-meddelanden](#daily-digest-notifications)
* [Meddelande om kommentarer](#notification-of-posted-comments)
* [Automatiska påminnelser](#automatic-reminders)
* [Påminnelsemeddelanden](#reminder-notifications)
* [Meddelanden från anslagstavlor](#boards-notifications)
* [Andra [!DNL Workfront] e-postmeddelanden](#other-workfront-emails)

### Händelsemeddelanden

Händelsemeddelanden utlöses vanligtvis av vissa fördefinierade händelser, som att du har tilldelats en uppgift eller att du får ett svar på en kommentar som du har gjort.

När händelsemeddelanden har aktiverats i ditt [!DNL Workfront]-system av [!DNL Workfront]-administratören eller gruppadministratören kan du välja vilka du vill få genom att redigera dina [!UICONTROL Notifications]-inställningar i din användarprofil. Du kan också välja om du vill få meddelanden när händelser inträffar eller om du vill få händelser summerade i ett dagligt meddelande.

Du kanske bara ser en delmängd av de här meddelandena i inställningarna, beroende på hur [!DNL Workfront]-administratören har konfigurerat händelsemeddelanden för [!DNL Workfront]-systemet. Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Standardstatusen visar vilka meddelanden (varje dag, direkt eller båda) som är aktiverade som standard för nya användare när du skapar nya användare.

En fullständig lista över händelsemeddelanden och information om hur de aktiveras och konfigureras på systemnivå, gruppnivå eller användarnivå finns i [Händelsemeddelanden tillgängliga i [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Mer information om hur du väljer vilka händelsemeddelanden du vill ta emot finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Händelsemeddelanden är de enda meddelanden som kan konfigureras för att levereras i dagliga sammandragsuppdateringar.

### Dagliga sammandrag-meddelanden

Ett dagligt sammandragsmeddelande är ett e-postmeddelande som innehåller alla meddelanden av en viss typ som du har fått 24 timmar före e-postmeddelandet.

En fullständig lista över vilka e-postmeddelanden som har aktiverats för en daglig e-postmeddelandeleverans samt information om alla kategorier för e-postmeddelanden finns i [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] skickar inga dagliga sammanfattningsmeddelanden för kategorierna [!UICONTROL Miscellaneous] och [!DNL Goals] av händelser. Du kan inte inaktivera Dagliga meddelanden för dessa kategorier.

Det finns flera saker som du bör vara medveten om när du får dagliga sammandrag:

* Varje [!UICONTROL notifications]-avsnitt på din **[!UICONTROL My Settings]**-panel genererar ett eget e-postmeddelande med daglig sammanfattning. Du kan ha så många e-postmeddelanden med dagliga sammandrag varje dag som meddelandeinställningar som är aktiverade för dagliga sammandrag via e-post.\
   Om du till exempel har valt att få ett dagligt sammandrag-e-postmeddelande för flera åtgärder under **[!UICONTROL Information about Projects I],** får du ett e-postmeddelande med en lista över alla händelser som har träffats för det här området.

* Meddelanden i ett dagligt meddelande grupperas efter olika kriterier. I fallet **[!UICONTROL Information about Projects I Own]** grupperas till exempel händelserna efter projektnamnet.

  För kategorin **[!UICONTROL Communication]** grupperas meddelandena efter det objekt som kommunikationen inträffade i.

  >[!NOTE]
  >
  >I kategorin Kommunikation kan du välja enskilda meddelanden som endast ska levereras omedelbart. Om du vill få meddelanden levererade i en daglig sammanfattning måste du markera alla.

* Den dagliga sammandraget visar händelser som har inträffat för åtgärder i ett visst område (som **Information om projekt jag äger**) inom 24 timmar före den leveranstid som valts.
* Tidszonen för den tid som valts för daglig sammandragsleverans matchar din tidszon så som den är konfigurerad i webbläsaren.
* De dagliga e-postmeddelandena med sammandraget har samma namn som avsnittet på ämnesraden samt det datum då de levereras.
* Minst en händelse måste utlösa ett meddelande för att den dagliga sammanfattningen ska kunna levereras. Dagliga sammanfattningar skickas inte om inga händelser som är markerade för dagliga e-postmeddelanden med sammandrag uppfylls.

### Meddelande om kommentarer

Meddelandena i kategorin [!UICONTROL Communication] varnar dig för kommentarer som har bokförts i dataströmmen [!UICONTROL Update] för ett visst objekt.

Dagliga e-postmeddelanden med sammandrag för kategorin [!UICONTROL Communication] har valts för alla tillgängliga meddelanden.

Informationen sammanfattas för objektet där kommunikationen inträffade och ett totalt antal kommunikationsmeddelanden visas för varje objekt.

Så här besvarar du kommentaren eller visar den i Workfront:

1. Klicka på knappen **[!UICONTROL Comment]** i e-postmeddelandet.

   Objektets [!UICONTROL Updates]-område öppnas med den specifika kommentaren konturerad i blått.

   En svarsruta är öppen, som du kan använda för att svara på kommentaren.

Mer information om hur du konfigurerar e-postmeddelanden, inklusive hur du aktiverar dagliga sammandragsmeddelanden, finns i [Visa och ändra inställningarna för e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatiska påminnelser

Automatiska påminnelser aktiveras av din [!DNL Workfront]-administratör för att informera dig om aktiviteter och problem som förfaller, förfaller eller ligger nära det planerade slutförandedatumet. För sena meddelanden skickas e-postmeddelandet varje natt tills uppgiften eller utgåvan har slutförts. När administratören har konfigurerat dessa kan du inte inaktivera dem. Du kan inte heller ändra innehållet eller ämnesraden i ett e-postmeddelande som utlöses av en automatisk påminnelse.

De kan skickas till ett eller flera av följande:

* Användare som har tilldelats en uppgift eller ett problem
* Användarens chef
* Direktörens chef

Automatiska påminnelsemeddelanden skickas från den e-postadress som din [!DNL Workfront]-administratör har valt för att hantera utgående e-postmeddelanden.

Beroende på vilken automatisk påminnelse som aktiveras finns följande typ av information i det automatiska påminnelsemeddelandet:

* Det datum då uppgiften eller utgåvan skapades
* Namn på aktivitet eller ärende
* Namnet på det projekt där uppgiften eller utgåvan finns
* Beskrivning av uppgift eller ärende
* En lista över användare som har tilldelats uppgiften eller utgåvan
* Namnet på den användare som angav uppgiften eller utgåvan
* Uppgiftens eller frågans prioritet
* Datum när aktiviteten eller utgåvan blev försenad

Mer information om hur du aktiverar automatiska påminnelser finns i [Konfigurera automatiska påminnelser](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Påminnelsemeddelanden

En [!DNL Workfront]-administratör (eller en användare med [!UICONTROL Planner] åtkomstnivå och administrativ åtkomst till påminnelsemeddelanden) kan utforma påminnelsemeddelanden om kommande deadlines och manuellt associera dem med projekt, uppgifter, utgåvor och tidrapporter.

>[!IMPORTANT]
>
>Om tidsgränsen ändras efter att en användare får en påminnelse om något av de objekt som nämns ovan, får användaren inte något nytt påminnelsemeddelande.

Påminnelsemeddelanden skickas från den e-postadress som administratören för [!DNL Workfront] har valt att hantera utgående e-postmeddelanden.

Mer information om hur du konfigurerar och aktiverar påminnelsemeddelanden finns i [Konfigurera påminnelsemeddelanden](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Mer information om hur du kan få nödvändig administrativ åtkomst finns i [Bevilja användare administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Meddelanden från anslagstavlor

[!DNL Adobe Workfront] [!UICONTROL Boards] skickar ett e-postmeddelande till dig när du läggs till på en anslagstavla och när du tilldelas ett kort. Du kan välja vilka e-postmeddelanden du vill få med dina inställningar för anslagstavlor.

Mer information finns i [E-postmeddelanden och inställningar för anslagstavlor](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Andra [!DNL Workfront] e-postmeddelanden

Det finns andra e-postmeddelanden som du kan ta emot från [!DNL Workfront] som inte kan konfigureras.

Följande e-postmeddelanden skickas automatiskt av [!DNL Workfront] när dessa villkor uppfylls:

* Återställ ett objekt: När administratören för [!DNL Workfront] återställer ett objekt från behållaren för [!UICONTROL Recycle] skickas ett e-postmeddelande till administratören för [!DNL Workfront].
* Det gick inte att återställa: När administratören [!DNL Workfront] försöker återställa ett objekt från papperskorgen och återställningen misslyckas skickas ett e-postmeddelande till administratören för [!DNL Workfront].

Följande e-postmeddelanden kan bara konfigureras på användarprofilnivå. De kan inte aktiveras eller inaktiveras på systemnivå:

* Slutförande av personlig uppgift: När en personlig uppgift som du har tilldelat någon annan har slutförts får du ett e-postmeddelande.
* Kommentar tillagd till användaren: När någon kommenterar din användarprofil får du ett e-postmeddelande.

## Meddelanden i appen

Du kan ta emot meddelanden i webbprogrammet [!DNL Workfront] när vissa händelser inträffar.

Mer information om meddelanden i appen finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-postmeddelanden i mobilappen

Du kan ta emot [!DNL Workfront] e-postmeddelanden i din mobilapp på din mobila enhet.

Om du har [!DNL Workfront]-mobilappen installerad på telefonen och trycker på länkarna i e-postmeddelandet öppnas de i [!DNL Workfront]-mobilappen. Detta inkluderar att trycka på någon av följande åtgärdsknappar:

* [!UICONTROL Work On It]
* [!UICONTROL Comment]
* [!UICONTROL Make Approval Decision]
* [!UICONTROL See All Notifications]
* [!UICONTROL Add]
* [!UICONTROL Get Started]
* [!UICONTROL See More Details]

Mer information om [!DNL Workfront]-mobilappen finns i [Använda  [!DNL Adobe Workfront] mobilappen](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
