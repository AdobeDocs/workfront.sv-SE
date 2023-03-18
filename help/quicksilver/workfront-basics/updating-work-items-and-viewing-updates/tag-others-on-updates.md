---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagga andra för uppdateringar
description: När du ger uppdateringskommentarer för ett Adobe Workfront-objekt kan alla användare i projektet se den inskickade informationen. Det kan dock finnas tillfällen då användare som inte är med i projektet skulle kunna dra nytta av att visa den här informationen. I stället för att inkludera användarna i projektet kan du tagga dem i uppdateringen och dela dem med dem. Taggade användare får ett händelsemeddelande.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Tagga andra för uppdateringar

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
Du kan tagga användare när de gör en uppdatering av ett objekt om du vill dra deras uppmärksamhet till ett objekt som de annars kanske inte följer.
I stället för att inkludera de användarna i objektet genom att tilldela dem eller få dem att prenumerera på det, kan du tagga dem på uppdateringen och dela dem med dem. Taggade användare får ett meddelande om den uppdatering du anger.

>[!NOTE]
>
>Ett händelsemeddelande måste aktiveras för att en användare ska kunna ta emot e-postmeddelandet. Administratörer kan aktivera meddelanden för hela systemet eller för en toppnivågrupp. En användare kan även aktivera och inaktivera enskilda händelsemeddelanden i sin egen användarprofil. Mer information finns i följande:
>
>* [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Visa och konfigurera händelsemeddelanden för en grupp](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
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
   <td> <p>Begär eller högre för frågor och dokument. Granska eller högre för alla andra objekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>begärande eller högre för frågor och dokument, Granskare eller högre för alla andra objekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Visa åtkomst till objektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Tagga andra för uppdateringar

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. Börja uppdatera en arbetsuppgift enligt beskrivningen i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. I **Meddela** börjar du skriva namnet på den användare eller det team som du vill inkludera och klickar sedan på namnet när det visas i listrutan.

   eller

   Skriv @-symbolen i **Starta en ny uppdatering** börjar du skriva namnet på den användare eller det team som du vill inkludera i uppdateringen och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Om du vill identifiera rätt användare när det finns användare med liknande eller identiska namn ska du lägga märke till avataren, användarens primära roll eller användarens e-postadress. Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du taggar dem i en uppdatering.

   ![](assets/tag-users-in-update.png)

1. (Valfritt) Aktivera **Privat till mitt företag** i uppdateringsrutans nedre högra hörn. Detta gör uppdateringen synlig endast för användare i ditt företag.

   >[!NOTE]
   >
   >Taggade användare utanför företaget kan fortfarande få ett meddelande eller e-postmeddelande i appen, även om de inte ser de privata kommentarerna på fliken Uppdateringar. Vi rekommenderar att du inte taggar externa användare vid en uppdatering om du inte vill dela informationen med dem.

1. (Valfritt) Om du vill lägga till flera användare och team upprepar du steg 2.

   >[!NOTE]
   >
   >Alla användare och teammedlemmar som visas i fältet Notify (Meddela) får ett meddelande i appen för uppdateringen och kan få ett e-postmeddelande, beroende på konfigurationen av deras e-postmeddelandeinställningar. Användare som taggar sig i en kommentar eller svarar får ett meddelande om kommentaren eller svaret och kan se sitt namn i fältet Meddela för resten av tråden, men de får inget annat meddelande om de inte taggar sig igen. Mer information finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) och [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicka **Uppdatera**.\
   Användare som ingår i uppdateringen får automatiskt behörigheten Visa för objektet och kan visa och svara på uppdateringar som gjorts för objektet.

   Du kan se vilka som har taggats i varje svar högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får ett meddelande varje gång en uppdatering eller ett svar görs för objektet.

   ![](assets/tagging-transparency-350x192.png)

   Mer information om de ytterligare funktioner som är tillgängliga när du uppdaterar en arbetsuppgift finns i [Uppdatera arbete](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->