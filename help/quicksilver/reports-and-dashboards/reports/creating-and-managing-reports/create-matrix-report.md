---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Skapa en matrisrapport
description: Matrisrapporter visar sammanfattningsinformation i ett aggregerat tabellformat, vilket gör det enklare att visa den än om den visades i en lista som i en traditionell rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

# Skapa en matrisrapport

Matrisrapporter visar sammanfattningsinformation i ett aggregerat tabellformat, vilket gör det enklare att visa den än om den visades i en lista som i en traditionell rapport.

## När en matrisrapport ska användas

Du kan skapa en matrisrapport för alla rapporter som innehåller 2 eller fler grupperingar. En traditionell rapport kan innehålla upp till tre grupperingar och en matrisrapport kan innehålla upp till fyra grupperingar.

Du vill till exempel skapa en timrapport som visar de timmar som loggats under en 3-månadersperiod, och du vill att rapporten ska vara ordnad efter vem som angav timmarna samt efter månad och vecka.

![Översikt över rapportmatrisen](assets/report-matrix-overview-350x123.png)

## Hur data visas i en matrisrapport

Informationen i matrisrapporten visas alltid som ett numeriskt värde. I de flesta fall är kolumner som innehåller ett numeriskt värde bäst för visning i en matrisrapport (till exempel loggade timmar och verkliga kostnader).

Andra kolumner (till exempel Status) kan dock fortfarande visas i matrisrapporten enligt följande bild:\
![Matrisstatus](assets/report-matrix-status-350x73.png)

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
      <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera en matrisrapport

1. Skapa en traditionell rapport som innehåller numeriska data i rapportutdata.\
   Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gå till rapporten som du skapade i steg 1, klicka på **Rapportåtgärder** och välj sedan **Redigera**.

1. (Villkorligt) Om du redan har skapat en vy och vill använda den på den här rapporten klickar du på **Använd en befintlig vy** och väljer sedan Visa i listrutan.
1. (Villkorligt) Om du vill skapa en ny vy för rapporten utför du följande steg:

   1. Klicka på fliken **Kolumner (Visa)** och markera sedan en kolumn som du vill ska sammanfattas i matrisrapporten.
   1. I området **Kolumninställningar** klickar du på listrutan **Sammanfatta den här kolumnen med** och väljer sedan ett av de tillgängliga alternativen för att sammanfatta informationen.

      >[!IMPORTANT]
      >
      >Om det här alternativet inte är markerat visas inte informationen från kolumnen korrekt i matrisrapporten.

      ![Matris summerad](assets/qs-report-matrix-summarized-350x392.png)

   1. Upprepa den här processen för varje kolumn på fliken Kolumner (Visa) och klicka sedan på **Klar**.

1. Klicka på fliken **Grupperingar**.
1. (Villkorligt) Om du redan har skapat en gruppering och vill använda den på den här rapporten klickar du på **Använd en befintlig gruppering** och väljer sedan Gruppering i listrutan.
1. (Villkorligt) Om du vill skapa en ny matrisgruppering för rapporten utför du följande steg:

   1. Välj **Växla till matrisgruppering** i det övre högra hörnet av Builder-gränssnittet.
   1. Identifiera radgrupperingen i avsnittet **Radgrupperingar**, som fastställer tabellens vågräta grupperingar.
   1. (Valfritt) Om du vill lägga till ytterligare en radgruppering klickar du på **Lägg till sekundär radgruppering**.
   1. Identifiera kolumngrupperingen i avsnittet **Kolumngrupperingar** som upprättar tabellens lodräta grupperingar.
   1. (Valfritt) Om du vill lägga till ytterligare en kolumngruppering klickar du på **Lägg till sekundär kolumngruppering**.
   1. (Villkorligt) Om du lägger till en gruppering efter datum anger du även om resultaten grupperas efter dag, vecka, månad, kvartal eller år.\
      ![Alternativ för gruppering efter datum](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Villkorligt) Om du har valt att gruppera efter datum och att visa resultat efter kvartal, till exempel, anger du om du vill visa kvartal utan data genom att markera kryssrutan **Visa kvartal utan resultat**.\
      ![Visa kvartal utan resultat](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >Fältet **Visa kvartal utan resultat** är bara tillgängligt för matrisgrupperingar, och inte för standardgrupperingar.\
      >Endast kvartal utan data som finns mellan två kvartal med giltiga data visar noll för datavärdena på matrisfliken. Kvartal som inte har några data som finns i början och slutet av den tidsram som valts av filtret visas inte alls i matrisgrupperingen. Kvartal utan resultat visas inte i en gruppering på rapportens flik Information.

1. (Valfritt och villkorligt) Klicka på **Matrisinställningar** och välj sedan något av följande alternativ:\
   **Visa antal poster:** Välj det här alternativet om du vill visa en rad med det totala antalet poster för det angivna fältet.\
   **Visa värdekolumn:** Välj det här alternativet om du vill visa följande information i matrisen:

   * Antal poster
   * Värdekolumnen

     >[!NOTE]
     >
     >Den här kolumnen innehåller information som beskriver vad data i varje rad representerar.\
     >Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du samlar värden för följande fält i grupperingar:
     >
     >   
     >   
     >   * Alla sifferfält och valutafält utom Faktiska timmar (till exempel Planerad/Faktisk arbetskostnad, Planerad/Faktisk utgiftskostnad, Planerad/Faktisk kostnad, Planerad timmar) samlar endast värdena för de underordnade aktiviteterna och fristående aktiviteter. De sammanställer inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
     >   * Faktiska timmar sammanställer värdena för de huvudsakliga överordnade och de fristående aktiviteterna. De sammanställer inte siffrorna för de överordnade aktiviteternas överordnade eller underordnade aktiviteternas överordnade uppgifter.
     >   * Anpassade datafält för tal- och valutavärden samlar alla uppgifter: överordnade, underordnade, överordnade och fristående uppgifter. Om du har skapat matrisrapporten för att visa Planerade timmar eller Faktiska timmar i kolumnen **Värde** ska du tänka på att timmar eller kostnadsinformation för eventuella överordnade objekt (till exempel överordnade uppgifter) inte visas i matrisrapporten. Om du vill visa timmar för överordnade objekt måste du visa fliken **Detaljer**.
     >   
     >   
     >**Villkorliga regler:** Ange eventuella formateringsregler för sammansatta värden.\

   När du har lagt till en regel kan du definiera fält- och textformat för hur fält som matchar den regeln visas. Klicka på **Lägg till regel** när du har definierat regeln och **Klar** för att spara regeln.

1. Klicka på fliken **Filter** för att definiera vilken information som ska visas i rapporten.
1. (Villkorligt) Om du redan har skapat ett filter och vill använda det på den här rapporten klickar du på **Använd ett befintligt filter** och väljer sedan filtret i listrutan.
1. (Villkorligt) Om du vill skapa ett nytt filter för den här rapporten läser du [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   om du vill ha information om de olika kvalificerare som du kan använda när du skapar filter.

1. Klicka på **Spara+Stäng** för att spara och visa matrisrapporten.
