---
product-area: setup
navigation-topic: notifications
keywords: ändra,e-post,meddelande,inställningar
title: Ändra dina egna e-postmeddelanden
description: I den här artikeln beskrivs hur du kan hantera e-postmeddelanden i din användarprofil.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Ändra dina egna e-postmeddelanden

<!-- Audited: 1/2024 -->

Din Adobe [!DNL Workfront]-administratör konfigurerar vilka e-postmeddelanden som användare får när händelser inträffar i Workfront (enligt beskrivningen i [[!UICONTROL Configure event] -meddelanden för alla i systemet ](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

Gruppadministratören kan också konfigurera vilka meddelanden som är aktiverade för dig och användarna i [!UICONTROL Home Group]. Om [!UICONTROL Home Group] är en undergrupp får du meddelanden som är aktiverade för den översta gruppen ovanför gruppen.

Du kan anpassa detta ytterligare genom att konfigurera vilka meddelanden du får. Du kan också välja om du vill få meddelanden när händelser inträffar eller i ett e-postmeddelande med en daglig sammanfattning.

Mer information om e-postmeddelanden finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Om du aktiverar en meddelandetyp och sedan upptäcker att du inte får meddelanden av den typen, kan det bero på att den typen inte gäller för din roll.
>* Administratören [!DNL Workfront] eller en gruppadministratör kan inte konfigurera meddelanden för [!DNL Workfront Goals]. Mer information om vilka meddelanden [!DNL Workfront]-administratören kan konfigurera finns i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Mer information om hur du konfigurerar enskilda meddelanden för [!DNL Workfront Goals] finns i den här artikeln.
>

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td>  <p>Nytt:</p> 
   <ul><li>Medarbetare eller högre</li></ul>
   <p>Aktuell:</p>
   <ul><li>Begäran eller högre</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och ändra inställningarna för e-postmeddelanden

{{step1-click-profile-pic}}

1. Klicka på ikonen **[!UICONTROL More]** ![Mer ](assets/more-icon.png) bredvid ditt namn och klicka sedan på **[!UICONTROL Edit]**.

1. Gå till avsnittet **[!UICONTROL Notifications]** i rutan **[!UICONTROL Edit Person]** som visas.

1. Klicka på en kategori om du vill visa meddelandeinställningarna för den kategorin.

   ![Mina profilmeddelanden](assets/my-profile-notifications.png)

1. Markera eller avmarkera kryssrutorna till höger för att ange om du vill få meddelanden varje dag, direkt eller båda.

   Du kan också använda kryssrutorna för en kategori för att aktivera eller inaktivera alla meddelanden i den kategorin.

   >[!NOTE]
   >
   >Om du är teammedlem i ett projekt får du även fortsättningsvis e-postmeddelanden om projektet tills du tas bort från teamet, även om du inte längre har tillgång till projektet. Instruktioner om hur du tar bort användare från ett team finns i [Ta bort användare från projekt](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   För kategorin **[!UICONTROL Communication]** kan du endast välja enskilda meddelanden för direktleverans. Om du vill få meddelanden levererade i en daglig sammanfattning måste du markera alla.

   Om alla e-postmeddelanden för en viss kategori är aktiverade visas rutan i kategorititeln som markerad. Om alla e-postmeddelanden i en viss kategori inaktiveras, avmarkeras rutan. Om vissa meddelanden aktiveras och andra inaktiveras visas kategorikryssrutan som en rak linje.\
   När du ändrar en aviseringsinställning visas etiketten **[!UICONTROL Edited]** för den aviseringsinställningen så att du ser att aviseringsinställningen har ändrats.

1. Om du har valt att skicka meddelanden som dagliga sammandrag, markerar du den tid på dagen som du vill ta emot det högst upp i avsnittet **[!UICONTROL Notifications]** på menyn **[!UICONTROL Email Daily Digest after]**.

   ![Daglig sammandrag väljer tid på dagen](assets/digest-time-stamp-my-settings-350x78.png)

   Den dagliga sammandraget innehåller händelser som uppfyller kriterierna i meddelandena 24 timmar före den valda tiden. Du får ett e-postmeddelande med en daglig sammanfattning för varje typ av meddelande.\
   Den dagliga sammandraget kan komma fram efter den tid du väljer, beroende på hur många e-postmeddelanden som står i kö för leverans i systemet. Den angivna tiden är din lokala tid enligt inställningarna i webbläsaren.

1. (Villkorligt och valfritt) Aktivera inställningen **[!UICONTROL Receive emails from this test environment]** för att ta emot e-postmeddelanden när du ändrar inställningarna för e-postmeddelanden i förhandsvisningsmiljön. E-postmeddelanden genereras inte automatiskt från förhandsvisningsmiljön.

   ![Ta emot e-postmeddelanden från sandlådan](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Klicka på **[!UICONTROL Save Changes]**.
