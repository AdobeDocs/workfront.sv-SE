---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Återanvända ett anpassat fält eller en resurswidget i ett anpassat formulär med det äldre formulärverktyget
description: När du skapar eller redigerar ett anpassat formulär kan du lägga till ett anpassat fält eller en anpassad widget som redan har lagts till i ett annat anpassat formulär.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Återanvända ett anpassat fält eller en resurswidget i ett anpassat formulär med det äldre formulärverktyget

{{form-designer-default}}

När du skapar eller redigerar ett anpassat formulär kan du lägga till ett anpassat fält eller en resurswidget som redan har lagts till i ett annat anpassat formulär.

Du kan också återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär. Instruktioner finns i [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md).

Mer information om anpassade fält och resurswidgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Återanvända ett anpassat fält eller en anpassad widget som redan används i ett annat anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Med **Lägg till ett fält** markerat, klicka **Fältbibliotek**.

1. Dra fältet eller widgeten hit du vill ha den i det anpassade formuläret.
1. (Valfritt) Upprepa de två föregående stegen för att lägga till andra fält eller widgetar.

   >[!NOTE]
   >
   >Du kan lägga till upp till 500 fält och widgetar i ett anpassat formulär. Prestandaförsämringen kan dock inträffa när det finns mer än 100 blanketter, beroende på hur komplex den är.
   >
   >
   >Exempel på komplexa formulär är formulär med överlappande parametrar, beräknade anpassade datafält och flera värdealternativ i ett enda fält.

1. Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Lägga till ett anpassat fält i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Lägga till en avsnittsbrytning i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Lägga till eller redigera en resurswidget i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Lägga till beräknade data i ett anpassat formulär med äldre formulärverktyg](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägg till visningslogik och hoppa över logik i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fyll i ett anpassat formulär med den äldre formulärbyggaren](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
