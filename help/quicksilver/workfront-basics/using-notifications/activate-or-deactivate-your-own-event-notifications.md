---
product-area: setup
navigation-topic: notifications
title: Aktivera eller inaktivera egna händelsemeddelanden
description: Din Adobe Workfront-administratör konfigurerar vilka händelsemeddelanden användare får när händelser inträffar i Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Aktivera eller inaktivera egna händelsemeddelanden

Din Adobe [!DNL Workfront] administratör konfigurerar vilka händelsemeddelanden som användare får när händelser inträffar i Workfront (enligt beskrivningen i [[!UICONTROL Configure event] meddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

Gruppadministratören kan också konfigurera vilka händelsemeddelanden som ska aktiveras för dig och användarna i hemgruppen. Om [!UICONTROL Home Group] är en undergrupp, du får händelseaviseringar aktiverade för den översta gruppen ovanför gruppen.

Du kan anpassa detta ytterligare genom att konfigurera vilka meddelanden du får. Du kan också välja om du vill få meddelanden när händelser inträffar eller i ett e-postmeddelande med en daglig sammanfattning.

Mer information om e-postmeddelanden finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Om du aktiverar en meddelandetyp och sedan upptäcker att du inte får meddelanden av den typen, kan det bero på att den typen inte gäller för din roll.
>* The [!DNL Workfront] administratör eller gruppadministratör kan inte konfigurera meddelanden för [!DNL Workfront Goals]. Om du vill ha mer information om vilka meddelanden [!DNL Workfront] administratörer kan konfigurera, se [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Mer information om hur du konfigurerar enskilda meddelanden för [!DNL Workfront Goals] fortsätta att läsa den här artikeln.
>


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
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill ta reda på vilken plan eller licenstyp du har kontaktar du [!DNL Workfront] administratör.

## Visa och ändra inställningarna för e-postmeddelanden

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]klickar du sedan på ditt användarnamn bredvid din profilbild.

1. Klicka på **[!UICONTROL More]** icon ![](assets/more-icon.png) och sedan klicka **[!UICONTROL Edit]**.

1. I **[!UICONTROL Edit Person]** går du till **[!UICONTROL Notifications]** -avsnitt.

1. Klicka på en kategori om du vill visa meddelandeinställningarna för den kategorin.

   ![](assets/my-profile-notifications.png)

1. Markera eller avmarkera kryssrutorna till höger för att ange om du vill få meddelanden varje dag, direkt eller båda.

   Du kan också använda kryssrutorna för en kategori för att aktivera eller inaktivera alla meddelanden i den kategorin.

   >[!NOTE]
   >
   >Om du är teammedlem i ett projekt får du även fortsättningsvis e-postmeddelanden om projektet tills du tas bort från teamet, även om du inte längre har tillgång till projektet. Instruktioner om hur du tar bort användare från ett team finns i [Ta bort användare från projekt](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   För **[!UICONTROL Communication]** kan du välja enskilda meddelanden för direktleverans. Om du vill få meddelanden levererade i en daglig sammanfattning måste du markera alla.

   Om alla e-postmeddelanden för en viss kategori är aktiverade visas rutan i kategorititeln som markerad. Om alla e-postmeddelanden i en viss kategori inaktiveras, avmarkeras rutan. Om vissa meddelanden aktiveras och andra inaktiveras visas kategorikryssrutan som en rak linje.\
   När du ändrar en meddelandeinställning visas etiketten **[!UICONTROL Edited]** visas för den meddelandeinställningen så att du ser att meddelandeinställningen har ändrats.

1. Om du har valt att skicka meddelanden som dagliga sammandrag, markerar du den tid på dagen som du vill ha den överst i **[!UICONTROL Notifications]** i **[!UICONTROL Email Daily Digest after]** -menyn.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   Den dagliga sammandraget innehåller händelser som uppfyller kriterierna i meddelandena 24 timmar före den valda tiden. Du får ett e-postmeddelande med en daglig sammanfattning för varje typ av meddelande.\
   Den dagliga sammandraget kan komma fram efter den tid du väljer, beroende på hur många e-postmeddelanden som står i kö för leverans i systemet. Den angivna tiden är din lokala tid enligt inställningarna i webbläsaren.

1. (Villkorligt och valfritt) Aktivera alternativet **[!UICONTROL Receive emails from this test environment]** inställning för att ta emot e-post. E-postmeddelanden genereras inte automatiskt från förhandsvisningsmiljön.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Klicka på **[!UICONTROL Save Changes]**.
