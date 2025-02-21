---
product-area: reporting
navigation-topic: text-mode-reporting
title: Redigera en gruppering i textläge
description: Du kan redigera en gruppering i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa grupperingar.
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---

# Redigera en gruppering i textläge

<!-- Audited: 1/2025 -->

Du kan redigera en gruppering i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa grupperingar.

>[!TIP]
>
>Vi rekommenderar att du skapar så mycket som möjligt av grupperingen i standardläge och sedan konverterar den till textläge för att redigera den.

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
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera grupper i en rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera grupperingar i en rapport</p> <p>Hantera behörigheter för en gruppering för att redigera den</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar använda textläge i en rapport eller lista bör du alltid kontrollera att du känner till Workfront textläge.

Mer information finns i:

* [Textläge - översikt](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Anpassad vy, filter och gruppering av exempel: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Redigera en gruppering i textläge

Att redigera en gruppering i textläge är identiskt för rapporter och listor. Åtkomsten till grupperingen från en rapport eller från en lista skiljer sig åt.

>[!NOTE]
>
>Grupperingar är ett obligatoriskt rapportelement för att skapa diagram i rapporter. Grupperingar i textläge stöds inte i diagram. Mer information om hur du lägger till diagram i rapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Mer information om hur du skapar grupperingar finns i [Skapa grupperingar i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gör något av följande:

   1. Om du vill komma åt grupperingen från en rapport går du till rapporten och klickar sedan på **Rapportåtgärder** > **Redigera** > fliken **Grupperingar**.
   1. Om du vill komma åt grupperingen från en lista går du till listan och från listrutan **Gruppering**, för musen över den gruppering som du vill ändra och klickar på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

      Grupperingsverktyget öppnas.

1. Klicka på **Lägg till gruppering** för att lägga till grupperingarna, klicka på **Växla till textläge** i det övre högra hörnet av verktyget och klicka sedan på **Redigera textläge**.

   >[!TIP]
   >
   >Du kan lägga till upp till tre grupperingar i standardgränssnittet. Du kan bara lägga till en fjärde gruppering i textläge, och du kan inte ha fler än fyra grupperingsnivåer i Workfront.

1. Börja skriva namnet på ett fält som du vill gruppera efter.

   Markera namnet på fältet när du ser det i listan.

1. Klicka på **Växla till textläge** i det övre högra hörnet av verktyget.

   Grupperingen visas sedan i textläge.

   När du redigerar en gruppering i textläge lägger Workfront till

   ```
   textmode=true
   ```

   kodraden till grupperingen. Detta anger att grupperingen har ändrats i textläge.

   **Exempel:** Om du vill gruppera en lista med uppgifter efter projektnamnet och sedan namnet på den primära tilldelaren, ska grupperingen se ut så här i textläge.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Raderna i fet stil är obligatoriska.

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
   >Nyckelraderna i en textlägesgruppering liknar de rader som behövs för att skapa textlägesvyer.

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
      <td><strong>grupp.&lt;tal&gt;.</strong> </td> 
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
      <td> <p>Detta är namnet på objektet eller på fältet så som det visas i databasen. Mer information om hur objekt och fält visas i databasen finns i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-utforskaren</a>.</p> <p>Följande scenarier finns:</p> 
       <ol> 
        <li value="1"> <p> Om namnet på fältet som du visar är en fras i stället för ett enda substantiv, måste du använda kamelversionssyntax för <code>valuefield</code>. Koden är till exempel för det planerade startdatumet för en åtgärd:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Om du vill visa ett anpassat fält är värdet <code>valuefield</code> fältets faktiska namn, som du ser det i gränssnittet. För ett anpassat fält med namnet "Mer information" är koden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Om du vill gruppera efter objekt som är relaterade till andra objekt med kodraden <code>valuefield</code> avgränsas objektnamnen och attributen av kolon.</p> <p>En gruppering efter Portfolio Name för en uppgiftslista har till exempel följande värde för värdefältraden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Detta anger att du kan komma åt nästa relaterade objekt (projekt) från rapportens (uppgiftens) objekt. Därifrån kan du komma åt följande relaterade objekt från projektet (portföljen) och sedan portföljens namn (namnet).</p> </li> 
       </ol> <p>Mer information om hur objekt ansluter till varandra finns i avsnittet <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Objektens inbördes beroende och hierarki</a> i <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</p> <p>Obs! Om du väljer ett fält i textläge som inte är giltigt i standardgränssnittet och växlar till standardgränssnittet, tas grupperingen bort.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>värdeformat=</strong> </td> 
      <td> <p>Den här raden representerar det format som används för att visa <code>valuefield</code>. <code>valueformat</code> identifierar om ett objekt eller fält visas som text, tal, procent eller datum.</p> <p>Vi rekommenderar att du använder <code>HTML</code> för din <code>valueformat</code>, särskilt när du använder <code>valueexpression</code>, för att se till att din information visas så korrekt som möjligt.</p> <p>Mer information om ytterligare värden för den här raden finns i <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Använd villkorsstyrd formatering i textläge</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>värdeuttryck=</strong> </p> </td> 
      <td> <p>Du kan lägga till den här raden för att ersätta <code>valuefield</code> om du vill gruppera listan med en beräkning mellan flera fält.</p> <p>Du måste omsluta <code>valuefield</code> av objekten inom klammerparenteser varje gång du använder dem i en <code>valueexpression</code>.</p> <p>Följande scenarier finns:</p> 
       <ol> 
        <li value="1"> <p>Om du vill visa namnet på en gruppering i versaler använder du:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>Objektets <code>valuefield</code> stavas så som det visas i API-utforskaren.</p> </li> 
        <li value="2">Om du vill lägga till flera <code>valuefields</code> genom att stränga dem tillsammans på en <code>valueexpression </code>rad måste du separera dem med en punkt.<p>Om du till exempel vill visa namnet på portföljen med stora bokstäver i en uppgiftslista använder du följande kod på raden <code>valueexpression</code>:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Om du vill använda ett anpassat fält på en <code>valueexpression</code>-rad måste du före fältets namn skriva <code>DE:</code> för att ange att det är ett anpassat fält. Fältets namn är rättstavat så som det visas i gränssnittet.</p><p>Viktigt: <span>När du använder ett anpassat fält som placeras i ett anpassat formuläravsnitt som har begränsade behörigheter för vissa användare, är beräkningen av <code>valueexpression </code> tom när dessa användare visar beräkningen i en rapport. Mer information om hur du justerar behörigheter i anpassade formuläravsnitt finns i </span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Skapa ett anpassat formulär</a></span>.</p><p>Om du till exempel har ett anpassat fält med namnet"Utvecklarnamn" och du vill gruppera efter det här fältet och visa det med versaler, kan du använda följande <code>valueexpression</code> för att ange detta:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>När du refererar till ett anpassat fält av typen Typeahead använder du följande uttryck för att referera till namnet på objektet som är markerat i ett fält med namnet "Utvecklarnamn":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Den här raden definierar grupperingsetiketten. I det här fallet används det förkortade värdet baserat på nyckeln.</p> <p>Om du vill ändra grupperingsnamnet kan du ändra värdet till följande:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> I kan du ange valfri text för grupperingsnamnet medan <code>namekey</code> kräver att du anger en nyckel som används för att översätta namnet på en gruppering.</p> <p>Om du vill ändra grupperingsnamnet kan du även lägga till raden <code>displayname </code>om det inte finns någon.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>visningsnamn =</strong> </td> 
      <td> <p>Du kan lägga till följande rad för att ändra namnet på en kolumn, som skriver över värdet <code>namekey/name</code>:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Vi rekommenderar att du tar bort alla rader som innehåller <code>name </code>när du byter namn på en gruppering.</p> </td> 
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
   >* När du justerar grupperingar manuellt när du visar en lista kommer Workfront ihåg dina manuella inställningar tills du loggar ut. När du loggar in igen visas listan enligt den här inställningen.
   >* Resultatet av en gruppering visas alltid expanderat när du har öppnat dem från ett diagramelement.

1. Klicka på **Klar** om du vill spara ändringarna och fortsätta redigera grupperingen eller rapporten.
1. Klicka på **Spara gruppering** i en lista eller **Spara + stäng** om du vill spara rapporten.
