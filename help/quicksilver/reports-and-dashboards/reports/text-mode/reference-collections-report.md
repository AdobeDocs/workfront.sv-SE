---
product-area: reporting
navigation-topic: text-mode-reporting
title: Referenssamlingar i en rapport
description: Referenssamlingar i en rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# Referenssamlingar i en rapport

<!-- Audited: 1/2025 -->

Om du skapar en rapport i Adobe Workfront kan du visa en uppsättning objekt, deras respektive fält eller länkade objekt i en lista, ett rutnät eller ett diagramformat.

Mer information om hur du skapar en rapport i Workfront finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Hantera behörigheter för en vy, ett filter eller en gruppering </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förstå samlingar

En samling är en lista med objekt som är länkade till ett annat objekt.

Du har följande två relationer mellan objekt i Workfront:

* **En 1:1-relation**: Ett objekt kan bara länkas till ett annat objekt i taget.\
  Ett projekt kan till exempel bara länkas till en portfölj i taget.

* **En 1:N-relation**: Ett objekt kan länkas till flera andra objekt i taget.\
  Ett projekt kan t.ex. ha flera uppgifter. I det här fallet utgör uppgiftslistan en samling för projektet.

>[!IMPORTANT]
>
>Du kan skapa en rapport som visar en-till-en-relationen mellan objekt med hjälp av standardrapportverktyget. Du kan dock bara skapa en rapport som visar en-till-många-relationen mellan objekt med hjälp av textlägesgränssnittet i rapportbyggaren.

Mer information om hur du skapar en rapport i standardrapportverktyget finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Mer information om hur du skapar en rapport med hjälp av textlägesgränssnittet finns i:

