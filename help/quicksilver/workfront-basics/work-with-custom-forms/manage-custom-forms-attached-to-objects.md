---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Hantera anpassade formulär som är kopplade till objekt
description: Du kan uppdatera den ordning i vilken anpassade formulär som är kopplade till ett objekt visas, tas bort eller gruppredigera hur anpassade formulär visas på flera objekt.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: b3534cccd4a06b8c5b8b7e742f63eeb898bd5b99
workflow-type: tm+mt
source-wordcount: '1147'
ht-degree: 0%

---

# Hantera anpassade formulär som är kopplade till objekt

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är tillgänglig för alla kunder i förhandsgranskningsmiljön och för en viss grupp av kunder i produktionsmiljön.</span>

Du kan uppdatera den ordning i vilken anpassade formulär som är kopplade till ett objekt visas, tas bort eller gruppredigera hur anpassade formulär visas på flera objekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till de objekt som du hanterar anpassade formulär för</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre till objekt som du hanterar anpassade formulär för</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

* Din Workfront-administratör eller en plananvändare med administrativ åtkomst till anpassade formulär måste skapa anpassade formulär i din miljö. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Du måste ha anpassade formulär kopplade till ett objekt.

  Mer information om hur du använder anpassade formulär för ett objekt finns i [Lägga till ett anpassat formulär för ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Ändra ordning på flera anpassade formulär som är kopplade till ett objekt {#reorder-multiple-custom-forms-attached-to-an-object}

1. Gå till objektet där du vill ändra ordningen på de tillagda anpassade formulären och börja sedan redigera objektet.

   **Exempel:** Om du till exempel vill hantera de anpassade formulären för ett projekt går du till projektet, klickar på menyn **Mer** ![](assets/more-icon.png) och sedan på **Redigera** .

1. Klicka på ikonen **bredvid namnet på ett anpassat formulär i avsnittet** Anpassad Forms![](assets/move-icon---dots.png) för projekt, uppgifter och utgåvor. För alla andra objekt klickar du på **Hantera Forms**. Det här alternativet visas bara om minst ett anpassat formulär är kopplat till objektet.
1. Dra ett formulär ![](assets/move-icon---dots.png) till en ny plats i listan.
1. Klicka på **Spara** för projekt, uppgifter och utgåvor av anpassade formulär.

   För alla andra objekt klickar du på **Jag har slutat hantera** > **Spara ändringar**.

## Ta bort ett anpassat formulär från ett objekt {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>När du tar bort ett anpassat formulär från ett objekt, försvinner all information som hämtats i de anpassade fälten i formuläret och kan inte återställas.

1. Gå till objektet där du vill ta bort det anpassade formuläret och börja redigera objektet.

   Gå till exempel till ett projekt, klicka på menyn **Mer** ![](assets/more-icon.png) och sedan på **Redigera** .

1. Klicka på **Anpassad Forms**.
1. För projekt, uppgifter och utleveranser av anpassade formulär klickar du på ikonen **X** till höger om ett formulär för att ta bort det från objektet.

   För alla andra objekt klickar du på **Hantera Forms** och sedan på ikonen **X** till höger om ett formulär för att ta bort det från objektet.

1. <span class="preview">Klicka på **Ta bort** i den dialogruta som öppnas.</span>

1. Klicka på **Spara** .

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

1. Markera de objekt som de anpassade formulären är kopplade till i ett listobjekt och klicka sedan på ikonen **Redigera** ![](assets/edit-icon.png) .
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
