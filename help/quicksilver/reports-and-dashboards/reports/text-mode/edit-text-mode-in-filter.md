---
product-area: reporting
navigation-topic: text-mode-reporting
title: Redigera ett filter i textläge
description: Du kan redigera ett filter i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa filter.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Redigera ett filter i textläge

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

Du kan redigera ett filter i en lista eller rapport i textläge för att komma åt fält som inte är tillgängliga i standardgränssnittet och skapa mer komplexa filter.

Fler exempel på textläge finns i avsnittet [Exempel på anpassade filter](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) i artikeln [Anpassad vy, filter och grupperingsexempel: artikelindex](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md) när du skapar ett filter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p>
    <p>eller</p>
    <p>Aktuell: Planera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till filter, vyer och grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att redigera rapportelement i en rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en rapport för att redigera filter i en rapport</p> <p>Hantera behörigheter för ett filter för att redigera det</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar använda textläge i en rapport eller lista bör du alltid kontrollera att du känner till Workfront textläge.

Mer information finns i:

* [Textläge - översikt](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Anpassad vy, filter och gruppering av exempel: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Redigera textläge i ett filter

Att redigera ett filter i textläge är identiskt för rapporter och listor. Åtkomsten till filtret från en rapport eller från en lista skiljer sig åt.

>[!TIP]
>
>Vi rekommenderar att du skapar så mycket som möjligt av filtret i standardläge och sedan konverterar filtret till textläge för att redigera det.

Mer information om hur du skapar filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Gör något av följande:

   1. Gå till rapporten och klicka sedan på **Rapportåtgärder** > **Redigera** > fliken **Filter** för att få åtkomst till filtret från en rapport.
   1. Om du vill komma åt filtret från en lista går du till listan och från menyn **Filter**, håller pekaren över filtret som du vill ändra och klickar på ikonen **Redigera** ![](assets/edit-icon.png) .

      Filterverktyget öppnas.

1. Klicka på **Lägg till en filterregel** för att börja lägga till villkoren för filtret och klicka sedan på **Textläge** eller **Växla till textläge** till höger om verktyget.
1. Lägg till filtersatser i textläge. Varje filterprogramsats kan innehålla följande rader och ytterligare information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filterrad/information</b></td> 
      <td><b>Exempel</b></td> 
     </tr> 
     <tr> 
      <td> <p>Fältnamn och det värde som är lika med det som de visas i Workfront-databasen.</p> <p>Denna rad är obligatorisk.</p> <p> Mer information om hur objekt och fält visas i databasen finns i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-utforskaren</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Använd följande rad om du vill filtrera efter pågående uppgifter:</p> <p><code>status=INP</code> </p> <p><b>TIPS</b>

   När du filtrerar efter status måste du använda statuskoden med tre bokstäver och inte namnet.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Fältnamnsmodifierare och vad modifieraren är lika med. Detta anger vilka villkor som fältet du filtrerar efter måste uppfylla.</p> <p>Denna rad är obligatorisk.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Om du vill ange att statusen för de uppgifter som du filtrerar efter måste vara samma som Pågår ska du använda följande rad förutom den ovan:</p> <p><code>status_Mod=in</code> </p> <p>Om modifieraren är ett intervall finns det två rader som anger modifieraren.</p> 
       <div> <span class="autonumber"><span><b>EXEMPEL </b></span></span> 
        <p>Det här är ett textlägesfilter som söker efter pågående uppgifter som har ett planerat slutförandedatum under den aktuella månaden och som tilldelas en användare med ett specifikt GUID:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>En fullständig lista över filtermodifierare i textläge finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- och villkorsmodifierare</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Programsatsoperator. Som standard är varje filterprogramsats kopplad av operatorn"AND". Detta visas inte i textlägesgränssnittet. Du kan också lägga till operatorn "OR" mellan två programsatser för att ange att du vill filtrera efter objekt som kan uppfylla det ena eller andra av två villkor.</p> <p>Filteroperatorer krävs bara för filter som har mer än en programsats.</p> <p>Tips:   
        <ul> 
         <li> <p>"OR" är skiftlägeskänsligt och måste alltid ha inledande versal.</p> </li> 
         <li> <p>När du ändrar operatorn från AND till OR kan antalet listobjekt öka.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EXEMPEL </b></span></span> 
        <p>Använd följande om du vill filtrera efter uppgifter med statusen Pågår eller med datumet för planerad slutförande: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Ett jokertecken, som gör att du kan skapa information i ett filter och referera till aktuell tid eller till användaren som är inloggad.</p> <p>Jokertecken är valfria.</p> <p>Tips:   <p>Vi rekommenderar att du använder jokertecken när det är möjligt för att göra filtren mer dynamiska och inte duplicera samma filter för varje användare eller liknande tidsramar.</p> <p>Mer information om jokertecken för filter finns i <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Översikt över filtervariabler för jokertecken</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EXEMPEL</b></span></span> 
        <p>Använd följande om du vill filtrera efter uppgifter som tilldelats användaren som är inloggad:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Så här lägger du till en filtersats som är ansluten till operatorn &quot;OR&quot;:

   1. Lägg till en ny kodrad och typ OR:1: följt av objektet eller attributet som du vill filtrera efter och värdet som du vill jämföra det med. Om du vill referera till aktiviteter som har någon status förutom Nytt använder du följande rad:

      `OR:1:status=NEW`

   1. Lägg till en andra rad och skriv OR:1: följt av objektet, modifieraren och modifieringskoden. Om du vill definiera modifieraren för den kodrad som refererar till alla aktivitetsstatusar utom för Nytt använder du följande modifieringsrad:

      `OR:1:status_Mod=notin`

      Varje rad i den nya programsatsen måste föregås av &quot;OR:`<number>`:&quot;.

      Mer information om hur du skapar OR-satser i ett filter finns i [Skapa OR-satser i textlägesfilter](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >Du kan ha flera &quot;OR&quot;-programsatser i samma filter. Varje gång du har en ny OR-programsats ökar siffran efter OR:.
      >
      >Om du vill filtrera efter uppgifter som har statusen Pågår eller som har tilldelats den inloggade användaren eller som har det planerade slutförandedatumet idag använder du följande:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Klicka på **Avsluta textläge** eller **Klar** om du vill spara textlägesändringarna och fortsätta redigera rapporten eller filtret.
1. Klicka på **Spara + stäng** om du vill spara rapporten eller på **Spara filter** om du vill spara filtret i listan.