* [Textläge - översikt](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Översikt över vanliga användningsområden för textläge](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Översikt över syntaxen i textläge](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Söka efter samlingsobjekt och deras fält i API-utforskaren {#find-collection-objects-and-their-fields-in-the-api-explorer}

Alla samlingar kan inte rapporteras.

Om du vill veta vilka objekt som kan kopplas till en samling med andra objekt måste du använda API-utforskaren.\
Mer information om API Explorer-tabellen finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

Så här tar du reda på vilka samlingar som kan rapporteras:

1. Gå till [API Explorer](../../../wf-api/general/api-explorer.md).
1. Hitta rapportens objekt.
1. Välj fliken **Samlingar**.

   >[!NOTE]
   >
   >Endast de objekt som visas på den här fliken kan representeras som en samling i en rapport för det markerade objektet.

1. Expandera objektet i din samling genom att klicka på det.
1. Klicka på länken som visas för att gå till objektet i din samling.\
   Då öppnas fliken **fält** för objektet i din samling.

   >[!NOTE]
   >
   >Det går endast att referera till fälten som visas på den här fliken i samlingsrapporten eller de fält som är kopplade till objekt som visas på den här fliken.

## Referenssamlingar i rapporter

Du kan referera till objekt från en samling i följande rapportelement:

* Vyer
* Filter
* Fråga

Du kan inte referera till objekt från en samling i följande rapportelement:

* Grupperingar
* Diagram

Du kan till exempel referera till uppgiften eller utleverans av samlingar från en projektrapport för att visa aktivitets- eller utleveransinformation på projektnivå.

* [Referera en samling i vyn för en rapport](#reference-a-collection-in-the-view-of-a-report)
* [Referera till en samling i filtret för en rapport](#reference-a-collection-in-the-filter-of-a-report)
* [Referera till en samling i den anpassade uppmaningen för en rapport](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Referera till en samling i rapportvyn {#reference-a-collection-in-the-view-of-a-report}

Du kan referera till en objektsamling i rapportvyn för att visa attribut för objekt som är kopplade till rapportens objekt.

Du kan till exempel visa uppgifter eller utleverans i en projektrapport genom att skapa en samlingskolumn för uppgifter eller utleverans i rapportvyn.

I samlingsvyn kan du visa information om uppgifter och utgåvor, t.ex. namn, datum, primära tilldelningar, procent färdigt osv.

Vyn visar uppgifter eller ärenden i ett listformat, där varje rad i listan representerar information om en uppgift eller ett problem. Listan med uppgifter eller problem och fälten för dem visas på samma rad som projektet som uppgifterna eller problemen tillhör.

![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png){width=400}

* [Lägg till en samlingskolumn i en rapportvy](#add-a-collection-column-in-a-report-view)
* [Förstå raderna i en samlingsvy i textläge](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Begränsningar för en samlingsvy](#limitations-of-a-collection-view)

### Lägga till en samlingskolumn i en rapportvy {#add-a-collection-column-in-a-report-view}

Så här lägger du till en samlingskolumn i en rapportvy:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport**.
1. Markera rapportens objekt.
1. Gå bort från rapporten och använd [API Explorer](../../../wf-api/general/api-explorer.md) för att avgöra vilka samlingar som är tillgängliga för det objekt som du har valt för rapporten.

   Mer information om hur du markerar objektet i din samling finns i avsnittet [Sök efter samlingsobjekt och deras fält i API-utforskaren](#find-collection-objects-and-their-fields-in-the-api-explorer) i den här artikeln.

   Notera namnet på objektet för samlingen.

1. Använd [API-utforskaren](../../../wf-api/general/api-explorer.md) och gå till listan med fält för objektet som du vill visa i samlingen.

   Mer information om hur du söker efter fälten för objektet i din samling finns i avsnittet [Sök efter samlingsobjekt och deras fält i API-utforskaren](#find-collection-objects-and-their-fields-in-the-api-explorer) i den här artikeln.

   Notera namnet på det fält som du vill visa i samlingen.

1. Gå tillbaka till rapporten och klicka på **Lägg till kolumn** på fliken **Kolumner (vy)**.
1. Klicka på **Växla till textläge**.
1. Klicka på **Redigera textläge**.
1. Markera all text i dialogrutan **Textläge** och ta bort den. Klistra sedan in följande kod om du refererar till ett fält i samlingsobjektet:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Ersätt **kolumnnamnet** med namnet på kolumnen på raden `displayname`.
1. Ersätt **samlingsobjektnamnet** med namnet på samlingsobjektet på raden `listmethod` så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md).

1. Ersätt **samlingsobjektfältet** med namnet på fältet för samlingsobjektet på raden `valuefield` så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md).

   Du kan ersätta **värdefält** med **värdesuttryck** om du vill skapa ett anpassat uttryck i vyn.

   Mer information om beräknade anpassade uttryck finns i [Översikt över beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Om du till exempel vill visa en lista med uppgifter i en projektrapport. Den här samlingen använder en `valuefield`-rad för att referera till aktiviteternas namn.

   Gör något av följande:

   * Använd följande kod för att skapa din kolumn:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Använd följande kod för att visa en lista med problem i rapporten:

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     Observera att i en samling måste du använda **issues** för raden **listmethod** i stället för **opTasks** som är databasnamnet för Issues. Mer information om när du ska använda **issue** och när du ska använda **opTask** när du refererar till problem finns i [Använd&quot;opTask&quot; och&quot;issue&quot; när du refererar till problem](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Om du vill visa en lista över aktiviteterna i en projektrapport tillsammans med deras primära tilldelare, använder du en **värdeuttrycksrad** för att referera till namnen på aktiviteterna intill namnen på deras primära tilldelningar i stället för **värdefält**.

     Använd följande kod för att skapa din kolumn:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. Följande kolumn visas i projektrapporten med alla uppgifter i varje projekt tillsammans med de primära tilldelningarna:

   ![Projektrapport med uppgift och tilldelad samling](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png){width=400}

1. Klicka på **Spara**.
1. (Valfritt) Fortsätt redigera rapporten.

   eller

   Klicka på **Spara + stäng** för att spara rapporten.

#### Förstå raderna i en samlingsvy i textläge

Raderna i ett textläge för en samling beskrivs i följande tabell:

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
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Du kan använda olika värden för den här raden, men vi rekommenderar att <code style="font-weight: normal;">valueformat</code> för en samlingslista ska vara <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Den här raden anger att kolumnen har konfigurerats i textläge. Om du tar bort den här raden läggs den tillbaka som standard i Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p><code>type</code> i en lista är alltid <code>iterate</code> när en vy skapas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Detta är avgränsaren som används för att separera värdena i listan.<br>Vi rekommenderar att du använder <code>&lt;p&gt;</code> som lägger till en radbrytning mellan värdena.</p> <p>Du kan även använda följande:</p> <p><code>&zwj;</code> (nollbreddsskarv). Värdena i samlingen har ingen separation mellan dem.<br><strong>,</strong> =kommaavgränsare. Samlingens värden avgränsas med ett kommatecken följt av inget blanksteg.<br><strong>/</strong> = snedstreck. Samlingens värden avgränsas med ett snedstreck.<br><strong>-</strong> = streckavgränsare. Samlingens värden avgränsas med ett streck.<br>Om du lämnar den här raden tom läggs ett kommatecken till följt av ett blanksteg mellan samlingens värden.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Kolumnnamn</em> </td> 
   <td> <p>Ersätt <strong>kolumnnamnet</strong> med det aktuella namnet på den nya kolumnen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Den här raden definierar den samling som du refererar till.</p> <p>Ersätt <strong>samlingsobjektnamnet</strong> med namnet på objektet som du refererar till i samlingen, så som det visas i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-utforskaren</a>. Det här värdet är vanligtvis samlingsobjektets plural-form.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Den här raden definierar vilket fält du refererar till från samlingsobjektet.</p> <p>Ersätt <strong>samlingsobjektfältet</strong> med namnet på fältet för det objekt som du refererar till i samlingen, så som det visas i <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-utforskaren</a>.</p> <p>Du kan ersätta raden med:</p> <p><strong>värdeuttryck</strong>=beräknat fält för samlingsobjekt</p> <p>Med <strong>valueExpression</strong> kan du  visar ett beräknat anpassat uttryck i kolumnen.</p> <p>Mer information om hur du formaterar <strong>värdesuttryck</strong> rader finns i <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Syntaxöversikt i textläge</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Begränsningar för en samlingsvy {#limitations-of-a-collection-view}

Tänk på följande begränsningar när du skapar en samlingsvy:

* Du kan inte styra i vilken ordning samlingsdata visas.
* Du kan inte använda villkorsstyrd formatering i en samlingsvy.
* Du kan inte göra ett objekt i en samling till en klickbar länk.
* Du kan inte skapa en samlingsvy för en annan samling.\
  Du kan till exempel inte visa alla tilldelningar för varje uppgift i en projektrapport. Du kan bara visa den primära tilldelaren för varje uppgift i en projektvy.

### Referera till en samling i ett rapportfilter {#reference-a-collection-in-the-filter-of-a-report}

Du kan referera till en samling objekt i filtret för en rapport om du vill filtrera efter attributen för objekt som är kopplade till rapportens objekt.

Du kan t.ex. filtrera efter uppgifter eller ärenden i en projektrapport genom att använda en referens till attributen för uppgifter eller ärenden i projektet i filtersatsen.

>[!NOTE]
>
>När det används på fält som innehåller flera värden (t.ex. en samling anteckningar i ett projekt), avgör filtret inkludering enligt följande:
>
>* Om alla objekt i en samling innehåller det angivna värdet tas hela posten inte med i resultatet.
>* Om minst ett objekt i samlingen inte innehåller det angivna värdet finns posten kvar i resultatet.



Så här lägger du till en referens till en samling i ett rapportfilter:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport**.
1. Markera rapportens objekt.
1. Gå bort från rapporten och använd [API Explorer](../../../wf-api/general/api-explorer.md) för att avgöra vilka samlingar som är tillgängliga för det objekt som du har valt för rapporten.

   Mer information om hur du markerar objektet i din samling finns i avsnittet [Sök efter samlingsobjekt och deras fält i API-utforskaren](#find-collection-objects-and-their-fields-in-the-api-explorer) i den här artikeln.

   Notera namnet på objektet för samlingen.

1. Använd [API-utforskaren](../../../wf-api/general/api-explorer.md) och gå till listan med fält för objektet som du vill visa i samlingen.

   Mer information om hur du söker efter fälten för objektet i din samling finns i avsnittet [Sök efter samlingsobjekt och deras fält i API-utforskaren](#find-collection-objects-and-their-fields-in-the-api-explorer) i den här artikeln.

   Anteckna det fält som du vill visa i samlingen.

1. Gå tillbaka till rapporten och klicka på **Växla till textläge** på fliken **Filter** och sedan på **Redigera textläge**.

1. Klistra in följande kod i området **Ange filterregler för rapporten**:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Ersätt **samlingsobjektnamnet** med namnet på samlingsobjektet så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md). Det här värdet är vanligtvis samlingsobjektets plural-form.

1. Ersätt **samlingsobjektfältet** med namnet på fältet för samlingsobjektet i, så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md).

1. Ersätt **samlingsobjektvärdet** med värdet för samlingsobjektet så som det visas i Workfront.
1. Ersätt värdet **för modifieraren** med en giltig modifierare.

   En lista med modifierare finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Om du till exempel vill skapa en projektrapport som endast visar projekt med aktiviteter som har &quot;Marknadsföring&quot; i sitt namn använder du följande kod:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Den här rapporten visar endast projekt som har minst en aktivitet med ordet&quot;marknadsföring&quot; i namnet.

   ![Marknadsföring av endast aktiviteter i projektet](assets/marketing-only-tasks-in-project-report-nwe-350x309.png){width=400}

1. Använd följande kod om du vill filtrera efter namnet på ett problem:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Observera att du måste använda `issues` som samlingsobjektsnamn i stället för `optask`, vilket är hur problem visas i API Explorer.

1. Klicka på **Klar**.
1. (Valfritt) Fortsätt redigera rapporten.

   eller

   Klicka på **Spara + stäng** för att spara rapporten.

### Referera till en samling i den anpassade uppmaningen för en rapport {#reference-a-collection-in-the-custom-prompt-of-a-report}

Du kan referera till en samling objekt i den anpassade uppmaningen för en rapport om du vill filtrera rapportens resultat efter attributen för de objekt som är kopplade till rapportens objekt.

Du kan till exempel fråga efter uppgiftsinformation i en projektrapport genom att använda en referens till attributen för uppgifter i projektet i den anpassade uppmaningen i rapporten.

>[!NOTE]
>
>Du kan inte referera till samlingar i en standardfråga.

En anpassad prompt är ett anpassat filter där programsatserna förenas med et-tecken. Vi rekommenderar att du skapar programsatsen i ett filter och sedan kopplar ihop raderna i programsatserna med et-tecken.

Mer information om hur du skapar en filtersats med en samlingsreferens finns i avsnittet [Referera till en samling i filtret för en rapport](#reference-a-collection-in-the-filter-of-a-report) i den här artikeln.

Så här lägger du till en referens till en samling i den anpassade uppmaningen för en rapport:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) och klicka sedan på **Rapporter**.
1. Klicka på **Ny rapport**.
1. Markera rapportens objekt.
1. Skapa ett filter med en samlingsreferens enligt beskrivningen i avsnittet [Referera en samling i filtret för en rapport](#reference-a-collection-in-the-filter-of-a-report) i den här artikeln.
1. Klicka på **Rapportinställningar**.
1. Klicka på **Rapportera frågor**.
1. Klicka på **Lägg till fråga**.
1. Klicka på **Egen fråga**.
1. Ange namnet på uppmaningen i fältet **Fält**&#x200B;**namn**.

1. Ange en **nedrullningsbar objektetikett**.
1. Ange följande i fältet **Villkor**:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Valfritt) Ange om det här alternativet visas som standard i uppmaningen.
1. Ersätt **samlingsobjektnamnet** med namnet på samlingsobjektet så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md). Det här värdet är vanligtvis samlingsobjektets plural-form.
1. Ersätt **samlingsobjektfältet** med namnet på fältet för samlingsobjektet så som det visas i [API-utforskaren](../../../wf-api/general/api-explorer.md).
1. Ersätt **samlingsobjektvärdet** med värdet för samlingsobjektet så som det visas i Workfront.

   Om du till exempel filtrerar efter projekt där aktivitetens namn innehåller&quot;Markering&quot; ersätter du **samlingsobjektets värde** med **Markering**.

1. Ersätt värdet **för modifieraren** med en giltig modifierare.

   En lista med modifierare finns i [Filter- och villkorsmodifierare](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Exempel:** Om du till exempel vill skapa en projektrapport med en anpassad fråga där du bara vill visa projekt som har minst en aktivitet tilldelad till en viss användare använder du koden nedan:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Detta genererar en rapport där alla projekt i listan har minst en uppgift tilldelad användaren vars GUID är 57cf1b7a00077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Du kan inte referera till namnet på den primära tilldelaren (&quot;Tilldelad till&quot;-fältet) för en aktivitet enligt [API-utforskaren](../../../wf-api/general/api-explorer.md). Du kan bara referera till ID:t för den primära tilldelade personen.

   Om du till exempel vill filtrera efter projekt där någon av projektnumren har tilldelats en viss användare använder du följande kod för din egen uppmaning:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Detta genererar en rapport där alla projekt i listan har minst ett problem tilldelat användaren vars GUID är 57cf1b7a00077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Observera att du måste använda **issues** som samlingsobjektsnamn. API Explorer har för närvarande inget samlingsobjektsnamn för problem.

1. Klicka på **Klar**.
1. (Valfritt) Fortsätt redigera rapporten.

   eller

   Klicka på **Spara + stäng** för att spara rapporten.
