---
title: Lägg till visningslogik och hoppa över logik med formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan bestämma vilka avsnitt i ett anpassat formulär som ska visas eller hoppas över baserat på vad användaren gör när han eller hon fyller i det.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 2280019a7cc02c0730f85c010dc8cc08834535aa
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 0%

---

# Lägg till visningslogik och hoppa över logik med formulärdesignern

<span class="preview">Informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Andra utgåvan, kvartal 2024, översikt](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Du kan bestämma vilka avsnitt i ett anpassat formulär som ska visas eller hoppas över baserat på vad användaren gör när han eller hon fyller i det.

>[!NOTE]
>
>Logiken används bara i ett formulär och kan inte baseras på val från ett annat formulär.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront </td> 
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
   <td>Administrativ åtkomst till anpassade formulär </td> 
  </tr>  
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Visa och hoppa över logiska ikoner

Anpassade formulär visar ikoner som anger vilken logik som används i vissa fält. Ikoner i ett fält i formulärdesignern anger att logik används i fältet.

| Ikon | Placering i fält i formulärdesignern | Definition |
|--- |--- |--- |
| ![Visningslogik för målfält](assets/display-logic-bottom-left.png) | Nederst till vänster | Fältet är målfält för visningslogik. Om du har gjort en viss markering i formuläret visas det här fältet. |
| ![Definiera ikon för visningslogik](assets/display-logic-bottom-right.png) | Nederst till höger | Fältet definierar visningslogik. Målfältet visas när du väljer eller anger ett värde i det här fältet. |
| ![Hoppa över logik för målfält](assets/skip-logic-bottom-left.png) | Nederst till vänster | Fältet är målfält för hopplogik. Om formuläret är markerat hoppar formuläret framför det här fältet och fälten däremellan döljs. |
| ![Definiera ikon för hopplogik](assets/skip-logic-bottom-right.png) | Nederst till höger | Fältet definierar hopplogik. En specifik markering eller ett specifikt värde i det här fältet hoppar över andra fält och går direkt till målfältet. |

![Logic icons](assets/logic-icons-3.png)

Välj ett fält med den logik som används för att visa de befintliga logikreglerna i fältinställningarna.

![Logikregler](assets/form-designer-view-only-logic.png)

## Att tänka på när du använder visningslogik och hopplogik

* Om du vill lägga till visningslogik i ett anpassat fält, en widget eller en avsnittsbrytning måste minst ett flervalsfält (alternativknappar, listrutor eller kryssrutor) placeras före det i formuläret.
Mer information om anpassade fält och widgetar i anpassade formulär finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Du kan inte lägga till hopplogik i en widget eller avsnittsbrytning. Du kan bara lägga till den i ett flervalsfält (alternativknappar, listrutor eller kryssrutor).
* Du kan lägga till både visningslogik och hopplogik i ett anpassat fält om allt av följande gäller för det anpassade fältet:

   * Det är ett flervalsfält (alternativknappar, listrutor eller kryssrutor)
   * Det föregås av ett flervalsfält
   * Därefter kommer ett annat anpassat fält

* När du kopierar formulär med visningslogik eller hopplogik kopieras logiken till det nya anpassade formuläret.
* När du redigerar flera objekt samtidigt visas alla anpassade fält i rutan Redigera objekt, inklusive de fält som hoppas över eller döljs.
* Tänk på följande när du skapar en visningslogikregel för ett anpassat formulär:

   * Anpassade fält som inte ingår i en programsats för visningslogik visas som standard i ett anpassat formulär.
   * Du kan skapa logiksatser för visning av flera fält.
   * Om alla fält under en avsnittsbrytning har visningslogik och alla är dolda som ett resultat av logiken, döljs hela avsnittet i det anpassade formuläret.

## Lägga till visningslogik i ett anpassat formulär

Visningslogik definierar vilka anpassade fält som visas i formuläret när användaren väljer ett specifikt värde i ett flervalsfält. Logiken läggs till i målfältet, som bara visas när värdet är markerat.

{{step-1-to-setup}}

1. Klicka **Anpassad Forms**.
1. Skapa ett nytt anpassat formulär eller öppna ett befintligt formulär. Se [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) för mer information.
1. Lägg till fält i formuläret efter behov. Minst ett flervalsfält (alternativknapp, listruta eller kryssruta) måste placeras före målfältet som ska visas.
1. Markera målfältet och klicka på **Lägg till logik** längst ned till vänster på skärmen.
1. Välj **Display Logic** -fliken.
1. Klicka **Lägg till visningsregel** på logikverktyget.

   ![Display logic builder](assets/custom-form-logic-builder-display-blank.png)

1. Följ stegen nedan i verktyget för att skapa logiksatsen.

   1. Det första alternativet är att välja definieringsfältet. Det här är fältet med det urvalsvärde som visar målet. Det måste vara ett flervalsfält.
   1. Det andra alternativet är att välja markeringsvärdet. Endast de värden som redan har definierats för det fältet är tillgängliga.
   1. Det tredje alternativet är **Markerad** eller **Inte markerad**. Välja **Markerad** innebär att när värdet är markerat visas målfältet. Välja **Inte markerad** innebär att när något annat värde är markerat i definitionsfältet visas målfältet.
   1. Lägga till en **Och** rule to the logic statement, click **Lägg till regel** direkt under den regel du just skapade. Följ samma instruktioner för att skapa regeln. Alla And-regler måste uppfyllas för att målfältet ska visas.

      ![Display logic builder](assets/custom-form-logic-builder-display1.png)

   1. Lägga till en **eller** rule to the logic statement, click **Lägg till regel** nära botten av logikbyggaren. Klicka sedan på **Lägg till regel** i området Eller och följ samma instruktioner för att skapa regeln. När en eller-regel är uppfylld visas målfältet.

1. Klicka **Spara** när du är klar med att skapa logiksatsen.

   Ikonerna för visningslogik läggs till i målfältet och i definitionsfältet i formulärdesignern.

>[!NOTE]
>
><span class="preview">Visningslogik är bara tillgänglig när du förhandsgranskar formuläret i formulärdesignern i förhandsgranskningsmiljön.</span>

## Lägga till hopplogik i ett anpassat formulär

Hopplogik definierar anpassade formulärfält som hoppas över när användaren väljer ett specifikt värde i ett flervalsfält. Överhoppade fält är dolda i formuläret. Logiken tillämpas på det definierande fältet där markeringen görs, inte på de fält som hoppas över.

{{step-1-to-setup}}

1. Klicka **Anpassad Forms**.
1. Skapa ett nytt anpassat formulär eller öppna ett befintligt formulär. Se [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) för mer information.
1. Lägg till fält i formuläret efter behov. Det definierande fältet för hopplogik måste vara ett flervalsfält (alternativknapp, listruta eller kryssruta).
1. Markera definitionsfältet och klicka på **Lägg till logik** längst ned till vänster på skärmen.
1. Välj **Hoppa över logik** -fliken.
1. Klicka **Lägg till hoppregel** på logikverktyget.

   ![Hoppa över logikbyggaren](assets/custom-form-logic-builder-skip-blank.png)

1. Följ stegen nedan i verktyget för att skapa logiksatsen.

   1. Definitionsfältet visas i byggaren. Det är fältet som du valde att tillämpa hopplogiken på.
   1. Det första alternativet är att välja markeringsvärdet. Endast de värden som redan definierats för fältet är tillgängliga.
   1. Det andra alternativet är **Markerad** eller **Inte markerad**. Välja **Markerad** innebär att när värdet är markerat visas målfältet och fälten däremellan hoppas över. Välja **Inte markerad** innebär att när något annat värde är markerat i definitionsfältet, visas målfältet och fälten däremellan hoppas över.
   1. Det tredje alternativet är målfältet eller var du vill hoppa till. Välj ett fältnamn eller **Formulärets slut**. Du kan behöva klicka på ordet&quot;tom&quot; innan du väljer ett alternativ.

      ![Hoppa över logikbyggaren](assets/custom-form-logic-builder-skip1.png)

   1. Lägga till en **eller** rule to the logic statement, click **Lägg till regel** nära botten av logikbyggaren. Välj sedan de alternativ som följer samma anvisningar för att skapa regeln. När en **eller** -regeln är uppfylld, målfältet visas.

1. Klicka **Spara** när du är klar med att skapa logiksatsen.

   Ikonerna för hopplogik läggs till i målfältet och definieringsfältet i formulärdesignern.

>[!NOTE]
>
><span class="preview">Hopplogik är bara tillgänglig när du förhandsgranskar formuläret i formulärdesignern i förhandsgranskningsmiljön.</span>
