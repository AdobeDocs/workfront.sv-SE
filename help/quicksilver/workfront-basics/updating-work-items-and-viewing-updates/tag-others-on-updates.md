---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagga andra om uppdateringar
description: När du ger uppdateringskommentarer för ett Adobe Workfront-objekt kan alla användare i projektet se den inskickade informationen. Det kan dock finnas tillfällen då användare som inte är med i projektet skulle kunna dra nytta av att visa den här informationen. I stället för att inkludera användarna i projektet kan du tagga dem i uppdateringen och dela dem med dem. Taggade användare får ett händelsemeddelande.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Tagga andra för uppdateringar

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

Du kan tagga användare när de gör en uppdatering av ett objekt om du vill dra deras uppmärksamhet till ett objekt som de annars kanske inte följer.

I stället för att inkludera de användarna i objektet genom att tilldela dem eller få dem att prenumerera på det, kan du tagga dem på uppdateringen och dela dem med dem. Taggade användare får ett Workfront-meddelande om den uppdatering du anger. Beroende på meddelandeinställningarna får de också ett e-postmeddelande om den uppdatering du anger.

## Att tänka på när du taggar användare i uppdateringar

* Användare som är taggade i uppdateringar måste aktivera ett personligt meddelande i sin profil för att kunna ta emot e-postmeddelandet. Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Mer information om hur du lägger till uppdateringar i Workfront-objekt finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* När ett problem konverteras till ett projekt eller en uppgift kopieras uppdateringarna till det nya projektet eller den nya uppgiften, men det är inte de taggade användarna. Om du vill fortsätta konversationen måste du tagga deltagarna igen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront package</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> <p>För ärenden och dokument:</p>

<ul><li><p>Medarbetare eller högre</p></li>
   <li><p>Begäran eller senare</p></li></ul>

<p>För alla andra objekt:</p>
   <ul><li><p>Ljus eller högre</p></li>
   <li><p>Granska eller högre</p></li></ul>

</td>  
  </tr>
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa eller ge senare åtkomst till objekt där du vill tagga användare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörighet</strong></td> 
   <td> <p>Visa eller högre behörigheter för de objekt där du vill tagga användare</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p>
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or higher access to the objects where you want to post the reply</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permission</strong></td> 
   <td> <p>View or higher permissions to the objects where you want to post the reply</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Tagga andra för uppdateringar

Du kan tagga andra vid uppdateringar på följande sätt:

* **Automatiskt**: När en användare startar en tråd, lägger till en kommentar eller lägger till ett svar, taggas de automatiskt och läggs till i taggarna för personer eller team i kommentarsrutan.
* **Manuellt**: När du lägger till en användare manuellt i taggområdet för kommenteringsrutan.

Du kan också ta bort användare som är taggade av misstag när du redigerar eller svarar på en kommentar.

1. Börja uppdatera en arbetsuppgift enligt beskrivningen i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Som kommentarsägare taggas du automatiskt och läggs till i taggarna för personer eller team i kommentarsrutan.

   >[!TIP]
   >
   >Kommentarägaren kan inte se sitt eget namn under Tagga personer eller team i kommenteringsrutan.

1. I fältet **Tagga personer eller team** börjar du skriva namnet på den användare eller det team som du vill ta med och klickar sedan på namnet när det visas i listrutan.

   eller

   Skriv @-symbolen i **Skriv en kommentar**, börja skriva namnet på den användare eller det team som du vill ska ingå i uppdateringen och klicka sedan på namnet när det visas i listrutan.

   >[!TIP]
   > 
   >Om du vill identifiera rätt användare när det finns användare med liknande eller identiska namn ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress.
   > 
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du taggar dem i en uppdatering.
   > 
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Tagga en användare](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Valfritt) Aktivera **Privat till mitt företag** i uppdateringsrutans nedre högra hörn om du vill göra uppdateringen privat. Detta gör uppdateringen synlig endast för användare i ditt företag.

   Alternativet **Privat till mitt företag** är bara tillgängligt när ett företag har angetts i din Workfront-profil.

   >[!NOTE]
   >
   >Taggade användare utanför företaget kan fortfarande få ett meddelande eller e-postmeddelande i appen, även om de inte ser de privata kommentarerna på fliken Uppdateringar. Vi rekommenderar att du inte taggar externa användare vid en uppdatering om du inte vill dela informationen med dem.

1. (Valfritt) Om du vill lägga till flera användare och team upprepar du steg 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alla användare och teammedlemmar som visas i fältet&quot;Tagga personer eller team&quot; får ett meddelande i appen för uppdateringen och kan få ett e-postmeddelande, beroende på konfigurationen av deras e-postaviseringsinställningar. Användare som taggar sig i en kommentar eller svarar får ett meddelande om kommentaren eller svaret och kan se sitt namn i listan som medlem i tråden för resten av tråden, men de får inget annat meddelande om de inte taggar sig igen. Mer information finns i [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) och [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicka på **Skicka**.\
   Användare som ingår i uppdateringen får automatiskt behörigheten Visa för objektet och kan visa och svara på uppdateringar som gjorts för objektet.

   Namnen på de taggade enheterna visas bredvid deras avatarer, upp till två enheter. Om fler än två enheter har taggats visas namnet på den första, förutom ett antal ytterligare enheter med taggar.

   ![Medlemsikoner utökade](assets/members-icons-expanded-unshimmed.png)

   När du är taggad i kommentarstexten markeras ditt namn i kommentarerna.

   Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) i det övre högra hörnet av kommentaren och klicka sedan på **Redigera**. Ta bort någon av de taggade användarna och klicka sedan på **Skicka**.

   >[!IMPORTANT]
   >
   >Du kan bara redigera en kommentar inom 15 minuter efter att du har skrivit in den. Du kan bara redigera kommentarer som du har lagt till.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Tag users in update](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![Tagging transparency](assets/tagging-transparency-350x192.png)
-->

Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



