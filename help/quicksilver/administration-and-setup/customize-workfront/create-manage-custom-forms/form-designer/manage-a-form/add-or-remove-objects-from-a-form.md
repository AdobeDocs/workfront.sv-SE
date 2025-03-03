---
title: Lägg till eller ta bort objekttyper från ett befintligt anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan lägga till eller ta bort objekttyper från anpassade formulär med formulärdesignern.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Lägga till eller ta bort objekttyper från ett befintligt anpassat formulär

Du kan lägga till eller ta bort objekttyper från ett befintligt anpassat formulär med formulärdesignern.

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
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td><p>Administrativ åtkomst till anpassade formulär</p></td> 
  </tr>  
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägga till objekttyper i ett befintligt anpassat formulär

Du kan lägga till ytterligare objekttyper i formuläret så att det kan kopplas till flera objekt.

>[!NOTE]
>
>Avsnittsbrytningsbehörigheter kan påverkas av objekttypen. Behörigheten för begränsad redigering för anpassade formuläravsnittsbrytningar är bara tillgänglig för objekttyperna Projekt, Aktivitet, Utgåva och Användare.
>
>Mer information finns i [Hur flera objekttyper kan påverka behörigheten för avsnittsbrytning](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Klicka på **Egen Forms** i den vänstra panelen.

   I den vy som visas kan du granska alla anpassade formulär som har skapats för din organisation. Du kan också se vem som har skapat varje formulär, vilken objekttyp det fungerar med och om det är aktivt.

1. Markera det anpassade formulär som du vill lägga till ytterligare objekttyper i och klicka sedan på ikonen ![Redigera](assets/edit-icon2.png) .

1. Klicka på plustecknet + efter **Objekttyper** längst upp i formuläret och välj sedan önskad typ på menyn som visas. Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

   ![Lägg till nytt objekt](assets/add-new-object.png)

1. Klicka på **Spara och stäng**.

   >[!TIP]
   >
   >Du kan klicka på **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

## Ta bort objekttyper i ett anpassat formulär

Du kan ta bort objekttyper från ett befintligt anpassat formulär. Ett anpassat formulär måste ha minst en objekttyp.

>[!CAUTION]
>
>Om någon redan har kopplat det anpassade formuläret till objekt av den typ som du vill ta bort och lagt till data i det, tas dessa data bort permanent när du tar bort den objekttypen i formuläret. Det kan innehålla historisk information som användarna behöver senare.
>
>I allmänhet rekommenderar vi att du minimerar antalet gånger som du redigerar ett anpassat formulär som redan används. Det finns inget meddelandesystem för att varna personer som använder det anpassade formuläret om dina ändringar.

Så här tar du bort en objekttyp:

{{step-1-to-setup}}

1. Klicka på **Egen Forms** i den vänstra panelen.
1. Markera det anpassade formulär som du vill redigera och klicka sedan på ikonen ![Redigera](assets/edit-icon2.png).
1. Klicka på X på någon av de **objekttyper** som du vill ta bort från formuläret.

   ![Ta bort objekttyper](assets/delete-object-types.png)

1. (Valfritt) Upprepa föregående steg för andra objekttyper som du vill ta bort från formuläret.
1. Klicka på **Använd** och sedan på **Spara och stäng**.
