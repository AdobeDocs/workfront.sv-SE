---
product-area: templates
navigation-topic: templates-navigation-topic
title: Ta bort projektmallar
description: Vi rekommenderar att du inaktiverar mallar som du inte längre använder, i stället för att ta bort dem så att du kan spara historik om dina projekt över tid.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Ta bort projektmallar

Vi rekommenderar att du inaktiverar mallar som du inte längre använder, i stället för att ta bort dem så att du kan spara historik om dina projekt över tid. Mer information om hur du inaktiverar en mall finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>När du tar bort en mall ändras inte de projekt som använder mallen på något sätt. Du kan dock inte längre se namnet på den ursprungliga mallen i fältet Mallar i projektet. Dessutom kan du inte längre visa namnen på malluppgifterna för aktiviteterna i projektet i en uppgiftsvy. Mallfältet i projektet och mallaktivitetsfältet för aktiviteterna är tomma när mallen som ursprungligen associerades med projektet har tagits bort.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar som inkluderar åtkomst till Ta bort</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till mallen som innehåller behörigheter för att ta bort den</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på vid borttagning av mallar

* De uppgifter som lades till i projekt när mallen bifogades finns kvar i projekten. Den malluppgiftsinformation som är kopplad till uppgifterna tas dock bort.
* Mallens namn visas inte längre i fältet **Mall** på underfliken **Översikt** i projektet.

* Du kan återställa en nyligen borttagen mall från papperskorgen. Mer information om hur du återställer objekt från papperskorgen finns i [Återställa borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Ta bort en mall

{{step1-to-templates}}

Då öppnas en lista med mallar

1. Markera mallen som du vill ta bort genom att klicka i kryssrutan till vänster om mallnamnet och klicka sedan på **Ta bort > Ja, ta bort** för att bekräfta borttagningen.

   eller

   Klicka på namnet på en mall för att komma åt den, klicka sedan på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) och sedan på **Ta bort mall > Ja, ta bort den**.

   Mallen är inte längre tillgänglig för att associeras med ett projekt.
