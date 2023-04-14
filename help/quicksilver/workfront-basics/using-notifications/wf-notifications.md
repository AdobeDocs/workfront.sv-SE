---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront-meddelanden
description: Adobe Workfront skickar e-postmeddelanden, meddelanden i appen och meddelanden till din mobila enhet.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 06e5f4eb275548c5f1d2740632963a0c2fee48ac
workflow-type: tm+mt
source-wordcount: '1261'
ht-degree: 0%

---

# [!DNL Adobe Workfront] meddelanden

{{highlighted-preview}}

[!DNL Adobe Workfront] skickar e-postmeddelanden, meddelanden i appen och meddelanden till din mobila enhet.

## E-postaviseringar

[!DNL Workfront] skickar ut ett antal e-postmeddelanden som varnar användare om aktiviteter i Workfront och ger användbar information och länkar.

>[!NOTE]
>
>Om du vill få e-postmeddelanden från sandlådemiljön måste du aktivera e-post från din användarprofil i den miljön.

Du kan få följande e-postmeddelanden från [!DNL Workfront]:

* [Händelsemeddelanden](#event-notifications)
* [Dagliga sammandragsmeddelanden](#daily-digest-notifications)
* [Meddelande om kommentarer](#notification-of-posted-comments)
* [Automatiska påminnelser](#automatic-reminders)
* [Påminnelsemeddelanden](#reminder-notifications)
* [Meddelanden från anslagstavlor](#boards-notifications)
* [Övriga [!DNL Workfront] e-post](#other-workfront-emails)

### Händelsemeddelanden

Händelsemeddelanden är fördefinierade i [!DNL Workfront]. De utlöses vanligtvis av vissa händelser.

När händelsemeddelandena har aktiverats av [!DNL Workfront] administratör eller gruppadministratör kan du välja vilka du vill få genom att redigera [!UICONTROL Notifications] inställningar i din användarprofil. Du kan också välja om du vill få meddelanden när händelser inträffar eller om du vill få händelser summerade i ett dagligt meddelande.

Beroende på hur [!DNL Workfront] administratören har konfigurerat händelsemeddelanden för din [!DNL Workfront] system (enligt beskrivning i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)) visas kanske bara en delmängd av dessa meddelanden i inställningarna.

Standardstatusen visar vilka meddelanden (varje dag, direkt eller båda) som är aktiverade som standard för nya användare när du skapar nya användare.

En fullständig lista över händelsemeddelanden och information om hur de aktiveras och konfigureras på systemnivå, gruppnivå eller användarnivå finns på [Händelsemeddelanden är tillgängliga i [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Mer information om hur du väljer vilka händelsemeddelanden du vill ta emot finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Händelsemeddelanden är de enda meddelanden som kan konfigureras för att levereras i dagliga sammandragsuppdateringar.

### Dagliga sammandragsmeddelanden

En fullständig lista över vilka e-postmeddelanden som har aktiverats för en daglig e-postleverans med sammanfattning samt information om alla kategorier för e-postmeddelanden finns i [Händelsemeddelanden](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] skickar inga Dagliga sammanfattningsmeddelanden för [!UICONTROL Miscellaneous] och [!DNL Goals] kategorier med händelser. Du kan inte inaktivera Dagliga meddelanden för dessa kategorier.

Det finns flera saker som du bör vara medveten om när du får dagliga sammandrag:

* Varje [!UICONTROL notifications] i **[!UICONTROL My Settings]** Panelen genererar ett eget e-postmeddelande med daglig sammanfattning. Du kan ha så många e-postmeddelanden med dagliga sammandrag varje dag som meddelandeinställningar som är aktiverade för dagliga sammandrag via e-post.\
   Om du till exempel har valt att få ett dagligt sammandrag-e-postmeddelande för flera åtgärder under **[!UICONTROL Information about Projects I]Own,** du får ett e-postmeddelande med en lista över alla händelser som har inträffat för det här området.

* Meddelanden i ett dagligt meddelande grupperas efter olika kriterier. I fallet med **[!UICONTROL Information about Projects I Own]**, grupperas händelserna efter projektnamnet.

   För **[!UICONTROL Communication]** -kategorin grupperas meddelandena efter det objekt som kommunikationen inträffade i.

* Den dagliga sammanfattningen visar händelser som har inträffat för åtgärderna i ett visst område (som **Information om projekt som jag äger**) inom 24 timmar före leveransdatum.
* Tidszonen för den tid som valts för daglig sammandragsleverans matchar din tidszon så som den är konfigurerad i webbläsaren.
* De dagliga e-postmeddelandena med sammandraget har samma namn som avsnittet på ämnesraden samt det datum då de levereras.
* Minst en händelse måste utlösa ett meddelande för att den dagliga sammanfattningen ska kunna levereras. Dagliga sammanfattningar skickas inte om inga händelser som är markerade för dagliga e-postmeddelanden med sammandrag uppfylls.

### Meddelande om kommentarer

Meddelandena i [!UICONTROL Communication] ger dig en kategorivarning om kommentarer som har bokförts i [!UICONTROL Update] dataström för ett visst objekt.

Dagliga e-postmeddelanden med sammanfattningar för [!UICONTROL Communication] har valts för alla tillgängliga meddelanden.

Informationen sammanfattas för objektet där kommunikationen inträffade och ett totalt antal kommunikationsmeddelanden visas för varje objekt.

Mer information om hur du konfigurerar e-postmeddelanden finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Anvisningar om hur du kommenterar [!UICONTROL Communication] e-post, se [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Mer information om [!UICONTROL Communication] e-post, se [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Mer information om hur du aktiverar dagliga sammandragsmeddelanden finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatiska påminnelser

Automatiska påminnelser aktiveras av [!DNL Workfront] för att informera dig om uppgifter och problem som förfaller, förfaller eller ligger nära det planerade slutdatumet. För sena meddelanden skickas e-postmeddelandet varje natt tills uppgiften eller utgåvan har slutförts. När administratören har konfigurerat dessa kan du inte inaktivera dem. Du kan inte heller ändra innehållet eller ämnesraden i ett e-postmeddelande som utlöses av en automatisk påminnelse.

De kan skickas till ett eller flera av följande:

* Användare som tilldelats en uppgift eller ett problem
* Användarens chef
* Direktörens chef

Automatiska påminnelser skickas från den e-postadress som din [!DNL Workfront] administratör har valts för att hantera utgående e-postmeddelanden.

Beroende på vilken automatisk påminnelse som aktiveras finns följande typ av information i det automatiska påminnelsemeddelandet:

* Det datum då uppgiften eller utgåvan skapades
* Namn på aktivitet eller ärende
* Namnet på det projekt där uppgiften eller utgåvan finns
* Beskrivning av uppgift eller ärende
* En lista över användare som har tilldelats uppgiften eller utgåvan
* Namnet på den användare som angav uppgiften eller utgåvan
* Uppgiftens eller frågans prioritet
* Datum när aktiviteten eller utgåvan blev försenad

Information om hur du aktiverar automatiska påminnelser finns i [Ställ in automatiska påminnelser](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Påminnelsemeddelanden

A [!DNL Workfront] administratör (eller en användare med [!UICONTROL Planner] åtkomstnivå och administrativ åtkomst till påminnelsemeddelanden) kan utforma påminnelser om snäva deadlines och bifoga dem till projekt, uppgifter, utgåvor och tidrapporter. Mer information om hur du får administratörsåtkomst finns i [Ge användarna administrativ åtkomst till vissa områden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>Om tidsgränsen ändras efter att en användare får en påminnelse om något av de objekt som nämns ovan, får användaren inte något nytt påminnelsemeddelande.

Påminnelsemeddelanden skickas från e-postadressen som [!DNL Workfront] administratör har valts för att hantera utgående e-postmeddelanden.

Mer information om hur du ställer in och aktiverar påminnelsemeddelanden finns i [Ställ in påminnelsemeddelanden](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

<span class="preview">

### Meddelanden från anslagstavlor

[!DNL Adobe Workfront] [!UICONTROL Boards] skickar ett e-postmeddelande till dig när du läggs till på en anslagstavla och när du tilldelas ett kort.

Du kan välja vilka e-postmeddelanden du vill få med dina inställningar för anslagstavlor. Mer information finns i [E-postmeddelanden och inställningar för anslagstavlor](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

</span>

### Övriga [!DNL Workfront] e-post

Det finns andra e-postmeddelanden du kan få från [!DNL Workfront] som inte kan konfigureras. Följande e-postmeddelanden skickas automatiskt av [!DNL Workfront] när dessa villkor är uppfyllda:

* Återställ ett objekt: När [!DNL Workfront] administratören återställer ett objekt från [!UICONTROL Recycle] Bin, ett e-postmeddelande skickas till [!DNL Workfront] administratör.
* Det gick inte att återställa: När [!DNL Workfront] administratören försöker återställa ett objekt från papperskorgen och återställningen misslyckas. Ett e-postmeddelande skickas till [!DNL Workfront] administratör.

Följande e-postmeddelanden kan bara konfigureras på användarprofilnivå. De kan inte aktiveras eller inaktiveras på systemnivå:

* Slutförande av personlig uppgift: När en personlig uppgift som du har tilldelat någon annan har slutförts får du ett e-postmeddelande.
* Kommentar tillagd till användaren: När någon kommenterar din användarprofil får du ett e-postmeddelande.

## Meddelanden i appen

Du kan få meddelanden inifrån [!DNL Workfront] webbprogram, när vissa händelser inträffar.

Mer information om meddelanden i appen finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-postmeddelanden i mobilappen

Du kan ta emot [!DNL Workfront] e-postmeddelanden i din mobilapp, på din mobila enhet.

Om du har [!DNL Workfront] Mobilappen som är installerad på telefonen och trycker på länkarna i e-postmeddelandet öppnas i [!DNL Workfront] Mobilapp. Detta inkluderar att trycka på någon av följande åtgärdsknappar:

* [!UICONTROL Work On It]
* [!UICONTROL Comment]
* [!UICONTROL Make Approval Decision]
* [!UICONTROL See All Notifications]
* [!UICONTROL Add]
* [!UICONTROL Get Started]
* [!UICONTROL See More Details]

Mer information om [!DNL Workfront] Mobilapp, se [Använd [!DNL Adobe Workfront] mobilapp](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
