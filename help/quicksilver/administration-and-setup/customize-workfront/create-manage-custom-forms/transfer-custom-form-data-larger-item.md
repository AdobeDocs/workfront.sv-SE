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
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Överför anpassade formulärdata vid konvertering av ett objekt

Beroende på organisationens affärsbehov kan arbetet som definieras i en uppgift eller ett problem bli för stort för att kunna hantera det i uppgiften eller problemet. I det här fallet kan du konvertera dem till en större arbetsuppgift:

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

## Första: Kopiera det anpassade formuläret {#first-copy-the-custom-form}

Först måste du se till att du behåller alla anpassade formulärdata för en uppgift eller ett problem som du vill konvertera. Eftersom anpassade formulärdata måste matcha det konverterade objektet är det bäst att duplicera formuläret så att du kan bifoga det till det nya objektet.

>[!TIP]
>
>Ett annat sätt att behålla anpassade formulärdata är att lägga till den större objekttypen i det anpassade formuläret. Instruktioner finns i avsnittet [Börja redigera ett eget formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) i artikeln [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms**.
1. Välj det anpassade formulär av aktivitets- eller problemtyp och klicka sedan på **Kopiera**.
1. I **Eget formulär** anger du ett namn för det nya formuläret.

1. Från **Formulärtyp** väljer du den typ av objekt som du vill skapa det nya anpassade formuläret för

   **Exempel:** Om du vill överföra anpassade formulärdata till ett projekt väljer du Projekt.

1. Klicka **Kopiera formulär**.

   Det här kopierade anpassade formuläret kan nu bifogas till en uppgift eller ett projekt.

1. Fortsätt till [Andra: Konvertera ärendet eller uppgiften och överför anpassade formulärdata](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Andra: Konvertera ärendet eller uppgiften och överför anpassade formulärdata {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Kopiera det anpassade formuläret för det problem eller den uppgift du konverterar, enligt anvisningarna i avsnittet [Första: Kopiera det anpassade formuläret](#first-copy-the-custom-form) i den här artikeln.
1. Konvertera ett problem eller en uppgift med **Anpassad Forms** i rutan som visas för att välja det anpassade formulär som du kopierade. Instruktioner finns i följande artiklar:

   * [Konvertera ett problem till ett projekt i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertera ett problem till en uppgift i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertera en uppgift till ett projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. I **Konvertera till (objekttyp)** som visas klickar du på **Lägg till Forms** och välj det formulär du kopierade i föregående avsnitt.

   Informationen som hämtas i de anpassade fälten för utgåvan överförs nu till det anpassade formuläret för uppgiften.

