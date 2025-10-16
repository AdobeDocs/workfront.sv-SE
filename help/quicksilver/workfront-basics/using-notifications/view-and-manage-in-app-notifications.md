---
navigation-topic: notifications
title: Visa och hantera meddelanden i appen
description: 'Meddelanden i appen håller dig informerad om två typer av information: meddelanden och meddelanden om arbetsobjekt. De är tillgängliga både från webbprogrammet och mobilprogrammet.'
author: Lisa
feature: Get Started with Workfront
exl-id: 4c5da114-33cc-422b-84f4-67bc7fcd67c6
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Visa och hantera meddelanden i appen

Meddelanden i appen håller dig informerad om två typer av information: meddelanden och meddelanden om arbetsobjekt. De är tillgängliga både från webbprogrammet och mobilprogrammet.

En lista över arbetsobjektet och meddelanden som du kan ta emot finns i [Översikt över meddelanden i appen](../../workfront-basics/using-notifications/in-app-notifications-overview.md).

>[!NOTE]
>
>* Meddelanden i appen för arbetsaktiviteter är inte knutna till e-postmeddelanden i [!DNL Workfront]. Mer information finns i [[!DNL Adobe Workfront] meddelanden](../../workfront-basics/using-notifications/wf-notifications.md)
>* Det går inte att anpassa meddelanden i appen.
>



## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] package</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> 
   <p>Medarbetare eller högre</p>
   <p>Begäran eller senare</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa meddelanden

Den numrerade ikonen i det övre högra hörnet av [!DNL Workfront] visar antalet meddelanden som du ännu inte har bekräftat.

