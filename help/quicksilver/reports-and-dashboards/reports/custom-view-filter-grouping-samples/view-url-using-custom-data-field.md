---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: Extern URL med anpassat datafält'
description: Du kan visa en länk till en intern anpassad URL genom att använda ett beräknat anpassat fält med namnet "Anpassad URL" i en uppgiftsvy.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Visa: extern URL med anpassat datafält

<!--Audited: 11/2024-->

Du kan visa en länk till en intern anpassad URL genom att använda ett **beräknat anpassat fält** med namnet &quot;Anpassad URL&quot; i en **uppgiftsvy**.

Det gör att du snabbt kan länka från vissa objekt i en vy till vissa delar av programmet direkt från dina rapporter.

När du skapar ett beräknat anpassat fält måste du först skapa fältet och sedan skapa vyn.

Följande avsnitt är ett exempel på ett beräknat anpassat fält för uppgifter. Det anpassade fältet kallas Anpassad URL. I den anpassade vyn visas fältets värde samt fältet **URL** för uppgifter.

Med samma steg kan du skapa liknande beräknade anpassade fält och anpassade vyer för alla objekt i systemet som har ett anpassat formulär.

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

## Skapa det beräknade anpassade fältet &quot;Anpassad URL&quot;

Mer information om hur du skapar ett beräknat anpassat fält finns i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Om du har tillgång till ett anpassat formulär kan du skapa ett beräknat anpassat fält för uppgifter som kallas &quot;Anpassad URL&quot;. Det här fältet länkar direkt till underfliken **Översikt** på fliken **Uppgiftsinformation**.

1. Skapa ett beräknat anpassat fält.
1. Ange följande kod i fältet Beräkning:

   CONCAT(&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Ersätt `<domain>` med ditt faktiska domännamn, utan hakparenteser. Delen `/overview` i den här URL:en dirigerar länken till avsnittet **Översikt** i aktivitetens vänstra panel.

1. När du har skapat ditt **beräknade anpassade fält** kopplar du det **anpassade formuläret** med det här fältet till flera uppgifter i Adobe Workfront som du vill visa i den nya vyn.

## Skapa vyn som visar fälten Anpassad URL och URL för aktiviteten

Aktiviteten **Visa** i exemplet nedan visar det **beräknade anpassade fältet** med namnet &quot;Anpassad URL&quot; som en direktlänk till underfliken **Översikt** på fliken **Information** samt aktivitetens **URL** -fält.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Så här anpassar du den här vyn:

1. Gå till en lista med uppgifter.
1. Expandera listrutan **Visa** högst upp i uppgiftslistan.
1. Klicka på **Anpassa vy**.
1. Ta bort alla kolumner i vyn, förutom den första kolumnen.
1. Klicka på den första kolumnens rubrik.
1. Klicka på **Växla till textläge** > **Redigera textläge**.
1. Ta bort texten i rutan **Redigera textläge** och ersätt den med följande kod:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   I det här exemplet är &#39;column.1.&#39; rader visar värdet i fältet Anpassad URL som en länk till aktivitetens **översiktsavsnitt**; kolumn.2. visar det värde som lagras i aktivitetens **URL-fält**.

1. Klicka på **Klar** > **Spara vy**.
