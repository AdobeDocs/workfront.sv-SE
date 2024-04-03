---
product-area: templates
navigation-topic: templates-navigation-topic
title: Ta bort projektmallar
description: Vi rekommenderar att du inaktiverar mallar som du inte längre använder, i stället för att ta bort dem så att du kan spara historik om dina projekt över tid.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Ta bort projektmallar

Vi rekommenderar att du inaktiverar mallar som du inte längre använder, i stället för att ta bort dem så att du kan spara historik om dina projekt över tid. Mer information om hur du inaktiverar en mall finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>När du tar bort en mall ändras inte de projekt som använder mallen på något sätt. Du kan dock inte längre se namnet på den ursprungliga mallen i fältet Mallar i projektet. Dessutom kan du inte längre visa namnen på malluppgifterna för aktiviteterna i projektet i en uppgiftsvy. Mallfältet i projektet och mallaktivitetsfältet för aktiviteterna är tomma när mallen som ursprungligen associerades med projektet har tagits bort.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar som inkluderar åtkomst till Ta bort</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till mallen som innehåller behörigheter för att ta bort den</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på vid borttagning av mallar

* De uppgifter som lades till i projekt när mallen bifogades finns kvar i projekten. Den malluppgiftsinformation som är kopplad till uppgifterna tas dock bort.
* Namnet på mallen visas inte längre i **Mall** fält på **Ökning** projektunderflik.

* Du kan återställa en nyligen borttagen mall från papperskorgen. Mer information om hur du återställer objekt från papperskorgen finns i [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Ta bort en mall

{{step1-to-templates}}

Då öppnas en lista med mallar

1. Markera mallen som du vill ta bort genom att klicka i kryssrutan till vänster om mallnamnet och sedan klicka på **Ta bort > Ja, ta bort den** för att bekräfta borttagningen.

   eller

   Klicka på namnet på en mall för att komma åt den och klicka sedan på **Mer** meny ![](assets/qs-more-icon-on-an-object.png) sedan **Ta bort mall > Ja, ta bort den**.

   Mallen är inte längre tillgänglig för att associeras med ett projekt.
