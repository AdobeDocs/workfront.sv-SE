---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Skapa en anpassad rapport
description: Du kan ge åtkomst till den information din organisation behöver inom Adobe Workfront genom att skapa rapporter. Du kan använda någon av de inbyggda rapporterna i Workfront eller skapa anpassade rapporter från grunden.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1817'
ht-degree: 0%

---


# Skapa en anpassad rapport

<!--Audited: 10/2024-->

Du kan ge åtkomst till den information din organisation behöver i Adobe Workfront genom att skapa rapporter. Du kan använda någon av de inbyggda rapporterna i Workfront eller skapa anpassade rapporter från grunden.

Mer information om inbyggda rapporter finns i [Använda inbyggda Adobe Workfront-rapporter](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Mer information om hur du skapar en rapport genom att kopiera den finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Mer information om hur du skapar och hanterar rapporter, inklusive klasser, videoklipp och självstudiekurser, finns i avsnittet Lär dig på Adobe Experience League-webbplatsen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Standard </p>
   eller
   <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Du får behörigheten Hantera för de rapporter du skapar.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en rapport {#create-a-report}

{{step1-to-reports}}

1. Klicka på **Ny rapport** och välj sedan önskad objekttyp för rapporten.

   Report builder läses in.

   Mer information om tillgängliga objektrapporter finns i avsnittet [Rapport om objekt](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![Välj ny rapport](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Du kan också skapa en rapport genom att skapa en kopia av en befintlig rapport. Mer information finns i [Skapa en kopia av en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. (Valfritt) Om du vill redigera titeln för den nya rapporten anger du önskad rapportrubrik i textfältet i det övre vänstra hörnet av rapportverktyget. Vi rekommenderar att du endast använder UTF-8-tecken för att undvika kompatibilitetsproblem.

1. Lägg till följande i rapporten i Report Builder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Funktion</th> 
      <th>Beskrivning</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Kolumner (vy)</td> 
      <td> <p>Om du lägger till kolumner i rapporten avgör du vilken information rapporten innehåller.</p> <p>Mer information om hur du lägger till en kolumn finns i <a href="#add-columns-view-to-a-report" class="MCXref xref">Lägga till kolumner (vy) i en rapport</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Grupperingar</td> 
      <td> <p>Om du lägger till grupperingar i rapporten avgör du hur rapporten är organiserad.</p> <p>Mer information om hur du lägger till en gruppering finns i <a href="#add-groupings-to-a-report" class="MCXref xref">Lägga till grupperingar i en rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filter</td> 
      <td> <p>Om du lägger till filterregler i rapporten avgör du vilken information som visas i rapporten.</p> <p>Mer information om hur du lägger till ett filter finns i <a href="#add-filters-to-a-report" class="MCXref xref">Lägga till filter i en rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Diagram</td> 
      <td> <p>Om du lägger till ett diagram i rapporten avgör du hur informationen i rapporten presenteras visuellt.</p> <p>Mer information om hur du lägger till ett diagram finns i <a href="#add-a-chart-to-a-report" class="MCXref xref">Lägga till ett diagram i en rapport</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Använd** när som helst under rapportskapandeprocessen för att spara ändringarna.
1. När du är klar klickar du på **Spara + stäng**.

### Lägga till kolumner (vy) i en rapport {#add-columns-view-to-a-report}

1. Börja skapa en rapport enligt beskrivningen i avsnittet [Skapa en rapport](#create-a-report) i den här artikeln.
1. I rapportbyggaren väljer du fliken **Kolumner (Visa)** för att identifiera de kolumner som ska visas i rapporten.
1. (Valfritt) Klicka på **Använd en befintlig vy** och klicka på namnet på en vy i listrutan om du vill använda en befintlig vy.

   Mer information om hur du skapar en vy finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Valfritt) Om du vill ta bort en befintlig kolumn klickar du på kolumnen som du vill ta bort och sedan på **x** bredvid det aktuella namnet i kolumnrubriken.

1. Om du vill lägga till en ny kolumn klickar du på **Lägg till kolumn**.

   eller

   Om du vill ändra en befintlig kolumn klickar du på kolumnen, klickar på ikonen **Ta bort** ![Ta bort kolumn-ikonen](assets/remove-column-icon.png) till höger om det aktuella fältet i området **Visa i det här kolumnfältet** i det övre vänstra hörnet i rapportverktyget och börjar skriva ett nytt fält och klickar sedan på det när det visas i listan.

   Mer information om fälten som visas i kolumnerna finns i [Ordlista för Adobe Workfront-terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![Lägg till kolumntyphuvud](assets/nwe-add-column-typeahead-350x459.png)

1. (Valfritt) I området **Kolumninställningar** väljer du **Sortera efter den här kolumnen** för att sortera värdena i kolumnen i stigande alfabetisk ordning och anger sedan om listan ska använda den här kolumnen som första sortering.

   Du kan ha flera sorteringsnivåer i en rapportvy om du vill sortera efter värdet i en kolumn först, värdet i en andra kolumn, osv.

   Om flera resultat är identiska enligt det första sorteringsvillkoret sorteras de i ordningen för det andra sorteringsvillkoret. Om flera resultat är identiska enligt det första och det andra sorteringsvillkoret, sorteras de efter den tredje sorteringen osv.

   >[!NOTE]
   >
   >Om du lägger till ett fält som refererar till ett objekt som är för långt bort från det objekt som du rapporterar om, kanske du inte kan sortera efter det här fältet.\
   >En problemrapport kan till exempel inte sorteras efter fältet Projektägare eftersom den refererar till ytterligare tre objekt: Projekt, Ägare och Namn. Du kan dock fortfarande lägga till det här fältet i en problemrapport och se informationen för det.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Valfritt) Om du använder grupperingar och vill sammanfatta (sammanfoga) informationen i en kolumn, klickar du på listrutan **Sammanfatta den här kolumnen med** i området **Kolumninställningar** och väljer sedan det alternativ som du vill använda för att samla informationen i kolumnen.

   Den aggregerade informationen visas i kolumnen i grupperingsraderna.

   ![Sammanställd sammanfattning för grupperingar](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Mer information om hur du summerar data i en kolumn finns i [Vyöversikt i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Följande undantag gäller för överordnade objekt (till exempel överordnade uppgifter) när du samlar värden för följande fält i grupperingar:
   >
   >* Alla sifferfält och valutafält utom Faktiska timmar (t.ex. Planerad eller Faktisk arbetskostnad, Planerad eller Faktisk kostnad, Planerad eller Faktisk kostnad, Planerad timmar) samlar endast värdena för de underordnade aktiviteterna och fristående aktiviteter. De sammanställer inte värdena för de överordnade uppgifterna eller de överordnade överordnade uppgifterna.
   >* Faktiska timmar sammanställer värdena för de huvudsakliga överordnade och de fristående aktiviteterna. De sammanställer inte siffrorna för de överordnade aktiviteternas överordnade eller underordnade aktiviteternas överordnade uppgifter.
   >* Anpassade datafält för tal- och valutavärden samlar alla uppgifter: överordnade, underordnade, överordnade och fristående uppgifter.

   Mer information om hur du använder grupperingar i en rapport finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Valfritt) Klicka på **Avancerade alternativ** för att ange följande information för kolumnen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett för anpassad kolumn</td> 
      <td> <p>Ange en anpassad etikett för kolumnen. Den här etiketten ersätter standardetiketten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fältformat</td> 
      <td> <p>Välj i vilket format du vill att värdena ska visas för fälten i kolumnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa den här kolumnen när du arbetar på en instrumentpanel</td> 
      <td> <p>Välj det här alternativet om du vill visa den här kolumnen på en kontrollpanel när rapporten visas sida vid sida med en annan rapport. När det här alternativet är avmarkerat visas inte den här kolumnen när du visar rapporten på en kontrollpanel där rapporter visas sida vid sida.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kolumnregler</td> 
      <td> <p>Klicka på <strong>Lägg till en regel för den här kolumnen</strong> om du vill lägga till villkorsstyrd formatering i kolumnen. När du har lagt till en regel kan du definiera fält- och textformat för hur fält som matchar den regeln visas. Klicka på <strong>Lägg till regel</strong> när du har definierat regeln. Mer information om villkorsstyrd formatering i en vy finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Använda villkorsstyrd formatering i vyer</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Använd** om du vill tillämpa ändringarna hittills och fortsätta redigera rapporten med följande alternativ.

   Klicka på **Spara + stäng** om du är klar med redigeringen av kolumnerna i rapporten och vill spara rapporten.

### Lägga till grupperingar i en rapport {#add-groupings-to-a-report}

1. Börja skapa en rapport enligt beskrivningen i avsnittet [Skapa en rapport](#create-a-report) i den här artikeln.
1. I rapportbyggaren väljer du fliken **Grupperingar** för att identifiera hur du vill gruppera objekt i rapporten.
1. Klicka på **Lägg till gruppering** om du vill lägga till en ny gruppering.

   eller

   Välj **Använd en befintlig gruppering** om du vill välja en befintlig gruppering när den visas i listan.

   ![Lägg till gruppering](assets/nwe-add-grouping-350x230.png)

1. Börja skriva det fält som du vill lägga till som en gruppering. Om fältet är tillgängligt fylls det i för varje objekt där det kan kopplas. Klicka på fältets namn för att lägga till det i den grupperingen.
1. (Valfritt) Du kan välja att skapa en gruppering i textläge genom att klicka på **Växla till textläge**. Mer information om hur du använder textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Mer information om hur du skapar nya grupperingar finns i [Översikt över grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Valfritt) Välj **Komprimera den här grupperingen som standard** om du vill att resultaten i den här grupperingen ska visas komprimerade i stället för expanderade.

   Den här inställningen är inaktiverad som standard och resultatet av grupperingen visas alltid i en utökad lista.

   >[!TIP]
   >
   >* När du justerar grupperingar manuellt när du visar en lista kommer Workfront ihåg dina manuella inställningar tills du loggar ut. När du loggar in igen visas listan enligt den här inställningen.
   >* Resultatet av en gruppering visas alltid expanderat när du har öppnat dem från ett diagramelement.

1. (Valfritt) Klicka på **Växla till matrisgruppering** om du vill skapa en matrisgruppering och visa resultatet i ett rutnätsformat.

   Mer information om hur du skapar en matrisrapport finns i [Skapa en matrisrapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicka på **Använd** om du vill tillämpa ändringarna hittills och fortsätta redigera rapporten med följande alternativ.

   Klicka på **Spara + stäng** om du är klar med redigeringen av grupperingarna i rapporten och du vill spara rapporten.

### Lägga till filter i en rapport {#add-filters-to-a-report}

1. Börja skapa en rapport enligt beskrivningen i avsnittet [Skapa en rapport](#create-a-report) i den här artikeln.
1. I rapportbyggaren väljer du fliken **Filter** för att identifiera den mängd information som du vill att rapporten ska innehålla.
1. Klicka på **Lägg till en filterregel** om du vill lägga till ett eget filter.\
   eller\
   Välj **Använd ett befintligt filter** om du vill använda ett befintligt filter.

   ![Lägg till ett filter](assets/nwe-add-a-filter-350x93.png)

1. Om du klickade på **Lägg till en filterregel** börjar du skriva det fält som du vill lägga till som ett filter. Om fältet är tillgängligt fylls det i för varje objekt där det kan kopplas. Klicka på namnet på fältet för att lägga till det i det filtret.\
   Använd filtermodifierare för att skapa filtret. Mer information om filtermodifierare finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Mer information om hur du skapar nya filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Valfritt) Du kan välja att skapa ett filter i textläge genom att klicka på **Växla till textläge**.

   Mer information om hur du använder textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Klicka på **Använd** när du är klar med redigeringen av filtren i rapporten för att tillämpa ändringarna hittills och fortsätta redigera rapporten med följande alternativ.

   Klicka på **Spara + stäng** om rapporten och du vill spara den.

### Lägga till ett diagram i en rapport {#add-a-chart-to-a-report}

1. Börja skapa en rapport enligt beskrivningen i avsnittet [Skapa en rapport](#create-a-report) i den här artikeln.
1. Välj fliken **Diagram** i Report Builder och välj sedan den typ av diagram som du vill lägga till.

   ![Lägg till ett diagram](assets/nwe-add-a-chart-350x247.png)

   Mer information om hur du skapar ett diagram i en rapport finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klicka på **Använd** om du vill tillämpa ändringarna hittills och fortsätta redigera rapporten med följande alternativ.

   Klicka på **Spara + stäng** om du är klar med redigeringen av rapporten och vill spara rapporten.
