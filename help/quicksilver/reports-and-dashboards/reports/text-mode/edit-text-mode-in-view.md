---
product-area: reporting
navigation-topic: text-mode-reporting
title: Redigera en vy i textläge
description: 'OBS! lägg till ett avsnitt i den här artikeln: Elements/create-customize-views.html *** Utkast till det här området i översiktsartikeln om textläge)'''
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 0%

---

# Redigera en vy i textläge

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Du kan redigera en vy i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa vyer.

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
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera vyer i en rapport</p> <p>Hantera behörigheter till en vy för att redigera den</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar använda textläge i en rapport eller lista bör du alltid kontrollera att du känner till Workfront textläge.

Mer information finns i:

* [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exempel på anpassad vy, filter och gruppering](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Redigera textläge i en vy

Att redigera en vy i textläge är identiskt för rapporter och listor. Åtkomsten till vyn från en rapport eller från en lista skiljer sig åt.

>[!TIP]
>
>Vi rekommenderar att du skapar så mycket som möjligt av vyn i standardläge och sedan konverterar den till textläge för att redigera den.

Mer information om hur du skapar vyer finns i [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gör något av följande:

   1. Gå till rapporten och klicka sedan på **Rapportåtgärder** > **Redigera** > **Kolumner (vy)** -fliken.
   1. Gå till listan och från **Visa** nedrullningsbar meny, för musen över vyn som du vill ändra och klicka på **Redigera** icon ![](assets/edit-icon.png).

      Vyverktyget öppnas.

1. Markera en kolumn i vyn.

   eller

   Välj **Kolumner (vy)** i Report Builder och välj sedan en kolumn.

   >[!TIP]
   >
   >Om du vill redigera en vy i textläge måste du redigera en kolumn i taget.

1. Klicka **Växla till textläge** i det övre högra hörnet av verktyget.

   >[!NOTE]
   >
   >När du redigerar en kolumn i textläge lägger Workfront till `textmode=true` kodraden till kolumnen. Detta anger att kolumnen ändras i textläge.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   Följande tabell visar nyckelraderna i textläge:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Exempelrad</th> 
      <th>Beskrivning</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>värdefält</strong>=</p> </td> 
      <td> <p>Detta är namnet på objektet eller på fältet så som det visas i databasen. Mer information om hur objekt och fält visas i databasen finns i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Följande scenarier finns:</p> 
       <ol> 
        <li value="1"> <p> Om namnet på fältet som du visar är en fras i stället för ett enda substantiv, måste du använda kamelversionssyntax för <code>valuefield</code>. Koden är till exempel för det planerade startdatumet för en åtgärd: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Om du vill visa ett anpassat fält visas <code>valuefield</code> värdet är fältets faktiska namn, som du ser det i gränssnittet. För ett anpassat fält med namnet "Mer information" är koden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Om du vill visa objekt som är relaterade till andra objekt i en vy med <code>valuefield</code> kodrad objektnamnen och attributen avgränsas med kolon. </p> <p>En kolumn i en uppgiftsvy som skulle visa namnet på Portfolio-ägaren har till exempel följande värde för värdefältraden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Detta anger att du från rapportens (uppgiftens) objekt kan komma åt nästa relaterade objekt (projekt) därifrån, du kan komma åt följande relaterade objekt från projektet (portföljen), portföljägaren (ägaren) och sedan deras namn (namnet). </p> </li> 
       </ol> <p>Mer information om hur objekt ansluter till varandra finns i avsnittet <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Objektens inbördes beroende och hierarki</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</p> <p>Obs! Om du väljer ett fält i textläge som inte är giltigt i standardgränssnittet kan du inte växla tillbaka till standardgränssnittet i kolumnen.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueFormat=</strong> </td> 
      <td> <p>Den här raden representerar det format som används för att visa <code>valuefield</code>. The <code>valueformat</code> identifierar om ett objekt eller fält visas som text, tal, procent eller datum.</p> <p>Vi rekommenderar att du använder <code>HTML</code> för <code>valueformat</code>, särskilt när du använder <code>valueexpression</code>, för att informationen ska visas på bästa sätt. </p> <p>Mer information om ytterligare värden för den här raden finns i <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Använda villkorsstyrd formatering i textläge</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Du kan lägga till den här raden som ska ersättas <code>valuefield</code>om du vill visa ett beräkningsfält i kolumnen.</p> <p>Du måste omge <code>valuefield</code> av objekten inom klammerparentes varje gång du använder dem i en <code>valueexpression</code>.</p> <p>Följande scenarier finns: </p> 
       <ol> 
        <li value="1"> <p>Om du vill visa ett fält i en kolumn med stora bokstäver använder du:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> objektets stavning så som den visas i API-utforskaren. </p> </li> 
        <li value="2">Om du vill lägga till flera <code>valuefields</code> genom att binda ihop dem måste du separera dem med en punkt.</li> 
        <li value="3"> <p>Om du till exempel vill visa namnet på den primära tilldelade personen för en uppgift med <code>valueexpression</code>använder du:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Om du vill använda ett anpassat fält i en <code>valueexpression</code> rad som du måste skriva före fältets namn med <code>DE:</code> för att ange att det är ett anpassat fält. Fältets namn är stavat så som det visas i gränssnittet. </p> <p>Viktigt: När du använder ett anpassat fält som placeras i ett anpassat formuläravsnitt som har begränsade behörigheter för vissa användare, är beräkningen av värdesuttrycket tom när dessa användare visar beräkningen i en rapport. Mer information om hur du justerar behörigheter i anpassade formuläravsnitt finns i <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a></span>.</p> <p>Om du t.ex. har ett anpassat fält med namnet"Utvecklarnamn" och vill visa det här fältet med versaler i en kolumn, kan du använda följande <code>valueexpression</code> för att ange detta:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>När du refererar till ett anpassat fält av typen Typeahead använder du följande uttryck för att referera till namnet på objektet som är markerat i ett fält med namnet "Utvecklarnamn":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Den här raden definierar texten i ett verktygstips när du för musen över namnet på kolumnen. I det här fallet används en nyckel för att översätta namnvärdet i beskrivningstexten. Om du vill ändra beskrivningen ändrar du den här raden till: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Den här raden definierar kolumnetiketten. I det här fallet används det förkortade värdet baserat på nyckeln.</p> <p>Om du vill ändra kolumnnamnet kan du ändra värdet till: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> gör att du kan ange valfri text för kolumnnamnet, medan<code>namekey</code> kräver att du anger en nyckel som används för att översätta namnet på en kolumn.</p> <p>Om du vill ändra kolumnnamnet kan du även lägga till <code>displayname </code>om det inte finns någon.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Du kan lägga till följande rad för att ändra namnet på en kolumn, vilket gör att <code>namekey/name</code> värde:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Den här raden definierar hur resultaten sorteras när du klickar på kolumnrubriken. Om den inte finns kan kolumnen inte sorteras efter att rapporten har körts.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Den här raden representerar antalet pixlar som används för kolumnen. Om raden utelämnas eller är inställd på 0 (noll) visas inte kolumnen i vyn.</p> <p>När du ändrar det här fältet manuellt i textläge måste du också lägga till <code>usewidths=true</code> till din kolumn.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Du måste använda den här raden förutom <code>width=</code> när du anpassar bredden på en kolumn. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Den här raden definierar om det värde som visas i en kolumn är redigerbart eller inte. Om den här raden är lika med <strong>true</strong>kan värdet i kolumnen redigeras. Om den här raden är lika med <code>false</code>, går det inte att redigera värdet i kolumnen.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Infoga bara den här raden när du vill att värdet ska visas i en kolumn som ska länka till det objekt som är associerat med den. Länken öppnar informationssidan för objektet. Detta värde ska matcha <code>valuefield=</code> linje. När du infogar detta måste du också lägga till <code>link.valueformat=</code> linje. </p> <p> Du kan till exempel infoga <code>link.valuefield=priority</code> i en problemvy och problemets prioritet visas som en länk. Om du klickar på den här länken öppnas sidan Problem.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Infoga bara den här raden när du har infogat <code>link.valuefield</code> rad för att lägga till en länk till värdet i en kolumn. Länken öppnar informationssidan för objektet. Detta värde ska matcha <code>valueformat=</code> och anger vilket format som används för att visa <code>valuefield</code>. </p> <p>Viktigt: När du visar textläget i en inbyggd kolumn som även innehåller en länk, ser du ett antal rader som refererar till länken. Vissa av dessa rader kanske inte längre stöds eller är onödiga när du skapar en egen anpassad kolumn i textläge och lägger till länksatserna i den. Raderna som är obligatoriska när du lägger till ett länkat värde är<code> link.valuefield</code> och <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Detta avser hur värdena i varje kolumn sammanfattas. Det finns flera rader som börjar med <code>aggregator.</code> och de hänvisar alla till den aggregator som sammanfattar resultatet av kolumnen. </p> <p>Som allmän regel gäller att <code>aggregator.</code> rader matchar kolumnobjektets linjer. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Exempel: </b></span></span> 
        <p>Kolumnen Planerade timmar i en uppgiftsrapport som summeras av Sum kan se ut så här: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valueField=workRequired</pre>
         <pre>valueFormat=compound</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        The <code>aggregator. </code>rader kan innehålla <code>valuefield </code>eller en <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Använd** om du vill spara ändringarna och fortsätta redigera vyn.
1. Klicka **Spara + Stäng** för att spara rapporten.

   eller

   Klicka **Spara vy** om du vill spara vyn i en lista.
