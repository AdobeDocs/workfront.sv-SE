---
title: Designa ett formulär från en kopia med formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan utforma ett anpassat formulär från en kopia med formulärdesignern.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Designa ett formulär från en kopia med formulärdesignern

Du kan utforma ett nytt anpassat formulär som baseras på ett befintligt. Du kan koppla anpassade formulär till olika Workfront-objekt för att samla in data om dessa objekt.

## Åtkomstkrav

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

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Kopiera ett anpassat formulär och skapa ett nytt

{{step-1-to-setup}}

1. Klicka **Anpassad Forms.**
1. Välj det anpassade formulär som du vill använda som bas för ett nytt anpassat formulär och klicka sedan på ![Kopiera, ikon](assets/copy-icon.png).
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
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Formuläret måste associeras med minst en objekttyp.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Kopiera**.

   Om beräkningsfält i det ursprungliga formuläret refererar till fält som inte är kompatibla med en objekttyp som du lägger till i det nya formuläret, uppmanas du att ändra beräkningarna i dessa fält.

   Om ett åtkomstalternativ för en avsnittsbrytning i det ursprungliga formuläret inte är kompatibelt med en objekttyp som du lägger till i den nya, uppmanas du att ändra alternativet.

1. Markera formuläret som du just kopierade och klicka sedan på ![Ikonen Redigera](assets/edit-icon.png).
1. Gör eventuella ändringar i formuläret enligt följande avsnitt i [Designa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) artikel:

   * [Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Lägg till textfält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Lägg till beräknade fält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Lägg till alternativknappar, kryssrutegrupp och listrutor](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Lägg till rubriker och datumfält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Lägga till bilder, PDF och videoklipp](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Lägg till Adobe XD-filer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Valfritt) När du har klickat **Spara+stäng** bifoga formuläret till det objekt där du vill använda det, enligt beskrivningen i [Lägga till ett anpassat formulär i ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
