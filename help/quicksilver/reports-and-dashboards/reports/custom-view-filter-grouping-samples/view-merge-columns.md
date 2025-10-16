---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Sammanfoga information från flera kolumner i en delad kolumn'
description: Du kan sammanfoga informationen som visas i flera separata kolumner och visa den i en delad kolumn.
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Visa: sammanfoga information från flera kolumner i en delad kolumn

<!-- Audited: 11/2024 -->

Du kan sammanfoga informationen som visas i flera separata kolumner och visa den i en delad kolumn.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller begäran om att ändra en vy </p>
   <p>Standard eller Plan för att ändra en rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Att tänka på när du delar eller sammanfogar kolumner

* Du kan sammanfoga två intilliggande kolumner och visa informationen från varje kolumn avgränsad med en radbrytning, eller så kan du sammanfoga informationen i två intilliggande kolumner utan någon avgränsare mellan informationen från varje kolumn.
* Du kan sammanfoga informationen från mer än två kolumner genom att tillämpa samma syntax som beskrivs i den här artikeln på en redan delad kolumn och en intilliggande kolumn.
* Raden `valueformat=HTML` är obligatorisk i en delad kolumn. Annars innehåller kolumnerna ingen information (de är tomma) när rapporten exporteras från Adobe Workfront.
* Villkorsstyrd formatering kanske inte stöds i sammanslagna kolumner.

  Följande undantag finns:

   * När du visar information i Workfront behålls formateringen för den första kolumnen och formateringen för alla andra kolumner ignoreras om de kolumner som utgör en sammanfogad kolumn har en annan formatering än den andra.
   * När du exporterar vyn till en PDF-fil används villkorsstyrd formatering på den första kolumnen i en sammanfogad kolumn.
   * När du exporterar vyn till en Excel-fil visas sammanslagna kolumner som separata kolumner. De enskilda kolumnerna visar också sina respektive villkorliga formateringsregler.

* Kolumner med attributet **viewalias** kan begränsa hur många kolumner du kan sammanfoga. Undvik dessa begränsningar genom att använda attributet **viewalias**. Om du måste ta med attributet **viewalias** i en kolumn kontrollerar du att det är det sista objektet i kolumnen.

* Om du exporterar en lista med delade kolumner till ett Excel- eller tabbavgränsat format separeras dessa kolumner i den exporterade filen.

* När en av eller båda kolumnerna visar ett `tile`-typfält, infogas automatiskt en fast radbrytning i den sammanfogade kolumnen. Textfält med formatering är till exempel `tile` textfält. I det här fallet finns radkoden `type=tile` när kolumnerna visas i textläge.

## Sammanfoga data från två kolumner utan radbrytning

Du kan sammanfoga data från flera separata kolumner så att de visas i en kolumn utan brytningar eller mellanslag mellan värdena från varje kolumn.

>[!TIP]
>
>Det här arbetssättet rekommenderas när du sammanfogar två kolumner som aldrig kan visa ett värde för samma post samtidigt. I en arbetsuppgiftsrapport kan till exempel kolumnerna Utgivningsnamn och Uppgiftsnamn sammanfogas utan en radbrytning mellan dem, eftersom en arbetsuppgift aldrig kan ha ett Frågenamn och ett Uppgiftsnamn samtidigt. En arbetsuppgift kan antingen vara en utgåva eller en uppgift i Workfront.

Så här sammanfogar du data från två kolumner utan radbrytning:

1. Gå till en lista med objekt.
1. I listrutan **Visa** markerar du en vy och klickar sedan på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) för att redigera vyn.
1. Gå till den första kolumnen som du vill sammanfoga och klicka sedan på **Växla till textläge** > **Redigera textläge**.
1. Lägg till följande text i den första kolumnen som du vill sammanfoga:

   `sharecol=true`

   När du sammanfogar de två första kolumnerna i en lista eller rapport kommer Workfront före varje textrad som innehåller information om objektet i den första kolumnen med `column.0.` och textraderna som innehåller information om den andra kolumnen med `column.1.` .

   Du måste före kolumnnumret i den första kolumnen skriva numret på den kolumnen. Kolumninventeringen börjar alltid med kolumnen längst till vänster i listan eller rapporten `column.0.`.

   Om du delar mer än en kolumn måste du lägga till kolumnnumret på de kodrader som innehåller delningsinformationen för varje kolumn.


   **EXEMPEL:** Följande är textlägeskoden för en sammanfogad kolumn som innehåller tre separata kolumner, med början från den andra kolumnen i listan. De sammanfogade värdena är Projektnamn, Planerat startdatum och Projektägarens namn och det finns ingen brytning mellan de tre värdena:

   ```
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.sharecol=true
   column.3.valuefield=owner:name
   column.3.valueformat=HTML
   ```

   ![Delad kolumn utan radbrytningar](assets/shared-column-no-line-breaks-350x142.png)


1. Klicka på **Klar** och sedan på **Spara vy**.

## Sammanfoga data från två kolumner med en radbrytning

Gör följande för att sammanfoga data från flera kolumner så att de visas i en gemensam kolumn med en radbrytning mellan värdena från varje kolumn:

1. Gå till en lista med objekt.
1. I listrutan **Visa** markerar du en vy och klickar sedan på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) för att redigera vyn.
1. Lägg till en tredje kolumn mellan de två kolumner som du vill sammanfoga.

   >[!TIP]
   >
   >* Kolumnerna som du vill sammanfoga måste ligga intill varandra.
   >* Du måste klicka på den första kolumnen som du vill sammanfoga.

1. Klicka på **Växla till textläge** > **Redigera textläge** och lägg till följande kod i den mittersta kolumnen som du lade till i steg 1:

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. Klicka på den första kolumnen och klicka på **Växla till textläge** > **Redigera textläge** och lägg sedan till följande text i kolumnen:

   `sharecol=true`

   När du sammanfogar de två första kolumnerna i en lista eller rapport, kommer Workfront före varje textrad som innehåller information om objektet i den första kolumnen med `column.0.`, kolumnen med delningsinformationen med `column.1.` och textraderna som innehåller information om den andra kolumnen med `column.2.`.

   Om den kombinerade kolumnen är i mitten av vyn numreras kolumnerna efter deras plats i vyn. Kolumninventeringen börjar alltid med kolumnen längst till vänster i listan eller rapporten `column.0.`.

   Om du delar mer än en kolumn måste du lägga till kolumnnumret i kodraderna som innehåller delningsinformationen.

   **EXEMPEL:** Följande är textlägeskoden för en delad kolumn som innehåller Projektnamn, Planerat startdatum och Projektägarens namn med en radbrytning. Den delade kolumnen är den andra kolumnen i en projektvy.

   ```
   column.1.displayname=Project_StartDate_Owner
   column.1.sharecol=true
   column.1.textmode=true
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.2.value=<br>
   column.2.width=1
   column.2.valueformat=HTML
   column.2.sharecol=true
   column.3.valuefield=plannedStartDate
   column.3.valueformat=atDate
   column.3.sharecol=true
   column.4.value=<br>
   column.4.width=1
   column.4.valueformat=HTML
   column.4.sharecol=true
   column.5.textmode=true
   column.5.valuefield=owner:name
   column.5.valueformat=HTML 
   ```

   ![Delad kolumn med radbrytningar](assets/shared-column-with-line-breaks-350x199.png)

1. Klicka på **Klar** och sedan på **Spara vy**.
