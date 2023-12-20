---
product-area: reporting
navigation-topic: text-mode-reporting
title: Redigera textläge i en gruppering
description: 'OBS! Gör alla FVG-artiklar likadana för redigering i textläge)'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Redigera textläge i en gruppering

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

Du kan redigera en gruppering i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa grupperingar.

>[!TIP]
>
>Vi rekommenderar att du skapar så mycket som möjligt av grupperingen i standardläge och sedan konverterar den till textläge för att redigera den.

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
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera grupper i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera grupperingar i en rapport</p> <p>Hantera behörigheter för en gruppering för att redigera den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar använda textläge i en rapport eller lista bör du alltid kontrollera att du känner till Workfront textläge.

Mer information finns i:

* [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Anpassad vy, filter och gruppering av exempel: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Redigera textläge i en gruppering

Att redigera en gruppering i textläge är identiskt för rapporter och listor. Åtkomsten till grupperingen från en rapport eller från en lista skiljer sig åt.

>[!NOTE]
>
>Grupperingar är ett obligatoriskt rapportelement för att skapa diagram i rapporter. Grupperingar i textläge stöds inte i diagram. Mer information om hur du lägger till diagram i rapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Mer information om grupperingar finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gör något av följande:

   1. Gå till rapporten och klicka sedan på **Rapportåtgärder** > **Redigera** > **Grupperingar** -fliken.
   1. Om du vill komma åt grupperingen från en lista går du till listan och från **Gruppering** nedrullningsbar meny, för musen över den gruppering som du vill ändra och klicka på **Redigera** icon ![](assets/edit-icon.png).

      Grupperingsverktyget öppnas.

1. Klicka **Lägg till gruppering** om du vill lägga till grupperingarna klickar du på **Växla till textläge** i det övre högra hörnet av verktyget.

   >[!TIP]
   >
   Du kan lägga till upp till tre grupperingar i standardgränssnittet. Du kan bara lägga till en fjärde gruppering i textläge, och du kan inte ha fler än fyra grupperingsnivåer i Workfront.

1. Börja skriva namnet på ett fält som du vill gruppera efter.

   Markera namnet på fältet när du ser det i listan.

1. Klicka **Växla till textläge** i det övre högra hörnet av verktyget.

   Grupperingen visas sedan i textläge.

   När du redigerar en gruppering i textläge lägger Workfront till

   ```
   textmode=true
   ```

   kodraden till grupperingen. Detta anger att grupperingen har ändrats i textläge.

   **Exempel:** Om du vill gruppera en lista med uppgifter efter projektnamn och sedan namnet på den primära tilldelaren, ska grupperingen se ut så här i textläge.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   Raderna i fet stil är obligatoriska.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Varje fält i grupperingen har flera kodrader som refererar till det fältet.

   Tabellen nedan visar nyckelraderna i en gruppering i textläge.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   Nyckelraderna i en textlägesgruppering liknar de rader som behövs för att skapa textlägesvyer.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Exempelrad</strong> </th> 
      <th><strong>Beskrivning</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>grupp.&lt;number&gt;.</strong> </td> 
      <td> <p>Varje kodrad föregås av den här texten. De kodrader som refererar till samma fält som är markerat i grupperingen numreras med samma nummer enligt följande:</p> 
       <ul> 
        <li>Den första grupperingen i rapporten har gruppnumret 0. Alla rader som refererar till den första grupperingen börjar med <code>group.0</code>.</li> 
        <li>Den andra grupperingen i rapporten har gruppnumret 1. Alla rader som refererar till den andra grupperingen börjar med <em><code>group.1</code></em>.</li> 
        <li>Den tredje grupperingen i rapporten har gruppnummer 2. Alla rader som refererar till den tredje grupperingen börjar med <em><code>group.2</code></em>.</li> 
        <li>Endast i textläge kan du lägga till gruppnumret 3 för en fjärde gruppering. Alla rader som refererar till den fjärde grupperingen börjar med <em><code>group.3</code></em>.</li> 
       </ul> <p>Obs! 4 grupperingar stöds inte i verktyget. De stöds bara i textläge. Workfront stöder inte fler än fyra nivåer av grupperingar.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>värdefält</strong>=</p> </td> 
      <td> <p>Detta är namnet på objektet eller på fältet så som det visas i databasen. Mer information om hur objekt och fält visas i databasen finns i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Följande scenarier finns:</p> 
       <ol> 
        <li value="1"> <p> Om namnet på fältet som du visar är en fras i stället för ett enda substantiv, måste du använda kamelversionssyntax för <code>valuefield</code>. Koden är till exempel för det planerade startdatumet för en åtgärd:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Om du vill visa ett anpassat fält visas <code>valuefield</code> värdet är fältets faktiska namn, som du ser det i gränssnittet. För ett anpassat fält med namnet "Mer information" är koden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Om du vill gruppera efter objekt som är relaterade till andra objekt med <code>valuefield</code> kodrad objektnamnen och attributen avgränsas med kolon.</p> <p>En gruppering efter Portfolio-namn för en uppgiftslista har till exempel följande värde för värdefältraden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Detta anger att du kan komma åt nästa relaterade objekt (projekt) från rapportens (uppgiftens) objekt. Därifrån kan du komma åt följande relaterade objekt från projektet (portföljen) och sedan portföljens namn (namnet).</p> </li> 
       </ol> <p>Mer information om hur objekt ansluter till varandra finns i avsnittet <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Objektens inbördes beroende och hierarki</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</p> <p>Obs! Om du väljer ett fält i textläge som inte är giltigt i standardgränssnittet och växlar till standardgränssnittet, tas grupperingen bort.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueFormat=</strong> </td> 
      <td> <p>Den här raden representerar det format som används för att visa <code>valuefield</code>. The <code>valueformat</code> identifierar om ett objekt eller fält visas som text, tal, procent eller datum.</p> <p>Vi rekommenderar att du <code>HTML</code> för <code>valueformat</code>, särskilt när du använder <code>valueexpression</code>, för att informationen ska visas på bästa sätt.</p> <p>Mer information om ytterligare värden för den här raden finns i <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Använda villkorsstyrd formatering i textläge</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Du kan lägga till den här raden som ska ersättas <code>valuefield</code>om du vill gruppera listan med hjälp av en beräkning mellan flera fält.</p> <p>Du måste omge <code>valuefield</code> av objekten inom klammerparentes varje gång du använder dem i en <code>valueexpression</code>.</p> <p>Följande scenarier finns:</p> 
       <ol> 
        <li value="1"> <p>Om du vill visa namnet på en gruppering i versaler använder du:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> objektets stavning så som den visas i API-utforskaren.</p> </li> 
        <li value="2">Om du vill lägga till flera <code>valuefields</code> genom att knyta ihop dem i en <code>valueexpression </code>måste du separera dem med en punkt.<p>Om du till exempel vill visa namnet på portföljen med stora bokstäver i en uppgiftslista använder du följande kod i <code>valueexpression</code> rad:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Om du vill använda ett anpassat fält i en <code>valueexpression</code> rad som du måste skriva före fältets namn med <code>DE:</code> för att ange att det är ett anpassat fält. Fältets namn är rättstavat så som det visas i gränssnittet.</p><p>Viktigt: <span>När du använder ett anpassat fält som placeras i ett anpassat formuläravsnitt som har begränsade behörigheter för vissa användare, beräknas <code>valueexpression </code>är tomt när dessa användare visar den här beräkningen i en rapport. Mer information om hur du justerar behörigheter i anpassade formuläravsnitt finns i</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a></span>.</p><p>Om du t.ex. har ett anpassat fält med namnet"Utvecklarnamn" och vill gruppera efter det här fältet och visa det med versaler, kan du använda följande <code>valueexpression</code> för att ange detta:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>När du refererar till ett anpassat fält av typen Typeahead använder du följande uttryck för att referera till namnet på objektet som är markerat i ett fält med namnet "Utvecklarnamn":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Den här raden definierar grupperingsetiketten. I det här fallet används det förkortade värdet baserat på nyckeln.</p> <p>Om du vill ändra grupperingsnamnet kan du ändra värdet till följande:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> kan du ange valfri text för grupperingsnamnet, medan <code>namekey</code> kräver att du anger en nyckel som används för att översätta namnet på en gruppering.</p> <p>Om du vill ändra grupperingsnamnet kan du även lägga till <code>displayname </code>om det inte finns någon.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Du kan lägga till följande rad för att ändra namnet på en kolumn, som skriver över <code>namekey/name</code> värde:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Vi rekommenderar att du tar bort alla rader som innehåller <code>name </code>när du byter namn på en gruppering.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Lägg till en av följande kodrader i en gruppering för att ange om resultaten i grupperingen ska visas i en utökad eller komprimerad lista. Som standard visas grupperingar som expanderade:


   ```
   group.0.iscollapsed=true
   ```

   om du vill att grupperingen ska visas med resultaten komprimerade

   ```
   group.0.iscollapsed=false
   ```

   om du vill att grupperingen ska visas med resultatet utökat

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * När du justerar grupperingar manuellt när du visar en lista kommer Workfront ihåg dina manuella inställningar tills du loggar ut. När du loggar in igen visas listan enligt den här inställningen.
   * Resultatet av en gruppering visas alltid expanderat när du har öppnat dem från ett diagramelement.

1. Klicka **Klar** om du vill spara ändringarna och fortsätta redigera grupperingen eller rapporten.
1. Klicka **Spara gruppering** i en lista eller **Spara + Stäng** för att spara rapporten.
