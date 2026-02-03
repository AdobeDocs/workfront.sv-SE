---
product-area: projects;user-management
keywords: redigera,formulär,formaterad,text,specialformat,fält,anpassad,information,anpassa,objekt
navigation-topic: work-with-custom-forms
title: Redigera information i anpassade formulärfält
description: Du kan redigera information i ett anpassat formulär när formuläret har kopplats till ett objekt. Mer information om hur du lägger till anpassade formulär till objekt finns i Lägga till ett anpassat formulär till ett objekt.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Redigera information i anpassade formulärfält

<!--Audited: 10/2025-->

Du kan redigera information i ett anpassat formulär när formuläret har kopplats till ett objekt. Mer information om hur du lägger till anpassade formulär till objekt finns i [Lägga till ett anpassat formulär till ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront package</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licens</p> </td> 
   <td> <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till objektet som du vill redigera det anpassade formuläret för</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektbehörigheter</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute eller högre behörigheter för det objekt som du vill redigera det anpassade formuläret för</p> </li> 
     <li><p>Visa behörigheter för de fält som du vill redigera.</p></li> 
     <li><p>Redigera behörigheter för de avsnitt i formuläret där fälten som du vill redigera finns</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

* Din Workfront-administratör eller en plananvändare med administrativ åtkomst till anpassade formulär måste skapa anpassade formulär i din miljö. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Du måste ha anpassade formulär kopplade till ett objekt.

  Mer information om hur du använder anpassade formulär för ett objekt finns i [Lägga till ett anpassat formulär för ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Redigera information i ett anpassat formulär

Att redigera information i ett anpassat formulär som är kopplat till ett objekt påminner om det som finns i de flesta objekt.

Mer information om vilka objekt som kan ha ett anpassat formulär finns i [Översikt över anpassade formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Gå till en lista med objekt som du vill redigera information för i det anpassade formuläret, förutom en lista med upprepningar.
1. Markera ett eller flera objekt i listan och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) längst upp i listan.
1. Klicka på **Egen Forms** i den vänstra panelen i rutan **Redigera &lt; objekt >**.

   När det finns ett anpassat formulär kopplat till objektet visas formulärets namn som ett område i avsnittet **Anpassad Forms** .
1. Börja ange information i alla fält som du har åtkomst till.

   ![Redigera ruta med anpassade formulär på faktureringsposten](assets/edit-box-with-custom-forms-on-billing-record.png)

   Om flera anpassade formulär är kopplade till objektet gör du detta för alla formulär.

   Beroende på vilken typ av fält du arbetar i kan du tänka på följande:

   * Du kan bara välja ett alternativ för alternativknappsfält.
   * Du kan välja ett eller flera alternativ i ett kryssrutefält, beroende på hur formulärskaparen konfigurerade fältet.
   * Du kan välja ett eller flera alternativ i ett flervalsfält, beroende på hur formulärskaparen konfigurerade fältet.
   * Du kan bara formatera textfält (fet, kursiv eller understruken) om användaren som skapade formuläret har ställt in dem som ett textfält med fälttypen Formatering. Det går inte att formatera textfält med en rad och textfält för stycken.
   * Du kan bara uppdatera tiden på dagen i en datumfälttyp om användaren som skapade formuläret har inkluderat den när fältet skapades.

   >[!NOTE]
   >
   >Fält som tillåter flera markeringar kan begränsa hur många alternativ du kan välja. Kryssrutor och flervalslistrutor är begränsade till 5 000 markeringar.

   Mer information om alla fälttyper finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Spara**.

   >[!IMPORTANT]
   >
   >Du måste fylla i alla obligatoriska fält i formuläret innan du kan spara formuläret. Namnet på ett obligatoriskt fält följs av en asterisk.
   >
   >![Obligatoriskt anpassat fält](assets/nwe-required-custom-field.png)

   När någon ändrar data i ett annat objekt som refereras av beräknade anpassade fält i objektet, återspeglas inte ändringarna automatiskt i objektet. Mer information om hur du uppdaterar alla beräknade anpassade fält i objektet manuellt finns i [Beräkna om alla beräknade anpassade fält för ett objekt](#recalculate-all-calculated-custom-fields-for-an-object) i den här artikeln.

   När beroende fält på sidan ändras, beräknas beräkningsfält i det anpassade formuläret dynamiskt om i realtid. Du kan se det nya beräknade fältvärdet utan att spara formuläret, men det används inte i själva verket i formuläret och objektet förrän du sparar ändringarna. Detta gäller även beräkningsfält i standardformulär och anpassade formulär.

   Du kan även uppdatera alla beräknade anpassade fält manuellt för ett objekt när du redigerar objektet gruppvis tillsammans med andra objekt i en lista. Instruktioner finns i [Beräkna om alla beräknade anpassade fält för flera objekt i en lista när du redigerar objekten](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) i den här artikeln.

1. (Villkorligt) Så här uppdaterar du anpassade fält för ett eget upprepningsformulär:

   1. Gå till en iteration.
   1. Klicka på **Egen Forms** i den vänstra panelen.
   1. Om du vill lägga till anpassade formulär börjar du skriva namnet på ett formulär i fältet **Lägg till anpassat formulär** i det övre högra hörnet på sidan

      eller

      Klicka på ikonen **Redigera** i samma område för att börja redigera fälten i de bifogade formulären.

      ![Redigera eget upprepningsformulär](assets/edit-iteration-custom-form.png)

   1. Klicka på **Spara ändringar**.

## Beräkna om anpassade fält för objekt

Beroende på ändringar som kan inträffa i anpassade formulär eller ändringar som görs i fält som refereras i anpassade fält, kan värdena för beräknade anpassade fält vara inaktuella. I det här fallet kan du behöva beräkna om anpassade fält eller beräkna om anpassade uttryck för objekt.

I följande avsnitt beskrivs hur du kan beräkna om anpassade uttryck för objekt med anpassade formulär.

>[!NOTE]
>
>Du kan inte beräkna om anpassade uttryck för grupper.

### Beräkna om alla beräknade anpassade fält från en objektsida

>[!IMPORTANT]
>
>Du måste ha ett eget formulär med beräknade fält kopplade till objektet innan du kan följa stegen i det här avsnittet.

1. Gå till huvudsidan för ett av följande objekt vars anpassade fält du vill beräkna om:

   * Projekt
   * Uppgift
   * Problem
   * Portfolio
   * Program
   * Dokument

1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-icon.png) till höger om objektets namn och klicka sedan på **Beräkna om uttryck**.

   Detta beräknar om alla anpassade fält i objektets formulär.

### Beräkna om alla beräknade anpassade fält för flera objekt i en lista när objekten redigeras {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Beroende på vilka objekt du vill beräkna om de anpassade uttrycken för kan du göra det i följande områden:

* I en lista med objekt går du till menyn Mer längst upp i listan.
* När du markerar och redigerar flera objekt samtidigt i rutan Redigera.

Så här beräknar du manuellt om anpassade fält för flera objekt genom att redigera dem i grupp från en lista eller rapport:

1. Gå till en lista med följande objekttyper vars objekt innehåller anpassade formulär med beräkningsfält:

   * Användare
   * Företag
   * Faktureringsposter

1. Markera de objekt vars beräknade anpassade fält du vill uppdatera.
1. Klicka på ikonen **Redigera**.
1. Klicka på **Anpassad Forms** på den vänstra menyn och välj sedan **Beräkna om anpassade uttryck**.
1. Klicka på **Spara** eller **Spara ändringar**.

   Workfront beräknar alla anpassade fält för alla markerade objekt.

Så här beräknar du om anpassade uttryck från en objektlista:

1. Gå till en projektlista eller rapport och välj en eller flera av följande objekttyper:

   * Projekt
   * Uppgifter
   * Problem
   * Portföljer
   * Program
   * Utgifter
1. Klicka på menyn **Mer** ![Mer](assets/more-icon.png) och klicka sedan på **Beräkna om anpassade uttryck**.

![Omberäkna uttryckets tidslinjeekonomi-listruta i projektlistor](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront beräknar omedelbart alla anpassade fält för alla valda projekt.
Alla listor med objekt har inte den här funktionen.

>[!NOTE]
>
>När du beräknar om uttryck för flera projekt, beroende på hur komplexa de är, rekommenderar vi att du inte väljer ett för stort antal projekt för att få optimala prestanda.
>
>Vissa saker som kan göra ett projekt för komplext kan vara flera beroenden, tilldelningar eller ett stort antal anpassade fält.

