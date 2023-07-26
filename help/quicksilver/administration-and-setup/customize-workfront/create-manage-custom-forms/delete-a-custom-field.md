---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ta bort ett anpassat fält eller en anpassad widget från systemet
description: För att förbättra systemets prestanda och göra formulären enklare att använda för användarna kan du ta bort anpassade fält och widgetar från systemet när de inte längre används.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Ta bort ett anpassat fält eller en anpassad widget från systemet

För att förbättra systemets prestanda och göra formulären enklare att använda för användarna kan du ta bort anpassade fält och widgetar från systemet när de inte längre används.

>[!CAUTION]
>
>När du tar bort ett anpassat fält tas även alla anpassade data som användarna har angett i fältet bort när de fyller i anpassade formulär som är kopplade till objekt. Det går inte att återställa borttagna data.
>
>Du kan visa alla anpassade formulär och rapporter som använder ett anpassat fält som du vill ta bort för att avgöra vilka återverkningar som kan uppstå. Mer information finns i [Visa alla anpassade formulär som använder ett visst anpassat fält eller en viss widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) och [Visa alla rapporter som använder ett visst anpassat fält eller en viss widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Du kan också, för att komma till en tillfällig lösning, undvika att förlora data i fält som inte längre används, se [Ta bort ett anpassat fält utan att förlora data som användarna har angett](#remove-a-custom-field-without-losing-data-that-users-have-entered) i den här artikeln.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Ta bort ett anpassat fält eller en anpassad widget från systemet

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms.**
1. Klicka på **Fält** -fliken.
1. Markera det anpassade fältet eller widgeten och klicka sedan på **Ta bort**.
1. Om du är säker på att du vill ta bort objektet permanent och (om det är ett anpassat fält) alla associerade data på objekt där det bifogades, klickar du på **Ja, ta bort den**.

## Ta bort ett anpassat fält utan att förlora data som användarna har angett {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Det går inte att ångra borttagning av ett anpassat fält från ett anpassat formulär som har fler än 500 fält och widgetar. Om du tar bort fältet kan du inte lägga till det igen förrän formuläret har färre än 500 fält och widgetar.

1. Avgör vilka anpassade fält som du vill ta bort från det ursprungliga anpassade formuläret, men ta inte bort dem just nu.
1. Skapa ett nytt anpassat formulär:

   1. Lägg till anpassade fält i det nya formuläret som du vill ta bort från det ursprungliga anpassade formuläret.

      * Om du använder det anpassade formulärverktyget läser du [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Om du använder formulärdesignern kan du läsa [Lägg till nya eller befintliga fält i det anpassade formuläret](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. Spara det nya anpassade formuläret.

1. Begränsa åtkomsten till det anpassade formuläret till användare med administrativ åtkomst, enligt beskrivningen i [Dela ett eget formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Använd det nya anpassade formuläret på de objekt där det ursprungliga anpassade formuläret redan används, enligt beskrivningen i [Lägga till ett anpassat formulär i ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Genom att använda det nya anpassade formuläret på dessa objekt säkerställs att historiska rapporteringsdata inte påverkas.

1. Ändra det ursprungliga anpassade formuläret och ta bort de anpassade fält som du har lagt till i det nya formuläret (i steg 2).

   Fälten som du tog bort från det ursprungliga anpassade formuläret är nu bara tillgängliga i det nya anpassade formuläret som du skapade. Användare kan se det anpassade formuläret på objektet, men användare utan administrativ åtkomst kan inte ändra det anpassade formuläret.
