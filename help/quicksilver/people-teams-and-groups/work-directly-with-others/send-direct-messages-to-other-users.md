---
content-type: reference
product-area: user-management
navigation-topic: people-teams-and-groups
title: Skicka direktmeddelanden till andra användare
description: Med Adobe Workfront kan du snabbt och enkelt skicka meddelanden som inte har med något att göra direkt till andra Workfront-användare.
author: Becky
feature: People Teams and Groups
exl-id: 82a1c304-176a-48c5-809d-40663ee768b7
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Skicka direktmeddelanden till andra användare

Med [!DNL Adobe Workfront] kan du snabbt och enkelt skicka meddelanden som inte är relaterade till något arbetsobjekt direkt till andra [!DNL Workfront]-användare. Meddelanden som skickas enligt beskrivningen i det här avsnittet visas på fliken [!UICONTROL Updates] på användarens profilsida och är synliga för alla användare. Mer information om uppdateringar finns i [Uppdatera arbetsobjekt och visa uppdateringar: artikelindex](../../workfront-basics/updating-work-items-and-viewing-updates/update-work-items-and-view-updates.md).

Användaren som du skickar meddelandet till får följande typer av meddelanden när du skickar ett meddelande enligt beskrivningen i det här avsnittet:

* Ett meddelande i appen, enligt beskrivningen i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)
* Ett e-postmeddelande

  Detta beror på vilka typer av e-postmeddelanden användaren har konfigurerats för att ta emot. Mer information finns i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md), [Visa och konfigurera händelsemeddelanden för en grupp](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md) och [Ändra dina egna e-postmeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Om du vill skicka ett meddelande från användarens profilsida måste du ha:</P>
   <p>Ljus eller högre</p>
   <p>Granska eller högre</p>
   <p>Om du vill skicka ett meddelande från användarlistan måste du ha:</p>
   <p>Standard</p>
   <p>Arbeta eller högre</p></td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skicka ett meddelande som inte är relaterat till ett arbetsobjekt till en annan användare från profilsidan

1. Gå till profilsidan för den användare som du vill skicka ett meddelande till.

   Om du vill gå till en användarprofilsida klickar du på användarens länkade namn så som det visas var som helst i [!DNL Workfront]-gränssnittet. Användarnamn visas i många områden, t.ex. i en kommentar som görs av användaren.

1. Klicka i textrutefältet på fliken **[!UICONTROL Updates]**.

   ![Meddelandeanvändare på fliken [!UICONTROL Updates]](assets/send-message-to-user-on-updates-tab.png)

1. Skriv ditt meddelande.
1. (Valfritt) Klicka i fältet **[!UICONTROL Notify]** och börja sedan skriva namnet på en annan användare som du vill inkludera i det här meddelandet.

1. (Valfritt) Välj **[!UICONTROL Private to my company]** om du bara vill att det här meddelandet ska vara synligt för andra användare i ditt företag.

   >[!TIP]
   >
   >Inställningen [!UICONTROL **Privat till mitt företag**] är bara tillgänglig när din Workfront-profil är associerad med ett företag.

1. Klicka på **[!UICONTROL Update].**
Meddelandet läggs upp högst upp i meddelandelistan på fliken **[!UICONTROL Updates]** på användarens profilsida.

## Skicka ett meddelande till en eller flera användare från användarlistan

Det här alternativet är bara tillgängligt om du har en Standard-, Plan- eller Work-licens.

{{step-1-to-users}}

1. Markera den eller de användare som du vill skicka ett meddelande till och klicka på [!UICONTROL **Skicka uppdatering till användare**].
1. Skriv meddelandet i fönstret [!UICONTROL Send update to user]. Använd textformateringsalternativen efter behov. Mer information finns i [Använd RTF i en Workfront-kommentar](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md#use-rich-text-in-a-workfront-comment) i artikeln [Uppdatera arbete](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![Meddelandeanvändare i fönstret Skicka uppdatering till ](assets/send-update-to-user-072825.png)

1. (Valfritt) Klicka på **Tagga personer** om du vill tagga ytterligare användare i meddelandet. Mer information finns i [Tagga andra om uppdateringar](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
1. (Valfritt) Välj **[!UICONTROL Private to my company]** om du bara vill att det här meddelandet ska vara synligt för andra användare i ditt företag.

   >[!TIP]
   >
   >Inställningen [!UICONTROL **Privat till mitt företag**] är bara tillgänglig när din Workfront-profil är associerad med ett företag.
1. Klicka på [!UICONTROL **Skicka**].
Meddelandet läggs upp högst upp i meddelandelistan på fliken **[!UICONTROL Updates]** på varje taggad användares profilsida.
