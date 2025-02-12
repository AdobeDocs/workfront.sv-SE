---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ta bort ett anpassat fält eller en widget från systemet
description: För att förbättra systemets prestanda och göra formulären enklare att använda för användarna kan du ta bort anpassade fält och widgetar från systemet när de inte längre används.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Ta bort ett anpassat fält eller en anpassad widget från systemet

För att förbättra systemets prestanda och göra formulären enklare att använda för användarna kan du ta bort anpassade fält och widgetar från systemet när de inte längre används.

>[!CAUTION]
>
>Om du tar bort ett anpassat fält tas även alla anpassade data som användarna har angett i fältet bort när de fyller i anpassade formulär som är kopplade till objekt. Det går inte att återställa borttagna data. Det finns heller inget meddelandesystem för att varna personer som använder det anpassade formuläret om att det har tagits bort.
>
>Du kan visa alla anpassade formulär och rapporter som använder ett anpassat fält som du vill ta bort för att avgöra vilka återverkningar som kan uppstå. Mer information finns i [Visa alla anpassade formulär som använder ett visst anpassat fält eller en viss widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) och [Visa alla rapporter som använder ett visst anpassat fält eller en viss widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Du kan också, för att komma runt problemet, undvika att förlora data i fält som inte längre används, se [Ta bort ett anpassat fält utan att förlora data som användare har angett](#remove-a-custom-field-without-losing-data-that-users-have-entered) i den här artikeln.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort ett anpassat fält eller en anpassad widget från systemet

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms.**
1. Klicka på **Fält** för att öppna fältområdet.
1. Markera det anpassade fältet eller widgeten och klicka sedan på **Ta bort**.
1. Om du är säker på att du permanent vill ta bort objektet och (om det är ett anpassat fält) alla associerade data på objekt där det bifogades, klickar du på **Ja, Ta bort**.

## Ta bort ett anpassat fält utan att förlora data som användarna har angett {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Det går inte att ångra borttagning av ett anpassat fält från ett anpassat formulär som har fler än 500 fält och widgetar. Om du tar bort fältet kan du inte lägga till det igen förrän formuläret har färre än 500 fält och widgetar.

1. Avgör vilka anpassade fält som du vill ta bort från det ursprungliga anpassade formuläret, men ta inte bort dem just nu.
1. Skapa ett nytt anpassat formulär:

   1. Lägg till anpassade fält i det nya formuläret som du vill ta bort från det ursprungliga anpassade formuläret.

      Mer information finns i avsnittet [Lägg till nya eller befintliga fält i ditt anpassade formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. Spara det nya anpassade formuläret.

1. Begränsa åtkomsten till det anpassade formuläret till användare med administrativ åtkomst, enligt beskrivningen i [Dela ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Använd det nya anpassade formuläret på de objekt där det ursprungliga anpassade formuläret redan används, vilket beskrivs i [Lägg till ett anpassat formulär till ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Genom att använda det nya anpassade formuläret på dessa objekt säkerställs att historiska rapporteringsdata inte påverkas.

1. Ändra det ursprungliga anpassade formuläret och ta bort de anpassade fält som du har lagt till i det nya formuläret (i steg 2).

   Fälten som du tog bort från det ursprungliga anpassade formuläret är nu bara tillgängliga i det nya anpassade formuläret som du skapade. Användare kan se det anpassade formuläret på objektet, men användare utan administrativ åtkomst kan inte ändra det anpassade formuläret.
