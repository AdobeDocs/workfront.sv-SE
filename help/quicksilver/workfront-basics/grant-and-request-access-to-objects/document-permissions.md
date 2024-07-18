---
title: Dela ett dokument
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera dokument när de tilldelar åtkomstnivåer enligt Bevilja åtkomst till dokument.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Dela ett dokument

Din Adobe Workfront-administratör ger användare åtkomst att visa eller redigera dokument när de tilldelar åtkomstnivåer, enligt beskrivningen i [Bevilja åtkomst till dokument](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Den åtkomstnivå som Workfront-administratören beviljar användare ger dem möjlighet att antingen visa eller redigera dokument. Förutom detta kan andra användare även ge andra behörighet att visa eller hantera specifika dokument som de har överfört själva eller som de har tillgång till.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet. Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Användaren som överför ett dokument till Workfront har som standard behörigheten Hantera.

Mer information om hur du delar en hel dokumentmapp finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Att tänka på vid dokumentdelning

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

* Att dela ett dokument påminner om att dela andra objekt i Workfront. Mer information om hur du delar dokument i Workfront finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Du kan ge följande behörigheter till dokument:

   * Visa
   * Hantera

* Du kan också dela ett dokument offentligt eller i hela systemet.

  >[!CAUTION]
  >
  >Vi rekommenderar att du använder försiktighet när du delar objekt som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

* Du kan dela ett dokument med någon som inte har ett Workfront-konto genom att lägga till deras e-postadress i fältet Ge dokumentåtkomst till.
* När du delar ett dokument har användarna samma åtkomst till alla dokumentversioner och alla dokumentkorrektur.\
  Mer information om korrektur i Workfront finns i avsnittet [Korrektur](../../review-and-approve-work/proofing/proofing.md).

* Du kan ärva behörigheter till dokument från de objekt de är kopplade till. Din Workfront-administratör kan begränsa arvet av behörigheter för dokument på din åtkomstnivå.

  Mer information om att begränsa ärvda behörigheter i dokument finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Du kan ta bort ärvda behörigheter i dokument manuellt. Mer information finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Ett bifogat dokument ärver endast behörigheter från det objekt som det bifogades till. Om du skapar en mapp på objektet och flyttar dokumentet till mappen, ärver den mappens behörigheter. Men om du skapar en mapp i ett överordnat eller indirekt överordnat objekt och flyttar dokumentet till den mappen, ärver den inte mappens behörigheter.

## Dokumentbehörigheter

I följande tabell visas vilka behörigheter du kan ge användarna när de får visa eller hantera dokument:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Åtgärd</strong> </p> </th> 
   <th> <p><strong>Hantera</strong> </p> </th> 
   <th> <p><strong>Visa</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Skapa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera dokumentinformation</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ta bort*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ladda ned</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Utcheckning</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till godkännare</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Godkänn dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Bifoga eget formulär</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Redigera anpassade fält</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Flytta till (objekt)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Skicka till (integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Uppdateringar/kommentarer</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ladda upp ny version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ta bort version</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visa dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Förhandsgranska</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Korrektur**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Generera korrektur**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ta bort korrektur**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dela*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dela hela systemet*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dela dokument offentligt*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dela med en extern e-postadress</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Lägg till/ta bort</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Byt namn</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Länk (med integration)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Bryt länk (med integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Åtgärden &#42; delas av både dokument och dokumentmappar.

&#42;&#42; Du måste ha en separat korrekturlicens kopplad till ditt Workfront-konto för att kunna bevisa dokument. Kontakta din kontoansvarige om du vill skaffa en korrekturlicens. Mer information om korrektur i Workfront finns i [Korrektur](../../review-and-approve-work/proofing/proofing.md).
