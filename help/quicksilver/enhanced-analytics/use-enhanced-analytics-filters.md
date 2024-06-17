---
title: Använda filter i Förbättrad analys
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Filtren i området Förbättrad analys i Adobe Workfront hjälper dig att fokusera på specifika projekt eller specifika typer av data.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1486'
ht-degree: 0%

---

# Använda filter i Förbättrad analys

<!-- Audited: 12/2023 -->

Filtren i området Förbättrad analys i Adobe Workfront hjälper dig att fokusera på specifika projekt eller specifika typer av data. De typer av filter du använder kan ge dig insikt i:

* Projekt du äger
* Specifika portfölj- eller programvyer
* Viktiga resultatindikatorer för en viss tidsram (vecka, kvartal, räkenskapsår)

Du kan lägga till och ta bort filter efter behov, så bevarar Workfront de filter som du tillämpar även om du loggar ut.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>
      <p>Nytt: Alla</p>
      <p>eller</p>
      <p>Aktuell: Business eller högre</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
      <p>Nytt: Ljus eller högre</p>
      <p>eller</p>
      <p>Aktuell: Granska eller senare</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till projekt</p> <p>Du måste också ha Visa-åtkomst till Uppgifter, Portfolio och Användare för att kunna se specifika filteralternativ för projektfält.</p> <p>Obs! Om begränsningar har valts i <strong>Ange ytterligare begränsningar</strong> i dialogrutan Redigera åtkomstnivå kanske du inte ser all information i filtren eller på sidan Förbättrad analys efter att filtret har tillämpats.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>Visa</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Information om vad som krävs för att använda den förbättrade analysen finns i [Förutsättningar](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Ändra datumintervallfilter {#change-the-date-range-filter}

Som standard visar visualiseringarna i området Förbättrad analys data för de senaste 60 dagarna och de kommande 15 dagarna. Du kan välja ett nytt datumintervall och använda det för alla visualiseringar i området Förbättrad analys. Om du navigerar bort från sidan används standarddatumintervallet nästa gång du går tillbaka.

>[!TIP]
>
>Du kan också använda tangenter på tangentbordet för att navigera till, öppna och välja ett datumintervall från kalenderwidgeten.\
>Mer information finns i [Kortkommandon](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) i artikeln [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

Så här väljer du ett nytt datumintervall:

{{step1-to-analytics}}

1. Klicka på datumintervallfältet längst upp till höger för att öppna kalendervyn.
1. Använd pilarna ovanför kalendern för att hitta månaden för startdatumet och välj sedan startdatumet.

   ![Välj datumintervall](assets/filters-select-date-range-350x344.png)

1. Använd pilarna ovanför kalendern för att hitta månaden för slutdatumet och välj sedan slutdatumet.
1. (Valfritt) Om du vill zooma in ett mindre datumintervall drar du musen från ett specifikt datum till ett annat på en av visualiseringarna.

   Alla visualiseringar på skärmen uppdateras så att de matchar den valda tidsramen, och ett tidsbildrutefilter visas bredvid eventuella befintliga filter. Det här filtret behålls inte om du loggar ut eller navigerar bort från området Förbättrad analys.

   ![Tidsramsfilter](assets/timeframe-filter-350x220.png)

## Lägga till ett filter

Du kan lägga till filter baserat på standardprojektfält, anpassade formulärfält och hemteam som har tilldelats projekt.

>[!TIP]
>
>Du kan också använda tangenterna på tangentbordet för att navigera till och lägga till ett nytt filter.\
>Mer information finns i [Kortkommandon](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) i artikeln [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

* [Lägga till ett projektfältfilter](#add-a-project-field-filter)
* [Lägga till ett anpassat formulärfilter för projekt](#add-a-project-custom-form-filter)
* [Lägg till ett teamfilter](#add-a-team-filter)

### Lägga till ett projektfältfilter {#add-a-project-field-filter}

Med projektfältfilter kan du filtrera data för projekt och uppgifter baserat på de värden som anges i fält som ingår i projekt som standard.

Följande filtertyper för projektfält är tillgängliga:

| Fält | Visade data |
|---|---|
| **Projekt** | Visar endast data för de markerade projekten |
| **Program** | Visar endast data för projekt i de valda programmen |
| **Portfolio** | Visar endast data för projekt i de valda portföljerna |
| **Villkor** | Visar endast data för projekt som senast hade de valda villkoren (på mål, risk eller i problem) |
| **Status** | Visar endast data för projekt som senast hade de valda statusvärdena (fullständig, aktuell, spärrad, avbruten osv.) |
| **Sponsorn** | Visar endast data för projekt med de valda sponsorerna |
| **Projektägare** | Visar endast data för projekt med de valda projektägarna |

Egna formulärfilter fungerar annorlunda. Mer information finns i [Lägga till ett anpassat formulärfilter för projekt](#add-a-project-custom-form-filter).

Så här lägger du till ett projektfältfilter:

{{step1-to-analytics}}

1. Klicka på uppe till vänster **Lägg till filter** väljer du sedan önskad filtertyp.

   >[!NOTE]
   >
   >Olika filtertyper visar olika data. Du kan bara använda en filtertyp i ett filter. När du har valt den går det inte att använda en filtertyp i ett annat projektfältfilter.

1. Leta reda på de värden som du vill se data för genom att ange minst tre tecken i textfältet **Sök** markerar du de värden som du vill inkludera i filtret.

   Om du vill markera alla aktuella värden klickar du på **Markera alla**.

   ![Välj filtervärde](assets/select-filter-value-350x251.png)

1. När du har valt alla önskade värden klickar du på **Använd filter**.

   Projektet räknar med de översta högra uppdateringarna för att återspegla de filter du använder.

1. Upprepa dessa steg för varje filter som du vill lägga till.

   När du lägger till filter visas data i visualiseringarna nedan för upp till 50 projekt.

   >[!TIP]
   >
   >Om du vill visa data för fler än 50 projekt som visas som standard kan du:
   >
   >   * Använd pilarna längst ned till vänster för att visa de kommande 50 projekten i den visualiseringen.\
   >     ![Sidnumreringspil](assets/pagination-350x118.png)
   >   
   >   * Använd **Sortera efter** listruta på en visualisering för att visa projekten i en annan ordning.\
   >     ![Sortera efter meny](assets/sort-by-menu-350x247.png)

   Information om hur du justerar datumintervallet finns i [Ändra datumintervallfilter](#change-the-date-range-filter).

### Lägga till ett anpassat formulärfilter för projekt

Med den anpassade formulärfiltertypen kan du filtrera data för projekt och uppgifter baserat på värdena som anges i anpassade formulärfält i projekt. Till skillnad från andra typer av förbättrade analysfilter kan du lägga till fler än ett anpassat formulärfilter. Varje eget formulärfilter innehåller värden som bara anges i det markerade fältet i ett specifikt anpassat formulär.

Så här lägger du till ett eget formulärfilter:

{{step1-to-analytics}}

1. Klicka på i skärmens övre vänstra hörn **Lägg till filter** väljer **Eget formulär**.

   ![Välj eget formulärfilter](assets/select-custom-form-filter-350x271.png)

1. Leta reda på det anpassade formuläret som du vill ha genom att ange minst tre tecken i texten **Sök** markerar du det anpassade formuläret.
1. Markera fältet som du vill använda och utför sedan en av följande åtgärder baserat på vilken typ av fält du lägger till i filtret:

   >[!NOTE]
   >
   >Alla anpassade korm-fälttyper kan inte läggas till i ett filter. Förbättrad analys har för närvarande bara stöd för de fälttyper som listas nedan.

   * **Kryssruta**, **nedrullningsbar**, eller **alternativknapp**: Välj varje värde i fältet som du vill ta med i filtret eller klicka på **Markera alla** kryssruta.\
     ![Kryssrutevärden](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Använd pilarna för att navigera till en viss månad och välj sedan datumet i fältet som du vill ta med i filtret.\
     ![Datumvärde](assets/custom-form-filter-date-350x348.png)

   * **Text**: Ange texten i fältet som du vill ta med i filtret.\
     ![Textvärde](assets/custom-form-filter-text-350x90.png)

   * **Nummer**: Ange numret i fältet som du vill ta med i filtret.\
     ![Nummervärde](assets/custom-form-filter-number-350x93.png)

1. När du har angett eller valt de värden som du vill filtrera efter klickar du på **Använd filter**.

   Projektet räknar med de översta högra uppdateringarna för att återspegla de filter du använder.

1. Upprepa dessa steg för varje filter som du vill lägga till.

   När du lägger till filter visas data i visualiseringarna nedan för upp till 50 projekt.

   >[!TIP]
   >
   >Om du vill visa data för fler än 50 projekt som visas som standard kan du:
   >  
   >   * Använd pilarna längst ned till vänster för att visa de kommande 50 projekten i den visualiseringen.\
   >     ![Sidbrytningspilar](assets/pagination-350x118.png)
   >   
   >   * Använd **Sortera efter** listruta på en visualisering för att visa projekten i en annan ordning.\
   >     ![Sortera efter meny](assets/sort-by-menu-350x247.png)

   Information om hur du justerar datumintervallet finns i [Ändra datumintervallfilter](#change-the-date-range-filter).

### Lägg till ett teamfilter {#add-a-team-filter}

{{step1-to-analytics}}

1. Klicka på i den vänstra panelen **Folk**.

   ![Välj personer](assets/people-area-cropped-qs-350x276.png)

1. Klicka på längst upp till vänster på skärmen **Lägg till filter** väljer du **Team** filter.
1. Hitta de team du vill se data för genom att ange minst tre tecken i **Sök** markerar du de team som du vill inkludera i filtret. Om du vill välja alla team klickar du **Markera alla**.

   ![Välj team](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Alla team inkluderas som filteralternativ, oavsett din åtkomstnivå.

1. När du har valt ut alla önskade team klickar du på **Använd filter**.

   När du lägger till filter visas data i visualiseringarna nedan.

   Information om hur du justerar datumintervallet finns i [Ändra datumintervallfilter](#change-the-date-range-filter).

## Ta bort ett filter

Du kan ta bort ett filter när du vill. Om du tar bort ett filter visas det inte nästa gång du besöker området Förbättrad analys.

>[!TIP]
>
>Du kan också använda tangenterna på tangentbordet för att navigera till och ta bort ett befintligt filter.\
>Mer information finns i [Kortkommandon](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) i artikeln [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

Ta bort ett filter:

{{step1-to-analytics}}

1. Om du vill ta bort ett projektfält eller ett eget formulärfilter finns du kvar i **Arbete** område.

   eller

   Om du vill ta bort ett teamfilter väljer du **Folk** till vänster.

1. Leta reda på det önskade filtret och klicka på **X** för att ta bort den.

   ![Ta bort](assets/remove-filter-350x213.png)

   Filtret är inte längre aktivt och visas inte om du inte lägger till det igen.
