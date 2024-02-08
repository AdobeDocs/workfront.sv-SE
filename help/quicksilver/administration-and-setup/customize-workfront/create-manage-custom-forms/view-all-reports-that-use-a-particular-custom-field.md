---
title: Visa alla rapporter som använder ett visst anpassat fält eller en viss widget
description: Du kan lägga till en anpassad vy i området Anpassad Forms som visar vilka rapporter som använder ett visst anpassat fält eller en viss widget. Det här är användbart när du behöver redigera eller ta bort fältet eller widgeten, eftersom det kanske redan har implementerats i en eller flera rapporter. Det är viktigt att utvärdera om dessa rapporter behöver justeras för att fortsätta fungera som de ska.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Visa alla rapporter som använder ett visst anpassat fält eller en viss widget

Du kan lägga till en anpassad vy i området Anpassad Forms som visar vilka rapporter som använder ett visst anpassat fält eller en viss widget. Det här är användbart när du behöver redigera eller ta bort fältet eller widgeten, eftersom det kanske redan har implementerats i en eller flera rapporter. Det är viktigt att utvärdera om dessa rapporter behöver justeras för att fortsätta fungera som de ska.

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Visa rapporter som använder ett visst anpassat fält eller en viss widget

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **Anpassad Forms**.
1. Klicka **Fält** om du vill visa en rapport med en lista över alla anpassade fält och widgetar i din Workfront-instans.

1. Klicka på **Visa** söker du efter anpassade vyer i listan som innehåller **Rapporter** -kolumn (som inte är en standardkolumn på den här fliken).

   I kolumnen Rapporter kan du se vilka rapporter som använder varje anpassat fält och widget som har lagts till i ett anpassat formulär i systemet. Det är möjligt att någon redan har skapat en vy som innehåller **Rapporter** kolumn.

1. Om du inte ser en vy som innehåller **Rapporter** skapar du en ny vy som innehåller den:

   1. Klicka på **Visa** menyn och klicka sedan på **Ny vy**.

   1. På **Ny vy** sida som visas i rutan uppe till vänster, ersätt **Ny parametervy** med ett beskrivande namn för vyn, till exempel *Fält och widgetar*.

   1. Klicka **Lägg till kolumn** nära det nedre högra hörnet.
   1. I **Visa i den här kolumnen** ruta som visas i det övre vänstra hörnet, börja skriva *rapport* väljer **Rapporter** när den visas i listan nedanför rutan.

   1. (Villkorligt) Om du vill flytta **Rapporter** kolumn som du just har lagt till i en annan vågrät position drar i sidhuvudet i **Förhandsgranska kolumn** området längst ned på sidan.

   1. Klicka **Klar** och sedan klicka **Spara vy**.

1. Klicka på **Visa** väljer du namnet på den anpassade vy du just skapade.
1. I **Namn** kolumn, hitta det anpassade fält eller den widget som du vill redigera eller ta bort och titta sedan på **Rapporter** på den raden för att se vilka rapporter som använder den, om det finns någon.

   För att hitta informationen för den här kolumnen söker Workfront efter anpassade fält och widgetar i alla rapportfilter, vyer, grupperingar.

   Om du ser ett plustecken kan du klicka på den textraden för att visa en ruta med alla ytterligare rapporter som använder fältet eller widgeten.

   >[!NOTE]
   >
   >Den inledande inläsningstiden för det här verktyget kan ta mellan 10 sekunder och 2,5 minuter, beroende på mängden data i systemet.

   >[!TIP]
   >
   >Om du inte har tid att undersöka de rapporter som använder det anpassade fältet eller widgeten kan du klicka på Exportera för att skapa en fil som visar dem. Du kan dela den här filen med alla som äger en rapport som använder fältet eller widgeten och diskutera den ändring som behöver göras, vilken effekt den kan ha på rapporten och vad som behöver göras för att se till att rapporten fortsätter att fungera korrekt.
   >
   >Den här vyn är även tillgänglig i en parameterrapport:
   >      
   > 1. Klicka på Huvudmenyn **Rapporter**.
   > 1. Klicka på i det övre vänstra hörnet **Ny rapport** och sedan klicka **Parameter** i listan som visas.
   > 1. Klicka **Lägg till kolumn** nära det nedre högra hörnet.
   > 1. I **Visa i den här kolumnen** ruta som visas i det övre vänstra hörnet, börja skriva *rapport* väljer **Rapporter** när den visas i listan nedanför rutan.
   > 1. (Villkorligt) Om du vill flytta **Rapporter** kolumn som du just har lagt till i en annan vågrät position drar i sidhuvudet i **Förhandsgranska kolumn** området längst ned på sidan.
   > 1. Klicka **Klar** och sedan klicka **Spara+stäng**.
   > 1. Skriv ett beskrivande namn för rapporten, till exempel *Fält och widgetar*.
