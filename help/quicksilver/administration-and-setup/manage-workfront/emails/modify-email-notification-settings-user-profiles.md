---
user-type: administrator
product-area: system-administration
keywords: ändra,e-post,meddelande,inställningar,massredigera,konfigurera,flera,användare
navigation-topic: emails-administration
title: Ändra inställningar för e-postmeddelanden i användarnas profiler
description: Om du är Adobe Workfront-administratör eller har en åtkomstnivå för Planering som gör att du kan redigera andra användares inställningar, kan du konfigurera meddelandeinställningarna för flera användare samtidigt. Detta inkluderar att ange om användare ska få meddelanden när händelser inträffar eller i ett dagligt e-postmeddelande med sammandrag, vilket beskrivs i Adobe Workfront-meddelanden. Mer information om åtkomstnivån som behövs för att redigera användare finns i Bevilja åtkomst till användare.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Ändra inställningar för e-postmeddelanden i användarnas profiler

Om du är Adobe Workfront-administratör eller har en åtkomstnivå för Planering som gör att du kan redigera andra användares inställningar, kan du konfigurera meddelandeinställningarna för flera användare samtidigt. Detta inkluderar att ange om användare ska få meddelanden när händelser inträffar, eller i ett e-postmeddelande med dagliga sammandrag enligt beskrivningen i [Adobe Workfront-meddelanden](../../../workfront-basics/using-notifications/wf-notifications.md). Mer information om åtkomstnivån som behövs för att redigera användare finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

När du konfigurerar meddelandeinställningar gruppvis kan du bara ändra de inställningar som de markerade användarna har gemensamt.

Du kan också konfigurera e-postmeddelanden för en användare i taget. Mer information finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan eller licenstyp du har.

## Ändra e-postmeddelandeinställningarna för flera användare samtidigt

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png). Markera användarna och klicka sedan på **Redigera**.
1. I **Redigera person** visas klickar du på **Meddelanden**.

1. Expandera en kategori om du vill visa meddelandeinställningar för den kategorin.

   Om minst en användare har valts där meddelandena inte matchar meddelandena från de andra valda användarna, innehåller kategorikryssrutan för meddelandet en vågrät rad ![](assets/straight-line-instead-of-checkmark.jpg) i stället för en bock.

1. Klicka på de meddelanden som du vill att användarna ska få dagligen eller omedelbart, eller rensa de meddelanden som du vill att de ska sluta ta emot.

   För **Kommunikation** kan du välja enskilda meddelanden för direktleverans. Du måste välja alla meddelanden som ska levereras i en daglig sammandrag.

   När du ändrar en meddelandeinställning visas etiketten **Redigerad** visas för den meddelandeinställningen så att du ser att meddelandeinställningen har ändrats.

1. Om du valde att meddelanden skulle skickas som en daglig sammanfattning, markerar du den tid på dagen som du vill att sammanfattningen ska levereras överst i dialogrutan **Meddelanden** i **E-posta daglig sammandrag efter** -menyn.

   När du har valt en leveranstid visas **E-posta daglig sammandrag efter** visas med en orange ram som anger att leveranstiden har redigerats.

   Den dagliga sammandraget innehåller händelser som uppfyller kriterierna i meddelandena 24 timmar före den valda tiden. Användarna får ett e-postmeddelande med dagliga sammandrag för varje meddelandetyp.

   Den dagliga sammandraget kan komma fram efter den tid du väljer, beroende på hur många e-postmeddelanden som står i kö för leverans i systemet. Den angivna tiden är din lokala tid enligt inställningarna i webbläsaren.
