---
title: Överför anpassade formulärdata vid konvertering av ett objekt
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: När arbetet som definieras i ett arbetsobjekt blir för stort kan du konvertera det till ett större arbetsobjekt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Överför anpassade formulärdata vid konvertering av ett objekt

Beroende på organisationens affärsbehov kan det arbete som definieras i en uppgift eller ett problem bli för stort för att kunna hanteras i uppgiften eller problemet. I det här fallet kan du konvertera dem till en större arbetsuppgift:

* Du kan konvertera utleveranser till uppgifter eller till projekt
* Du kan konvertera uppgifter till projekt

Om du vill överföra anpassade formulärdata från en utgåva till en uppgift eller ett projekt, måste du slutföra de två uppgifterna i den här artikeln i den ordning som anges nedan.

Mer information finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) eller [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Först: Lägg till ytterligare objekt i det anpassade formuläret

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms**.
1. Leta reda på formuläret som du behöver och klicka sedan på ![Redigera-ikonen](assets/edit-icon.png).
1. Längst upp i formuläret lägger du till objektet som du vill konvertera uppgiften eller utgåvan till.

   >[!INFO]
   >
   >**Exempel**: Om du vill överföra anpassade formulärdata till ett projekt väljer du Projekt.

1. Klicka på **Använd** längst ned i formuläret.

1. Fortsätt till [Sekund: Konvertera problemet eller aktiviteten och överför anpassade formulärdata](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Andra: Konvertera problemet eller uppgiften och överför anpassade formulärdata {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Lägg till ytterligare objekt i det anpassade formuläret för det problem eller den uppgift som du konverterar, enligt beskrivningen i avsnittet [Första: Lägg till ytterligare objekt i det anpassade formuläret](#first-add-additonal-objects-to-the-custom-form) i den här artikeln.
1. Konvertera utgåvan eller aktiviteten med alternativet **Anpassad Forms** i rutan som visas för att välja det anpassade formulär som du behöver. Instruktioner finns i följande artiklar:

   * [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertera ett problem till en uppgift i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertera en uppgift till ett projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. I dialogrutan **Konvertera till (objekttyp)** som visas klickar du på listrutan **Lägg till Forms** och väljer det formulär som du kopierade i föregående avsnitt.

   Informationen som hämtas i de anpassade fälten för utgåvan överförs nu till det anpassade formuläret för uppgiften.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->