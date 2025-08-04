---
product-area: projects
navigation-topic: use-predecessors
title: Skapa en föregående relation i uppgiftslistan
description: Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Skapa en föregående relation i uppgiftslistan

<!-- Audited: 5/2025 -->

Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).

I den här artikeln beskrivs hur du skapar föregående aktiviteter i uppgiftslistan.

Du kan visa föregående aktiviteter för uppgifter i följande områden i Adobe Workfront:

* I uppgiftslistan i kolumnen Föregående.
* I Gantt-diagrammet.
* I avsnittet Föregående aktiviteter för en beroende uppgift.

Mer information finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard </p><p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en föregående

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på **Åtgärder** i den vänstra panelen.
1. I listrutan **Vyer** väljer du en vy som visar kolumnen **Föregående** eller lägger till kolumnen i den aktuella vyn.

1. Välj den uppgift som du vill ange som beroende uppgift.
1. Klicka inuti aktivitetens **Föregående**-kolumn.
1. Skriv in det aktivitetsnummer som du vill ange som föregångare för den markerade aktiviteten och tryck sedan på **Retur**.

   >[!TIP]
   >
   >Så här lägger du till en föregångare för flera projekt:
   >
   >1. Klicka på ikonen **Planeringsläge** och välj **Spara automatiskt**.
   >
   >1. Skriv in referensnumret för föregående projekt följt av kolon och uppgiftens nummer. Om du t.ex. skriver *765021:12* anger det att referensnumret för föregående projekts projekt är 765021 och föregångaren är aktivitetsnummer 12 i projektet.
   >
   >1. Lägg till beroendetypen för den här föregångaren. Mer information finns i [Skapa föregående projekt mellan projekt](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >1. Tryck på **Retur**.
   >
   >**VIKTIGT**
   >
   >Du kan inte lägga till en föregångare för flera projekt när uppgiftslistan visas i manuellt sparläge.

   Föregående-ikonen blir grön när föregående aktivitet har markerats som slutförd. Detta signalerar att den beroende aktiviteten är klar för arbete.

   Mer information om de relationstyper som finns i kolumnen Föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visa föregående information

Du kan snabbt visa information om föregående i uppgiftslistan.

1. Håll markören över föregående nummer i kolumnen **Föregående** i uppgiftslistan. En ruta med information om föregångaren visas.

   ![Föregående information](assets/predecessor-details-in-task-list.png)

   Följande information visas:

   **Föregående namn:** Namnet på den föregångare som refereras. Föregångarens aktivitetsnummer inkluderas. Klicka på aktivitetsnamnet för att öppna det.

   **Projektnamn:** Namnet på det projekt där föregångaren finns. Projektet identifieras som det aktuella projektet om föregående projekt tillhör samma projekt som aktiviteten, eller som ett korsprojekt om föregående projekt tillhör ett annat projekt. Mer information om föregående projekt finns i [Skapa föregångare mellan projekt](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Du kan expandera projektinformationen för att se projektets planerade start- och slutdatum, villkor, status, procent slutfört och ägare. För ett korsprojekt kan du sedan klicka på **Se projekt** för att öppna projektet.

   **ID:** Referensnumret för det projekt där föregångaren finns.

   **Planerad start:** Det planerade startdatumet för föregående aktivitet.

   **Planerat slut:** Det planerade slutförandedatumet för föregående aktivitet.

   **Antal föregångare:** Antalet föregångare för den föregångare som refereras.

   **Antal efterföljande:** Antalet efterföljande (eller beroende) aktiviteter för föregående som refereras.
