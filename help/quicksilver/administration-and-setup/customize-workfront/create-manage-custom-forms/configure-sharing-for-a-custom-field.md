---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Konfigurera delning för anpassade fält och widgetar
description: När du lägger till ett nytt anpassat fält eller en ny widget i ett anpassat formulär kan alla i systemet som har tillgång till anpassade formulär redigera egenskaperna för det objektet, till exempel dess etikett och namn. Du kan ändra detta genom att styra vem det kan delas med.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 0%

---

# Konfigurera delning för anpassade fält och widgetar

När du lägger till ett nytt anpassat fält eller en ny widget i ett anpassat formulär kan alla i systemet som har tillgång till anpassade formulär redigera egenskaperna för det objektet, till exempel dess etikett och namn. Du kan ändra detta genom att styra vem det kan delas med.

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Konfigurera delning för ett anpassat fält eller en anpassad widget

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Anpassad Forms**.
1. Om du konfigurerar delning för ett anpassat fält eller en anpassad widget i din organisations Workfront-instans gör du följande:

   1. Klicka på **Fält** -fliken.
   1. Markera objektet som du vill konfigurera delning för och klicka sedan på **Dela**.

   Om du konfigurerar delning för ett anpassat fält eller en anpassad widget i ett befintligt anpassat formulär gör du så här:

   1. Markera det anpassade formuläret och klicka sedan på **Redigera**.
   1. Markera det objekt som du vill konfigurera delning för i formulärredigeringsområdet till höger.
   1. Klicka på i den vänstra panelen **Delningsfält**.


1. I **Anpassad fältåtkomst** som visas anger du vem du vill dela objektet med och hur du vill dela det:

   1. Nära det nedre vänstra hörnet av **Anpassad fältåtkomst** ruta, under **Ge åtkomst till anpassade fält** börjar du skriva namnet på en användare, ett team, en jobbroll, en grupp eller ett företag som du vill dela objektet med och klickar sedan på namnet när det visas.

      ![](assets/share-field-give-access-to.jpg)

   1. Om du vill ange mer information om hur du vill dela objektet klickar du på listrutan till höger om namnet och använder sedan något av följande alternativ:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Se det</td> 
         <td> <p>Du kan klicka <strong>Avancerade inställningar</strong> för att ange om du vill att användaren eller användarna ska kunna använda sin åtkomst för att lägga till objektet i ett anpassat formulär eller dela det med andra användare.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Hantera det</td> 
         <td> <p>Tillåter åtkomst för att redigera det anpassade fältet och visa det i fältbiblioteket och på sidan där du skapar anpassade formulär.</p> <p>Du kan klicka <strong>Avancerade inställningar</strong> för att ange om du vill att användaren eller användarna ska kunna använda sin åtkomst för att ta bort objektet från systemet eller dela det med andra användare.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra namn i listan och konfigurera deras alternativ.
1. (Valfritt) Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) i det övre högra hörnet om du vill välja ett systemomfattande delningsalternativ för fältet.

   Alla följande alternativ visas inte på den här listrutan samtidigt. Den andra visas till exempel bara när en av de andra två är markerad.

   * **Gör detta redigerbara i hela systemet så att alla i Workfront kan redigera det** (standardalternativet)

      När du lägger till ett anpassat fält eller en anpassad widget, och du inte begränsar delning för det, kan alla i systemet som har tillgång till anpassade formulär visa det och redigera dess egenskaper.

   * **Ta bort redigeringsåtkomst för hela systemet**

      Begränsar åtkomsten till endast dem som du har lagt till i listan.

   * **Gör detta synligt i hela systemet så att alla i Workfront kan se det**

1. Klicka **Spara** eller **Spara + Stäng**.

## Ärvd åtkomst till anpassade fält och widgetar när ett anpassat formulär delas

När någon delar ett anpassat formulär med en grupp, en jobbroll, ett team eller ett företag ärver mottagarna Visa-åtkomst till anpassade fält och widgetar som finns i formuläret. Denna åtkomstnivå till dessa objekt i formuläret behålls alltid så att formuläret kan fungera för mottagarna som det är tänkt av den person som skapade det. Detta gäller även för mottagare som har Redigera-åtkomst till formuläret.

Du kan ta reda på vem som har ärvt åtkomst till ett anpassat fält eller en anpassad widget och du kan ta bort åtkomsten till den.

>[!NOTE]
>
>Om en mottagare har Hantera-åtkomst till ett anpassat fält eller en anpassad widget i det delade anpassade formuläret, behålls åtkomsten för mottagaren.

* [Ta reda på vem som har ärvt åtkomst till ett anpassat fält eller en anpassad widget](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Ta bort åtkomst till ett anpassat fält eller en anpassad widget i ett anpassat formulär som delas](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Ta reda på vem som har ärvt åtkomst till ett anpassat fält eller en anpassad widget {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Anpassad Forms**.
1. Klicka på **Fält** och sedan markera fältet, bilden eller åtkomstwidgeten.
1. I rutan som visas klickar du på **Ärvda behörigheter** och visa namnen som visas.
1. Klicka **Avbryt**.

### Ta bort åtkomst till ett anpassat fält eller en anpassad widget i ett anpassat formulär som delas {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Om du behöver ta bort åtkomsten till ett anpassat fält eller en anpassad widget i ett anpassat formulär som delats, måste du ta bort delningen av formuläret. Instruktioner finns i avsnittet [Ta bort åtkomst till ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) i artikeln [Dela ett eget formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
