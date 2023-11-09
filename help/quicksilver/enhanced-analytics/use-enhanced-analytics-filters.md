---
title: Använda filter i Förbättrad analys
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Filtren i området Förbättrad analys hjälper dig att fokusera på specifika projekt eller specifika typer av data.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 0%

---

# Använda filter i Förbättrad analys

Filtren i området Förbättrad analys hjälper dig att fokusera på specifika projekt eller specifika typer av data. De typer av filter du använder kan ge dig insikt i:

* Projekt du äger
* Specifika portfölj- eller programvyer
* Viktiga resultatindikatorer för en viss tidsram (vecka, kvartal, räkenskapsår)

Du kan lägga till och ta bort filter efter behov, så bevarar Adobe Workfront de filter som du tillämpar även om du loggar ut.

## Åtkomstkrav

Du måste ha följande för att kunna slutföra den här uppgiften:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront</a>*</p> </td> 
   <td>Företag eller högre</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>*</p> </td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Åtkomstnivå*</b> </td> 
   <td> <p>Visa åtkomst till projekt</p> <p>Du måste också ha Visa-åtkomst till Uppgifter, Portfolio och Användare för att kunna se specifika filteralternativ för projektfält.</p> <p>Obs! Om begränsningar har valts i avsnittet Ange ytterligare begränsningar i dialogrutan Redigera åtkomstnivå kanske du inte ser all information i filtren eller på sidan Förbättrad analys efter att filtret har tillämpats. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Objektbehörigheter</b> </p> </td> 
   <td> <p>Visa</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Information om vad som krävs för att använda den förbättrade analysen finns i [Förutsättningar](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

## Ändra datumintervallfilter {#change-the-date-range-filter}

Som standard visar visualiseringarna i området Förbättrad analys data för de senaste 60 dagarna och de kommande 15 dagarna. Du kan välja ett nytt datumintervall och använda det för alla visualiseringar i området Förbättrad analys. Om du navigerar bort från sidan används standarddatumintervallet nästa gång du går tillbaka.

>[!TIP]
>
>Du kan också använda tangenter på tangentbordet för att navigera till, öppna och välja ett datumintervall från kalenderwidgeten.\
>Mer information finns i [Kortkommandon](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) i artikeln [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

Så här väljer du ett nytt datumintervall:

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Klicka på datumintervallfältet i skärmens övre högra hörn för att öppna kalendervyn.
1. Använd pilarna ovanför kalendern för att hitta månaden för startdatumet och välj sedan startdatumet.

   ![](assets/filters-select-date-range-350x344.png)

1. Använd pilarna ovanför kalendern för att hitta månaden för slutdatumet och välj sedan slutdatumet.
1. (Valfritt) Om du vill zooma in ett mindre datumintervall drar du musen från ett specifikt datum till ett annat på en av visualiseringarna.

   Alla visualiseringar på skärmen uppdateras för att matcha den valda tidsramen och ett tidsbildrutefilter visas bredvid eventuella befintliga filter. Det här filtret behålls inte om du loggar ut eller navigerar bort från området Förbättrad analys.

   ![](assets/timeframe-filter-350x220.png)

## Lägga till ett filter

Du kan lägga till filter baserat på standardprojektfält, anpassade formulärfält och hemteam som tilldelats projekt.

>[!TIP]
>
>Du kan också använda tangenterna på tangentbordet för att navigera till och lägga till ett nytt filter.\
>Mer information finns i [Kortkommandon](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) i artikeln [Förbättrad analys - översikt](../enhanced-analytics/enhanced-analytics-overview.md).

* [Lägga till ett projektfältfilter](#add-a-project-field-filter)
* [Lägga till ett projektfältfilter](#add-a-project-field-filter)
* [Lägg till ett teamfilter](#add-a-team-filter)

### Lägga till ett projektfältfilter {#add-a-project-field-filter}

Med projektfältfilter kan du filtrera data för projekt och uppgifter baserat på de värden som anges i fält som ingår i projekt som standard.

Följande filtertyper för projektfält är tillgängliga:

| **Projekt** | Visar endast data för de markerade projekten |
|---|---|
| **Program** | Visar data endast för projekt i de markerade programmen |
| **Portfolio** | Visar data endast för projekt i de valda portföljerna |
| **Villkor** | Visar data endast för projekt som senast hade de valda villkoren (på mål, risk eller i problem) |
| **Status** | Visar data endast för projekt som senast hade de markerade statusarna (fullständig, aktuell, spärrad, avbruten osv.) |
| **Sponsorn** | Visar data endast för projekt med de valda sponsorerna |
| **Projektägare** | Visar data endast för projekt med de valda projektägarna |

{style="table-layout:auto"}

Egna formulärfilter fungerar annorlunda. Mer information finns i [Lägga till ett projektfältfilter](#add-a-project-field-filter).

Så här lägger du till ett projektfältfilter:

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Klicka på i skärmens övre vänstra hörn **Lägg till filter** väljer du sedan önskad filtertyp.

   >[!NOTE]
   >
   >Olika filtertyper visar olika data. Du kan bara använda en filtertyp i ett filter. När du har valt det här alternativet är en filtertyp inte tillgänglig för användning i ett annat projektfältfilter.

1. Leta upp de värden som du vill se data för genom att ange minst tre tecken i textfältet **Sök** markerar du de värden som du vill inkludera i filtret.

   Om du vill markera alla aktuella värden klickar du på **Markera alla**.

   ![](assets/select-filter-value-350x251.png)

1. När du har valt alla önskade värden klickar du på **Använd filter**.\
   Projektantalet i det övre högra hörnet av sidan uppdateras för att återge de filter som används.
1. Upprepa dessa steg för varje filter som du vill lägga till.

   När du lägger till filter visas data i visualiseringarna nedan för upp till 50 projekt.

   >[!TIP]
   >
   >Om du vill visa data för fler än 50 projekt som visas som standard kan du:
   >
   >   
   >   
   >   * Använd pilarna i det nedre vänstra hörnet för att visa de nästa 50 projekten i den visualiseringen.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Använd listrutan Sortera efter i en visualisering för att visa projekten i en annan ordning.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Information om hur du justerar datumintervallet finns i [Ändra datumintervallfilter](#change-the-date-range-filter).

### Lägg till ett anpassat formulärfilter för projekt

Med filtertypen Anpassat formulär kan du filtrera data för projekt och uppgifter baserat på de värden som anges i anpassade formulärfält i projekt. Till skillnad från andra typer av förbättrade analysfilter kan du lägga till fler än ett filter för anpassade formulär. Varje filter för anpassat formulär innehåller värden som bara anges i det valda fältet i ett specifikt anpassat formulär.

Så här lägger du till ett eget formulärfilter:

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Klicka på i skärmens övre vänstra hörn **Lägg till filter** väljer **Eget formulär**.

   ![](assets/select-custom-form-filter-350x271.png)

1. Leta reda på det anpassade formuläret som du vill ha genom att ange minst tre tecken i texten i dialogrutan **Sök** markerar du det anpassade formuläret.
1. Markera fältet som du vill använda och utför sedan en av följande åtgärder baserat på vilken typ av fält du lägger till i filtret:

   >[!NOTE]
   >
   >Alla anpassade formulärfältstyper kan inte läggas till i ett filter. Förbättrad analys har för närvarande bara stöd för de fälttyper som listas ovan.

   * **Kryssruta**, **nedrullningsbar**, eller **alternativknapp**: Välj varje värde i det markerade fältet som du vill ta med i filtret eller klicka på **Markera alla** kryssrutan.\
     ![](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Använd pilarna för att navigera till en viss månad och välj sedan datumet i det markerade fältet som du vill ta med i filtret.\
     ![](assets/custom-form-filter-date-350x348.png)

   * **Text**: Ange texten i det markerade fältet som du vill ta med i filtret.\
     ![](assets/custom-form-filter-text-350x90.png)

   * **Nummer**: Ange numret i det markerade fältet som du vill ta med i filtret.\
     ![](assets/custom-form-filter-number-350x93.png)

1. När du har angett eller valt de värden som du vill filtrera efter klickar du på **Använd filter**.

   Projektantalet i det övre högra hörnet av sidan uppdateras för att återge de filter som används.

1. Upprepa dessa steg för varje filter som du vill lägga till.

   När du lägger till filter visas data i visualiseringarna nedan för upp till 50 projekt.

   >[!TIP]
   >
   >Om du vill visa data för fler än 50 projekt som visas som standard kan du:
   >
   >   
   >   
   >   * Använd pilarna i det nedre vänstra hörnet för att visa de nästa 50 projekten i den visualiseringen.\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * Använd listrutan Sortera efter i en visualisering för att visa projekten i en annan ordning.\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   Information om hur du justerar datumintervallet finns i [Ändra datumintervallfilter](#change-the-date-range-filter).

### Lägg till ett teamfilter {#add-a-team-filter}

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Klicka på i den vänstra panelen **Folk**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. Klicka på i skärmens övre vänstra hörn **Lägg till filter** väljer du **Team** filter.
1. Hitta de team du vill se data för genom att ange minst tre tecken i **Sök** markerar du de team som du vill inkludera i filtret. Om du vill välja alla team klickar du **Markera alla**.

   ![](assets/select-team-value-350x253.png)

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

1. Klicka på ikonen Huvudmeny ![](assets/main-menu-icon-16x12.png)väljer **Analyser**.
1. Om du vill ta bort ett arbetsfilter finns det kvar i **Arbete** område.

   eller

   Om du vill ta bort ett personfilter väljer du **Folk** till vänster.

1. Leta reda på det önskade filtret och klicka på **X** för att ta bort den.

   ![](assets/remove-filter-350x213.png)

   Filtret är inte längre aktivt och visas inte om du inte lägger till det igen.
