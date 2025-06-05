---
user-type: administrator
product-area: system-administration
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: Importera data till Workfront med en snabbstartsmall
description: Quick-Starts är Excel-arbetsböcker som är särskilt formaterade och som du kan fylla med data som du vill importera till Workfront. Adobe Workfront tillhandahåller en snabbstartsmall som du kan använda för att göra detta, vilket förklaras i Kickstarts-dataimporteraren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 0%

---

# Importera data till Workfront med en snabbstartsmall

<!--Audited: 12/2023-->

Quick-Starts är Excel-arbetsböcker som är särskilt formaterade och som du kan fylla med data som du vill importera till Workfront. Adobe Workfront tillhandahåller en snabbstartsmall som du kan använda för att göra detta, vilket förklaras i [Kickstart-dataimporteraren](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Den här processen är uppdelad i tre huvuduppgifter:

* Först exporterar du en snabbstartsmall som en kalkylbladsfil
* Därefter fyller du i kalkylbladet med dina data
* Till sist importerar du kalkylbladet till Workfront

Var och en av dessa procedurer beskrivs i rätt ordning i den här artikeln.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p> Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begränsningar

Du kan importera ett stort antal objekt till Workfront med hjälp av en snabbstartsmall. Tänk dock på följande begränsningar:

* Om du importerar data på det här sättet uppdateras inte information om poster som redan finns i Workfront.
* Du kan bara importera nya poster och deras information.
* Importera högst 2 000 poster i taget för att säkerställa att importen inte tar slut

## Exportera en snabbstartsmall som en kalkylbladsfil

När du exporterar en snabbstartsmall får du en tom Excel-kalkylbladsarbetsbok. När kalkylbladet har laddats ned till datorn kan du använda det för att fylla i informationen och sedan importera den tillbaka till Workfront.

Så här exporterar du en snabbstartsmall:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. Klicka på **System** > **Importera data (snabbstart)**.

1. Välj de typer av information som du vill inkludera.

   Varje alternativ som du väljer representerar en samling med flera flikar i det exporterade kalkylbladet. Om du till exempel väljer alternativet **Rapport** inkluderas alla objekt som behövs för att skapa en rapport i kalkylbladet (vyer, filter, grupperingar, rapporter).

   Du kan använda alla objekttyper som listas nedan för att importera data till Workfront. (Det enda undantaget är alternativet Åtkomstnivåer. Databladet Åtkomstnivåer i en export tillhandahålls i referenssyfte, vilket gör att du kan tilldela en åtkomstnivå till ett nytt användarkonto via ID.)

   Mallen för varje objekttyp kan exporteras i följande filformat och innehåller följande blad:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objekt</strong> </p> </th> 
      <th> <p><strong>Exporterar som</strong> </p> </th> 
      <th> <p><strong>Blad i det exporterade kalkylbladet</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Kontrollpanel</p> <p>Alla offentligt delade instrumentpaneler i systemet är tillgängliga för export. Det går inte att exportera instrumentpaneler som inte delas över hela systemet. Du kan välja upp till 100 specifika kontrollpaneler i en enda export.</p> </td> 
      <td scope="col">Exporterar som ZIP-fil</td> 
      <td scope="col"> <p>Parameter</p> <p>Beskrivning</p><p>Parameteralternativ</p> <p>Parametergrupp</p> <p>Kategoriparameter</p> <p>Kategori</p> <p>Rapport</p> <p>Portal Tab Section</p> <p>Kontrollpanel</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapport</p> <p>Alla rapporter i systemet är tillgängliga för export. Du kan välja upp till 100 specifika rapporter i en enda export.</p> <p>Quick-Starts stöder inte textlägesfilter eller -grupperingar. För att exporten ska lyckas måste rapportfiltren och grupperingarna växlas till standardläge.</p> </td> 
      <td scope="col">Exporterar som ZIP-fil </td> 
      <td scope="col"> <p scope="col">Parameter</p> <p scope="col">Beskrivning</p> <p scope="col">Parameteralternativ</p> <p scope="col">Parametergrupp</p> <p scope="col">Kategoriparameter</p> <p scope="col">Kategori</p> <p scope="col">Rapport</p> <p scope="col">Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Godkännande</p> </td> 
      <td scope="col"> <p>Exporterar som Excel-fil</p> </td> 
      <td scope="col"> <p>Scengodkännare</p> <p>Godkännandefas</p> <p>Godkännande</p> <p>Godkännandeprocess</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Anpassade data</p> </td> 
      <td scope="col"> <p>Exporterar som Excel-fil</p> </td> 
      <td scope="col"> <p>Parameter</p> <p>Beskrivning</p>  <p>Parameteralternativ</p> <p>Parametergrupp</p> <p>Kategoriparameter</p> <p>Kategori</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Utgiftstyp</p> </td> 
      <td scope="col"> <p>Exporterar som Excel-fil</p> </td> 
      <td> <p>Utgiftstyp</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Timtyp</p> </td> 
      <td scope="col"> <p>Exporterar som Excel-fil</p> </td> 
      <td> <p>Timtyp</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Team</p> </td> 
      <td scope="col"> <p>Exporterar som Excel-fil</p> </td> 
      <td> <p> Teammedlem</p> <p>Team</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Användare</p> </td> 
      <td> <p>Exporterar som Excel-fil. Klicka på <strong>Fler alternativ</strong> om du vill se en fullständig lista över alternativ.</p> </td> 
      <td> <p>Användare</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td>Åtkomstnivå</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p>Åtkomstnivå</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td>Tilldelning</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p>Tilldelning</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td>Företag</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Företag</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>E-postmall</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p>E-postmall</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Utgift</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Utgift</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Extern sida</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Extern sida</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Filter</td> 
      <td>Exporterar som en ZIP-fil</td> 
      <td> <p> Filter</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Grupp</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Grupp</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Gruppering</td> 
      <td>Exporterar som en ZIP-fil</td> 
      <td> <p> Gruppering</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Timme</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Timme</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Problem</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Problem</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Jobbroll</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Jobbroll</p> <p>Inställningar </p> </td> 
     </tr>

   <tr> 
      <td>Sökväg för milstolpe</td> 
      <td> Exporterar som Excel-fil</td> 
      <td> <p> Milstolpe</p> <p>Sökväg för milstolpe</p> <p>Inställningar </p> </td> 
     </tr>

   <tr> 
      <td>Anteckning</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Anteckning</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Portfolio</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Kö</p> <p>Projekt</p> <p>Cirkulationsregel</p> <p>Köämne</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Resursberäkning</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Resursberäkning</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>risk</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> risk</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Risktyp</td> 
      <td> Exporterar som Excel-fil</td> 
      <td> <p> Risktyp</p> <p>Inställningar</p> </td> 
     </tr> 
     <tr> 
      <td>Styrkort</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p>Styrkortfråga</p> <p>Styrkortsalternativ</p> <p>Styrkort</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Uppgift</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Uppgift</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Mall</td> 
      <td> Exporterar som Excel-fil</td> 
      <td> <p> Kö</p> <p>Mall</p> <p>Cirkulationsregel</p> <p>Köämne</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Malltilldelning</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Malltilldelning</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Malluppgift</td> 
      <td>Exporterar som Excel-fil</td> 
      <td> <p> Malluppgift</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Tidrapport</td> 
      <td> Exporterar som Excel-fil</td> 
      <td> <p> Tidrapportprofil</p> <p>Tidrapport</p> <p>Inställningar </p> </td> 
     </tr> 
     <tr> 
      <td>Visa </td> 
      <td> <p>Exporterar som ZIP-fil</p> </td> 
      <td> <p> Visa</p> <p>Inställningar </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Hämta**.
1. Fortsätt med [Fyll i kalkylbladsmallen med dina data](#populate-the-spreadsheet-template-with-your-data) för att fylla i det tomma mallkalkylbladet med din information.

## Fyll i kalkylbladsmallen med dina data {#populate-the-spreadsheet-template-with-your-data}

* [Översikt över flikarna (datablad) i kalkylbladet](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importera en post](#import-a-record)
* [Inkludera datum](#include-dates)
* [Använd jokertecken](#use-wildcards)
* [Ersättning av attributnamn för ID](#attribute-name-substitution-for-ids)

### Översikt över flikarna (datablad) i kalkylbladet

>[!TIP]
>
>För att bättre förstå hur du behöver formatera informationen i varje kolumn när du fyller i Spark-Start-mallen kan du överväga att göra en övning genom att exportera en Snabbstart med befintliga Workfront-data för de objekt du försöker importera. Instruktioner finns i [Exportera data från Adobe Workfront via Quick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

När du öppnar en tom snabbstartsmall finns ett antal flikar (datablad) tillgängliga. De beror på vilka objekt du har valt för nedladdning. Var och en representerar ett objekt i programmet, till exempel projekt, uppgifter, timmar, kontrollpanel och användare:

När du öppnar någon av dessa flikar visas på rad 2 fälten för varje objekt som kan ställas in under en import. I en kolumnrubrik, efter ordet &quot;set&quot;, visas fältets namn som det visas i databasen. Dessa fält fungerar som kolumnrubriker.

>[!IMPORTANT]
>
>Undvik fel genom att kontrollera följande:
>
>* Ta inte bort den tomma första raden i ett snabbstartskalkylblad.
>* Ta inte bort, ändra eller ordna om dessa fält (kolumnrubriker) på något sätt. Ändra t.ex. inte deras ordning eller namn.
>* Lägg till värden i alla fält som visas i fet stil i kolumnrubriken. Dessa representerar obligatoriska fält.
>
>     Om ett obligatoriskt fält innehåller ett standardvärde som angetts i systeminställningarna behöver du inte fylla i det.
>
>     På fliken **PROJ-projekt** kan till exempel fälten **setCondition** och **setConditionType** lämnas tomma, men det går inte att använda kolumnerna **setGroupID** och **setName** .
>
>* Vissa fält, inklusive **setResourceRevenue** och **setEnteredByID**, genereras automatiskt av systemet. Om du anger data för de här fälten i kalkylbladet åsidosätter snabbstartsprocessen dem när du överför kalkylbladet.

### Importera en post  {#import-a-record}

Varje rad i tabellen motsvarar ett unikt objekt.

1. Lägg till information i kolumnen **isNew**:

   * Om objektet som du importerar är nytt skriver du **TRUE** för att importera data i raden. Det här värdet är skiftlägeskänsligt och måste alltid anges med versaler
   * Om objektet redan finns i Workfront skriver du **FALSE** i kolumnen **isNew** för att ignorera raden. Det här värdet är skiftlägeskänsligt och måste alltid anges med versaler

      * Poster som redan finns i Workfront uppdateras inte.
      * Om du hämtade en mall med data från Workfront är befintliga objekt redan markerade med **FALSE**.
      * Om du har laddat ned en tom mall behöver du inte lägga till nya rader för befintliga objekt.

1. Lägg till information i kolumnen **ID** på något av följande sätt:

   * Om objektet som du importerar är nytt (och du skrev **TRUE** i kolumnen **isNew**) skriver du valfritt nummer för ID:t. Numret måste vara unikt i kalkylbladet. Om du till exempel importerar tre objekt kan du ge dem ID 1, 2 respektive 3.

   * Om objektet redan finns i Workfront (och **FALSE** finns i kolumnen **isNew** ) och du importerar ny information om befintliga objekt, måste ID:t vara det alfanumeriska GUID som finns i Workfront för det objektet.

   >[!TIP]
   >
   > Om du vill ta reda på ett objekts unika GUID i Workfront kan du skapa en rapport för det objektet och lägga till ID-kolumnen i rapporten. Värdet för varje objekt i den kolumnen är objektets GUID.

   * Poster som redan finns i Workfront uppdateras inte.
   * Om du hämtade en mall med data innehåller befintliga objekt redan GUID som ID.
   * Du kan importera ett nytt objekt baserat på ett befintligt objekt genom att ändra **FALSE** till **TRUE** i kolumnen **isNew**, ändra ID:t och göra nödvändiga datajusteringar innan du importerar.

   ![Exempel-ID för en grupp](assets/kick-start-group-example.png)

   * När du importerar ett projekt måste du ange ett grupp-ID.

      * Om gruppen redan finns i Workfront måste du lägga till dess unika ID i fältet **setGroupID** för projektet.
      * Om gruppen inte finns i Workfront kan du lägga till bladet **GRUPPgrupp** i importfilen, ange fältet **isNew** till **TRUE** på gruppbladet och ange ett numeriskt ID för den nya gruppen i kolumnen **ID** . Fältet **setGroupID** för det nya projektet måste matcha det numeriska **ID** för den nya gruppen.

     **Exempel:** För ett projekt måste värdet som visas i kolumnen **setGroupID** något av följande:

      * GUID för en befintlig grupp i din Workfront-instans
      * Värdet (tal) i ID-kolumnen på bladet **GRUPPgrupp** om du skapar en ny grupp under importen

1. Indatavärden för obligatoriska fält och andra fält som du vill fylla i under importen.
1. (Valfritt) Så här lägger du till anpassade data:

   * Skapa en ny kolumn för varje anpassat fält som du vill ta med i importprocessen.
   * Namnge varje ny kolumn för motsvarande anpassade fält enligt följande: **DE:[Namn på det anpassade fältet så som det visas i Workfront]**. Du kan till exempel skapa följande anpassade fält:&quot;DE: Avdelningar&quot;.
   * I kolumnen **setCategoryID** skriver du GUID för det befintliga anpassade formuläret som det här anpassade fältet finns på. Det här fältet är obligatoriskt vid import av anpassade data.
   * Om du behöver lägga till flera datavärden i det anpassade fältet (t.ex. alternativknappar, kryssrutor eller listor), ska du separera värdena med hjälp av den anpassade datamängdsavgränsaren | i det lodräta fältet, som finns på fliken Inställningar.

     **Exempel:** Skriv A|D under kolumnen DE:Departments för att fylla i avdelning A och avdelning D i ditt anpassade formulär.

     >[!NOTE]
     >
     >Använd bara avgränsaren &quot;|&quot; för att separera anpassade fältvärden. Du kan inte använda den i någon av de andra kalkylbladskolumnerna, inklusive **setCategoryID**.

### Inkludera datum  {#include-dates}

Workfront kan bearbeta de flesta datumformat. Du måste dock se till att datumkolumnen i kalkylbladet är formaterad som ett datum. Importen misslyckas om kolumnen är formaterad som allmän, ett tal eller text.

>[!TIP]
>
>Det vanligaste formatet är formatet MM/DD/ÅÅÅÅ.
>
>Exempel: 07/10/2023.

Workfront godkänner också tidsvärden som en del av datumet.

Exempel: 07/10/2022 01:30 eller 07/10/2022 1:00 PM.

Om du utelämnar en tid i datumet gör Workfront något av följande:

* Anta att tiden är 12:00. Systemets tidszon måste matcha din tidszon för att du ska kunna se det förväntade datumresultatet.
* Om den finns i ett objekt som är associerat med ett schema, flyttas tiden till den tidigaste tidpunkt som schemat tillåter.

>[!NOTE]
>
>När du använder en UNIX-tidsstämpel måste du ta med ytterligare tre nollor i slutet av värdet.
>
>Om tidsstämpeln till exempel är 7336899000, skriver du 7336899000000 i cellen.

### Använd jokertecken {#use-wildcards}

Du kan använda följande jokertecken när du fyller i kalkylbladet för snabbstartsmallen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Jokertecken</strong> </p> </th> 
   <th> <p><strong>Beteende</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$IDAG</p> </td> 
   <td> <p>När det används i ett <strong>setDate</strong>-fält anger jokertecknet datumet som midnatt den dag du importerar Spark-Start.</p> <p>Du kan ändra jokertecknet med den standardsyntax som är tillåten med jokertecknet i ett filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du vill att ett projekt ska börja på måndagen i veckan som det importeras på, oavsett vilken dag du faktiskt importerar, kan du använda <strong>$$TODAYbw</strong>. Detta ställer in projektets planerade startdatum till kl. 12.00 på söndag. Eftersom schemat för projektet förmodligen inte tillåter arbete vid den tidpunkten börjar det kl. 09.00 måndag morgon.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NU</p> </td> 
   <td> <p>När det används i ett <strong>setDate</strong>-fält anger jokertecknet datumet enligt den tidpunkt då du skapade posten under Quick-Start-importen.</p> <p>Du kan ändra jokertecknet med den standardsyntax som är tillåten med jokertecknet i ett filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du vill att ett projekt ska starta 3 timmar efter att det har importerats kan du använda <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>När det används i ett <strong>setAssignedToID</strong>- eller annat userID-baserat fält tilldelar jokertecknet arbetet eller associerar posten på annat sätt med den person som utför importen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$KUND</p> </td> 
   <td> <p>Det här jokertecknet har lagts till specifikt för import från Spark-Start-användare. När ett Workfront-konto skapas skapas en användare med åtkomstnivån Systemadministratör. Det användarnamn som tilldelats standardadministratören kan användas som prefix när andra användare skapas i kontot.</p> <p>Eftersom användarnamn måste vara unika för alla kunder är detta användbart när du har flera personer med mycket vanliga användarnamn, som t.ex. John Smith, som kan ha användarnamnet"jsmith". Genom att föregå användarnamnstilldelningen med standardadministratörens användarnamn, garanterar du att varje användarnamn är unikt (till exempel: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Tips! Ett mer elegant sätt att se till att användarnamn är unika för hela systemet är att ange den enskilda personens e-postadress i fältet <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ersättning av attributnamn för ID  {#attribute-name-substitution-for-ids}

Även om det är en god vana att använda ID:n när det är möjligt, är det ibland opraktiskt att korsreferens-ID:n från ett ark till ett annat när du anger ett **setAttributeID** -värde. Du kan referera till värden efter namn genom att ändra kolumnrubriken.

**Exempel:**

* **Importera projekt**

  När du importerar projekt anger du **setGroupID** för projekten genom att gå till **GROUP Group**-bladet, anteckna respektive Group ID och klistra in dem i rätt celler (**setGroupID** -kolumn) på **PROJ Project** -bladet.

  Detta är möjligt när du arbetar med bara ett fåtal grupper och projekt, men om du arbetar med flera av varje är det inte praktiskt.

  Om du vill ersätta attributnamn för det exempel som beskrivs ovan ändrar du kolumnrubriken **setGroupID** till **#setGroupID GROUP name**. Sedan kan du referera till varje projekts grupp efter namn.

  >[!NOTE]
  >
  >Alternativet att använda attributnamnsersättning är begränsat till referenser enbart för befintliga poster. Du kan inte använda namnersättning för objekt som du skapar i samma import.

* **Användarimport**

  Fyll i **setRoleID** från en lista med roller på fliken **ROLE Role** när du importerar användare.

  Vissa roll-ID:n är för poster som redan finns i kontot, medan andra skapas under importen.

  Du kan använda namnersättning för de nya användarposter som har tilldelats befintliga roller. Det går inte att använda nya användarposter som tilldelats nyligen importerade roller.

  Så här kan du använda båda metoderna för samma importfil:

   * Lägg till en kolumn i kalkylbladet till vänster om kolumnen **setRoleID** .
   * Ge den nya kolumnen namnet **#setRoleID ROLE**.
   * För rolltilldelningar till befintliga poster anger du rollnamnen i kolumnen **#setRoleID ROLE name** .

     För rolltilldelningar till nya rollposter anger du det ID som du tilldelade på ROLE-rollbladet i setRoleID.

     ![Roll-ID för användare](assets/set-role-id.png)

## Importera kalkylbladsdata till Workfront

När du har fyllt i Excel-mallen med dina data kan du överföra dess data till Workfront.

Quick-Start-importen stöder följande filtyper:

* Excel (.xls eller .xlsx)
* Zippad fil (.ZIP) (som endast innehåller .xlsx- eller .xls-filer)

  >[!NOTE]
  >
  >Du måste använda en ZIP-fil när du importerar Excel-kalkylblad som refererar till följande objekt:
  >
  >* Rapporter
  >* Dokument
  >* Avatarer
  >* Visa, filtrera eller gruppera egenskapsfiler
  >
  >När du använder en ZIP-importfil måste ZIP-filen ha samma namn som .xlsx- eller .xls-filen och alla filer måste ha samma strukturnivå (inga mappar).

Så här importerar du mallkalkylbladsdata till Workfront:

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Klicka på **System** > **Importera data (snabbstart)**.

1. Klicka på **Välj fil** i avsnittet **Överför data med snabbstartskalkylblad** och bläddra sedan till och markera det ifyllda kalkylbladet.

   Filen överförs automatiskt och ett meddelande om att importen lyckades visas.

   Om det tar längre tid än fem minuter att överföra Excel-filen till Workfront, tar det längre tid att överföra filen och Workfront kan inte överföra den. Prova att importera data i mindre grupper av objekt.

1. (Villkorligt) Om importen inte lyckades får du ett felmeddelande som anger vad problemet är. Försök att identifiera fältet, bladet och radnumret som problemet påträffades i och korrigera informationen i Excel-filen. Försök sedan att importera filen en gång till.
1. (Villkorligt) Om du använder Workfront Fusion kan du nu aktivera dina FLO:er eller scenarier när importen är klar.
