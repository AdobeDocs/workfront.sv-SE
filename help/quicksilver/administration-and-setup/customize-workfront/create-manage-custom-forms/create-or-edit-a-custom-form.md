---
title: Skapa eller redigera ett anpassat formulär med det äldre formulärverktyget
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan skapa eller redigera nya anpassade formulär.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Skapa eller redigera ett anpassat formulär med det äldre formulärverktyget

<!--Audited: 01/2024-->

{{form-designer-default}}

Du kan skapa ett nytt anpassat formulär eller redigera ett befintligt. Båda uppgifterna förklaras i den här artikeln.

Mer information om hur du skapar ett nytt anpassat formulär från ett befintligt finns i [Kopiera ett anpassat formulär och skapa ett nytt med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

I den här artikeln beskrivs hur du kan skapa ett anpassat formulär med det äldre formulärverktyget. Mer information om hur du skapar ett anpassat formulär med hjälp av formulärdesignern finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr>  
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Börja skapa ett anpassat formulär

{{step-1-to-setup}}

1. Klicka **Anpassad Forms** till vänster.

   Anpassade formulär visas i en lista. Du kan granska alla anpassade formulär och anpassade fält som har skapats för din organisation. Du kan också se vem som har skapat varje formulär, vilka objekt som är kopplade till det och om det är aktivt.

1. Klicka **Nytt anpassat formulär.**
1. Markera minst en objekttyp som du vill associera med det anpassade formuläret och klicka sedan på **Fortsätt**.

   ![](assets/choose-object-type.jpg)

1. På **Formulärinställningar** -flik som öppnas, skriv en **Formulärtitel** och ett valfritt **Beskrivning** för det anpassade formuläret.

1. (Valfritt) Om du vill lägga till fler objekttyper i formuläret så att det kan kopplas till fler objekt klickar du på **plus** signera efter **Objekttyper** väljer du sedan den objekttyp som du vill använda på menyn som visas.

   Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

1. (Valfritt) Klicka på **X** på en objekttyp för att ta bort den från formuläret.

   Mer information om hur du tar bort objekttyper från ett anpassat formulär som du redan har sparat finns i [Ta bort objekttyper i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klicka **Klar** i skärmens nedre vänstra hörn.

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

{{step-1-to-setup}}

1. Klicka **Anpassad Forms** till vänster.

   Anpassade formulär visas i en lista. Du kan granska alla anpassade formulär och anpassade fält som har skapats för din organisation. Du kan också se vem som har skapat varje formulär, vilka objekt som är kopplade till det och om det är aktivt.

1. Markera det anpassade formulär som du vill redigera och klicka sedan på ![Ikonen Redigera](assets/edit-icon.png).
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
