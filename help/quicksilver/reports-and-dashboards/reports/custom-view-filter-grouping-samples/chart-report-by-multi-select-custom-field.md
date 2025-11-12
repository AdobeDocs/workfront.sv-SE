---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Schemalägg en rapport med ett anpassat fält som har valts flera gånger
description: Du kan bara skapa ett diagram över en rapport med ett anpassat fält som består av flera val efter att du har skapat ytterligare ett beräkningsfält som fångar de val som har valts i det anpassade fältet som består av flera val.
author: Jenny
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# Diagrama en rapport med ett anpassat fält som har flera val

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

I stället för att skapa ett diagram med ett anpassat fält som består av flera markeringar rekommenderar vi att du skapar separata fält för varje alternativ i ett anpassat fält som består av flera markeringar.

Exempel på anpassade fält med flera val är:

* Kryssrutor
* Flervalsmenyer

Mer information om hur du använder textläge finns i artikeln [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Men om det inte går att ha separata fält för varje alternativ i ett flervalsfält kan du schemalägga en rapport med ett anpassat flervalsfält genom att använda beräknade anpassade fält för att gruppera valen från flervalsfältet först. Efter det kan du diagram rapporten efter beräkningsfälten.

>[!NOTE]
>
>Artiklar som har något av alternativen markerat räknas bara en gång.
>
>Om du till exempel har ett anpassat kryssrutefält med alternativen Val 1 och Val 2 som och bifogar formuläret till uppgifter, visas de uppgifter som har både Val 1 och Alternativ 2 i ett separat diagramelement än de uppgifter som bara har Val 1 eller Val 2 markerade.
>
>Aktiviteter som har alternativet 1 markerat visas inte i samma diagramelement som de uppgifter som har alternativet 1 och Alternativ 2 markerat.

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
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar måste du skapa ett beräknat anpassat fält som visar de värden som har valts i det anpassade fältet för flera val. Mer information finns i avsnittet [Skapa ett beräknat anpassat fält som refererar till ett anpassat fält som består av flera val](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) i den här artikeln.

## Skapa en rapport med hjälp av anpassade fält som har valts flera gånger

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Du kan inte skapa ett diagram i en rapport genom att referera till ett anpassat fält med flera val. I stället kan du skapa ett beräkningsfält som registrerar värdena för det anpassade fältet med flera val för ett visst objekt och en viss grupp med hjälp av beräkningsfältet. 

* [Skapa ett beräknat anpassat fält som refererar till ett anpassat fält med flera val](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Skapa ett diagram som refererar till ett beräknat anpassat fält](#build-a-chart-that-references-a-calculated-custom-field)

### Skapa ett beräknat anpassat fält som refererar till ett anpassat fält som består av flera val {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Om du vill skapa ett beräknat fält som refererar till ett anpassat fält med flera val måste du ha följande krav:

* Ett anpassat flervalsfält i ett anpassat formulär.\
  Mer information om hur du skapar anpassade formulär och lägger till anpassade fält till dem finns i artikeln [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Ett anpassat formulär med det anpassade fältet för flera markeringar kopplat till objekt.
* Värden för det anpassade fältet för flera markeringar för varje objekt.

Så här skapar du det beräknade anpassade fältet som refererar till det anpassade fältet för flera val:

1. Skapa ett eget formulär eller redigera ett befintligt.

   Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Markera objektet eller objekten som du vill använda med det anpassade formuläret.
1. Klicka på **Lägg till ett fält** och sedan på **Beräknat** för att lägga till det anpassade flervalsfältet i formuläret.

1. I rutan **Etikett** ger du det nya beräknade fältet ett namn som anger att det refererar till det anpassade fältet för flera val.

   Exempel: &quot;Beräknat flervalsfält&quot;.

1. Ange följande kod i rutan **Beräkning**:

   `{DE:Multi-select Custom Field}`

   Detta lägger till de val som är markerade i det anpassade fältet med flera val till det beräknade anpassade fältet. Om formuläret t.ex. är kopplat till uppgifter och du väljer Alternativ 1 i det anpassade fältet för flera val, visas värdet &quot;Alternativ 1&quot; i det beräknade anpassade fältet. Om du väljer Alternativ 1 och Alternativ 2 för en annan uppgift visar det beräknade anpassade fältet värdet &quot;Val 1, Val 2&quot;.

1. Ersätt&quot;Flervalsfält&quot; med det faktiska namnet på det anpassade fältet med flera val, så som det visas i Workfront.

   ![Beräknat anpassat flervalsfält](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Valfritt) Om det anpassade fältet för flera val redan finns i det här formuläret och om formuläret redan är kopplat till objekt, aktiverar du alternativet **Använd för befintliga beräkningar**.

   Detta garanterar att det nya beräknade fältet automatiskt fylls i med värdet från det anpassade fältet som består av flera val när det läggs till i de formulär som redan är kopplade till objekten.

1. Klicka på **Använd**.
1. Klicka på **Spara och stäng**.

   Det beräknade anpassade fältet läggs till i det anpassade formuläret och om formuläret är kopplat till objekt fylls fältet i med information från det anpassade fältet som består av flera val.

### Skapa ett diagram som refererar till ett beräknat anpassat fält {#build-a-chart-that-references-a-calculated-custom-field}

1. (Valfritt) Om du vill vara säker på att alla beräknade fält som du vill rita efter fylls i med värden, måste du beräkna om de anpassade uttrycken för alla objekt i rapporten.
Mer information om hur du beräknar om uttryck finns i [Redigera information i anpassade fält](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

   <!--from the Details tab of the report select all the objects that contain the custom form with both the multi-select custom field and the calculated custom field, then click **Edit**. 
   1. (Optional and conditional) Select the **Recalculate Custom Expressions** field, then click **Save Changes**.  
   ![Recalculate custom expressions](assets/recalculate-custom-expressions-350x259.png) 
   >[!NOTE]
   >
   >This option has been eliminated from editing projects in bulk.  You can still recalculate expressions for projects in bulk by clicking the **More** icon ![More icon](assets/more-icon-45x33.png) at the top of a project list, then **Recalculate Expressions**. -->

1. Gå till rapporten där du vill lägga till diagrammet för det beräknade fältet som refererar till det anpassade fältet för flera val.
1. Klicka på **Rapportera åtgärder** och sedan på **Redigera**.

1. Välj fliken <strong>Grupperingar</strong> och klicka sedan på <strong>Lägg till gruppering</strong>.
1. Lägg till det <strong>beräknade flervalsfältet</strong> som du skapade som gruppering.
1. Välj fliken <strong>Diagram</strong> och lägg till ett diagram i rapporten.

   Välj till exempel ett **kolumndiagram**.
   <br>Mer information om hur du lägger till ett diagram i en rapport finns i avsnittet <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Lägg till ett diagram i en rapport</a> i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.
1. Markera det **beräknade flervalsfältet** som ska visas i diagrammet i fältet <strong>Nedre (X) axel</strong>.
1. Klicka på <strong>Spara + Stäng</strong>.

   I rapporten visas resultaten grupperade efter fältet Beräknat flerval i ett diagram.

   ![Flervalsfält i diagram](assets/chart-multi-select-field-column-chart-example.png)
