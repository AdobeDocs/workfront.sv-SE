---
title: Skapa ett formulär från en kopia
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan skapa ett anpassat formulär från en kopia med formulärdesignern.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Skapa ett formulär från en kopia

<!--add preview tags and see below in comment out-->

Du kan utforma ett nytt anpassat formulär som baseras på ett befintligt. Du kan koppla anpassade formulär till olika Workfront-objekt för att samla in data om dessa objekt.

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

## Kopiera ett anpassat formulär och skapa ett nytt

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms.**
1. Markera det anpassade formulär som du vill använda som bas för ett nytt anpassat formulär och klicka sedan på ikonen ![Kopiera](assets/copy-icon.png).
1. I rutan **Egen formulärkopia** som visas skriver du följande information:

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
      <td> <p>Markera de objekttyper som du vill att det anpassade formuläret ska fungera med i rutan <b>Formulärtyp</b> och klicka på X:et bredvid de typer som du vill ta bort. Typer som redan är kopplade till formuläret är inaktiverade i listan.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Formuläret måste associeras med minst en objekttyp.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Kopiera**.

   Om beräkningsfält i det ursprungliga formuläret refererar till fält som inte är kompatibla med en objekttyp som du lägger till i det nya formuläret, uppmanas du att ändra beräkningarna i dessa fält.

   Om ett åtkomstalternativ för en avsnittsbrytning i det ursprungliga formuläret inte är kompatibelt med en objekttyp som du lägger till i den nya, uppmanas du att ändra alternativet.

1. Markera formuläret som du just kopierade och klicka sedan på ![Redigera-ikonen](assets/edit-icon.png).
1. Gör eventuella ändringar i formuläret enligt följande avsnitt i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md):

   * [Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Lägg till textfält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Lägg till beräknade fält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Lägga till alternativknappar, kryssrutegrupper och listrutor](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Lägg till rubriker och datumfält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [Lägga till bilder, PDF-filer och videor](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Lägg till Adobe XD-filer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [Lägg till planeringsanslutningsfält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. (Valfritt) När du har klickat på **Spara och stäng** kopplar du formuläret till det objekt där du vill använda det, enligt beskrivningen i [Lägg till ett anpassat formulär till ett objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
