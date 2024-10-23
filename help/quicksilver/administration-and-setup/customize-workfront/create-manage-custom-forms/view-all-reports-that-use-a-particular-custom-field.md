---
title: Visa alla rapporter som använder ett visst anpassat fält eller en viss widget
description: Du kan lägga till en anpassad vy i området Anpassad Forms som visar vilka rapporter som använder ett visst anpassat fält eller en viss widget. Det här är användbart när du behöver redigera eller ta bort fältet eller widgeten, eftersom det kanske redan har implementerats i en eller flera rapporter. Det är viktigt att utvärdera om dessa rapporter behöver justeras för att fortsätta fungera som de ska.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Visa alla rapporter som använder ett visst anpassat fält eller en viss widget

Du kan lägga till en anpassad vy i området Anpassad Forms som visar vilka rapporter som använder ett visst anpassat fält eller en viss widget. Det här är användbart när du behöver redigera eller ta bort fältet eller widgeten, eftersom det kanske redan har implementerats i en eller flera rapporter. Det är viktigt att utvärdera om dessa rapporter behöver justeras för att fortsätta fungera som de ska.

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa rapporter som använder ett visst anpassat fält eller en viss widget

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms** i den vänstra panelen.
1. Klicka på **Fält** om du vill visa en rapport över alla anpassade fält och widgetar i din Workfront-instans.

1. Klicka på menyn **Visa** och sök efter anpassade vyer i listan som innehåller kolumnen **Rapporter** (som inte är en standardkolumn på den här fliken).

   I kolumnen Rapporter kan du se vilka rapporter som använder varje anpassat fält och widget som har lagts till i ett anpassat formulär i systemet. Det är möjligt att någon redan har skapat en vy som innehåller kolumnen **Rapporter**.

1. Om du inte ser en vy som innehåller kolumnen **Rapporter** skapar du en ny vy som innehåller den:

   1. Klicka på menyn **Visa** och sedan på **Ny vy**.

   1. Ersätt **Ny parametervy** med ett beskrivande namn för vyn, till exempel *Fält och widgetar*, på sidan **Ny vy** som visas i rutan nära det övre vänstra hörnet.

   1. Klicka på **Lägg till kolumn** i det nedre högra hörnet.
   1. I rutan **Visa i den här kolumnen** som visas nära det övre vänstra hörnet börjar du skriva *rapport* och väljer sedan **Rapporter** när den visas i listan nedanför rutan.

   1. (Villkorligt) Om du vill flytta kolumnen **Rapporter** som du just har lagt till till i en annan vågrät position drar du dess rubrik i området **Förhandsvisning av kolumn** längst ned på sidan.

   1. Klicka på **Klar** och sedan på **Spara vy**.

1. Klicka på listrutan **Visa** och välj sedan namnet på den anpassade vy som du just skapade.
1. I kolumnen **Namn** letar du reda på det anpassade fält eller den widget du vill redigera eller ta bort och tittar sedan i kolumnen **Rapporter** på den raden för att se vilka rapporter som använder det, om det finns några.

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
   > 1. Klicka på **Rapporter** på huvudmenyn.
   > 1. I närheten av det övre vänstra hörnet klickar du på **Ny rapport** och sedan på **Parameter** i listan som visas.
   > 1. Klicka på **Lägg till kolumn** i det nedre högra hörnet.
   > 1. I rutan **Visa i den här kolumnen** som visas nära det övre vänstra hörnet börjar du skriva *rapport* och väljer sedan **Rapporter** när den visas i listan nedanför rutan.
   > 1. (Villkorligt) Om du vill flytta kolumnen **Rapporter** som du just har lagt till till i en annan vågrät position drar du dess rubrik i området **Förhandsvisning av kolumn** längst ned på sidan.
   > 1. Klicka på **Klar** och sedan på **Spara+stäng**.
   > 1. Skriv ett beskrivande namn för rapporten, till exempel *Fält och widgetar*.
