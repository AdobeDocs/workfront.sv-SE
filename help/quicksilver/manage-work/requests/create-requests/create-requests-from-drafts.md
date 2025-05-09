---
product-area: requests
navigation-topic: create-requests
title: Skapa begäranden från utkast
description: Förutom att använda tillgängliga utkast som Workfront föreslår när du anger en ny begäran, kan du även få åtkomst till ett utkast från sektionen Utkast och slutföra den därifrån.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Skapa begäranden från utkast

Förutom att använda tillgängliga utkast som Workfront föreslår när du anger en ny begäran, kan du även få åtkomst till ett utkast från sektionen Utkast och slutföra den därifrån.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Medarbetare eller högre</p>
   eller
   <p>Aktuell: Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav för att skapa begäranden från utkast

Du måste göra följande innan du kan skapa en begäran från ett utkast: 

* Börja skapa en begäran. Då sparas begäran som ett utkast automatiskt i avsnittet Utkast.

  Mer information om hur du skapar begäranden finns i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Skapa begäranden från utkast

{{step1-to-requests}}

1. Välj **Utkast** på den vänstra panelen.

   Ett utkast för varje köämne i varje begärandekö visas i den här listan.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Valfritt) Klicka på en kolumnrubrik om du vill sortera listan efter den kolumnen.

1. Granska informationen om varje utkast i följande kolumner i listan Utkast:

   | Ämne | Det här namnet gav du din begäran när du började skapa den. |
   |---|---|
   | Bana | Namnet på begärandekön, ämnesgrupper och köämnen där du ursprungligen tänkte skicka begäran. |
   | Anmälningsdatum | Det datum då du initierade skapandet av begäran. |
   | Senaste uppdateringsdatum | Den sista uppdateringen. Om du inte har uppdaterat det sedan du först startade begäran ska transaktionsdatumet och det senaste uppdateringsdatumet vara samma. |

   {style="table-layout:auto"}

1. (Valfritt) Använd snabbfiltret i det övre högra hörnet av listan Utkast för att börja skriva namnet på en utkast, begärandekö, köämne eller ämnesgrupp och klicka sedan på namnet på ett utkast för att öppna det.

   >[!TIP]
   >
   >Du kan inte använda permanenta filter i delen Utkast i området Förfrågningar. Det finns heller inga alternativ för att ändra eller ändra visningen av utkastlistan.

1. Uppdatera informationen för begäran enligt beskrivningen i [Skapa och skicka Adobe Workfront-begäranden](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Valfritt och villkorligt) Klicka på **Ignorera** utkast när du vill ta bort utkastet. Detta tar bort utkastet som inte kan återställas. Mer information om hur du tar bort utkast finns i [Ta bort ett utkast för en begäran](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Valfritt) Klicka på **Avbryt** i det nedre vänstra hörnet på sidan om du vill återställa åtgärden och behålla utkastet.

1. När du är klar med informationen för begäran gör du något av följande:

   * Klicka på **Skicka** om du är redo att skicka begäran. Begäran sparas i avsnittet Skickat. Beroende på hanteringsregeln för begärandekön kan den här begäran dirigeras till ett annat projekt än det som angetts som en begärandekö. Mer information om routningsregler finns i [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     eller

     Klicka på **Stäng** om du inte är redo att skicka det och du kanske kommer tillbaka och slutför det senare. Din begäran sparas i avsnittet Utkast och blir tillgänglig nästa gång du skickar en begäran för den här kön.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     När du skickar begäran tas utkastet bort och kan inte återställas.
