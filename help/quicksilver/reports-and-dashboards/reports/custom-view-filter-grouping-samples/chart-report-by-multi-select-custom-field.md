---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Diagrama en rapport med ett anpassat fält som har flera val
description: Du kan inte diagramma en rapport med ett anpassat fält som har flera val. Du måste skapa ytterligare ett beräkningsfält som refererar till det anpassade fältet för flera val för att kunna diagram rapporten med värdet för det anpassade fältet för flera val.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Diagrama en rapport med ett anpassat fält som har flera val

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Du kan inte diagramma en rapport med ett anpassat fält som har flera val. Du måste skapa ytterligare ett beräkningsfält som refererar till det anpassade fältet för flera val för att kunna diagram rapporten med värdet för det anpassade fältet för flera val.

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

## Förutsättningar

Innan du börjar måste du skapa ett beräknat anpassat fält som visar de värden som har valts i det anpassade fältet för flera val. Mer information finns i [Skapa ett beräknat anpassat fält som refererar till ett anpassat fält som består av flera val](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) i den här artikeln.

## Skapa en rapport med hjälp av anpassade fält som har valts flera gånger

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Du kan inte skapa ett diagram i en rapport genom att referera till ett anpassat fält med flera val. I stället kan du skapa ett beräkningsfält som registrerar värdena för det anpassade fältet med flera val för ett visst objekt och en viss grupp med hjälp av beräkningsfältet. 

* [Skapa ett beräknat anpassat fält som refererar till ett anpassat fält som består av flera val](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Skapa ett diagram som refererar till ett beräknat anpassat fält](#build-a-chart-that-references-a-calculated-custom-field)

### Skapa ett beräknat anpassat fält som refererar till ett anpassat fält som består av flera val {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

För att kunna skapa ett beräknat fält som refererar till ett anpassat fält med flera val måste du ha följande krav:

* Bygg det anpassade flervalsfältet i ett anpassat formulär.\
   Mer information om hur du skapar anpassade formulär och lägger till anpassade fält till dem finns i artikeln [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Koppla det anpassade formuläret till objekt.
* Fyll det anpassade fältet för flera val med ett värde för varje objekt.

Så här skapar du det beräknade anpassade fältet som refererar till det anpassade fältet för flera val:

1. Skapa ett eget formulär eller redigera ett befintligt.\
   Mer information om hur du skapar anpassade formulär finns i artikeln [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Markera objektet eller objekten som du vill använda med det anpassade formuläret.
1. Klicka **Lägg till ett fält** sedan **Beräknat** om du vill lägga till det anpassade fältet med flera markeringar i formuläret.

1. I **Etikett** ger du det nya beräknade fältet ett namn som anger att det refererar till det anpassade fältet för flera val.\
   Till exempel: &quot;Beräknat flervalsfält.&quot;

1. I **Beräkning** anger du följande kod:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Ersätt&quot;Flervalsfält&quot; med det faktiska namnet på det anpassade fältet med flera val, så som det visas i Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Valfritt) Aktivera alternativet **Uppdatera tidigare beräkningar** alternativ.\
   Detta garanterar att det nya fältet automatiskt fylls i med värdet från det anpassade fältet som består av flera markeringar när det läggs till i formulären som redan är kopplade till objekten.

1. Klicka **Klar**.
1. Klicka **Spara +Stäng**.

### Skapa ett diagram som refererar till ett beräknat anpassat fält {#build-a-chart-that-references-a-calculated-custom-field}

1. (Valfritt) Om du vill vara säker på att alla beräknade fält som du vill rita efter är ifyllda med värden, markerar du alla objekt i rapporten som innehåller det anpassade formuläret med både det anpassade fältet för flera val och det beräknade anpassade fältet. Klicka sedan på **Redigera**.
1. (Valfritt och villkorligt) Aktivera **Beräkna om anpassade uttryck** fält och klicka sedan på **Spara ändringar**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Det här alternativet har tagits bort från gruppredigering.  Du kan fortfarande beräkna om uttryck för projekt i grupp genom att klicka på **Mer** icon ![](assets/more-icon-45x33.png) högst upp i en projektlista, och sedan **Beräkna om uttryck**.


1. Gå till rapporten där du vill lägga till diagrammet för det beräknade fältet som refererar till det anpassade fältet för flera val.
1. Klicka **Rapportåtgärder** sedan **Redigera**.

1. Välj <strong>Grupperingar</strong> tabbtangenten och sedan klicka <strong>Lägg till gruppering</strong>.
1. Lägg till<strong>Beräknat flervalsfält</strong> som du har skapat som gruppering.
1. Välj <strong>Diagram</strong> och lägga till ett diagram i rapporten.<br>Mer information om hur du lägger till ett diagram i en rapport finns i avsnittet <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Lägga till ett diagram i en rapport</a> i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.
1. Välj <strong>Beräknat flervalsfält</strong> som ett av fälten som ska visas i diagrammet.
1. Klicka <strong>Spara + Stäng</strong>.<br>Rapporten visar resultaten grupperade efter det beräknade flervalsfältet i ett diagram.
