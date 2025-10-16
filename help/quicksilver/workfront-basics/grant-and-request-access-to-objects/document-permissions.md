---
title: Dela ett dokument
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Din Adobe Workfront-administratör ger användarna åtkomst till att visa eller redigera dokument när de tilldelar åtkomstnivåer enligt Bevilja åtkomst till dokument.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Dela ett dokument

Workfront-administratören styr vilka som kan visa eller redigera dokument i området Åtkomstnivåer i installationsprogrammet. Mer information finns i [Bevilja åtkomst till dokument](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Användarna kan också dela dokument som de har överfört eller har åtkomst till, vilket ger andra behörighet att visa eller hantera dem.

* Behörigheter gäller för enskilda objekt och definierar vilka åtgärder någon kan vidta.
* Den person som överför ett dokument får automatiskt full kontroll (Hantera behörigheter).
* Mer information om hur du delar en hel mapp finns i [Dela en dokumentmapp](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

>[!NOTE]
>
>Om din Workfront-instans använder Adobe Enterprise Storage kan du inte dela enskilda dokument. Istället får du åtkomst på projektnivå. Tänk på att delning av projektet kan ge åtkomst till känslig projektinformation, t.ex. finansiella data, beroende på vilken behörighetsnivå du väljer.



## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
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



## Dela ett dokument

Användaren som överför ett dokument till Workfront har som standard behörigheten Hantera.

{{step1-to-documents}}

1. På sidan **Dokument** för du muspekaren över dokumentet som du vill dela och klickar på länken **Dokumentinformation** som visas. Sidan **Dokumentinformation** öppnas.

   ![Länk för dokumentinformation](assets/document-details-link.png)

1. Klicka på ikonen **Mer** ![Mer &#x200B;](assets/more-icon.png) till höger om dokumentnamnet och klicka sedan på **Dela**. Dialogrutan **Dela [dokumentnamn]** öppnas.

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
   * **Hantera**: Användaren har fullständig åtkomst till dokumentet utan administratörsbehörighet, som ges på åtkomstnivån (inklusive alla visningsbehörigheter).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter i dokumentet.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-options-icon.png)

1. (Valfritt) Om du vill inaktivera ärvda behörigheter för dokumentets underordnade objekt klickar du på **Inaktivera** inline med **Ärvda behörigheter**.

1. (Villkorligt) Om du vill kopiera den offentliga länken som gör att du kan dela dokumentet med externa användare klickar du på **Kopiera offentlig länk**.

   >[!CAUTION]
   >
   >Du bör vara försiktig när du delar dokument som innehåller konfidentiell information med externa användare. På så sätt kan de visa information utan att vara Workfront-användare eller del av organisationen.

1. Klicka på **Spara**.

## Dela flera dokument samtidigt

{{step1-to-documents}}

1. På fliken **Alla dokument** på sidan **Dokument** håller du ned **Kommando** (Mac) eller **Ctrl** (Windows) på tangentbordet och klickar sedan på de dokument du vill dela.

1. Klicka på ikonen **Dela** ![Dela](assets/share-icon.png) överst på sidan. Delningen modal öppnas.

   ![Ikonen Dela](assets/share-documents-in-bulk.png)

1. I fältet **Bevilja dokumentåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela dokumenten med och klickar sedan på namnet när det visas i listrutan.

   >[!TIP]
   >
   >Du kan bara dela dokument med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj dokumentets åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till dokumenten har åtkomst till det (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa dokumenten utan en inbjudan.

1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för dokumenten:

   * **Visa**: Användaren kan granska och dela dokumenten.
   * **Hantera**: Användaren har fullständig åtkomst till dokumenten utan administratörsbehörighet, som ges på åtkomstnivån (inklusive alla visningsbehörigheter).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för dokumenten.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-options-icon.png)

1. Klicka på **Spara**.

## Dokumentdelning med Adobe Enterprise-lagring

Workfront går över till Adobe lagringslösning för företag för att kunna erbjuda bättre anslutningsmöjligheter med Adobe Creative Cloud-produkter. Befintliga kunder kommer att flyttas till den nya modellen stegvis. Mer information om fördelarna med Adobe Enterprise-lagring finns på [Adobe Enterprise-lagringsöversikt](/help/quicksilver/review-and-approve-work/esm-overview.md).

Om din Workfront-instans använder Adobe Enterprise-lagring kan du inte dela enskilda dokument direkt. Du måste i stället bevilja åtkomst på projektnivå.

>[!IMPORTANT]
>
>Om du delar ett projekt kan användarna även få tillgång till känslig projektinformation, t.ex. ekonomisk information, beroende på vilken behörighetsnivå du väljer.
>
>Granska behörighetsinställningarna noga innan du delar dem.

## Dokumentbehörigheter

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder man kan vidta för det objektet. Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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