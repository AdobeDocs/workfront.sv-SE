---
title: Skapa eller redigera ett anpassat formulär med det äldre formulärverktyget
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan skapa eller redigera nya anpassade formulär.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# Skapa eller redigera ett anpassat formulär med det äldre formulärverktyget

Du kan skapa eller redigera nya anpassade formulär. Båda uppgifterna förklaras i den här artikeln.

Mer information om hur du skapar ett nytt anpassat formulär från ett befintligt finns i [Kopiera ett anpassat formulär och skapa ett nytt med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

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
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Börja skapa ett anpassat formulär

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** till vänster.

   I den vy som visas kan du granska alla anpassade formulär och anpassade fält som har skapats för din organisation. Du kan också se vem som har skapat respektive formulär och vilka fält som är kopplade till det.

1. Klicka **Nytt anpassat formulär.**
1. Markera minst en objekttyp som du vill associera med det anpassade formuläret och klicka sedan på **Fortsätt**.

   ![](assets/choose-object-type.jpg)

1. På **Formulärinställningar** -flik som öppnas, skriv en **Formulärtitel** och ett valfritt **Beskrivning** för det anpassade formuläret.

1. (Valfritt) Om du vill lägga till fler objekttyper i formuläret så att det kan kopplas till fler objekt klickar du på plustecknet efter objekttyper och väljer sedan den objekttyp som du vill använda på menyn som visas.

   Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.Du kan också klicka på X för en objekttyp om du vill ta bort den från formuläret.

   Mer information om hur du tar bort objekttyper från ett anpassat formulär som du redan har sparat finns i [Ta bort objekttyper i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klicka **Klar**.

   >[!TIP]
   >
   >Klicka **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

1. Om du vill lägga till ett nytt anpassat fält i formuläret fortsätter du med [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) eller [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   eller

   Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till en avsnittsbrytning i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Börja redigera ett anpassat formulär

Du kan redigera ett anpassat formulär när som helst efter att det har skapats.

>[!CAUTION]
>
>Mer information om hur du tar bort fält från ett anpassat formulär utan att förlora data som användare har angett i dessa fält finns i avsnittet [Ta bort ett anpassat fält utan att förlora data som användarna har angett](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) i artikeln [Ta bort ett anpassat fält eller en anpassad widget från systemet](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>I allmänhet rekommenderar vi att du minimerar antalet gånger som du redigerar ett anpassat formulär som redan används. Det finns inget meddelandesystem för att varna personer som använder det anpassade formuläret om dina ändringar.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** till vänster.

   I den vy som visas kan du granska alla anpassade formulär som har skapats för din organisation. Du kan också se vem som har skapat varje formulär, vilken objekttyp det fungerar med och om det är aktivt.

1. Markera det anpassade formulär som du vill redigera och klicka sedan på **Redigera**.
1. (Valfritt) Om du vill ändra rubriken och beskrivningen för det anpassade formuläret klickar du på knappen **Formulärinställningar** tabben och sedan skriva en **Formulärtitel** och **Beskrivning**.

1. (Valfritt) Om du vill lägga till fler objekttyper i formuläret så att det kan kopplas till fler objekt klickar du på plustecknet + efter **Objekttyper** väljer du sedan önskad typ på menyn som visas.

   ![](assets/add-object-type-existing-form.png)

   Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

   Du kan också klicka på X för en objekttyp för att ta bort den från formuläret. Detta bör göras med försiktighet när du vill ta bort en objekttyp från ett anpassat formulär som du redan har sparat. Mer information finns i [Ta bort objekttyper i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klicka **Klar**.

   >[!TIP]
   >
   >Klicka **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

1. Om du vill lägga till ett nytt anpassat fält i formuläret fortsätter du med [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) eller [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   eller

   Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till en avsnittsbrytning i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
