---
user-type: administrator
product-area: system-administration
keywords: skapa,anpassad,formulär,kopiera,bas,annan
navigation-topic: create-and-manage-custom-forms
title: Kopiera ett anpassat formulär och skapa ett nytt med det äldre verktyget
description: Du kan skapa ett nytt anpassat formulär som baseras på ett befintligt.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Kopiera ett anpassat formulär och skapa ett nytt med det äldre verktyget

Du kan skapa ett nytt anpassat formulär som baseras på ett befintligt.

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

## Kopiera ett anpassat formulär och skapa ett nytt

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms.**
1. Välj det anpassade formulär som du vill använda som bas för ett nytt anpassat formulär och klicka sedan på **Kopiera**.
1. I **Egen formulärkopia** anger du följande information i rutan som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Formulärnamn</td> 
      <td>Skriv ett namn för det kopierade formuläret.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Formulärtyper </p> </td> 
      <td> <p>I <b>Formulärtyp</b> markerar du de objekttyper som du vill att det anpassade formuläret ska fungera med och klickar på X bredvid de typer som du vill ta bort. Typer som redan är kopplade till formuläret är inaktiverade i listan.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>Formuläret måste associeras med minst en objekttyp.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Kopiera formulär**.

   Om beräkningsfält i det ursprungliga formuläret refererar till fält som inte är kompatibla med en objekttyp som du lägger till i det nya formuläret, uppmanas du att ändra beräkningarna i dessa fält.

   Om ett åtkomstalternativ för en avsnittsbrytning i det ursprungliga formuläret inte är kompatibelt med en objekttyp som du lägger till i den nya, uppmanas du att ändra alternativet.

1. Markera formuläret som du just kopierade och klicka sedan på **Redigera**.
1. Gör eventuella ändringar i formuläret enligt följande artiklar:

   * [Kopiera ett anpassat formulär och skapa ett nytt med det äldre formulärverktyget](#Add2)
   * [Lägga till beräknade data i ett anpassat formulär med äldre formulärverktyg](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till eller redigera en resurswidget i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägg till visningslogik och hoppa över logik i ett anpassat formulär med det äldre formulärverktyget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fyll i ett anpassat formulär med den äldre formulärbyggaren](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Valfritt) När du har klickat **Spara+stäng** bifoga formuläret till det objekt där du vill använda det, enligt beskrivningen i [Lägga till ett anpassat formulär i ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
