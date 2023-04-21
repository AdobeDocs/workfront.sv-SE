---
title: Överför anpassade formulärdata vid konvertering av ett objekt
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: När arbetet som definieras i ett arbetsobjekt blir för stort kan du konvertera det till ett större arbetsobjekt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 7b378fdf3530d5e1c06f09d03c23c31afac6aa47
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Överför anpassade formulärdata vid konvertering av ett objekt

Beroende på organisationens affärsbehov kan det arbete som definieras i en uppgift eller ett problem bli för stort för att kunna hanteras i uppgiften eller problemet. I det här fallet kan du konvertera dem till en större arbetsuppgift:

* Du kan konvertera utleveranser till uppgifter eller till projekt
* Du kan konvertera uppgifter till projekt

Om du vill överföra anpassade formulärdata från en utgåva till en uppgift eller ett projekt, måste du slutföra de två uppgifterna i den här artikeln i den ordning som anges nedan.

Mer information finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) eller [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Första: Lägga till fler objekt i det anpassade formuläret

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms**.
1. Hitta det formulär du behöver och klicka sedan på **Redigera**.
1. Längst upp i formuläret lägger du till objektet som du vill konvertera uppgiften eller utgåvan till.
   >[!INFO]
   >
   >**Exempel**: Om du vill överföra anpassade formulärdata till ett projekt väljer du Projekt.

1. Klicka **Använd** längst ned i formuläret.

1. Fortsätt till [Andra: Konvertera ärendet eller uppgiften och överför anpassade formulärdata](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Andra: Konvertera ärendet eller uppgiften och överför anpassade formulärdata {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Lägg till ytterligare objekt i det anpassade formuläret i det problem eller den uppgift du konverterar, enligt anvisningarna i avsnittet [Första: Lägga till ytterligare objekt i det anpassade formuläret](#first-add-additonal-objects-to-the-custom-form) i den här artikeln.
1. Konvertera ett problem eller en uppgift med **Anpassad Forms** i rutan som visas för att välja det anpassade formulär som du behöver. Instruktioner finns i följande artiklar:

   * [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertera ett problem till en uppgift i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertera en uppgift till ett projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. I **Konvertera till (objekttyp)** som visas klickar du på **Lägg till Forms** och välj det formulär du kopierade i föregående avsnitt.

   Informationen som hämtas i de anpassade fälten för utgåvan överförs nu till det anpassade formuläret för uppgiften.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->