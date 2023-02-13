---
product-area: projects
navigation-topic: use-predecessors
title: Skapa en föregående relation i uppgiftslistan
description: Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Skapa en föregående relation i uppgiftslistan

Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).

I den här artikeln beskrivs hur du skapar föregående aktiviteter i uppgiftslistan.

Du kan visa föregående aktiviteter för följande områden i Adobe Workfront:

* I uppgiftslistan i kolumnen Föregående.
* I Gantt-diagrammet
* I avsnittet Föregående aktiviteter för en beroende uppgift

Mer information finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa en föregångare

1. Gå till ett projekt.
1. Klicka **Uppgifter** i den vänstra panelen.
1. Kontrollera att den aktuella vyn visar **Föregående** kolumn.

   Om kolumnen Föregående inte visas i vyn kan du ändra till en vy som gör det eller lägga till kolumnen i vyn.

1. Välj den uppgift som du vill ange som beroende uppgift.
1. Klicka inuti **Föregående** kolumn.
1. Ange det aktivitetsnummer som du vill ange som föregångare för den valda uppgiften och tryck sedan på **Retur**.

   Föregående-ikonen blir grön när föregående aktivitet har markerats som slutförd. Detta signalerar att den beroende aktiviteten är klar för arbete.

   Mer information om de relationstyper som finns i kolumnen Föregångare finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visa föregående information

Du kan snabbt visa information om föregående i uppgiftslistan.

1. Håll markören över föregående nummer i uppgiftslistan **Föregående** kolumn.

   En ruta med information om föregående visning visas.

   ![Föregående information](assets/predecessor-details-in-task-list.png)

   Följande information visas:

   **Föregående namn:** Namnet på den föregångare som refereras. Föregångarens aktivitetsnummer inkluderas. Klicka på aktivitetsnamnet för att öppna det. I exemplet ovan är föregångaren Produktion/utförande/leverans.

   **Projektnamn:** Namnet på det projekt där föregångaren finns. Projektet identifieras som det aktuella projektet om föregående projekt tillhör samma projekt som aktiviteten, eller som ett korsprojekt om föregående projekt tillhör ett annat projekt. I ovanstående exempel är projektnamnet Digital Asset Production (Integrated) - Project. Mer information om föregående projekt finns i [Skapa föregångare mellan projekt](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Du kan expandera projektinformationen för att se projektets planerade start- och slutdatum, villkor, status, procent slutfört och ägare. För ett korsprojekt kan du sedan klicka **Se projekt** för att öppna projektet.

   **ID:** Referensnumret för det projekt där föregångaren finns.

   **Planerad start:** Det planerade startdatumet för föregående aktivitet.

   **Planerat slut:** Det planerade slutförandedatumet för föregående aktivitet.

   **Antal föregångare:** Antalet föregångare för den föregångare som refereras. I exemplet ovan har föregångaren 1.

   **Antal efterträdare:** Antalet efterföljande (eller beroende) uppgifter för föregående som refereras. I exemplet ovan har den föregående som refereras 1 efterföljande.
