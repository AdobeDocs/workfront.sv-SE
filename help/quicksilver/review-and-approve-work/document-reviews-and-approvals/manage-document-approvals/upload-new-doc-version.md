---
product-area: documents
navigation-topic: approvals
title: Överför en ny dokumentversion och begär godkännande
description: Du kan överföra en ny dokumentversion och begära godkännande från andra användare i Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 162f63d52c97c6d4894d35565c68eb2858369b53
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Överför en ny dokumentversion och begär godkännande

Om ett dokument har markerats behöver arbete i en tidigare granskning, kan du överföra en ny version till originaldokumentet och starta en ny godkännandeomgång. När du har överfört en ny version av dokumentet är de tidigare versionerna låsta.

Om den nya versionens filnamn skiljer sig från den tidigare versionens filnamn visas dokumentet med det nya filnamnet i Workfront.

När en ny version läggs till i ett dokument med enastående godkännanden visas godkännandet för den föregående versionen som Återkallat. Den föregående godkännandeprocessen avslutas, även om vissa deltagare ännu inte har fattat något beslut.

Om den senaste dokumentversionen tas bort förblir de tidigare versionerna låsta. Om du behöver redigera en tidigare version måste du låsa upp den manuellt.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Aktuell: Begäran eller senare</p>
   eller
   <p>Nytt: Medarbetare eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till objektet som är associerat med dokumentet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Lägg till en ny version genom att dra och släppa

>[!NOTE]
>
>Det går inte att dra och släppa i Internet Explorer.

1. Gå till området Dokument där dokumentet överförs.
1. Dra den nya versionen av dokumentet från skrivbordet eller en separat webbläsarflik över den befintliga versionen i Workfront.

   När du drar den nya versionen kan du hålla muspekaren över en Workfront-dokumentmapp för att öppna den. Du kan sedan rulla uppåt och nedåt genom att dra filerna till skärmens övre eller nedre del.

1. Släpp den nya versionen ovanpå den befintliga filen på fliken **Dokument**.

1. När dokumentet har överförts klickar du på det och öppnar dokumentsammanfattningspanelen.

1. Bläddra ned till avsnittet **Godkännanden** i rutan Dokumentsammanfattning och klicka sedan på **Lägg till**.

![](assets/doc-summary-add-approvers.png)

1. (Valfritt) Ange en tidsgräns för godkännandet. Användare och team meddelas via e-post 72 timmar, sedan 24 timmar före den angivna tidsgränsen.

1. Om du snabbt vill lägga till granskare och godkännare från den tidigare versionen klickar du på knappen Lägg till bredvid namnen nedan.
   <!--need screenshot when working-->

1. (Valfritt) Ändra roll från godkännare/granskare.

1. Om du vill lägga till nya godkännare och granskare klickar du på **Granskare** eller **Godkännare** och börjar skriva in användaren eller teamet.

   ![](assets/add-approver-and-deadline.png)
