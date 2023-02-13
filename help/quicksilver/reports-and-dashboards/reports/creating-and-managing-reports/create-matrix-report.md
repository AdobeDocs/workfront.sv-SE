---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Skapa en matrisrapport
description: Matrisrapporter visar sammanfattningsinformation i ett aggregerat tabellformat, vilket gör det enklare att visa den än om den visades i en lista som i en traditionell rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Skapa en matrisrapport

Matrisrapporter visar sammanfattningsinformation i ett aggregerat tabellformat, vilket gör det enklare att visa den än om den visades i en lista som i en traditionell rapport.

## När en matrisrapport ska användas

Du kan skapa en matrisrapport för alla rapporter som innehåller 2 eller fler grupperingar. En traditionell rapport kan innehålla upp till tre grupperingar och en matrisrapport kan innehålla upp till fyra grupperingar.

Du vill till exempel skapa en timrapport som visar de timmar som loggats under en 3-månadersperiod, och du vill att rapporten ska vara ordnad efter vem som angav timmarna samt efter månad och vecka.

![](assets/report-matrix-overview-350x123.png)

## Hur data visas i en matrisrapport

Informationen i matrisrapporten visas alltid som ett numeriskt värde. I de flesta fall är kolumner som innehåller ett numeriskt värde bäst för visning i en matrisrapport (till exempel loggade timmar och verkliga kostnader).

Andra kolumner (till exempel Status) kan dock fortfarande visas i matrisrapporten enligt följande bild:\
![](assets/report-matrix-status-350x73.png)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera en matrisrapport

1. Skapa en traditionell rapport som innehåller numeriska data i rapportutdata.\
   Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gå till rapporten som du skapade i steg 1 och klicka på **Rapportåtgärder** väljer **Redigera**.

1. (Villkorligt) Om du redan har skapat en vy och vill använda den på den här rapporten klickar du på **Använd en befintlig vy** väljer du sedan Visa i listrutan.
1. (Villkorligt) Om du vill skapa en ny vy för rapporten utför du följande steg:

   1. Klicka på **Kolumner (vy)** markerar du en kolumn som du vill sammanfatta i matrisrapporten.
   1. I **Kolumninställningar** klickar du på **Sammanfatta den här kolumnen med** och välj sedan ett av de tillgängliga alternativen för att sammanfatta informationen.

      >[!IMPORTANT]
      >
      >Om det här alternativet inte är markerat visas inte informationen från kolumnen korrekt i matrisrapporten.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Upprepa den här processen för varje kolumn på fliken Kolumner (Visa) och klicka sedan på **Klar**.

1. Klicka på **Grupperingar** -fliken.
1. (Villkorligt) Om du redan har skapat en gruppering och vill använda den i den här rapporten klickar du på **Tillämpa en befintlig gruppering** väljer du sedan Gruppering i listrutan.
1. (Villkorligt) Om du vill skapa en ny matrisgruppering för rapporten utför du följande steg:

   1. Välj **Växla till matrisgruppering** i det övre högra hörnet av Builder-gränssnittet.
   1. I **Radgrupperingar** identifierar du radgrupperingen som anger tabellens vågräta grupperingar.
   1. (Valfritt) Om du vill lägga till ytterligare en radgruppering klickar du på **Lägg till sekundär radgruppering**.
   1. I **Kolumngrupperingar** identifierar du kolumngrupperingen som anger tabellens lodräta grupperingar.
   1. (Valfritt) Om du vill lägga till ytterligare en kolumngruppering klickar du på **Lägg till sekundär kolumngruppering**.
   1. (Villkorligt) Om du lägger till en gruppering efter datum anger du även om resultaten grupperas efter dag, vecka, månad, kvartal eller år.\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Villkorligt) Om du valde att gruppera efter datum och att visa resultat efter kvartal, till exempel, anger du om du vill visa kvartal utan data genom att markera **Visa kvartal utan resultat** kryssrutan.\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >The **Visa kvartal utan resultat** -fältet är bara tillgängligt för matrisgrupperingar, och inte för standardgrupperingar.\
      >Endast kvartal utan data som finns mellan två kvartal med giltiga data visar noll för datavärdena på matrisfliken. Kvartal som inte har några data som finns i början och slutet av den tidsram som valts av filtret visas inte alls i matrisgrupperingen. Kvartal utan resultat visas inte i en gruppering på rapportens flik Information.

1. (Valfritt och villkorligt) Klicka på **Matrisinställningar** väljer du sedan något av följande alternativ:\
   **Visa antal poster:** Välj det här alternativet om du vill visa en rad med det totala antalet poster för det angivna fältet.\
   **Visa värdekolumn:** Välj det här alternativet om du vill visa följande information i matrisen:

   * Antal poster
   * Kolumnen Värde

      >[!NOTE]
      >
      >Den här kolumnen innehåller information som beskriver vad data i varje rad representerar.\
      >Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du samlar värden för följande fält i grupperingar:
      >
      >   
      >   
      >   * Alla sifferfält och valutafält utom Faktiska timmar (till exempel Planerad/Faktisk arbetskostnad, Planerad/Faktisk utgiftskostnad, Planerad/Faktisk kostnad, Planerad timmar) samlar endast värdena för de underordnade aktiviteterna och fristående aktiviteter. De sammanställer inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
      >   * Faktiska timmar sammanställer värdena för huvuduppgiften och de fristående uppgifterna. de sammanställer inte siffrorna för överordnade och underordnade uppgifters överordnade uppgifter.
      >   * Anpassade datafält för tal- och valutavärden samlar alla uppgifter: föräldrar, barn, föräldrar till föräldrar och fristående uppgifter. Om du skapade matrisrapporten för att visa Planerade timmar eller Faktiska timmar i **Värde** Tänk på att timmar- och kostnadsinformation för överordnade objekt (t.ex. överordnade uppgifter) inte visas i matrisrapporten. Om du vill visa timmar för överordnade objekt måste du visa **Detaljer** -fliken.

   **Villkorliga regler:** Ange eventuella formateringsregler för sammansatta värden.\
   När du har lagt till en regel kan du definiera fält- och textformat för hur fält som matchar den regeln visas. Klicka **Lägg till regel** när du är klar med att definiera regeln **Klar** för att spara regeln.

1. Klicka på **Filter** för att definiera vilken information som ska visas i rapporten.
1. (Villkorligt) Om du redan har skapat ett filter och vill använda det i den här rapporten klickar du på **Använd ett befintligt filter** väljer du därefter Filter i listrutan.
1. (Villkorligt) Om du vill skapa ett nytt filter för den här rapporten kan du läsa mer i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   för information om de olika kvalificerare som du kan använda när du skapar filter.

1. Klicka **Spara+stäng** för att spara och visa matrisrapporten.
