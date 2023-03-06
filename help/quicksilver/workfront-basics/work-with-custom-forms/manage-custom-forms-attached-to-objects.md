---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Hantera anpassade formulär som är kopplade till objekt
description: Du kan uppdatera den ordning i vilken anpassade formulär som är kopplade till ett objekt visas, tas bort eller gruppredigera hur anpassade formulär visas på flera objekt.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Hantera anpassade formulär som är kopplade till objekt

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>  -->

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
   <td> <p>Redigera åtkomst till de objekt som du hanterar anpassade formulär för</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute-behörigheter eller högre till objekt som du hanterar anpassade formulär för</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

* Din Workfront-administratör eller en plananvändare med administrativ åtkomst till anpassade formulär måste skapa anpassade formulär i din miljö. Mer information finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Du måste ha anpassade formulär kopplade till ett objekt.

   Mer information om hur du använder anpassade formulär för ett objekt finns i [Lägga till ett anpassat formulär i ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Ändra ordning på flera anpassade formulär som är kopplade till ett objekt {#reorder-multiple-custom-forms-attached-to-an-object}

1. Gå till objektet där du vill ändra ordningen på de tillagda anpassade formulären och börja sedan redigera objektet.

   **Exempel:** Om du till exempel vill hantera de anpassade formulären för ett projekt går du till projektet och klickar på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Redigera** .

1. I **Anpassad Forms** för projekt, uppgifter och ärenden, klicka på ![](assets/move-icon---dots.png) -ikonen bredvid namnet på ett anpassat formulär. För alla andra objekt klickar du på **Hantera Forms**. Det här alternativet visas bara om minst ett anpassat formulär är kopplat till objektet.
1. Dra ett formulär ![](assets/move-icon---dots.png) till en ny plats i listan.
1. Klicka på **Spara**.

   För alla andra objekt klickar du på **Jag är klar med hanteringen** > **Spara ändringar**.

## Ta bort ett anpassat formulär från ett objekt {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>När du tar bort ett anpassat formulär från ett objekt, försvinner all information som hämtats i de anpassade fälten i formuläret och kan inte återställas.

1. Gå till objektet där du vill ta bort det anpassade formuläret och börja redigera objektet.

   Gå till ett projekt och klicka på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Redigera** .

1. Klicka **Anpassad Forms**.
1. För projekt, uppgifter och ärenden, anpassade formulär klickar du på **X** till höger om ett formulär för att ta bort det från objektet.

   För alla andra objekt klickar du på **Hantera Forms** klickar du på **X** till höger om ett formulär för att ta bort det från objektet.

1. Klicka **Spara** .

## Hantera flera anpassade formulär som innehåller samma anpassade fält

Du kan ha samma fält på flera anpassade formulär som är kopplade till samma objekt. I det här fallet bör du tänka på följande:

* Fältets värde är identiskt i alla former.

   Du kan inte ha olika värden för samma fält i olika formulär kopplade till samma objekt.

* Om du har samma beräkningsfält på två olika objekt måste deras beräkningar vara identiska för att undvika fel. Mer information om hur du lägger till beräknade fält i anpassade formulär, inklusive flera formulär, finns i [Lägga till beräknade data i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Hantera flera anpassade formulär vid gruppredigering av objekt

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:

>[!NOTE]
>
><span class="preview">For information about managing custom forms on projects in bulk in the Preview environment, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

-->

När du gruppredigerar objekt som har flera anpassade formulär tillämpade kan du redigera hur anpassade formulär visas på dessa objekt samt redigera gemensamma fält bland de anpassade formulären.

Endast de anpassade formulär som är kopplade till alla markerade objekt kan redigeras i en gruppredigering.

Så här redigerar du flera anpassade formulär samtidigt när du redigerar objekt:

1. I ett listobjekt markerar du de objekt där de anpassade formulären är kopplade och klickar sedan på **Redigera** icon ![](assets/edit-icon.png).
1. Klicka **Anpassad Forms**.

   Du kan bara redigera anpassade formulär som är kopplade till alla markerade objekt.

   Anpassade formulär som bara är kopplade till vissa av objekten visas inte.

1. Börja redigera fält i anpassade formulär.

   När fält redigeras visas en visuell indikator i fältet som visar att fältet har redigerats.

   Om ett fält finns i mer än ett anpassat formulär, uppdateras alla värden för dessa fält i varje formulär när du uppdaterar fältet i ett av formulären.

1. Klicka på **Gör en markering** och välj ytterligare formulär som ska läggas till i alla markerade objekt.

   Tänk på följande när du använder ytterligare formulär:

   * Objekt kan ha upp till 10 anpassade former.
   * Du kan bara använda formulär när formuläret inte redan har tillämpats på något av de objekt som du redigerar. Ett formulär som redan är kopplat till ett av objekten visas inte i listrutan.
   * När du har tillämpat ytterligare ett formulär, visas alla fält som har samma format som andra formulär i **Vanliga fält** så kan de redigeras.

1. (Valfritt) Om du har lagt till anpassade formulär till alla objekt, men inte har sparat objekten än, kan du ändra i vilken ordning de anpassade formulären visas på objekten.

   Mer information om hur du ändrar ordningen på formulären finns i [Ändra ordning på flera anpassade formulär som är kopplade till ett objekt](#reorder-multiple-custom-forms-attached-to-an-object) i den här artikeln.

1. Klicka **Ta bort formulär** om du vill ta bort ett anpassat formulär från objekten.

   Mer information om hur du tar bort anpassade formulär från objekt finns i [Ta bort ett anpassat formulär från ett objekt](#remove-a-custom-form-from-an-object).

   Tänk på följande när du tar bort flera formulär samtidigt från flera objekt:

   * Om du har ändrat formuläret och tar bort det går ändringarna förlorade och kan inte återställas.
   * När du har tagit bort ett formulär, alla fält från formuläret som fanns i **Vanliga fält** -avsnittet har tagits bort från det här avsnittet och kan inte längre redigeras här.

1. Klicka **Återställ formulär** för att återställa formuläret till det tillstånd det hade innan du redigerade objekten.
1. (Valfritt) Klicka på komprimeringspilen bredvid namnet på formuläret för att komprimera ett formulär i taget.

   eller

   Klicka **Komprimera Forms** om du vill komprimera alla formulär samtidigt.

1. (Valfritt) Klicka på pilen bredvid namnet på formuläret för att expandera ett formulär i taget.

   eller

   Klicka **Expandera Forms** om du vill expandera alla formulär samtidigt. 

1. Klicka **Spara ändringar**.
