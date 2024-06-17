---
product-area: setup
navigation-topic: notifications
keywords: ändra,e-post,meddelande,inställningar
title: Ändra dina egna e-postmeddelanden
description: I den här artikeln beskrivs hur du kan hantera e-postmeddelanden i din användarprofil.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: f9afe7c8f04777dd547ea1e202e7844bdfd3518e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Ändra dina egna e-postmeddelanden

<!-- Audited: 1/2024 -->

Din Adobe [!DNL Workfront] administratör konfigurerar vilka e-postmeddelanden användare får när händelser inträffar i Workfront (enligt beskrivningen i [[!UICONTROL Configure event] meddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

Gruppadministratören kan också konfigurera vilka meddelanden som ska aktiveras för dig och användarna i [!UICONTROL Home Group]. Om [!UICONTROL Home Group] är en undergrupp, du får de meddelanden som är aktiverade för den översta gruppen ovanför gruppen.

Du kan anpassa detta ytterligare genom att konfigurera vilka meddelanden du får. Du kan också välja om du vill få meddelanden när händelser inträffar eller i ett e-postmeddelande med en daglig sammanfattning.

Mer information om e-postmeddelanden finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Om du aktiverar en meddelandetyp och sedan upptäcker att du inte får meddelanden av den typen, kan det bero på att den typen inte gäller för din roll.
>* The [!DNL Workfront] administratörer eller gruppadministratörer kan inte konfigurera meddelanden för [!DNL Workfront Goals]. Om du vill ha mer information om vilka meddelanden [!DNL Workfront] administratörer kan konfigurera, se [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Mer information om hur du konfigurerar enskilda meddelanden för [!DNL Workfront Goals] fortsätta att läsa den här artikeln.
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

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa och ändra inställningarna för e-postmeddelanden

{{step1-click-profile-pic}}

1. Klicka på **[!UICONTROL More]** icon ![](assets/more-icon.png) bredvid ditt namn och klicka sedan på **[!UICONTROL Edit]**.

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
