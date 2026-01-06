---
title: Dela en uppgift
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera uppgifter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till uppgifter finns i Bevilja åtkomst till uppgifter.
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# Dela en uppgift

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera uppgifter när de tilldelar åtkomstnivåer. Mer information om hur du beviljar åtkomst till aktiviteter finns i [Bevilja åtkomst till aktiviteter](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Förutom den åtkomstnivå som användarna har beviljats kan du även ge dem behörighet att visa, Contribute eller hantera specifika uppgifter som du har åtkomst till att dela.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet.


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
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du delar en uppgift

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Den som har skapat en uppgift har som standard behörigheten Hantera.
* Du kan dela uppgifter individuellt eller dela flera av dem samtidigt i grupp.\
  Att dela uppgifter är detsamma som att dela andra objekt. Mer information om objektdelning i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Du kan ge följande behörigheter till en uppgift:

   * Visa
   * Hantera
   * Contribute
* När du delar en uppgift ärver användarna som standard samma behörigheter för alla underordnade objekt som är kopplade till uppgiften. De ärver till exempel samma behörigheter för de underordnade uppgifterna, utgåvorna och dokumenten som är kopplade till uppgiften.\
  Mer information om objekthierarkin i Workfront finns i   [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Workfront-administratören kan ange om dokument ska ärva behörigheter från högre objekt på användarens åtkomstnivå. Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Du kan ta bort ärvda behörigheter från en uppgift.\
  Mer information om hur du tar bort ärvda behörigheter från objekt finns i   [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Olika sätt att dela en uppgift

Du kan dela en uppgift på följande sätt:

* Manuellt, antingen individuellt eller gruppvis.

* Automatiskt genom att göra följande:

   * Ange behörigheter för något av de överordnade objekten för uppgiften: projekt, program eller portfölj. Aktiviteter ärver behörigheter från sina överordnade objekt. Mer information om hur du visar ärvda behörigheter för objekt finns i [Visa ärvda behörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Lägg till entiteter i projektdelning på en mall som används för att skapa det projekt som aktiviteten är i. Mer information om att dela projekt från mallar finns i [Dela en mall](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Ange behörigheter för alla uppgifter i ett projekt när du redigerar projektet.  Information om hur du hanterar åtkomsten till aktiviteter i projektet baserat på en användares behörigheter till projektet finns i avsnittet [](../../manage-work/projects/manage-projects/edit-projects.md#access) i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Om du inte anger vilka aktivitetsbehörigheter du vill att användarna ska ha när de tilldelas till aktiviteterna i projektet får de som standard samma behörigheter som de har i projektet.

## Dela en uppgift

1. Navigera till uppgiften som du vill dela.

1. Klicka på **Dela** till höger om aktivitetsnamnet. Dialogrutan **Dela [aktivitetsnamn]** öppnas.

   ![Knappen Dela aktivitet](assets/share-task-button.png)

1. I fältet **Bevilja aktivitetsåtkomst till** börjar du med att skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela uppgiften med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela en uppgift med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj aktivitetens åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till aktiviteten har åtkomst till den (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa uppgiften utan en inbjudan.

1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för den här uppgiften:

   * **Visa**: Användaren kan granska och dela uppgiften.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela aktiviteten (inklusive alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till uppgiften utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för uppgiften.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. (Valfritt) Om du vill inaktivera ärvda behörigheter för aktivitetens underordnade objekt klickar du på **Inaktivera** inline med **Ärvda behörigheter**.

1. (Valfritt) Om du snabbt vill dela uppgiften med hjälp av en länk klickar du på **Kopiera länk** och vidarebefordrar den till mottagaren.

1. Klicka på **Spara**.


## Dela aktiviteter satsvis

1. Navigera till det projekt som innehåller de uppgifter du vill dela.

1. På fliken **Uppgifter** på projektsidan markerar du rutan till vänster om varje uppgift som du vill dela och klickar sedan på ikonen **Dela** ![Dela](assets/share-icon.png) längst upp på sidan. Delningen modal öppnas.

   ![Dela aktiviteter gruppvis](assets/bulk-share-tasks.png)

1. I fältet **Bevilja aktivitetsåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela aktiviteterna med och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Du kan bara dela uppgifter med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj åtkomstnivå för aktiviteterna:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till uppgifterna har åtkomst till dem (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa uppgifter utan en inbjudan.


1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för uppgifterna:

   * **Visa**: Användaren kan granska och dela aktiviteterna.
   * **Contribute**: Användaren kan göra uppdateringar, logga information, göra mindre ändringar och dela aktiviteterna (inklusive alla visningsbehörigheter).
   * **Hantera**: Användaren har fullständig åtkomst till uppgifterna utan administratörsbehörighet, som ges på åtkomstnivån (inkluderar även behörigheterna Visa och Contribute).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för aktiviteterna.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-permission-options.png)

1. Klicka på **Spara**.

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
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till föregående aktiviteter</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
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
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Redigera allmän uppgift<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Ändra aktivitetsstatus</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera aktivitetsbegränsning</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
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
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Loggtimmar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Ändra planerade datum</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Acceptera tilldelning</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Gör ett uppdrag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Bifoga eget formulär</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera anpassade fält</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Skapa en godkännandeprocess</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
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
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till/redigera utgifter</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
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
   <td>  </td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontrolleras av åtkomstnivå och behörigheter för projektet.
