---
title: Lägga till visningslogik och hoppa över logik i ett anpassat formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan bestämma vilka avsnitt i ett anpassat formulär som ska visas eller hoppas över baserat på vad användaren gör när han eller hon fyller i det.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Lägga till visningslogik och hoppa över logik i ett anpassat formulär

Du kan bestämma vilka avsnitt i ett anpassat formulär som ska visas eller hoppas över baserat på vad användaren gör när han eller hon fyller i det.

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

## Att tänka på när du använder visningslogik och hopplogik

* Om du vill lägga till visningslogik i ett anpassat fält, en widget eller en avsnittsbrytning måste minst ett flervalsfält (alternativknappar, listrutor eller kryssrutor) placeras före det i formuläret.

   Mer information om anpassade fält och widgetar i anpassade formulär finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) och [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Du kan inte lägga till hopplogik i en widget eller avsnittsbrytning. Du kan bara lägga till den i ett flervalsfält (alternativknappar, listrutor eller kryssrutor).

* Du kan lägga till både visningslogik och hopplogik i ett anpassat fält. Följande gäller för det anpassade fältet:

   * Det är ett flervalsfält (alternativknappar, listrutor eller kryssrutor)
   * Det föregås av ett flervalsfält
   * Därefter kommer ett annat anpassat fält

* När du kopierar formulär med visningslogik eller hopplogik kopieras logiken till det nya anpassade formuläret.
* Tänk på följande när du skapar en visningslogikregel för ett anpassat formulär

   * Anpassade fält som inte ingår i en programsats för visningslogik visas som standard i ett anpassat formulär.
   * Du kan skapa logiksatser för visning av flera fält.

* När du redigerar flera objekt samtidigt visas alla anpassade fält i rutan Redigera objekt, inklusive de fält som hoppas över eller döljs.

## Skapa ett exempel på ett anpassat formulär som har visnings- och hopplogik

Det bästa sättet att lära sig att lägga till visnings- och hopplogik i ett anpassat formulär är att använda det praktiska exemplet som förklaras i de två följande avsnitten:

* [Visningslogik](#display-logic)
* [Hoppa över logik](#skip-logic)

### Visningslogik {#display-logic}

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Anpassad Forms** ![](assets/custom-forms-icon.png).

1. Skapa exempelformuläret:

   1. Klicka **Nytt anpassat formulär** och sedan klicka **Projekt** i listrutan.

   1. I **Formulärtitel** ruta, typ **Exempel på eget formulär - Utbildningslogik och hopplogik**.

   1. Klicka **Lägg till ett fält** i det övre vänstra hörnet.
   1. Lägg till ett listrutefält med namnet *Ärendefält* genom att klicka **Listruta** och sedan skriva **Ärendefält** i **Etikett** box.

   1. Under **Val** lägger du till följande alternativ i textrutorna:

      Forskning krävs

      Ingen mer forskning

   1. Klicka **Spara + Stäng** i det nedre vänstra hörnet.

1. Välj den nya **Exempel på eget formulär - Utbildningslogik och hopplogik** eget formulär och klicka sedan på **Redigera**.

1. Lägg till ett nytt textfält med en rad *Annan forskning* genom att klicka **Textfält med en rad** och sedan skriva **Annan forskning** i **Etikett** box.

1. Klicka **Lägg till logik** nära den nedre vänstra sidan av **Redigera eget formulär** skärm.

1. I rutan som visas med **Display Logic** öppnar, ställer in logiken för när **Annan forskning** fältet visas i formuläret genom att klicka **Ärendefält** i den första listrutan, **Forskning krävs** i den andra listrutan, och **Markerad** i den tredje listrutan.
1. Klicka **Spara** för att stänga **Fältlogik** fönster och sedan klicka **Klar** i **Fältinställningar** område.

   Nu när någon väljer **Forskning krävs** i **Ärendefält** nedrullningsbar meny, **Annan forskning** fältet visas.

1. Klicka **Förhandsgranska** för att säkerställa att logiken ser ut som du vill ha den i formuläret.
1. Klicka **Avsluta förhandsgranskning** när du ser att logiken fungerar som förväntat.
1. Klicka **Spara + Stäng** på **Redigera eget formulär** för att spara formuläret och sedan fortsätta till [Hoppa över logik](#skip-logic) nedan.

### Hoppa över logik {#skip-logic}

Hopplogik fungerar ungefär som visningslogik, men fungerar som omvänd: I stället för att visa specifika anpassade flervalsfält baserat på specifika val, bestämmer du vilka som ska hoppas över baserat på användarens val.

Du kan lära dig mer om detta genom att fortsätta att arbeta med exempelformuläret som du skapade i avsnittet [Visningslogik](#display-logic) i den här artikeln:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms**.
1. Markera formuläret **Exempel på eget formulär - Utbildningslogik och hopplogik** som du skapade i stegen ovan och sedan klickar du **Redigera**.

1. Välj det nedrullningsbara fält som du skapade med namnet *Ärendefält*.
1. Klicka på **Lägg till logik** i **Fältinställningar** sidofält.

1. I **Fältlogik** ska du kontrollera att **Hoppa över logik** -fliken är markerad.

1. Ange den första listrutan till **Ingen mer forskning** och den andra listrutan till **Markerad**.

1. I **Hoppa sedan till** nedrullningsbar meny, välja **Formulärets slut.**

   Nu när någon väljer **Ingen mer forskning** i **Ärendefält** det nedrullningsbara fältet, formuläret hoppar över direkt till formulärets slut utan att visa **Annan forskning** fält.

1. Klicka **Spara**.
1. Klicka **Förhandsgranska**  för att säkerställa att logiken används på det sätt du vill.
1. Klicka **Klar** i formulärets nedre vänstra sida.
