---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Hantera anpassade formulär som är kopplade till objekt
description: Du kan uppdatera den ordning i vilken anpassade formulär som är kopplade till ett objekt visas, tas bort eller gruppredigera hur anpassade formulär visas på flera objekt.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 0%

---

# Hantera anpassade formulär som är kopplade till objekt

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Du kan uppdatera den ordning i vilken anpassade formulär som är kopplade till ett objekt visas, tas bort eller gruppredigera hur anpassade formulär visas på flera objekt.

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
   <td><p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till de objekt som du hanterar anpassade formulär för</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre till objekt som du hanterar anpassade formulär för</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the objects for which you manage custom forms</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

* Din Workfront-administratör eller en plananvändare med administrativ åtkomst till anpassade formulär måste skapa anpassade formulär i din miljö. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Du måste ha anpassade formulär kopplade till ett objekt.

  Mer information om hur du använder anpassade formulär för ett objekt finns i [Lägga till ett anpassat formulär för ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Ändra ordning på flera anpassade formulär som är kopplade till ett objekt {#reorder-multiple-custom-forms-attached-to-an-object}

1. Gå till objektet där du vill ändra ordningen på de tillagda anpassade formulären och börja sedan redigera objektet.

   **Exempel:** Om du till exempel vill hantera de anpassade formulären för ett projekt går du till projektet, klickar på menyn **Mer** ![Mer](assets/more-icon.png) och sedan på **Redigera** .

1. Klicka på ikonen **Flytta** bredvid namnet på ett anpassat formulär i avsnittet ![Anpassad Forms](assets/move-icon---dots.png) för projekt, uppgifter och utgåvor. För alla andra objekt klickar du på **Hantera Forms**. Det här alternativet visas bara om minst ett anpassat formulär är kopplat till objektet.
1. Dra ett formulär ![Flytta ikon](assets/move-icon---dots.png) till en ny plats i listan.
1. Klicka på **Spara** för projekt, uppgifter och utgåvor av anpassade formulär.

   För alla andra objekt klickar du på **Jag har slutat hantera** > **Spara ändringar**.

## Ta bort ett anpassat formulär från ett objekt {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>När du tar bort ett anpassat formulär från ett objekt, försvinner all information som hämtats i de anpassade fälten i formuläret och kan inte återställas.

1. Gå till objektet där du vill ta bort det anpassade formuläret och klicka sedan på avsnittet **Detaljer** i den vänstra panelen för objektet.

   Gå till exempel till ett projekt och klicka på avsnittet **Projektinformation**.

1. Klicka på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) i det övre högra hörnet på objektets sida och klicka sedan på **Redigera alla**.
1. Klicka på ikonen **Ta bort** ![Ta bort &#x200B;](assets/delete-icon.png) till höger om ett anpassat formulärnamn, klicka sedan på **Ta bort** för att bekräfta och ta bort formuläret från objektet eller på **Avbryt** för att förhindra att det tas bort.
1. Klicka på **Spara ändringar** .

## Hantera flera anpassade formulär som innehåller samma anpassade fält

Du kan ha samma fält på flera anpassade formulär som är kopplade till samma objekt. I det här fallet bör du tänka på följande:

* Fältets värde är identiskt i alla former.

  Du kan inte ha olika värden för samma fält i olika formulär kopplade till samma objekt.

* Om du har samma beräkningsfält på två olika objekt måste deras beräkningar vara identiska för att undvika fel. Mer information om hur du lägger till beräknade fält i anpassade formulär, inklusive flera formulär, finns i [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Hantera flera anpassade formulär vid gruppredigering av objekt

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Att hantera anpassade formulär till objekt är identiskt för alla objekt utom projekt.
>
>Mer information om hur du lägger till anpassade formulär till projekt i grupp finns i artikeln [Redigera projekt](../../manage-work/projects/manage-projects/edit-projects.md).

När du gruppredigerar objekt som har flera anpassade formulär tillämpade kan du redigera hur anpassade formulär visas på dessa objekt samt redigera gemensamma fält bland de anpassade formulären.

Endast de anpassade formulär som är kopplade till alla markerade objekt kan redigeras i en gruppredigering.

Så här redigerar du flera anpassade formulär samtidigt när du redigerar objekt:

1. Markera de objekt som de anpassade formulären är kopplade till i ett listobjekt och klicka sedan på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) .
1. Klicka på **Anpassad Forms**.

   Du kan bara redigera anpassade formulär som är kopplade till alla markerade objekt.

   Anpassade formulär som bara är kopplade till vissa av objekten visas inte.

1. Börja redigera fält i anpassade formulär.

   När fält redigeras visas en visuell indikator i fältet som visar att fältet har redigerats.

   Om ett fält finns i mer än ett anpassat formulär, uppdateras alla värden för dessa fält i varje formulär när du uppdaterar fältet i ett av formulären.

1. Klicka på listrutan **Gör en markering** och välj ytterligare formulär som ska läggas till i alla markerade objekt.

   Tänk på följande när du använder ytterligare formulär:

   * Objekt kan ha upp till 10 anpassade former.
   * Du kan bara använda formulär när formuläret inte redan har tillämpats på något av de objekt som du redigerar. Ett formulär som redan är kopplat till ett av objekten visas inte i listrutan.
   * När du har tillämpat ytterligare ett formulär visas alla fält som har gemensamma funktioner för andra formulär i avsnittet **Gemensamma fält**, och de kan redigeras.

1. (Valfritt) Om du har lagt till anpassade formulär till alla objekt, men inte har sparat objekten än, kan du ändra i vilken ordning de anpassade formulären visas på objekten.

   Mer information om hur du ändrar formulärordningen finns i [Ändra ordning på flera anpassade formulär som är kopplade till ett objekt](#reorder-multiple-custom-forms-attached-to-an-object) i den här artikeln.

1. Klicka på **Ta bort formulär** om du vill ta bort ett anpassat formulär från objekten.

   Mer information om hur du tar bort anpassade formulär från objekt finns i [Ta bort ett anpassat formulär från ett objekt](#remove-a-custom-form-from-an-object).

   Tänk på följande när du tar bort flera formulär samtidigt från flera objekt:

   * Om du har gjort ändringar i formuläret och tar bort det går ändringarna förlorade och kan inte återställas.
   * När du har tagit bort ett formulär tas alla fält från det formuläret som fanns i avsnittet **Gemensamma fält** bort från det här avsnittet och kan inte längre redigeras här.

1. Klicka på **Återställ formulär** om du vill återställa formuläret till det tillstånd det hade innan du redigerade objekten.
1. (Valfritt) Klicka på komprimeringspilen bredvid namnet på formuläret för att komprimera ett formulär i taget.

   eller

   Klicka på **Komprimera Forms** om du vill komprimera alla formulär samtidigt.

1. (Valfritt) Klicka på pilen bredvid namnet på formuläret för att expandera ett formulär i taget.

   eller

   Klicka på **Expandera Forms** om du vill expandera alla formulär samtidigt.

1. Klicka på **Spara ändringar**.
