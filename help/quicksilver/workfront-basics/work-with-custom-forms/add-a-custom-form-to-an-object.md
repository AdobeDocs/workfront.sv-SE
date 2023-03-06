---
product-area: projects;user-management
keywords: bifoga,använd
navigation-topic: work-with-custom-forms
title: Lägga till ett anpassat formulär i ett objekt
description: Du kan lägga till ett befintligt anpassat formulär till något av objekten som listas nedan. Ett anpassat formulär innehåller anpassade fält där du kan lagra information om objektet.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 0b0140245a636db73ae1b6dc2e4abac2eecc6909
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Lägga till ett anpassat formulär i ett objekt

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Du kan lägga till ett befintligt anpassat formulär till något av objekten som listas nedan. Ett anpassat formulär innehåller anpassade fält där du kan lagra information om objektet.

* Projekt (inklusive affärsärenden)
* Uppgifter
* Problem
* Företag
* Portfolio
* Program
* Dokument
* Användare
* Iterationer
* Utgifter
* Faktureringsposter

Du kan bara lägga till ett anpassat formulär till de typer av objekt som formuläret skapades för.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till de objekt som du hanterar anpassade formulär för</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för objektet som du vill bifoga ett anpassat formulär för.</p> <p>Visa eller högre behörigheter i det anpassade formuläret, med behörighet att <b>Bifoga till anpassade data</b> objekt (projekt, uppgifter och ärenden). Mer information finns i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Dela ett eget formulär</a>.</p> <p>Viktigt: Om du inte har någon planlicens med administrativ åtkomst till Custom Forms måste du ha specifika behörigheter för att åtminstone visa det anpassade formuläret, vilket beskrivs i <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Dela ett eget formulär</a>. Dessa behörigheter måste beviljas dig även om formuläret är synligt i hela systemet. </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättning

Din Workfront-administratör eller en användare med en planlicens och administrativ åtkomst till anpassade formulär måste skapa anpassade formulär i din miljö innan du kan lägga till dem i objekt. Mer information finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Lägga till ett anpassat formulär i ett objekt

Du kan lägga till ett anpassat formulär till ett objekt på två sätt:

* [Lägga till ett anpassat formulär till ett objekt genom att redigera objektet](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Lägga till ett anpassat formulär till ett objekt från området Detaljer](#add-a-custom-form-to-an-object-from-the-details-area)

### Lägga till ett anpassat formulär till ett objekt genom att redigera objektet {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Gå till objektet där du vill lägga till det anpassade formuläret.
1. Klicka på **Mer** meny ![](assets/more-icon.png)och sedan klicka **Redigera** ![](assets/edit-icon.png).
1. Klicka **Anpassad Forms** > **Lägg till Forms** väljer du upp till 10 formulär i listrutan.

1. (Valfritt) Uppdatera informationen i de redigerbara fälten i det anpassade formuläret.

   Du måste uppdatera alla obligatoriska fält i formulären som du lägger till.

1. Klicka **Spara**.

### Lägga till ett anpassat formulär till ett objekt från området Detaljer {#add-a-custom-form-to-an-object-from-the-details-area}

1. Gå till objektet där du vill lägga till det anpassade formuläret.
1. Klicka på **`<Object type>`Detaljer** i den vänstra panelen. Klicka till exempel på **Projektinformation** för att lägga till anpassade formulär i ett projekt eller **Ärendeinformation** för att lägga till anpassade formulär i ett problem.
1. Klicka på **Lägg till anpassat formulär** i det övre högra hörnet och välj sedan upp till 10 anpassade formulär i listan som visas.

   Om formuläret innehåller obligatoriska fält (markerade med en röd asterisk) behöver du inte fylla i dem just nu.

   De markerade formulären kopplas automatiskt till objektet.

1. (Valfritt) Uppdatera informationen i de anpassade fälten i formuläret och klicka sedan på **Spara ändringar**.

## Flera anpassade formulär i ett objekt

Du kan lägga till upp till 10 anpassade formulär för ett givet objekt, så att du kan göra fält tillgängliga för vissa användare och inte för andra, eller så kan du bättre uppfylla formulärkraven för flera projekt.

**Exempel:** Om ett befintligt projekt redan har ett anpassat formulär och fler anpassade fält behövs som finns i ett annat anpassat formulär, kan du lägga till ett andra formulär i projektet med de ytterligare fälten, i stället för att lägga till fälten i det befintliga anpassade formuläret, om dessa fält behövs bara för det här projektet.

## Lägga till ett anpassat formulär till flera objekt samtidigt

Du kan lägga till anpassade formulär till flera objekt genom att markera dem i en lista.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:

>[!NOTE]
>
><span class="preview">For information about adding custom forms to projects in bulk in the Preview environment, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

-->

1. Navigera till en lista med objekt.
1. Markera flera objekt i listan.

1. Klicka på **Mer** meny ![](assets/more-icon.png)klickar du på **Redigera** icon  ![](assets/edit-icon.png)eller bara klicka på **Redigera** icon ![](assets/edit-icon.png).
1. Klicka **Anpassad Forms** i den vänstra panelen.
1. Markera det formulär som du vill koppla till alla markerade objekt i **Gör en markering** nedrullningsbar meny.
   >[!NOTE]
   >
   >Om du inte hittar formuläret i listrutan innebär det att minst ett av objekten redan har det kopplade formuläret. Bestäm vilket objekt som är och ta bort det från markeringen innan du kan lägga till formuläret till de återstående objekten.

1. Klicka **Spara ändringar**.

   Om formuläret innehåller obligatoriska fält (markerade med en röd asterisk) behöver du inte fylla i dem just nu.