>[!NOTE]
>
>Du kan visa alla meddelanden i appen både från webbprogrammet och mobilprogrammet. Endast vissa av dessa meddelanden skickas som push-meddelanden i mobilprogrammet. Mer information om meddelanden i mobilappen finns i [[!DNL Adobe Workfront] för iOS](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) och [[!DNL Adobe Workfront] för Android](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

1. Klicka på den numrerade ikonen ![Notifications (Meddelanden)](assets/notifications-icon-jewel.jpg) i det övre högra hörnet av [!DNL Workfront] för att öppna din lista över meddelanden.

   De senaste olästa meddelandena visas under den numrerade ikonen, med den senaste längst upp.

   ![Senaste olästa meddelanden](assets/qs-notifications-350x330.png)

   Numerikonen visar en rullningsbar lista med upp till 80 meddelanden. Om du vill se mer kan du klicka **[!UICONTROL All notifications]** längst ned i listan för att visa upp till 500 meddelanden. Meddelanden tas automatiskt bort efter 30 dagar.

   Längst ned i varje meddelande visas [!UICONTROL notification type] och en motsvarande identifieringsikon. De här hjälper dig att identifiera vad som hände med det angivna [!DNL Workfront]-objektet och varna dig om du har ett åtgärdsobjekt:

   * Meddelandemeddelanden indikeras av ikonen [!UICONTROL announcements]. ![Anteckningsikon](assets/announcement.png)

   * Alla andra meddelanden indikeras av ikoner som föreslår vilken typ av arbetsuppgift de är kopplade till.

     ![Meddelandeikoner](assets/ntfcntype&icon-350x330.png)
Ikonen till höger om den blå punkten visar något av följande:

   * Profilfotot för personen som skrev informationen, vanligtvis en uppdatering om ett [!DNL Workfront]-objekt som du arbetar med.
   * [!DNL Workfront]-logotypen, om meddelandet är ett systemmeddelande.


1. (Valfritt) Om du vill visa datumet när du fick ett meddelande håller du musen över indikatorn för dag eller tid i det övre högra hörnet av meddelandet.

   ![Hovra över datum](assets/hoveroverdate-350x437.png)

1. Klicka på meddelandet som du vill visa:

   * Om meddelandet som du klickar på gäller ett arbetsobjekt, öppnas det associerade [!DNL Workfront]-objektet och det fullständiga meddelandet visas på fliken **[!UICONTROL Updates]**. Du kan **[!UICONTROL Start a new update area]** eller **[!UICONTROL Type a reply]**.

     ![Uppdatera eller svara](assets/object-opens-click-work-ntfctn-qs-350x183.png)

   * Om det meddelande du klickar på är för ett meddelande ![Meddelandeikon](assets/announcement.png) visas sidan **[!UICONTROL Announcements]** med alla meddelanden. Meddelandet som du klickade på markeras till vänster och meddelandet visas till höger.

     ![Sidan Meddelanden](assets/announcements-page-qs-350x210.png)

1. (Valfritt) Hämta eventuella bilagor i meddelandet eller hämta alla bilagor som en ZIP-fil.

   ![Hämta bifogade filer](assets/download-attachments-350x106.png)

## Bekräfta meddelanden

När du har visat meddelanden kan du bekräfta dem för att ta bort dem från listan [!UICONTROL Notifications] eller låta dem svara senare.

På sidan [!UICONTROL Notifications] kan du visa aktuella och rensade meddelanden. Du kan även få tillbaka rensade meddelanden till listan [!UICONTROL Notifications].

* [Bekräfta meddelanden](#acknowledge-notifications)
* [Visa bekräftelsemeddelanden](#view-acknowledged-notifications)

### Bekräfta meddelanden

Om du klickar på den numrerade ikonen för att öppna meddelandelistan bekräftas inte automatiskt att du har läst alla meddelanden.

Så här bekräftar du ett meddelande och tar bort det från meddelandelistan:

1. Klicka på den numrerade ikonen ![Notifications (Meddelanden)](assets/notifications-icon-jewel.jpg) i det övre högra hörnet av [!DNL Workfront] för att öppna din lista över meddelanden.
1. Gör något av följande:

   * Klicka på den blå punkten i det övre vänstra hörnet av meddelandet.
   * Om meddelandet avser en arbetsuppgift (i stället för ett meddelande) klickar du på meddelandet för att gå till posten.
   * Om meddelandet gäller ett meddelande klickar du på meddelandet för att öppna sidan **[!UICONTROL Announcements]**.
   * Klicka på **[!UICONTROL All Notifications]** i det nedre högra hörnet av listan över meddelanden för att visa sidan **[!UICONTROL Notifications]** och klicka sedan på **[!UICONTROL Mark all as seen]** i det övre högra hörnet av Workfront.

### Visa bekräftelsemeddelanden

Så här visar du meddelanden som du redan har bekräftat:

1. Klicka på den numrerade ikonen ![Notifications (Meddelanden)](assets/notifications-icon-jewel.jpg) i det övre högra hörnet av [!DNL Workfront] för att öppna din lista över meddelanden.
1. Klicka på **[!UICONTROL All Notifications]** i det nedre högra hörnet i listan över meddelanden.
1. Bläddra nedåt på sidan **[!UICONTROL Notifications]** som visas för att visa dina tidigare meddelanden.
1. (Valfritt) Om du vill få tillbaka ett bekräftat meddelande till din lista över meddelanden klickar du på den blå cirkeln bredvid meddelandet.

## Ta bort ett meddelande

Du kan inte ta bort meddelanden om arbetsobjekt. [!DNL Workfront] tar bort alla meddelanden (vare sig de är lästa eller olästa) efter 30 dagar.

Du kan dock ta bort ett meddelande. Du kan även komma åt ett meddelande som du har tagit bort inom 30 dagar efter att du tagit bort det. [!DNL Workfront] tar inte bort meddelanden automatiskt.

* [Ta bort ett meddelande](#delete-an-announcement)
* [Få åtkomst till och återställ ett meddelande som du nyligen har tagit bort](#access-and-restore-an-announcement-you-deleted-recently)

### Ta bort ett meddelande

1. Klicka på den numrerade ikonen ![Notifications (Meddelanden)](assets/notifications-icon-jewel.jpg) i det övre högra hörnet av [!DNL Workfront] för att öppna din lista över meddelanden.
1. Klicka på **[!UICONTROL Announcements]** eller **[!UICONTROL View All Announcements]**.

1. På sidan **[!DNL Announcements]** som visas klickar du på meddelandet som du vill ta bort i listan till vänster och sedan på **[!UICONTROL Delete]** i det övre högra hörnet på sidan.

### Få åtkomst till och återställ ett meddelande som du nyligen har tagit bort

Du kan komma åt ett meddelande som du har tagit bort under de senaste 30 dagarna.

1. Klicka på den numrerade ikonen ![Notifications (Meddelanden)](assets/notifications-icon-jewel.jpg) i det övre högra hörnet av [!DNL Workfront] för att öppna din lista över meddelanden.
1. Klicka på **[!UICONTROL Announcements]** eller **[!UICONTROL View All Announcements]**.

1. Klicka på **[!UICONTROL Announcements]** på sidan **[!UICONTROL Deleted]** som visas.

1. Klicka på det meddelande som du vill visa.
1. (Valfritt) Om du vill återställa meddelandet klickar du på **[!UICONTROL Move to Inbox]** ovan och till höger om meddelandet.
