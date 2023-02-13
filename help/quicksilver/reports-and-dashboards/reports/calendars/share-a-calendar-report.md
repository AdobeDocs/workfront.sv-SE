---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Dela en kalenderrapport
description: Du kan dela en kalender med andra användare och göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront] för att visa den.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Dela en kalenderrapport

Du kan dela en kalender med andra användare och göra den tillgänglig för allmänheten, så att någon utan en [!DNL Adobe Workfront] för att visa den.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst [!UICONTROL to Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] eller högre behörigheter till kalenderrapporten, med tillgång till delning</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Dela en kalender med [!DNL Workfront] användare {#share-a-calendar-with-workfront-users}

Att dela en kalender påminner om att dela andra objekt. Mer information om att dela objekt i [!DNL Adobe Workfront], se [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Kalendrar som har delats med dig visas med en asterisk (&#42;) bredvid kalendernamnet.

Dela en kalender i [!DNL Workfront]:

1. Gå till kalendern som du vill dela.
1. Klicka **[!UICONTROL Calendar Actions]** och sedan klicka **[!UICONTROL Sharing]**.

1. I **[!UICONTROL Give Calendar access to]** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela kalendern med och klickar sedan på namnet i listrutan.\
   Mer information om hur du anger behörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Upprepa steg 3 för varje användare, team, roll eller grupp som du vill ge åtkomst till kalendern.
1. Ange behörigheter för varje användare, team, roll, grupp eller företag som du har lagt till i steg 3 genom att klicka på den nedrullningsbara menyn och sedan välja den behörighetsnivå som du vill ge:

   * **[!UICONTROL View]:** Användare kan granska och dela kalendern.

      ![Dela kalender med Visa åtkomst](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL Manage]:** Användarna har fullständig åtkomst till kalendern, minus administrativa behörigheter, som ges på åtkomstnivån, plus alla visningsbehörigheter.

      ![Dela kalender med Hantera åtkomst](assets/calendar-share-manage-permissions-350x241.png)

      >[!NOTE]
      >
      >The [!DNL Workfront] administratör och den som har skapat kalendern kan ta bort behörigheter från dessa entiteter.

1. (Valfritt) Beroende på en användares roll kan du klicka **[!UICONTROL Advanced Options]** och sedan klicka **[!UICONTROL Share]**&#x200B; att låta användaren dela kalendern med andra användare.

   Mer information om behörighetsnivåer finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Valfritt) Gör kalendern tillgänglig för alla [!DNL Workfront] klickar du på kugghjulsikonen och klickar sedan på **[!UICONTROL Make this visible system-wide]** för att göra objektet tillgängligt för alla [!DNL Workfront] -användare.\
   Alla användare kan se objektet baserat på de behörigheter som du anger.

1. Klicka på **[!UICONTROL Save]**.

## Dela en kalender med en offentlig länk

Du kan göra en kalender offentlig och dela en länk med personer som inte har en [!DNL Workfront] licens.

1. Gå till kalendern som du vill dela.
1. Klicka **[!UICONTROL Calendar Actions]** och sedan klicka **[!UICONTROL Sharing]**.

1. Klicka på kugghjulsikonen och sedan på **[!UICONTROL Make this public to external users]**.
1. Klicka på **[!UICONTROL Copy link]**.
1. Klicka på **[!UICONTROL Save]**.

## Dela en kalender med en privat länk

Du kan dela en privat kalenderlänk med [!DNL Workfront] -användare. Användarna måste logga in för att kunna visa kalendern när de använder länken.

1. Gå till kalendern som du vill dela.
1. Klicka **[!UICONTROL Calendar Actions]** och sedan klicka **[!UICONTROL Get Sharable Link]**.

1. Klicka på **[!UICONTROL Copy Link]**.

   >[!NOTE]
   >
   >[!DNL Workfront] -användare måste ha tillgång till kalendern för att kunna komma åt den via länken. Information om hur du beviljar åtkomst finns i [Dela en kalender med [!DNL Workfront] användare](#share-a-calendar-with-workfront-users).\
   >Om användarna inte har åtkomst kan de begära det efter att länken har klistrats in i webbläsaren.
