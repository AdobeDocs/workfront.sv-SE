---
product-area: requests
navigation-topic: create-requests
title: Skapa begäranden från utkast
description: Förutom att använda tillgängliga utkast som Workfront föreslår när du anger en ny begäran, kan du även få åtkomst till ett utkast från sektionen Utkast och slutföra den därifrån.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 345f63fc78d9bc2b2eff8f19a8a9196641567764
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Skapa begäranden från utkast

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>

Förutom att använda tillgängliga utkast som Workfront föreslår när du anger en ny begäran, kan du även få åtkomst till ett utkast från sektionen Utkast och slutföra den därifrån.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Krav för att skapa begäranden från utkast

Du måste göra följande innan du kan skapa en begäran från ett utkast: 

* Börja skapa en begäran. Då sparas begäran som ett utkast automatiskt i avsnittet Utkast.

   Mer information om hur du skapar begäranden finns i [Skapa och skicka Adobe Workfront-förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Skapa begäranden från utkast

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront.
1. Klicka **Begäranden** > **Utkast**.

   Ett utkast för varje köämne i varje begärandekö visas i den här listan.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. <span class="preview">(Valfritt) Klicka på en kolumnrubrik om du vill sortera listan efter den kolumnen.</span>

1. Granska informationen om varje utkast i följande kolumner i listan Utkast:

   | Ämne | Det här namnet gav du din begäran när du började skapa den. |
   |---|---|
   | Bana | Namnet på begärandekön, ämnesgrupper och köämnen där du ursprungligen tänkte skicka begäran. |
   | Anmälningsdatum | Det datum då du initierade skapandet av begäran. |
   | Senaste uppdateringsdatum | Den sista uppdateringen. Om du inte har uppdaterat det sedan du först startade begäran ska transaktionsdatumet och det senaste uppdateringsdatumet vara samma. |

   {style="table-layout:auto"}

1. <span class="preview">(Valfritt) Använd snabbfiltret i det övre högra hörnet av listan Utkast för att börja skriva namnet på en utkast, begärandekö, köämne eller ämnesgrupp och klicka sedan på namnet på ett utkast för att öppna det. </span>
1. Uppdatera informationen för begäran enligt beskrivningen i [Skapa och skicka Adobe Workfront-förfrågningar](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Valfritt och villkorligt) När som helst när du anger en begäran klickar du på **Ignorera** utkast om du vill ta bort utkastet. Detta tar bort utkastet som inte kan återställas. Mer information om hur du tar bort utkast finns i [Ta bort ett begärandeutkast](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Valfritt) Klicka på **Avbryt** i det nedre vänstra hörnet av sidan om du vill återställa åtgärden och behålla utkastet.

1. När du är klar med informationen för begäran gör du något av följande:

   * Klicka **Skicka** om du är redo att skicka begäran. Begäran sparas i avsnittet Skickat. Beroende på hanteringsregeln för begärandekön kan den här begäran dirigeras till ett annat projekt än det som angetts som en begärandekö. Mer information om routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      eller

      Klicka **Stäng** om du inte är redo att skicka in den och du kanske kommer tillbaka och slutför den senare. Din begäran sparas i avsnittet Utkast och blir tillgänglig nästa gång du skickar en begäran för den här kön.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

      När du skickar begäran tas utkastet bort och kan inte återställas.
