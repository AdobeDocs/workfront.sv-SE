---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa ämnesgrupper
description: Ämnesgrupper är associerade med frågeköer. De gör att du kan placera dina begärandeköer i flera kategorier, beroende på vilken typ av begäran det är.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 46c86c1a5e4bb5379409c46669a348ddb53e260b
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Skapa ämnesgrupper

<!-- Audited: 2/2024 -->

Ämnesgrupper är associerade med frågeköer. Du kan placera dina frågeköer i flera kategorier, beroende på vilken typ av begäranden det gäller, genom att använda ämnesgrupper.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-licens</p> </td> 
   <td>   
      <p>Nytt: Standard</p>
      <p>eller</p> 
      <p>Aktuell: Planera</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter för projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över ämnesgrupper

Om du till exempel har en frågekö för marknadsföringsförfrågningar kan du ha en ämnesgrupp för&quot;Mors Day Campaign&quot;, med en ämnesgrupp på andra nivån&quot;Digital Media&quot; och ytterligare en ämnesgrupp för&quot;Print Media&quot;. Sedan kan du ha flera köämnen i varje ämnesgrupp. Exempel: &quot;Banner Ad&quot; och &quot;Blog&quot; kan vara köämnen för ämnesgruppen &quot;Digital Media&quot;.

Mer information om hur du skapar frågeköer finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Tänk på följande när du arbetar med ämnesgrupper:

* Du kan skapa upp till 10 nivåer med ämnesgrupper i en begärandekö.
* Det finns ingen gräns för hur många köämnen som kan kopplas till en ämnesgrupp.
* Ämnesgrupper är ett objekt som kan rapporteras.
* Du kan inte flytta ämnesgrupper från ett projekt till ett annat.

## Skapa ämnesgrupper

Vi rekommenderar att du skapar ämnesgrupper innan du skapar ett köämne. En ämnesgrupp kan dock skapas i köämnesbyggaren. Mer information om hur du skapar köämnen finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Så här skapar du en ämnesgrupp:

1. Gå till projektet som du publicerade som en kö för hjälpbegäran.\
   Mer information om hur du publicerar ett projekt som en kö för hjälpbegäranden finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicka på **Ämnesgrupper** i den vänstra panelen. Du kan behöva klicka på **Visa fler** och sedan på **Ämnesgrupper**.
1. Klicka på **Ny ämnesgrupp**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Ange följande information:

   * **Namn**: Namnet visas för användare som skickar begäranden till den här begärandekön.
   * **Beskrivning**: Beskrivningen visas när användare väljer ämnesgruppen när en ny begäran skickas.
   * **Lägg till i ämnesgrupp**: Du kan lägga till den nya ämnesgruppen i en befintlig ämnesgrupp eller lägga till den direkt i projektet som publicerats som en kö för hjälpbegäran.

1. Klicka på **Spara**.\
   Detta skapar en ny ämnesgrupp i din begärandekö. Nu kan du välja ytterligare kategorier från den första listrutan under en frågekö.\
   Mer information om hur du skickar begäranden finns i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).
