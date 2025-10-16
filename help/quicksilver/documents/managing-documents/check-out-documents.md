---
product-area: documents
navigation-topic: manage-documents
title: Checka ut dokument
description: Du kan checka ut ett dokument för att förhindra att andra användare tar bort det eller överför en ny version av det. Endast en användare kan checka ut ett dokument åt gången. Du kan checka ut alla dokument som överförts till Adobe Workfront samt dokument som är länkade till tredjepartsleverantörer av dokument (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint eller någon annan anpassad leverantör).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# Checka ut dokument

Du kan checka ut ett dokument för att förhindra att andra användare tar bort det eller överför en ny version av det. Endast en användare kan checka ut ett dokument åt gången. Du kan checka ut alla dokument som överförts till Adobe Workfront samt dokument som är länkade till tredjepartsleverantörer av dokument (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint eller någon annan anpassad leverantör). 

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller högre</p>
   <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera åtkomst till dokumentet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åtgärder tillåts för utcheckade dokument

Användare som hanterar åtkomst till dokumentet kan göra följande:

* Redigera dokumentet (dokumentnamn, beskrivning, anpassade data)
* Flytta dokumentet
* Dela dokumentet
* Förhandsgranska dokumentet
* Ladda ned dokumentet

  >[!TIP]
  >
  > Även om en användare kan hämta ett dokument när det är utcheckat av en annan användare, rekommenderar vi att användare väntar tills dokumentet har checkats in igen innan de hämtar det. När ett dokument är utcheckat visar det ofta att det fortfarande pågår arbete med dokumentet. Väntar tills ett dokument har checkats in igen för att laddas ned ser till att användaren har den senaste versionen.

* Godkänn ett dokument eller tillämpa ett godkännande för dokumentet.
* Granska dokumentet i korrekturläsaren

  Mer information om korrektur finns i [Korrektur](../../review-and-approve-work/proofing/proofing.md)

## Checka ut ett dokument

Om du har behörighet att hantera ett dokument kan du checka ut det för att förbjuda vissa åtgärder i dokumentet. 

1. Gå till den plats där dokumentet är lagrat och markera sedan dokumentet. 

   Mer information om hur du lägger till dokument finns i [Lägga till dokument i Adobe Workfront från filsystemet](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Klicka på ikonen **Checka ut** ![Checka ut](assets/check-out-25x23.png).

1. En låsikon ![Lås-ikon](assets/lock-icon-locked-qs.png) visas till höger om dokumentnamnet. Dokumentet förblir utcheckat när du har loggat ut från Workfront.
1. Endast den användare som checkade ut dokumentet eller Workfront-administratören kan checka in dokumentet.

## Hantera utcheckade dokument

Tänk på följande när det gäller utcheckade dokument:

* Innan du kan ta bort ett objekt där ett utcheckat dokument lagras måste du checka in dokumentet igen. 
* Om Workfront-administratören tar bort en användare som har checkat ut ett dokument som de inte äger checkas dokumentet ut automatiskt i Workfront.
* Om Workfront-administratören tar bort en användare som har checkat ut ett dokument som han/hon äger och dokumentet överförs till ett objekt, förblir dokumentet utcheckat. Endast en Workfront-administratör kan checka in den igen.
* Om Workfront-administratören tar bort en användare som har checkat ut ett dokument som han/hon äger och dokumentet bara överförs i dokumentområdet (inte på ett objekt), tas dokumentet bort med användaren.

  Mer information om hur du tar bort användare finns i [Ta bort användare](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Om Workfront-administratören inaktiverar en användare förblir alla dokument som har checkats ut utcheckade. Endast en Workfront-administratör kan checka in dem igen. 

## Checka in ett dokument

Du måste checka in ett dokument igen innan du kan överföra en ny version eller ta bort den. 

Så här checkar du in ett dokument:

1. Gå till det område där dokumentet är lagrat och markera dokumentet. 

   En låsikon ![Lås-ikon](assets/lock-icon-locked-qs.png) visas till höger om dokumentnamnet.

1. Klicka på ikonen **Checka in** ![Checka in](assets/check-in-25x22.png).
