---
title: Dela ett dokument
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera dokument när de tilldelar åtkomstnivåer enligt Bevilja åtkomst till dokument.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Dela ett dokument

Din Adobe Workfront-administratör ger användare åtkomst att visa eller redigera dokument när de tilldelar åtkomstnivåer, enligt beskrivningen i [Bevilja åtkomst till dokument](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Den åtkomstnivå som Workfront-administratören beviljar användare ger dem möjlighet att antingen visa eller redigera dokument. Förutom detta kan andra användare även ge andra behörighet att visa eller hantera specifika dokument som de har överfört själva eller som de har tillgång till.

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet. Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Användaren som överför ett dokument till Workfront har som standard behörigheten Hantera.

Mer information om hur du delar en hel dokumentmapp finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna dela objekt:

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
   <td> <p>Nytt: Standard</p> 
   eller
   <p>Aktuell: Arbete eller högre</p>
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

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

## Dela ett dokument

{{step1-to-documents}}

1. På sidan **Dokument** för du muspekaren över dokumentet som du vill dela och klickar på länken **Dokumentinformation** som visas. Sidan **Dokumentinformation** öppnas.

   ![Länk för dokumentinformation](assets/document-details-link.png)

1. Klicka på ikonen **Mer** ![Mer ](assets/more-icon.png) till höger om dokumentnamnet och klicka sedan på **Dela**. Dialogrutan **Dela [dokumentnamn]** öppnas.

   ![Dela ett dokument](assets/share-a-document-350x160.png)

1. I fältet **Bevilja dokumentåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela dokumentet med och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Du kan bara dela ett dokument med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj dokumentets åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till dokumentet har åtkomst till det (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa dokumentet utan en inbjudan.

1. (Valfritt) Om du vill göra dokumentet offentligt klickar du på kugghjulsikonen ![Välj kugghjulsikonen](assets/gear-icon.png) och klickar sedan på rutan i linje med **Gör den offentlig för externa användare**. Knappen **Kopiera offentlig länk** visas längst ned i dialogrutan.

1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för det här dokumentet:

   * **Visa**: Användaren kan granska och dela dokumentet.
   * **Hantera**: Användaren har fullständig åtkomst till programmet utan administratörsbehörighet, som ges på åtkomstnivån (inklusive alla visningsbehörigheter).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för programmet.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-options-icon.png)

1. (Valfritt) Om du vill inaktivera ärvda behörigheter för dokumentets underordnade objekt klickar du på **Inaktivera** i linje med **Ärvda behörigheter**.

1. (Villkorligt) Om du vill kopiera den offentliga länken som gör att du kan dela dokumentet med externa användare klickar du på **Kopiera offentlig länk**.

   >[!CAUTION]
   >
   >Du bör vara försiktig när du delar dokument som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

1. Klicka på **Spara**.


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
