---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Visa alla anpassade Forms som använder ett visst anpassat fält eller en viss widget
description: Du kan ta reda på vilka anpassade formulär som använder ett anpassat fält eller en anpassad widget som du vill ändra eller ta bort. Det är viktigt att utvärdera om dessa anpassade formulär behöver justeras för att fortsätta fungera som de ska eller för att fortsätta vara användbart efter att du har ändrat eller tagit bort fältet eller widgeten.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 40722f2b-f8b2-4dc5-805e-2b434a0d46c3
source-git-commit: f4043daeb7a7dad84b6232b5ac133fd59ca64292
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# Visa alla anpassade formulär som använder ett visst anpassat fält eller en viss widget

Du kan ta reda på vilka anpassade formulär som använder ett anpassat fält eller en anpassad widget som du vill ändra eller ta bort. Det är viktigt att utvärdera om dessa anpassade formulär behöver justeras för att fortsätta fungera som de ska eller för att fortsätta vara användbart efter att du har ändrat eller tagit bort fältet eller widgeten.

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr>  
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta reda på vilka anpassade formulär som använder ett visst anpassat fält eller en viss widget

Så här visar du hur ett fält används i listan över alla anpassade fält:

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms** i den vänstra panelen.
1. Klicka på **Fält**, leta efter fältet eller widgeten i kolumnen **Namn** och visa sedan kolumnen **Forms** för att se vilka anpassade formulär som använder fältet eller widgeten.
1. (Valfritt) Klicka på namnet på något av dessa anpassade formulär för att gå till formuläret och fundera på vilka ändringar du behöver göra där om du ändrar fältet eller widgeten.

Så här ser du hur ett fält används i ett anpassat formulär:

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms** i den vänstra panelen.
1. Öppna ett anpassat formulär och lägg till ett fält från biblioteket eller markera ett befintligt fält i formuläret.

   Användningsindikatorn till höger om formulärdesignern visar hur många andra anpassade formulär som använder det här fältet.

1. Klicka på **Visa relaterade Forms**.

   I formulärlistan kan du klicka på ett formulärnamn för att öppna formuläret och se hur fältet används. En indikator visar om varje formulär är aktivt eller inaktivt.


