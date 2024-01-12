---
product-area: projects
navigation-topic: use-predecessors
title: Skapa en föregående relation i uppgiftslistan
description: Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Skapa en föregående relation i uppgiftslistan

Du kan använda föregående aktiviteter (eller bara föregående aktiviteter) för att länka aktiviteter som är beroende av andra uppgifter som ska startas eller slutföras. Du vill till exempel inte vara värd för en part (beroende uppgift) innan du skickar ut inbjudningarna (föregående uppgift).

I den här artikeln beskrivs hur du skapar föregående aktiviteter i uppgiftslistan.

Du kan visa föregående aktiviteter för uppgifter i följande områden i Adobe Workfront:

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
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard </p><p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för aktiviteterna och projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Skapa en föregående

1. Gå till ett projekt.
1. Klicka **Uppgifter** till vänster.
1. Kontrollera att den aktuella vyn visar **Föregående** kolumn.

   Om kolumnen Föregående inte visas i vyn kan du ändra till en vy som gör det eller lägga till kolumnen i vyn.

1. Välj den uppgift som du vill ange som beroende uppgift.
1. Klicka inuti **Föregående** kolumn.
1. Ange det aktivitetsnummer som du vill ange som föregångare för den valda uppgiften och tryck sedan på **Retur**.

   >[!TIP]
   >
   >Så här lägger du till en föregångare för flera projekt:
   >
   >1. Klicka på **Planläge** ikon och välj **Spara automatiskt**.
   >
   >1. Skriv in referensnumret för föregående projekts projekt följt av kolon och uppgiftens nummer. Skriv till exempel: 765021:12. Detta anger att referensnumret för föregående projekt är 765021 och föregående är uppgiftsnummer 12 i projektet.
   >
   >1. Lägg till beroendetypen för den här föregångaren. Mer information finns i [Skapa föregångare mellan projekt](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Tryck **Retur**.
   >
   >**VIKTIGT**
   >
   >Du kan inte lägga till föregångare för flera projekt när uppgiftslistan visas i läget Manuell sparning.

   Föregående-ikonen blir grön när föregående aktivitet har markerats som slutförd. Detta signalerar att den beroende aktiviteten är klar för arbete.

   Mer information om de relationstyper som finns i kolumnen Föregångare finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Visa föregående information

Du kan snabbt visa information om föregående i uppgiftslistan.

1. Håll markören över föregående nummer i uppgiftslistan **Föregående** kolumn.

   En ruta med information om föregående visning visas.

   ![Föregående information](assets/predecessor-details-in-task-list.png)

   Följande information visas:

   **Föregående namn:** Namnet på den föregångare som refereras. Föregångarens aktivitetsnummer inkluderas. Klicka på aktivitetsnamnet för att öppna det. I exemplet ovan är föregångaren Produktion/Körning/Leverans.

   **Projektnamn:** Namnet på det projekt där föregångaren finns. Projektet identifieras som det aktuella projektet om föregående projekt tillhör samma projekt som aktiviteten, eller som ett korsprojekt om föregående projekt tillhör ett annat projekt. I ovanstående exempel är projektnamnet Digital Asset Production (Integrated) - Project. Mer information om föregående projekt finns i [Skapa föregångare mellan projekt](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Du kan expandera projektinformationen för att se projektets planerade start- och slutdatum, villkor, status, procent slutfört och ägare. För ett korsprojekt kan du sedan klicka **Se projekt** för att öppna projektet.

   **ID:** Referensnumret för det projekt där föregångaren finns.

   **Planerad start:** Det planerade startdatumet för föregående aktivitet.

   **Planerat slut:** Det planerade slutförandedatumet för föregående aktivitet.

   **Antal föregående:** Antalet föregångare för den föregångare som refereras. I exemplet ovan har föregångaren 1.

   **Antal efterföljande:** Antalet efterföljande (eller beroende) uppgifter för föregående som refereras. I exemplet ovan har den föregående som refereras 1 efterföljande.
