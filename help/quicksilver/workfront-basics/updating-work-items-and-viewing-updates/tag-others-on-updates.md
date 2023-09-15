---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagga andra för uppdateringar
description: När du ger uppdateringskommentarer för ett Adobe Workfront-objekt kan alla användare i projektet se den inskickade informationen. Det kan dock finnas tillfällen då användare som inte är med i projektet skulle kunna dra nytta av att visa den här informationen. I stället för att inkludera användarna i projektet kan du tagga dem i uppdateringen och dela dem med dem. Taggade användare får ett händelsemeddelande.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 0%

---

# Tagga andra för uppdateringar

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>\
<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>

<span class="preview">Information om det aktuella releaseschemat finns i [Versionsöversikt för fjärde kvartalet 2023](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>Vi håller på att omarbeta kommentarsfunktionerna i Adobe Workfront.
>Beroende på vilken miljö och vilka objekt du har tillgång till kommentarfunktionerna från kan du se olika funktioner i uppdateringsavsnittet.
>
>Mer information om den nya kommentarsfunktionen och dess tillgänglighet finns på [Ny kommentarsfunktion](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Den nya kommentarsupplevelsen är bara tillgänglig för uppdateringsavsnittet och är inte tillgänglig för följande områden:
>
> * Startsida
> * Panelen Sammanfattning i listor
> * Sammanfattningspanelen i tidrapporter


<!--old note before August 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

-->

Du kan tagga användare när de gör en uppdatering av ett objekt om du vill dra deras uppmärksamhet till ett objekt som de annars kanske inte följer.
I stället för att inkludera de användarna i objektet genom att tilldela dem eller få dem att prenumerera på det, kan du tagga dem på uppdateringen och dela dem med dem. Taggade användare får ett meddelande om den uppdatering du anger.

>[!NOTE]
>
>Användaren måste aktivera ett personligt meddelande i sin profil för att kunna ta emot e-postmeddelandet. Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

Mer information om hur du lägger till uppdateringar till Workfront-objekt finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>När ett problem konverteras till ett projekt eller en uppgift kopieras uppdateringarna till det nya projektet eller den nya uppgiften, men det är inte de taggade användarna. Om du vill fortsätta konversationen måste du tagga deltagarna igen.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Begär eller högre för problem och dokument; Granska eller högre för alla andra objekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Begärande eller högre för problem och dokument; Granskare eller högre för alla andra objekt</p> 
   <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Tagga andra för uppdateringar

Om du taggar andra i en uppdatering varierar beroende på vilken upplevelse och vilket objekt du väljer.

### Tagga andra om uppdateringar i det aktuella uppdateringsavsnittet

<!--change "current" to "legacy" at the October 26, 2023 release-->

Du kan tagga användare manuellt i det aktuella uppdateringsavsnittet.

1. Börja uppdatera en arbetsuppgift enligt beskrivningen i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. I **Meddela** börjar du skriva namnet på den användare eller det team som du vill inkludera och klickar sedan på namnet när det visas i listrutan.

   eller

   Skriv @-symbolen i **Starta en ny uppdatering** börjar du skriva namnet på den användare eller det team som du vill inkludera i uppdateringen och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Om du vill identifiera rätt användare när det finns användare med liknande eller identiska namn ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress.
   >
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du taggar dem i en uppdatering.
   >
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Valfritt) Aktivera **Privat till mitt företag** i uppdateringsrutans nedre högra hörn. Detta gör uppdateringen synlig endast för användare i ditt företag. The **Privat till mitt företag** är bara tillgängligt när ett företag anges i din Workfront-profil.

   >[!NOTE]
   >
   >Taggade användare utanför företaget kan fortfarande få ett meddelande eller e-postmeddelande i appen, även om de inte ser de privata kommentarerna på fliken Uppdateringar. Vi rekommenderar att du inte taggar externa användare vid en uppdatering om du inte vill dela informationen med dem.

1. (Valfritt) Om du vill lägga till flera användare och team upprepar du steg 2.

   >[!NOTE]
   >
   >Alla användare och teammedlemmar som visas i fältet Notify (Meddela) får ett meddelande i appen för uppdateringen och kan få ett e-postmeddelande, beroende på konfigurationen av deras e-postaviseringsinställningar. Användare som taggar sig i en kommentar eller svarar får ett meddelande om kommentaren eller svaret och kan se sitt namn i fältet Meddela för resten av tråden, men de får inget annat meddelande om de inte taggar sig igen. Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) och [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicka **Uppdatera**.\
   Användare som ingår i uppdateringen får automatiskt behörigheten Visa för objektet och kan visa och svara på uppdateringar som gjorts för objektet.

   Du kan se vilka som har taggats i varje svar högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet.

   ![](assets/tagging-transparency-350x192.png)

   Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### Tagga andra om uppdateringar i den nya kommentarsfunktionen

Du kan tagga andra vid uppdateringar på följande sätt:

* **Automatiskt**: När en användare startar en tråd, lägger till en kommentar eller lägger till ett svar, taggas de automatiskt och läggs till i taggarna för personer eller team i kommentarsrutan. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >När tråden startar i den gamla kommentarsfunktionen taggas inte deltagare i tråden automatiskt.

* **Manuellt**: När du lägger till en användare manuellt i taggområdet i kommentarsrutan.

Du kan också ta bort användare som är taggade av misstag när du redigerar eller svarar på en kommentar.

1. Börja uppdatera en arbetsuppgift enligt beskrivningen i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Som kommentarsägare taggas du automatiskt och läggs till i taggarna för personer eller team i kommentarsrutan.

   >[!TIP]
   >
   >Kommentarägaren kan inte se sitt eget namn under Tagga personer eller team i kommenteringsrutan.

1. I **Tagga personer eller team** börjar du skriva namnet på den användare eller det team som du vill inkludera och klickar sedan på namnet när det visas i listrutan.

   eller

   Skriv @-symbolen i **Skriv en kommentar** börjar du skriva namnet på den användare eller det team som du vill inkludera i uppdateringen och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   > 
   >Om du vill identifiera rätt användare när det finns användare med liknande eller identiska namn ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress.
   > 
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du taggar dem i en uppdatering.
   > 
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-others-unified-commenting.png)

