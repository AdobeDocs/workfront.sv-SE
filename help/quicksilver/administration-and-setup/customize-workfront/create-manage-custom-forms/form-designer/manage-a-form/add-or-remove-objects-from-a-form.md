---
title: Lägga till eller ta bort objekttyper från ett befintligt anpassat formulär med formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan lägga till eller ta bort objekttyper från anpassade formulär med formulärdesignern.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# Lägga till eller ta bort objekttyper från ett befintligt anpassat formulär med formulärdesignern

Du kan lägga till eller ta bort objekttyper från ett befintligt anpassat formulär med formulärdesignern.

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
   <td>
   <p>Aktuell plan: Standard</p>
   <p>eller</p>
   <p>Äldre plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td><p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Lägga till objekttyper i ett befintligt anpassat formulär

Du kan lägga till ytterligare objekttyper i formuläret så att det kan kopplas till flera objekt.

>[!NOTE]
>
>Avsnittsbrytningsbehörigheter kan påverkas av objekttypen. Behörigheten för begränsad redigering för anpassade formuläravsnittsbrytningar är bara tillgänglig för objekttyperna Projekt, Aktivitet, Utgåva och Användare.
>
>Mer information finns i [Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** i den vänstra panelen.

   I den vy som visas kan du granska alla anpassade formulär som har skapats för din organisation. Du kan också se vem som har skapat varje formulär, vilken objekttyp det fungerar med och om det är aktivt.

1. Markera det anpassade formulär som du vill lägga till ytterligare objekttyper i och klicka sedan på **Redigera**.

1. Klicka på plustecknet + efter längst upp i formuläret **Objekttyper** väljer du sedan önskad typ på menyn som visas. Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

   ![](assets/add-new-object.png)

1. Klicka **Spara och stäng**.

   >[!TIP]
   >
   >Du kan klicka **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

## Ta bort objekttyper i ett anpassat formulär

Du kan ta bort objekttyper från ett befintligt anpassat formulär. Ett anpassat formulär måste ha minst en objekttyp.

>[!CAUTION]
>
>Om någon redan har kopplat det anpassade formuläret till objekt av den typ som du vill ta bort och lagt till data i det, tas dessa data bort permanent när du tar bort den objekttypen i formuläret. Det kan innehålla historisk information som användarna behöver senare.
>
>I allmänhet rekommenderar vi att du minimerar antalet gånger som du redigerar ett anpassat formulär som redan används. Det finns inget meddelandesystem för att varna personer som använder det anpassade formuläret om dina ändringar.

Så här tar du bort en objekttyp:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** i den vänstra panelen.
1. Markera det anpassade formulär som du vill redigera och klicka sedan på **Redigera**.
1. Klicka på krysset på någon av **Objekttyper** som du vill ta bort från formuläret, och sedan klicka på **Ta bort** på det varningsmeddelande som visas.

   ![](assets/delete-object-types.png)

1. (Valfritt) Upprepa föregående steg för andra objekttyper som du vill ta bort från formuläret.
1. Klicka **Klar** och sedan klicka **Stäng och spara**.
