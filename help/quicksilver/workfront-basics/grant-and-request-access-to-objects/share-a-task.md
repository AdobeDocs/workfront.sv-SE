---
title: Dela en uppgift
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera uppgifter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till uppgifter finns i Bevilja åtkomst till uppgifter.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Dela en uppgift

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera uppgifter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till aktiviteter finns i [Bevilja åtkomst till aktiviteter](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Förutom den åtkomstnivå som användare har beviljats kan du även ge dem behörighet att visa, Contribute eller Hantera specifika uppgifter som du har åtkomst till att dela.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.

## Att tänka på när du delar en uppgift

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Den som har skapat en uppgift har som standard behörigheten Hantera.
* Du kan dela uppgifter individuellt eller dela flera av dem samtidigt i grupp.\
  Att dela uppgifter är detsamma som att dela andra objekt. Mer information om objektdelning i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Du kan ge följande behörigheter till en uppgift: 

   * Visa
   * Hantera
   * Contribute\
     ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* När du delar en uppgift ärver användarna som standard samma behörigheter för alla underordnade objekt som är kopplade till uppgiften. De ärver till exempel samma behörigheter för de underordnade uppgifterna, utgåvorna och dokumenten som är kopplade till uppgiften.\
  Mer information om objekthierarkin i Workfront finns i  [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Workfront-administratören kan ange om dokument ska ärva behörigheter från högre objekt på användarens åtkomstnivå. Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Du kan ta bort ärvda behörigheter från en uppgift.\
  Mer information om hur du tar bort ärvda behörigheter från objekt finns i  [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Olika sätt att dela en uppgift

Du kan dela en uppgift på följande sätt:

* Manuellt, antingen individuellt eller gruppvis. Att dela uppgifter manuellt påminner om att dela andra objekt i Workfront.

  Mer information om hur du delar objekt i Workfront finns i  [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automatiskt genom att göra följande:

   * Ange behörigheter för något av de överordnade objekten för uppgiften: projekt, program eller portfölj. Aktiviteter ärver behörigheter från sina överordnade objekt. Mer information om hur du visar ärvda behörigheter för objekt finns i [Visa ärvda behörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Lägg till entiteter i projektdelning på en mall som används för att skapa det projekt som aktiviteten är i. Mer information om att dela projekt från mallar finns i [Dela en mall](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Ange behörigheter för alla uppgifter i ett projekt när du redigerar projektet. Information om hur du hanterar åtkomsten till aktiviteter i projektet baserat på en användares behörigheter till projektet finns i avsnittet [](../../manage-work/projects/manage-projects/edit-projects.md#access) i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Om du inte anger vilka aktivitetsbehörigheter du vill att användare ska ha när de tilldelas till aktiviteterna i projektet får de som standard samma behörigheter som de har i projektet.

## Uppgiftsbehörigheter

I följande tabell visas vilka behörigheter du kan ge användare när de får visa, Contribute eller hantera en uppgift:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Åtgärd</strong> </th> 
   <th><strong>Hantera</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>Visa</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Lägg till uppgift(er)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till föregående aktiviteter</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ta bort uppgift</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Redigera allmän uppgift<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ändra aktivitetsstatus</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera aktivitetsbegränsning</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visa uppgift</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Kopiera uppgift*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Flytta aktivitet*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Loggtimmar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ändra planerade datum</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Acceptera tilldelning</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Gör ett uppdrag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Bifoga eget formulär</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera anpassade fält</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Skapa en godkännandeprocess</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Godkänn en uppgift</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera ekonomi*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till/redigera utgifter</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visa ekonomi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Uppdateringar/kommentarer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dela</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dela hela systemet</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontrolleras av åtkomstnivå och behörigheter för projektet.