1. (Valfritt) Aktivera **Privat till mitt företag** i uppdateringsrutans nedre högra hörn. Detta gör uppdateringen synlig endast för användare i ditt företag. The **Privat till mitt företag** är bara tillgängligt när ett företag anges i din Workfront-profil.

   >[!NOTE]
   >
   >* Det här alternativet visas bara när användaren är associerad med ett företag.
   >* Taggade användare utanför företaget kan fortfarande få ett meddelande eller e-postmeddelande i appen, även om de inte ser de privata kommentarerna på fliken Uppdateringar. Vi rekommenderar att du inte taggar externa användare vid en uppdatering om du inte vill dela informationen med dem.

1. (Valfritt) Om du vill lägga till flera användare och team upprepar du steg 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alla användare och teammedlemmar som visas i fältet&quot;Tagga personer eller team&quot; får ett meddelande i appen för uppdateringen och kan få ett e-postmeddelande, beroende på konfigurationen av deras e-postaviseringsinställningar. Användare som taggar sig i en kommentar eller svarar får ett meddelande om kommentaren eller svaret och kan se sitt namn i listan som medlem i tråden för resten av tråden, men de får inget annat meddelande om de inte taggar sig igen. Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) och [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicka **Skicka**.\
   Användare som ingår i uppdateringen får automatiskt behörigheten Visa för objektet och kan visa och svara på uppdateringar som gjorts för objektet.

   <span class="preview">Namnen på de taggade enheterna visas bredvid deras avatarer, upp till två enheter. Om fler än två enheter har taggats visas namnet på den första, förutom ett antal ytterligare enheter med taggar.</span>

   ![](assets/members-icons-expanded-unshimmed.png)

   Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på **Mer** meny ![](assets/more-menu.png) <span class="preview">i kommentarens övre högra hörn</span>och sedan klicka **Redigera**. Ta bort alla taggade användare och klicka sedan på **Skicka**. Du kan bara redigera en kommentar inom 15 minuter efter att du har skrivit in den. Du kan bara redigera kommentarer som du har lagt till.

   >[!TIP]
   >
   >När du använder den äldre kommentarsfunktionen för att lägga till kommentarer och svar, kan de som inte är specifikt taggade inte tas bort manuellt av dem som använder den nya kommentarsfunktionen.



