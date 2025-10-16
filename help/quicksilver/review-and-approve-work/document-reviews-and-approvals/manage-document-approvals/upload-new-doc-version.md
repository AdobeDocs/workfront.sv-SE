---
product-area: documents
navigation-topic: approvals
title: Överför en ny dokumentversion och begär godkännande
description: Du kan överföra en ny dokumentversion och begära godkännande från andra användare i Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Överför en ny dokumentversion och begär godkännande

Om ett dokument har markerats behöver arbete i en tidigare granskning, kan du överföra en ny version till originaldokumentet och starta en ny godkännandeomgång. När du har överfört en ny version av dokumentet är de tidigare versionerna låsta.

Om den nya versionens filnamn skiljer sig från den tidigare versionens filnamn visas dokumentet med det nya filnamnet i Workfront.

När en ny version läggs till i ett dokument med enastående godkännanden visas godkännandet för den föregående versionen som Återkallat. Den föregående godkännandeprocessen avslutas, även om vissa deltagare ännu inte har fattat något beslut.

Om den senaste dokumentversionen tas bort förblir de tidigare versionerna låsta. Om du behöver redigera en tidigare version måste du låsa upp den manuellt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> <p>Begäran eller senare</p>
   <p>Medarbetare eller högre</p>
   <p>Om du använder Frame.io-integreringen måste du ha en standardlicens för att skapa arbetsflöden för godkännande.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till objektet som är associerat med dokumentet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till en ny version genom att dra och släppa

>[!NOTE]
>
>Det går inte att dra och släppa i Internet Explorer.


Om du behöver en ny granskningsrunda och ett godkännande av ett dokument kan du skapa en ny dokumentversion i Workfront.

Du kan lägga till föregående deltagare, nya deltagare eller en blandning av båda. Du kan visa information om tidigare versioner och deltagare på sidan Dokumentinformation.

Lägga till en ny version:

1. Navigera till dokumentet i Workfront.
1. Dra och släpp den nya filen ovanpå det föregående dokumentet. En ny version skapas automatiskt.

1. När dokumentet har överförts markerar du dokumentet och klickar sedan på **Dokumentinformation**.
   ![Öppna dokumentinformationssidan](assets/open-doc-details.png)


1. Klicka på **Godkännanden** i den vänstra panelen och klicka sedan på **Lägg till**.

1. Om du vill lägga till alla tidigare deltagare klickar du på **Lägg till alla**. Du kan också lägga till nya deltagare eller ta bort tidigare deltagare efter behov.


1. Om du vill lägga till en befintlig godkännandemall klickar du på knappen Mall och börjar skriva in ett mallnamn.

   >[!TIP]
   >
   >   Användare med en standardlicens kan skapa återanvändbara godkännandemallar under Konfigurera. Mer information finns i [Skapa en godkännandemall för resurser och dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Valfritt) Ange en tidsgräns för godkännandet. Användare och team meddelas via e-post 72 timmar, sedan 24 timmar före den angivna tidsgränsen.

1. När du har lagt till alla granskare och godkännare klickar du på **Skicka begäran**. Deltagare meddelas via e-post.

   ![skicka ny version för godkännande](assets/add-previous-participants.png)


